#VERY IMPORTANT READ OR YOU CANT DOWNLOAD THIS APP


# Nooklet

Nooklet is the best place for small forums, for macOS and Windows.

## Download and launch Nooklet

Download the build for your computer from [GitHub Releases](https://github.com/krgkonekpro04-cpu/Nooklet/releases). These alpha builds are unsigned, so your computer may show a first-launch security warning.

### macOS

1. Download [Nooklet for Mac](https://github.com/krgkonekpro04-cpu/Nooklet/releases/download/v0.2.0-alpha.10/Nooklet-darwin-arm64-0.2.0-alpha.10.zip). This build is for Apple silicon Macs (M1/M2/M3/M4).
2. In Finder, open Downloads and double-click the ZIP to extract it.
3. Drag Nooklet.app into your Applications folder and try opening it.
4. If macOS says “Nooklet is damaged and can’t be opened,” open Terminal and type xattr -dr com.apple.quarantine followed by a space. Drag Nooklet.app from Finder into the Terminal window, then press Return. This inserts the app’s actual path, so the instruction works whether your Applications folder is inside your home folder or at the top level of your Mac.
5. Open Nooklet again. This removes the download-quarantine flag from this app; it does not turn off Gatekeeper. Only do this for a copy downloaded from the official Nooklet release page.

### Windows

1. Download [Nooklet for Windows](https://github.com/krgkonekpro04-cpu/Nooklet/releases/download/v0.2.0-alpha.10/Nooklet-win32-x64-0.2.0-alpha.10.zip). This build is for 64-bit Windows computers.
2. In File Explorer, open Downloads, right-click the ZIP, and choose Extract All.
3. Open the extracted Nooklet-win32-x64 folder and double-click Nooklet.exe.
4. If Microsoft Defender SmartScreen appears, select More info, check that the app is Nooklet, then select Run anyway. If Windows shows a different warning or your organization blocks the app, stop and contact the developer.

## App updates

Nooklet checks the public releases when it opens. When a newer interface bundle is available, click Install update. The update keeps sign-in and saved local forums in the app's existing storage.

The updater changes the interface bundle. Changes to the Electron desktop runtime still need a new app download.

## Publish an interface update

1. Build the interface on the developer Mac using the private .env file.
2. Refresh nooklet-source.zip with the source and compiled dist folder. Do not include .env.
3. Commit the updated archive and create a version tag beginning with v.

GitHub Actions packages the interface, creates a SHA-256 checksum, and attaches both to that release.

The public source archive and downloads are on [GitHub Releases](https://github.com/krgkonekpro04-cpu/Nooklet/releases).
