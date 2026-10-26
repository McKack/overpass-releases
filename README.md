# OverPass releases

Builds of OverPass, a Mac app for installing and playing Windows games, published here while its source
repository is private. OverPass checks this page for updates by itself (OverPass › Check for Updates…).

## Install

Paste this into Terminal:

```sh
curl -fsSL https://raw.githubusercontent.com/McKack/overpass-releases/main/install.sh | bash
```

It downloads the newest release from this page, puts OverPass in your Applications folder and opens it.

Or download `OverPass-<version>.zip` from [Releases](https://github.com/McKack/overpass-releases/releases),
unzip it and move OverPass to Applications. OverPass isn't notarized by Apple yet, so the first time macOS
says it can't verify the app: open System Settings › Privacy & Security and click **Open Anyway**.

Needs macOS 15 or later on Apple silicon. Updates after that install from inside OverPass.

## Components

OverPass downloads what it runs Windows programs with on first launch, from their own public releases:

- [OverPass Wine](https://github.com/McKack/overpass-wine): Wine with CodeWeavers' open-source changes and
  OverPass's patches.
- [OverPass Runtime](https://github.com/McKack/overpass-runtime): Direct3D 10, 11 and 12, NVAPI and DLSS
  through Metal.
