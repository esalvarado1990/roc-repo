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

## 2026-11-10 — Launch train FINAL: skin 2.0.23 (stamp revision) + rocui 0.6.8
Supersedes the interim launch commit 82b831c (reverted in 84a7c4c before any stick installed): Eric's 12:10 stamp call replaced the picker art. Final skin.rocos-2.0.23 = 2.0.21 looks dedup + 2.0.22 VPN region label + STAMP picker medallions (picker-eroc 1b3316a7 ember-gold studded ring, picker-august 54dd7d86 pearl ring; girls untouched), zipped from the icon-fix stage tree in the exact 2.0.22 package shape: 695 entries, md5 96ae379fdd2c1ae4856e19a5780e2060; diff vs 2.0.22 = addon.xml + the 2 picker files only. script.rocui 0.6.8 md5 7e865fe14fcf5f79bc9fd2a575586a4b (news XML escape fix applied pre-publish; code byte-identical to the staged build). Fleet install follows immediately per UPDATE GATE LAW.

Re-drive note (2026-11-10): the FINAL launch commit 4d3770c (skin 2.0.23 stamp revision + rocui 0.6.8, addons.xml md5 eac4cc8c2faab8a83660bb7f8e28e03a) pushed clean, but the GitHub Pages deploy had not landed after ~2.5 min of live fetches (live was still serving the reverted 2.0.20 state, addons.xml md5 f088c1edacf37d72f2e1c4ddf89f34fb). This note commit re-triggers the Pages build+deploy; payload unchanged.

## 2026-11-10 — Launch train R2 correction: E-Roc stamp round 2
Eric (12:26) approved Nue/Jama/August stamps off the set-proof sheet but rejected E-Roc's own stamp R1 (darker/muddier than the set). The stamp hand rebuilt E-Roc's stamp (round 2: picker-eroc 59053373, launcher profile_eroc from profile_eroc_r2) and re-revised both packages before any stick installed R1. This commit swaps ONLY the skin zip: skin.rocos-2.0.23 md5 49d9aa951a4e7111bcc0db86b4b79358 (695 entries, same 2.0.22 package shape; diff vs 2.0.22 = addon.xml + picker-eroc + picker-august 54dd7d86). addons.xml unchanged (still md5 eac4cc8c2faab8a83660bb7f8e28e03a — same version, art-only swap). script.rocui 0.6.8 unchanged. Launcher 5.7 R2 (md5 306b82b4ae262f257699f2c2380900f7) ships wire-side per stick, not through this repo.

Re-drive note 2 (2026-11-10): the R2 correction commit 1a67586 (skin zip md5 49d9aa951a4e7111bcc0db86b4b79358, art-only swap, addons.xml unchanged) pushed clean, but the live channel still serves the R1 zip (96ae379f) minutes later — the Pages deploy is lagging again. This note commit re-triggers the deploy; payload unchanged. Fleet installs must not start until the live zip md5 reads 49d9aa95.

R3 correction (2026-11-10): skin zip swapped to the round-3 E-Roc stamp build (zip md5 148c352f0c83de93a2489c3cf7b70889; single-entry swap picker-eroc -> b92cdf1d; addons.xml unchanged, md5 eac4cc8c). Supersedes the R2 zip 49d9aa95 before any stick pulled it. Fleet installs must verify the picker-eroc md5 on-device (b92cdf1d), not the zip md5.

R4 correction (2026-11-10): skin zip swapped to the round-4 build (zip md5 9c003e9bc7456ae817c090c2694f45fc; diff vs R3 = the 4 picker entries only — real transparency outside the rings: picker-eroc 3225f434, picker-august d027bbfd, picker-nue 00a70729, picker-jama a2ce3da1; addons.xml unchanged, md5 eac4cc8c). Supersedes R3 148c352f. Fleet installs verify picker md5s on-device.

R5 correction (2026-11-10): skin zip swapped to the round-5 smoky-edge build (zip md5 04a1c3975defaad8d5f81b2052286b5d; diff vs R4 = picker-eroc e4e586e1 + picker-august de80e8f7 only; girls byte-untouched; addons.xml unchanged, md5 eac4cc8c). Supersedes R4 9c003e9b. Fleet installs verify picker md5s on-device.
