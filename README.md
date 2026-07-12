# NextGen Progress Sync for KOReader

`cwasync.koplugin` synchronizes reading progress between KOReader devices and a Calibre-Web NextGen server.

## Install

1. Open the repository's **Releases** page and download `cwasync.koplugin.zip` from the latest release.
2. Extract the archive into KOReader's `plugins` directory. The resulting path must be `plugins/cwasync.koplugin/main.lua`.
3. Restart KOReader.
4. Open **Tools → NextGen Progress Sync → Login to NextGen Server** and enter the server URL and credentials.

Existing installations can use KOReader's Updates Manager with this repository. Release tags and the plugin version use the same semantic version (for example, tag `v4.1.11` contains plugin version `4.1.11`). A release appears here only when the plugin itself changes.

## Source and releases

The canonical source is maintained in the Calibre-Web NextGen monorepo under `koreader/plugins/cwasync.koplugin/`. Releases in this repository are produced from a published Calibre-Web NextGen tag, preserving an auditable one-to-one source reference.

## License

GPL-3.0-or-later. See the source-file headers in release artifacts.
