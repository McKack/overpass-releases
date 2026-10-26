# Credits

OverPass is a front end. Almost everything that makes Windows games run on a Mac was built by the people and
projects below, over many years. If OverPass is useful to you, please support them first: buy CrossOver,
donate to Wine, sponsor the developers whose work you rely on. OverPass wouldn't exist without any of them.

## Wine and CodeWeavers

- **[Wine](https://www.winehq.org)** runs Windows programs on macOS, Linux and BSD, and is the core of
  OverPass Wine. LGPL-2.1. [Donate to Wine](https://www.winehq.org/donate).
- **[CodeWeavers](https://www.codeweavers.com)** employs many of Wine's developers and funds much of its
  development, including the macOS support OverPass depends on. OverPass Wine is built from Wine and from the
  LGPL Wine source CodeWeavers publishes for CrossOver. CodeWeavers also funds DXMT (below). The best way to
  support this work is to [buy CrossOver](https://www.codeweavers.com/crossover), their polished,
  supported product. OverPass contains no CrossOver code beyond that LGPL Wine source.

## Graphics

- **[DXMT](https://github.com/3Shain/dxmt)** by Feifan He (for CodeWeavers) translates Direct3D 10, 11 and 12
  to Metal. OverPass Runtime is DXMT with our patches. LGPL-2.1.
- **[DXVK](https://github.com/doitsujin/dxvk)** by Philip Rebohle and contributors translates Direct3D 8-11
  to Vulkan; DXMT builds on parts of it too. zlib licence.
- **[MoltenVK](https://github.com/KhronosGroup/MoltenVK)** runs Vulkan on Metal, with the
  **[Vulkan loader](https://github.com/KhronosGroup/Vulkan-Loader)**. Apache-2.0.
- **[LLVM](https://llvm.org)** powers DXMT's shader compiler. Apache-2.0 with LLVM exception.
- **[Apple's Game Porting Toolkit](https://developer.apple.com/games/game-porting-toolkit/)** provides
  D3DMetal, an optional graphics engine OverPass can download. Apple's licence; not part of OverPass.

## Inside OverPass Wine

- **[GStreamer](https://gstreamer.freedesktop.org)** and **[GLib](https://gitlab.gnome.org/GNOME/glib)**
  play game video and audio. LGPL-2.1.
- **[FFmpeg](https://ffmpeg.org)** decodes Windows Media formats (an LGPL build).
  [Donate to FFmpeg](https://ffmpeg.org/donations.html).
- **[libvpx](https://chromium.googlesource.com/webm/libvpx)** (VP8, VP9), and Xiph's
  **[Ogg, Vorbis and Opus](https://xiph.org)**. BSD licences. [Donate to Xiph](https://xiph.org/donate/).
- **[FreeType](https://freetype.org)** renders fonts. FreeType Licence.
- **[GnuTLS](https://www.gnutls.org)**, **[Nettle](https://www.lysator.liu.se/~nisse/nettle/)** and
  **[GMP](https://gmplib.org)** handle secure connections. LGPL.
- **[SDL](https://www.libsdl.org)** handles game controllers. zlib licence.
- **[libinotify-kqueue](https://github.com/libinotify-kqueue/libinotify-kqueue)** lets programs watch folders
  for changes. MIT.
- ORC, PCRE2, libffi and proxy-libintl, used by GStreamer and GLib. BSD, MIT and LGPL.

Each build of OverPass Wine carries these projects' licence texts in its `licenses` folder.

## Tools

- **[winetricks](https://github.com/Winetricks/winetricks)** installs Windows components into bottles.
  LGPL-2.1. [Sponsor its maintainer](https://github.com/sponsors/austin987).

## Kindred projects

- **[Highball](https://gethighball.com)** shares OverPass's goals. Its
  [credits page](https://gethighball.com/docs/credits/) inspired this one, and its
  [open compatibility database](https://github.com/gauthierpiarrette/highball-db) is worth a look.

## Supporting OverPass

If you'd like to support OverPass itself too, there's [Ko-fi](https://ko-fi.com/mckack). Thank you.
