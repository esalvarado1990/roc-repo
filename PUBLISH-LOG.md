# Roc Repo — publish log

- 2026-11-10 (MST): August Wall Completion re-publish landed in
  commit ca4285b — script.rocui 0.6.7 zip md5
  8ad74b5d3c9749e0c3389209e8d3a7ee (trending feed fix +
  wrestling drop in August's search; checker PASS x2). The
  GitHub Pages deploy for ca4285b failed (build succeeded,
  deploy failed ~10m28s; live channel kept serving the prior
  zip 6307ac10a98fc0eb5cd20147532a7e1f). This note is the
  re-drive commit: a fresh push to trigger a new Pages
  build+deploy so the channel serves the ca4285b payload.

## 2026-11-10 — Raven Removal re-drive
Commit bfa5114 (skin.rocos 2.0.20 raven-removal re-publish, zip md5 9cec62174fb5078d10620718ee99b430, addons.xml md5 f088c1edacf37d72f2e1c4ddf89f34fb) pushed clean, but the GitHub Pages deploy did not land: 9 live fetches over ~12 min all still served the old addons.xml (50e37e931a021eeb7c2b2d4ffc428886). This note commit re-triggers the Pages build+deploy; payload unchanged.
