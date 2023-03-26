
## 鲁虺在线网页版操作系统

# http://os.luhui.net

# 有些时候，想单纯的体验一下这个系统的各方面ui界面操作等等，并不是拿来生产力的，然儿又懒于安装虚拟机（内存不够带不起），那么可以试试几个在线网页版操作系统，打开就能体验，可以操作上网的那种，非常棒！
[![Netlify Status](https://api.netlify.com/api/v1/badges/938bc804-c3e5-449c-9b05-6296e8c9de7a/deploy-status)](https://app.netlify.com/sites/daedalos/deploys)
Windows11：https://win11.blueedge.me/

Windows93：http://www.windows93.net/

Windows96：https://windows96.net/

daedaIOS：https://dustinbrett.com/


## 🌌 **daedalOS** 🌌

## _Desktop environment in the browser_

# Feature Overview

[![Feature Overview](https://img.youtube.com/vi/CkvKPspIPLs/mqdefault.jpg)](http://www.youtube.com/watch?v=CkvKPspIPLs)

# Try It 🏁

### Clone repo

- [Git](https://git-scm.com/downloads)

```
git clone https://github.com/DustinBrett/daedalOS.git
cd daedalOS
```

### Yarn

- [Node.js](https://nodejs.org/en/download/) (**v16**)
- [Yarn](https://classic.yarnpkg.com/en/) (`npm install --global yarn`)

```
yarn
```

##### Development

```
yarn build:fs
yarn dev
```

##### Production

```
yarn build
yarn start
```

### Docker

- [Docker Desktop](https://www.docker.com/products/docker-desktop)

```
docker build -t daedalos .
docker run -dp 3000:3000 --rm --name daedalos daedalos
```

# System 🧠

### [File System](https://github.com/jvilk/BrowserFS)

- File Explorer
  - Back, Forward, Recent locations, Up one level, Address bar, Search
- [Drag & Drop](https://developer.mozilla.org/en-US/docs/Web/API/HTML_Drag_and_Drop_API) File Support (internal & external)
  - Loading progress dialog
- ZIP ([write support](https://www.npmjs.com/package/fflate)), [ZIP](https://github.com/jvilk/BrowserFS/blob/master/src/backend/ZipFS.ts)/[ISO](https://github.com/jvilk/BrowserFS/blob/master/src/backend/IsoFS.ts) read support, [7Z/GZ/RAR/TAR/etc. extract](https://github.com/use-strict/7z-wasm) support
- Writes to [IndexedDb](https://developer.mozilla.org/en-US/docs/Web/API/IndexedDB_API)
- Group selection/manipulation & drag to sort/arrange
- Dynamic and auto cached icons for [music](https://github.com/Borewit/music-metadata-browser), images, video & game saves
- Context Menus
  - Cut, Copy, Create shortcut, Delete, Rename
  - [Add file(s)](https://developer.mozilla.org/en-US/docs/Web/API/File/Using_files_from_web_applications), [Map directory](https://developer.mozilla.org/en-US/docs/Web/API/File_System_Access_API)
  - Open with, Open file/folder location, Open in new window, Open Terminal here
  - Download, Add to archive, Extract here, Set as wallpaper, Convert audio/video/photo/spreadsheets
  - Sort by, New Folder, New Text Document
  - Screen Capture
- Keyboard Shortcuts
  - CTRL+C, CTRL+V, CTRL+X, CTRL+A, Delete
  - F2, F5, Backspace, Arrows, Enter
  - SHIFT+CTRL+R, SHIFT+F10, SHIFT+F12
  - In Fullscreen: Windows Key, Windows Key + R
- File information tooltips
- Allow sorting by name, size, type or date
  - Persists icon position/sort order

### Windows

- [Resizable and Draggable](https://github.com/bokuweb/react-rnd)
- Minimize, Maximize & Close
- Persists size/position/maximized states
- [Animates](https://www.framer.com/motion/) opening and closing

### Start Menu

- Expandable Sidebar
  - Apps list, Documents/Pictures/Videos shortcuts, Power (clears session)
- Spotlight visual effect
- Folder support
- Keyboard shortcut opens with **_SHIFT+ESC_**
  - Or Windows Key when in fullscreen

### Taskbar

- [Peek](https://github.com/bubkoo/html-to-image) hover preview of windows
- Focused window indicator

### Clock

- Runs in a [Web Worker](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers)
  - Drawn in an [OffscreenCanvas](https://developer.mozilla.org/en-US/docs/Web/API/OffscreenCanvas)
- NTP server time mode ([ntp.js](http://www.ntpjs.org/))
- Synced to system clock on load
- Date tooltip

### Background

- Dynamic animated wallpapers ([OffscreenCanvas](https://developer.mozilla.org/en-US/docs/Web/API/OffscreenCanvas)/[Web Worker](https://developer.mozilla.org/en-US/docs/Web/API/Web_Workers_API/Using_web_workers))
  - [Waves](https://www.vantajs.com/?effect=waves)
  - [Hexells](https://znah.net/hexells/)
  - [Matrix](https://rezmason.github.io/matrix/)
  - [Coastal Landscape](https://www.shadertoy.com/view/fstyD4)
- Set via images (Fill, Fit, Stretch, Tile, Center)
- Picture Slideshow
- [Astronomy Picture of the Day](https://api.nasa.gov/#apod)

### URL

- Query parameter loading
  - Examples:
    - `/?url=/CREDITS.md`
    - `/?app=Browser`

# Apps 🧪

### [BoxedWine](http://www.boxedwine.org/) (**_.exe, .zip_**)

- Runs 16/32-bit Windows applications

### Browser (**_.htm, .html_**)

- Loads websites (_w/HTTP header support_)
- Bookmark bar
- Favicon support
- Back/Forward & Reload
- Google search via Address bar

### [DevTools](https://eruda.liriliri.io/)

- Console, Elements, Network, Resources, Sources, DOM
- Activate from Start Menu or **_SHIFT+F12_**

### [EmulatorJS](https://github.com/ethanaobrien/emulatorjs) (**_.32x, .a26, .a52, .a78, .gb, .gba, .gbc, .gen, .gg, .j64, .jag, .lnx, .n64, .nds, .nes, .ngc, .ngp, .pce, .sfc, .smc, .smd, .sms, .v64, .vb, .vboy, .ws, .wsc, .z64_**)

- Plays console game roms

### [IRC](https://kiwiirc.com/)

- Internet Relay Chat Client
- Connects over WebSockets

### [js-dos](https://js-dos.com/) (**_.exe, .jsdos, .zip_**)

- DOS emulator
- Automatic save states on close
  - /Users/Public/Snapshots
- Automatic window resize

### [Marked](https://marked.js.org/) (**_.md_**)

- Markdown Viewer

### [Monaco Editor](https://microsoft.github.io/monaco-editor/)

- Code/text editor
- Supports all file types
- Save files via **_CTRL+S_**
- Line count, cursor position, language id
- [Prettier](https://prettier.io/) formatting
  - json, js/ts, css/sass/less, html, markdown

### [Paint](https://github.com/1j01/jspaint) (**_.bmp, .gif, .ico, .jpg, .png, .tiff, .webp,_**)

- Create & edit images

### [PDF](https://mozilla.github.io/pdf.js/) (**_.pdf_**)

- Render/Print PDF's
- Page current/count & Zoom

### Photos

- [Supported Formats](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/img#supported_image_formats)
  - [JPEG XL](https://github.com/niutech/jxl.js) (**_.jxl_**)
  - [QOI](https://gist.github.com/nicolaslegland/f0577cb49b1e56b729a2c0fc0aa151ba) (**_.qoi_**)
  - [TIFF](https://github.com/photopea/UTIF.js) (**_.tif, .tiff_**)
- Fullscreen & [Zoom](https://github.com/anvaka/panzoom)

### [Ruffle](https://ruffle.rs/) (**_.swf, .spl_**)

- Flash Player emulator

### [Terminal](https://xtermjs.org/)

- File system support
- Autocomplete & history
- Command list via `help`
- [Git support](https://isomorphic-git.org/) (checkout & clone)
- [Python support](https://pyodide.org/) (**_.py_**)
- [WebAssembly Package Manager](https://wapm.io/)
  - Ex: `wapm cowsay moo` ([\#](https://wapm.io/package/cowsay))
- [Weather information](https://wttr.in/)
- [eSheep](https://adrianotiger.github.io/web-esheep/)
- Activate from Start Menu or **_SHIFT+F10_**
- Neofetch

### [TinyMCE](https://www.tiny.cloud/tinymce/) (**_.rtf, .whtml_**)

- Read & WYSIWYG modes
- File save support

### [Virtual x86](https://copy.sh/v86/) (**_.img, .iso_**)

- x86 emulator
- Automatic save states on close
  - /Users/Public/Snapshots
- Automatic window resize

### [Video Player](https://videojs.com/)

- [Supported Formats](https://developer.mozilla.org/en-US/docs/Web/Media/Formats/Video_codecs)
- Plays [YouTube](https://github.com/videojs/videojs-youtube) videos/shortcuts
- Keyboard Shortcuts (Volume, Seek, Scale, Fullscreen)

### [Vim](https://github.com/coolwanglu/vim.js)

- Code/text editor
- Supports all file types

### [Webamp](https://webamp.org/) (**_.mp3, .wsz_**)

- Winamp audio player
- [Skin support](https://skins.webamp.org/)
- Playlist & streaming support
- Visualization support (["Milkdrop"](https://github.com/jberg/butterchurn))

<a href='https://simone.computer/#/webdesktops'><img src="logo.png" alt="logo" height="90" /></a><br />
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
# Awesome Web Desktops

The web's biggest curated directory of apps, portfolios and experiments that mimic the appearance and functionality of desktop operating systems, these are commonly known as [Web Desktops](https://en.wikipedia.org/wiki/Web_desktop).

![info](https://win98icons.alexmeub.com/icons/png/msg_information-2.png) The links are **actively monitored** but if you notice a dead link or would like to contribute with your own creation you're more than welcome to do so, see [contribution guide](contributing.md).<br>
![warning](https://win98icons.alexmeub.com/icons/png/msg_warning-2.png) Seizure warning: some of these websites may contain flashy animations. Viewer discretion is advised.

## Websites

| Site name | Source code |
| --- | --- |
[WorldWideWeb](https://worldwideweb.cern.ch/browser) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Nightwave Plaza](https://plaza.one) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Poolsuite](https://poolsuite.net) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Ash Kyd](https://ash.ms) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/AshKyd/ui95) |
[Cyberspace & Time](http://cyberspaceandtime.com/Gaano9Y6KAU.video+related) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[WWWTXT](https://wwwtxt.org/about) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Windows 93](https://www.windows93.net) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[The Restart Page](http://www.therestartpage.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Webamp](https://webamp.org) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/captbaritone/webamp) |
[It is as if you were doing work](https://pippinbarr.github.io/itisasifyouweredoingwork) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/pippinbarr/itisasifyouweredoingwork) |
[frankenSim](http://frankensim.animade.tv) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Geek Prank](https://geekprank.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Eric Bernacchi](http://eeerik.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[OS.js Demonstration](https://demo.os-js.org) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/os-js/OS.js) |
[Mariano Pascual](http://www.marianopascual.me) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[AfterStep WM](http://www.afterstep.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[98.js](https://98.js.org) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/1j01/98) |
[Broken Reality](https://brokenrealitygame.tumblr.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[WindowMaker](https://www.windowmaker.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Whimsy Space](https://whimsy.space) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/STRd6/zine) |
[WinXP](https://winxp.now.sh) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/ShizukuIchi/winXP/) |
[zach.dev // Software & Adventure](https://zach.dev) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[www.chiptune.com](http://www.chiptune.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Virtual Desktop](http://www.virtualdesktop.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[mattOS](https://mattos-1.webflow.io) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[waller.is](https://waller.is) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Windows 98 Icon Viewer](https://win98icons.alexmeub.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Jurassic Systems](https://jurassicsystems.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/tojrobinson/jurassicsystems.com) |
[The Macpaint Gallery](http://www.macpaint.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[N10.AS RADIO](http://www.n10.as) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Rahul.io](https://rahul.io) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/lolstring/window98-html-css-js) |
[EmuOS](https://emupedia.net/beta/emuos/) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/Emupedia/emupedia.github.io) |
[AaronOS](https://aaronos.dev/AaronOS/aosBeta.php) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/MineAndCraft12/AaronOS) |
[CloudDesk](http://altaica.altervista.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Windows 98 -- Packard Belle](https://packard-belle.netlify.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/padraigfl/packard-belle-desktop) |
[vue win3.1](https://disjfa.github.io/vue-win-3.1/) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/disjfa/vue-win-3.1) |
[Minesweeper](https://winmine-exe.now.sh) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/1000hz/winmine-exe) |
[Gamithra OS](https://gamithra.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[maple's website!](https://maple.pet) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[baz's PC](https://niceware.neocities.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Victor Ribeiro](https://victorribeiro.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/victorqribeiro/fos) |
[Nirrius Creative Studio](https://nirri.us) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Hillary Churchill - Copywriter](http://hillarychurchill.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Bill's World Wide Boutique](https://billsworld.neocities.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[NyjaOS](https://signal3.neocities.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Windows 95 Replica](https://derplayer.neocities.org/repo/win/) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[The Indie Web](https://theindieweb.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/tholman/tholman-blog) |
[hannah blair \| developer & designer](https://hannahblair.co.uk) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[98 KAGE](https://ka.ge) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/pkage/98) |
[erdOS](https://erd-os.iamerd.xyz) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Windows 1.0](https://win1.krnl386.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[glenda.party](https://glenda.0x46.net) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[VirusvAV](https://os.virusav.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[some kind of blog](https://blog.aimen.me) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Repeater](https://repeater.space) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[WuerfelDev](https://wuerfeldev.de) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Glass Animals OPEN SOURCE](https://opensource.glassanimals.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Make WordArt](https://makewordart.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[ytOS](https://ytcracker.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Windows XP](https://windows-xp.netlify.app) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[56k-modem](https://56k-modem.online) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[RACER TRASH](https://racertrash.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Vuindows](https://marcmascarell.github.io/Vuindows) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/marcmascarell/Vuindows) |
[Gustavo Chico](https://gustavochico.com/desktop) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[digital-r41n](https://digital-r41n.neocities.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Online Hacker Simulator](https://pranx.com/hacker/) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Tetrageddon Games](http://tetrageddon.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[My Second PC](https://koas.dev/m2pc) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/koas/my-second-pc) |
[ToxicCode.com](http://toxiccode.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[HyNET Geocity](https://hyena.network/geocity/) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[FLEXEDUPSHAWTY.COM](https://flexedupshawty.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[aconfuseddragon's art and nostalgia corner](https://aconfuseddragon.neocities.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[RaccOS 9](https://violet.pm) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[daedalOS](https://dustinbrett.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/DustinBrett/daedalOS) |
[MSOS Concept](https://msos.midspike.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Novov - Software I use](https://novov.neocities.org/liked/software.html) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Team3D](https://team3d.io) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Day Job](https://dayjob.work) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[PUBLIC DOMAIN](https://public---domain.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[WE=LINK](http://we-link.chronusartcenter.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Thoughts On Glitch[Art]v2.0](http://nickbriz.com/thoughtsonglitchart) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/nbriz/thoughtsonglitchart) |
[Big Desk Energy](https://www.bigdeskenergy.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Github95](https://github95.now.sh) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/edwardpayton/github95) |
[An Ordinary Portfolio Page of Derya](https://deryasdesktop.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/D-Antonelli/portfolio) |
[Yahya J. Aifit](https://yja.me) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[jQuery Desktop](https://desktop.sonspring.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/nathansmith/jQuery-Desktop) |
[Windows 96](https://windows96.net) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[The Coding Forge](https://thecodingforge.com.au) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/Yalgie/website) |
[Vivek Patel - Computer Science Student](https://vivek9patel.github.io) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/vivek9patel/vivek9patel.github.io) |
[Winampify](https://winampify.io) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/remigallego/winampify) |
[Try Andy's Desk](https://desk.glitchy.website) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[tildeOS](https://tilde.town/~selfsame/) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Jack Adam](https://jackadam.cc) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Xiaohan Zou's Portfolio](https://portfolio.zxh.io) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/Renovamen/playground-macos) |
[macOS in Preact](https://macos.vercel.app) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/puruvj/macos-web) |
[Deepin Linux](https://goodmanwen.github.io/) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/GoodManWEN/GoodManWEN.github.io) |
[Win7](https://khang-nd.github.io/win7) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/khang-nd/windows7) |
[Heather Vandervecht](https://heathervv.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/heathervv/portfolio-chatbot) |
[Tony Dinh](https://dinhquangtrung.net/windows7/) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/trungdq88/dinhquangtrung.net) |
[Fizzygum](http://fizzygum.org/sandboxes/latest-stable/) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/davidedc/Fizzygum) |
[RexOS](https://itzrex.neocities.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Joeyonng's Backyard](https://joeyonng.github.io) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/Joeyonng/joeyonng-backyard) | 
[Win11React](https://win11.blueedge.me/) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/blueedgetechno/win11React) |
[Win7 Simu](https://win7simu.visnalize.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Rimet Desktop](https://geocities.ws/rimet/) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[AtheOS](https://al1-ce.dev) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/al1-ce/AtheOS) |
[NeXT](https://www.levenez.com/NeXTSTEP/) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Hunter Hodnett XP](https://hunterhodnett.dev) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/hunterchristian/personal-site-v2) |
[Don chia](https://www.donchia.tech) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/dhs17y2adonchia/win95) |
[LUMISET](https://lumiset.se) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[clickbecause.net](https://clickbecause.net) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[9/11 Realtime](https://911realtime.org) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/robbiebyrd/rt911) |
[Core-OS](https://coreos.io) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/timhow38/Resume-WebApplication) |
[Frank Force - Generative Art](https://generative.3d2k.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/KilledByAPixel/OS13k) |
[Noam Rubin](https://noam-rubin.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/noamrubin22/noam-portfolio-react-ts) |
[Insaf Khamzin](https://insafkhamzin.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/InsafKhamzin/portfolio) |
[Cobra!'s Website](https://cobradile.neocities.org) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Jonathan Zavialov](https://jonzav.me) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/JonZavialov/portfolio2) |
[Alina Sava](https://sava.io) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[KANYE 2049](https://kanye2049.com/) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Windows 11 in Preact](https://win11.vercel.app) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/piyushsuthar/windows-11-web) |
[RebornXP](https://rebornxp.js.org) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/RebornXP/rebornxp) |
[WWWerd](https://theoldnet.com/desktop/) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Puter](https://puter.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Things](https://things.inc) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[1997box](https://1997.pooftie.me) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/middlepot/1997) |
[FoundationOS](https://os.foundation.app) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Orb](https://desktop.leisink.net) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://gitlab.com/hsleisink/orb) |
[RobbieByrd.com](https://robbiebyrd.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/robbiebyrd/platinum) |
[HeadOffice](http://www.headofffice.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Browso](https://www.browso.app) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Harrison's Home](https://harrisonm.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Janne Koivisto](https://janneilkka.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Kayo Felipe Silva](https://kaiofelipejs.dev) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/kaiofelipejs/kaiofelipejs.dev) |
[H4CK1NG G00GL3](https://h4ck1ng.google) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Hudson Mohawke](https://www.hudsonmohawke.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Sam Likes Code](https://samlikescode.dev) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/Goggwell/newfolio/) |
[The Amiga Workbench Simulation](https://taws.ch) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[TAWS@aSCIIaRENA](https://workbench.asciiarena.se) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Amiga34 Germany](http://www.amiga34.de/WB.html) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Richard Eisenmenger](https://amiga.richard-eisenmenger.com/WB.html) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Money Simulator](https://simulator.money/play) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Pangolin Desktop](https://web.dahliaos.io) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/dahliaOS/pangolin_desktop) |
[SantaOS](http://jeremymakes.com/SantaOS/) | ![locked](https://i.imgur.com/cONIqLv.png) n/a  |
[WebXP](https://konsti.club/webSys/) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[HoleNet Cobalt](https://holenet.info) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Hugo Doueli \| Portfolio 2022](https://hugodoueil.fr) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/Ormidales/portfolio/) |
[Chrisbin’s MacBook Pro](https://chrisbinsunny.github.io/chrishub) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/chrisbinsunny/chrishub) |
[Ignasi Monreal](https://www.ignasimonreal.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Jazmin Jones](https://www.jazminjones.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Mastodon Flock](https://mastodon-flock.vercel.app/desktop) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/WesSouza/mastodon-flock) |
[Ɀeus' Stadt](https://zeusofthecrows.neocities.org) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/ZeusOfTheCrows/zeusofthecrows.github.io) |
[Win11 Svelte](https://win11-svelte.vercel.app) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/yashash-pugalia/win11-svelte) |
[Sergio Diaz Schiaffino](https://www.sergiodiazschiaffino.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[holidayOS \| tonik](https://holidayos.tonik.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[chloédigital](https://chloedigital.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[The Secret History of Mac Gaming](https://secrethistoryofmacgaming.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Ubuntu Tour](https://malisipi.github.io/ubuntu-tour) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/malisipi/ubuntu-tour) |
[KeYGeN!!!](https://keyge.nz) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[sue roh](https://sueroh.com) | ![locked](https://i.imgur.com/cONIqLv.png) n/a |
[Windows 11 Web](https://rajaniraiyn.github.io/windows11/) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/Rajaniraiyn/windows11) |
[SilveOS.com](https://www.silveos.com) | [![open](https://i.imgur.com/NBf3juI.png) Available](https://github.com/SilveOS) |

## Archived

See [Archived Web Desktops](archived.md)

## Author

Simone `syx` Marzulli & [contributors](https://github.com/syxanash/awesome-web-desktops/graphs/contributors)

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)
