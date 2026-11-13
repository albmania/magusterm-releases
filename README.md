# MagusTerm releases

Downloads of **MagusTerm**, an SSH / SFTP workstation for macOS (Apple Silicon) by Magus Group Albania.

This repository holds **release files only**: no source code.

## Download

Open the [latest release](https://github.com/albmania/magusterm-releases/releases/latest) and download
`MagusTerm_X.Y.Z_aarch64.dmg`. Open it and drag MagusTerm into Applications. The app is signed with an Apple
Developer ID and notarized by Apple.

To check the download, compare its SHA-256 with the `.sha256` file of the same release:

```
shasum -a 256 MagusTerm_X.Y.Z_aarch64.dmg
```

## Updates

An installed MagusTerm looks here about once a day (Settings ▸ General ▸ Updates ▸ Check now does it at once). When
a newer version exists, the sidebar shows **Update to X.Y.Z**; nothing is installed until you press
**Install and restart**. Your vault, connections and settings are kept: they are not inside the app.

Every update archive (`.app.tar.gz`) is signed with MagusTerm's update key, and the app refuses an archive whose
signature does not match the key built into it, or that was signed for another version.
