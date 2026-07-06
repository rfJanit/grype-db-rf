# RapidFort Grype Vulnerability Database

This repository hosts the vulnerability database consumed by the RapidFort variant
of [Grype](https://github.com/rfJanit/grype). It contains **no code and no git-tracked
DB files** — the DB is published exclusively as release assets on this repo's `v6`
release (a rolling release, updated on every DB refresh).

## Consumption

The `grype` binary from `github.com/rfJanit/grype` reads this DB automatically. End
users do not need to interact with this repo.

To inspect the current DB manifest:

    curl https://github.com/rfJanit/grype-db-rf/releases/download/v6/latest.json

## Refresh cadence

The DB is rebuilt every 6 hours by a scheduled workflow in `rfJanit/vunnel`. See
`RELEASE-GUIDE-GRYPE.md` in the Grype Repos workspace for the full pipeline.
