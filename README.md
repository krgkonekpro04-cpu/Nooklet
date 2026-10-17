# Nooklet

Nooklet is the best place for small forums, for macOS and Windows.

## App updates

Nooklet checks the public releases when it opens. When a newer interface bundle is available, click **Install update**. The update keeps sign-in and saved local forums in the app's existing storage.

The updater changes the interface bundle. Changes to the Electron desktop runtime still need a new app download.

## Publish an interface update

1. Build the interface on the developer Mac using the private `.env` file.
2. Refresh `nooklet-source.zip` with the source and compiled `dist` folder. Do not include `.env`.
3. Commit the updated archive and create a version tag beginning with `v`.

GitHub Actions packages the interface, creates a SHA-256 checksum, and attaches both to that release.

The public source archive and downloads are on [GitHub Releases](https://github.com/krgkonekpro04-cpu/Nooklet/releases).
