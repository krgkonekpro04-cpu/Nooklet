# Nooklet

Nooklet is the best place for small forums, for macOS and Windows.

The app checks GitHub Releases when it opens. When an interface update is available, click Install update in Nooklet. Sign-in and local data stay in the app's existing storage.

## Source and release workflow

The public source archive is nooklet-source.zip. GitHub Actions builds nooklet-ui.zip and a SHA-256 checksum when a version tag beginning with v is pushed. The GitHub Actions secrets VITE_SUPABASE_URL and VITE_SUPABASE_ANON_KEY must be configured privately before publishing future releases.

Interface updates do not update Electron itself; changes to the desktop runtime need a new app package.
