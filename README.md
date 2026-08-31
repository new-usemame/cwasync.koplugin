# NextGen Progress Sync for KOReader — moved

> **This repository is frozen.** The plugin was renamed `cwasync.koplugin` → `cwngsync.koplugin` in
> Calibre-Web NextGen v4.1.44. KOReader identifies a plugin by its directory name, so that is a real
> identity change rather than a label, and the plugin now publishes from a different repository:
>
> **https://github.com/new-usemame/cwngsync.koplugin**
>
> Nothing here will be released again. The move was not a GitHub rename, so **there is no redirect** —
> an update manager left pointed at this repository will report "no new release available" forever,
> which looks exactly like an up-to-date plugin. Its last release here is `v4.1.39`.

## What to do

1. In KOReader's [Updates Manager](https://github.com/advokatb/updatesmanager.koplugin) or
   [appstore.koplugin](https://github.com/kaz-utashiro/appstore.koplugin), change the configured
   repository to `new-usemame/cwngsync.koplugin`.
2. Install the new plugin so the directory is `plugins/cwngsync.koplugin/`. On first start it copies
   your existing sync settings across, and your server-side device registration is untouched.
3. Remove the old `plugins/cwasync.koplugin/` directory and restart KOReader. `cwngsync` refuses to
   start while a `cwasync.koplugin` is still present — installed, enabled or disabled — because two
   copies would both push position and highlight updates for the same book.

Your server's `/kosync` page always serves the plugin bundled with the version you are running, if
you would rather update by hand.

## License

GPL-3.0-or-later. See the source-file headers in release artifacts.
