# RecordLah releases

Published builds of RecordLah!, and the manifest the app reads to find them.

* `version.json` -- what the running app compares itself against: the newest
  version and build, where to download it, and the checksum to verify it by.
* Each release carries one `RecordLah-vX.Y-B.zip`, which the app unpacks
  itself. A disk image downloaded in a browser is quarantined by macOS; a file
  the app fetches is not, so updates after the first install need no
  permission dance.

The app's source lives in a separate, private repository. Nothing here is
built by hand -- `release.py` in that repository cuts, uploads and points at
every one of these.
