# Screenroll

A screenshot and screen-recording app for macOS. Capture an area, a window or the whole screen, mark it up with
arrows, shapes, text, numbered steps, blur and pixelate, record video or GIFs, and find every capture again in a
history roll one shortcut away. Includes a `screenroll` command for scripts.

This repository only holds the signed downloads. Website: <https://screenroll.prerakgada.in/>

## This is an alpha

Screenroll 0.1.0 is the first build. It is signed and notarized by Apple and passes its own automated checks,
but capturing and recording the real screen have had very little use so far. Expect rough edges, and keep a
second copy of anything you cannot lose. There is no in-app updater in this version.

## Requirements

- A Mac with Apple Silicon (M1 or later)
- macOS 26 or newer

## Install

With Homebrew:

```sh
brew install --cask prerakgada/tap/screenroll
open -a Screenroll
```

Homebrew also links the `screenroll` command-line tool.

Or [download the DMG](https://github.com/PrerakGada/screenroll-releases/releases/download/v0.1.0/Screenroll-0.1.0.dmg):

1. Open the downloaded disk image.
2. Drag **Screenroll** onto the **Applications** shortcut.
3. Open Screenroll from Applications, then eject the disk image.

Checksums (SHA-256) are attached to every [release](https://github.com/PrerakGada/screenroll-releases/releases).

## Permissions

Screenroll asks for nothing when it starts. Each permission is requested only when you press its button in the
welcome window or in Settings, or when you first use the feature that needs it:

- **Screen Recording**, to take screenshots and record the screen.
- **Microphone**, only if you record with your voice.

## Privacy

Your captures stay on your Mac: history in `~/Library/Application Support/Screenroll`, saved files where you choose
(`~/Pictures/Screenroll` by default). Screenroll has no account, no analytics and no telemetry, and makes no network
requests.

## Uninstall

```sh
brew uninstall --cask screenroll          # or drag Screenroll.app to the Bin
brew uninstall --zap --cask screenroll    # also removes its history and settings (never your saved files)
```

---

© 2026 Engaze
