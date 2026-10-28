# OverPass

[![Support OverPass on Ko-fi](https://img.shields.io/badge/Ko--fi-Support%20OverPass-FF5E5B?logo=ko-fi&logoColor=white)](https://ko-fi.com/arctim)

OverPass is built on Wine, DXMT and many other open-source projects: see [CREDITS](CREDITS.md), and please support them too.

Run Windows games on macOS without managing Wine yourself. Pick a game or launcher, click Install, and OverPass downloads Wine, creates the container, installs the runtimes the game needs and adds it to your library.

Status: early release (0.1.0). Expect rough edges.

This repository holds OverPass's builds while its source repository is private. OverPass checks it for updates by itself (OverPass › Check for Updates…).

## Install

Paste this into Terminal:

```sh
curl -fsSL https://raw.githubusercontent.com/McKack/overpass-releases/main/install.sh | bash
```

It downloads the newest release, puts OverPass in your Applications folder and opens it.

Or download `OverPass-<version>.zip` from [Releases](https://github.com/McKack/overpass-releases/releases),
unzip it and move OverPass to Applications. OverPass isn't notarized by Apple yet, so the first time macOS
says it can't verify the app: open System Settings › Privacy & Security and click **Open Anyway**.

Needs macOS 15 or later on Apple silicon. Updates after that install from inside OverPass.

## Features

- Its own open-source Direct3D 10, 11 and 12 runtime (OverPass Runtime, built on DXMT), with DLSS translated to MetalFX, Shader Model 6.8, mesh shaders, tessellation and tiled resources.
- Per-program rules that also reach programs a launcher starts, so a game started by Steam gets its own settings.
- Profile editor, with import and export of profiles.
- Report Issue: the log, your Mac's details and the game's settings in a zip and a prefilled GitHub issue, from a new logged run or the last one.
- A fix for GOG Galaxy in OverPass Wine (rpcrt4), which makes it work.
- Game clients installed in one click: Steam, Epic, GOG Galaxy, EA app, Battle.net, Ubisoft Connect and Rockstar.
- Self-updating app: a daily update check, and Check for Updates… with install and relaunch.
- One-click install of games and launchers. OverPass downloads Wine, creates the container, installs the runtimes and adds the program to your library.
- Container defaults like CrossOver's: DLL preferences, Chinese, Japanese and Korean font replacements and appearance settings, for new and existing containers.
- Components window for Wine, OverPass Runtime and Winetricks, with update checks.
- Per-app profiles: Windows version, runtimes, environment, DLL overrides and graphics backend. Profiles are plain `.ini` files you can edit and share.
- Home and library views, with a sidebar category for each launcher.
- Utilities such as Notepad++ and MusicBee.
- Optional D3DMetal: if you have Apple's Game Porting Toolkit, OverPass can import D3DMetal from your own copy. It is not needed and not redistributed.

## Screenshots

Home lists featured games and launchers. Pick one and click Install:

![Home: featured games and launchers, each with an Install button](docs/screenshots/home.png)

The library holds everything you have installed, grouped by category:

![Library: installed games and apps](docs/screenshots/library.png)

The profile editor changes a program's Windows version, runtimes, environment, DLL overrides and graphics backend:

![Profile editor](docs/screenshots/editor.png)

[More screenshots…](docs/SCREENSHOTS.md)

## Open source

[OverPass Wine](https://github.com/McKack/overpass-wine) and [OverPass Runtime](https://github.com/McKack/overpass-runtime) are free for anyone to use in their own projects and game ports. Neither needs Apple's Game Porting Toolkit or any closed part.

- OverPass Wine is upstream Wine plus CodeWeavers' LGPL changes plus OverPass's patches. Wine is LGPL.
- OverPass Runtime is DXMT's main branch with D3D12, NVAPI and NGX enabled, plus OverPass's additions. It is under the LGPL 2.1.

## Coming

- Engine detection
- Game presets
- Debug Tools
- Xbox app support

## Report problems

In OverPass, right-click the game and choose **Report Issue…**. It saves the log in a zip on your Desktop and opens an issue at [McKack/overpass-releases](https://github.com/McKack/overpass-releases/issues) with your Mac, macOS and OverPass details filled in; drag the zip into it and say what happened. See [CONTRIBUTING.md](CONTRIBUTING.md).
