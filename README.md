# Screenroll

A screenshot and screen-recording app for macOS. Capture an area, a window or the whole screen, mark it up with
arrows, shapes, text, numbered steps, blur and pixelate, record video or GIFs, and find every capture again in a
history roll one shortcut away. Includes a `screenroll` command for scripts.

This repository only holds the signed downloads. Website: <https://screenroll.prerakgada.in/>

## This is an alpha

Screenroll 0.1.2 is the third alpha. It is signed and notarized by Apple and passes its own automated checks,
but capturing and recording the real screen have had very little use so far. Expect rough edges, and keep a
second copy of anything you cannot lose. There is no in-app updater yet: update with `brew upgrade --cask screenroll`
or the newest disk image.

New in 0.1.2: **Report a Problem…** and **Send Feedback…**, in the menu-bar menu, the Help menu and Settings › About.

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

Or [download the DMG](https://github.com/PrerakGada/screenroll-releases/releases/download/v0.1.2/Screenroll-0.1.2.dmg):

1. Open the downloaded disk image.
2. Drag **Screenroll** onto the **Applications** shortcut.
3. Open Screenroll from Applications, then eject the disk image.

Checksums (SHA-256) are attached to every [release](https://github.com/PrerakGada/screenroll-releases/releases).

## Permissions

Screenroll asks for nothing when it starts. Each permission is requested only when you press its button in the
welcome window or in Settings, or when you first use the feature that needs it:

- **Screen Recording**, to take screenshots and record the screen.
- **Microphone**, only if you record with your voice.

Since 0.1.1, ⇧⌘3, ⇧⌘4 and ⇧⌘5 are Screenroll's default shortcuts. macOS keeps its own screenshot shortcuts on those
keys until you press **Use Screenroll for ⇧⌘3, 4 and 5** in the welcome window or Settings › Shortcuts; **Give Them
Back to macOS** restores them.

Screenroll opens at login by default. The first time an installed copy starts, it adds itself to your login items
once. Turn it off in the welcome window or Settings › General, and it stays off.

## Privacy

Your captures stay on your Mac: history in `~/Library/Application Support/Screenroll`, saved files where you choose
(`~/Pictures/Screenroll` by default), and they are never uploaded. Screenroll has no account, no analytics and no
telemetry, and does not check for updates. Its only network request is the feedback you send from Report a Problem… or
Send Feedback…, and only when you press Send: your message, the name and email if you added them, and the Screenroll
version, macOS version and Mac model. The server notes a rough location (country, region and city) from your
connection and stores no IP address.

## Uninstall

```sh
brew uninstall --cask screenroll          # or drag Screenroll.app to the Bin
brew uninstall --zap --cask screenroll    # also removes its history and settings (never your saved files)
```

---

© 2026 Engaze
