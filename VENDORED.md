# Vendored addons — Roc Repo

These third-party addons are hosted by Roc Repo itself after screening, per Eric's ruling of 2026-10-23 (the packager makes the calls to the finish). No standing third-party repository is required for them.

## plugin.video.iatheater

- **origin:** PythonTrousers (Internet Archive Theater)
- **source:** https://pythontrousers.github.io/kodi/plugin.video.iatheater/plugin.video.iatheater-1.0.0.zip
- **fetched:** 2026-10-23
- **upstream_sha256:** ade1aafeeb1eed525030b8c5588b466f0579717ae24ca5864cdb0cc42e6c4735
- **screening:** Full code read at vendoring: network endpoints are archive.org only (search/metadata/stream/art); no eval/exec/subprocess, no obfuscation, no third-party beacons. Staged tree byte-identical to the upstream zip.
- **ruling:** Eric, 2026-10-23 14:42 MST — vendor Archive Theater into Roc Repo; the PythonTrousers repository addon is removed from all packages.
