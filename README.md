# Nooklet

Nooklet is the best place for small forums, for macOS and Windows.

## Download and launch Nooklet

Download the build for your computer from [GitHub Releases](https://github.com/krgkonekpro04-cpu/Nooklet/releases). The current downloads are unsigned alpha builds, so macOS or Windows may show a security warning the first time you open Nooklet.

### macOS

1. Download Nooklet-darwin-arm64-<version>.zip from the release. This build is for Apple silicon Macs (M1/M2/M3/M4).
2. In Finder, open Downloads and double-click the ZIP to extract it.
3. Drag Nooklet.app into Applications.
4. Control-click Nooklet.app, choose Open, then choose Open again if macOS asks you to confirm. Launch it from Applications afterward.

If macOS still says Nooklet is damaged or refuses to open it, stop and contact the developer for a signed release. Do not run Terminal commands or disable Gatekeeper.

### Windows

1. Download Nooklet-win32-x64-<version>.zip from the release. This build is for 64-bit Windows computers.
2. In File Explorer, open Downloads, right-click the ZIP, and choose Extract All.
3. Open the extracted Nooklet-win32-x64 folder and double-click Nooklet.exe.
4. If Microsoft Defender SmartScreen appears, select More info, check that the app is Nooklet, then select Run anyway.

If Windows shows a different security warning or your organization blocks the app, do not bypass it; contact the developer.

These steps are for the unsigned alpha builds. A signed and notarized release will no longer need the first-launch approval on macOS and should show a verified publisher on Windows.

## App updates

Nooklet checks the public releases when it opens. When a newer interface bundle is available, click Install update. The update keeps sign-in and saved local forums in the app's existing storage.

The updater changes the interface bundle. Changes to the Electron desktop runtime still need a new app download.

## Publish an interface update

1. Build the interface on the developer Mac using the private .env file.
2. Refresh nooklet-source.zip with the source and compiled dist folder. Do not include .env.
3. Commit the updated archive and create a version tag beginning with v.

GitHub Actions packages the interface, creates a SHA-256 checksum, and attaches both to that release.

The public source archive and downloads are on [GitHub Releases](https://github.com/krgkonekpro04-cpu/Nooklet/releases).
