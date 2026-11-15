<h1 align="center">Fleet Official Bucket</h1>

<p align="center">
  <strong>Discovery catalogue for official Fleet extensions and themes.</strong><br />
  JSON listings under <code>bucket/</code> with ids <code>org.fleet.*</code> — disable anytime from Fleet settings or the UI.
</p>

<p align="center">
  <a href="https://github.com/krate-apps/fleet"><img src="https://img.shields.io/badge/Fleet-official%20bucket-0B1220" alt="Fleet official bucket" /></a>
  <img src="https://img.shields.io/badge/id-org.fleet.official-informational" alt="org.fleet.official" />
  <a href="https://github.com/krate-apps/fleet"><img src="https://img.shields.io/badge/host-krate--apps%2Ffleet-blue" alt="Fleet host" /></a>
</p>

---

## Layout

```text
bucket.json                 # id, name, official: true
bucket/<id>.json            # extension or theme listing
packages/…                  # optional local trees (dev / offline)
archives/…                  # optional cached .tar.gz assets
.github/workflows/          # krate-apps/fleet-bucket-action (validate, hashcheck, excavate)
```

Each listing may include `homepage`, `architecture.linux-amd64.url` + `hash`, and optional `checkver` / `autoupdate`. Remote installs require a pinned GitHub Releases asset URL and sha256 hash.

## Listings

| Kind | Repositories |
| --- | --- |
| **Extensions** | [`fleet-ext-*`](https://github.com/orgs/krate-apps/repositories?q=fleet-ext-) |
| **Themes** | [`fleet-theme-slate`](https://github.com/krate-apps/fleet-theme-slate) · [`ocean`](https://github.com/krate-apps/fleet-theme-ocean) · [`sand`](https://github.com/krate-apps/fleet-theme-sand) |

Official ids skip the third-party consent gate. Community buckets remain available for everything else.

## Publishing

1. Tag a release on the extension/theme repo with a `.tar.gz` asset.
2. Set `architecture.linux-amd64.url` + `hash` on the matching `bucket/<id>.json` (or run excavator / `fleet-bucket-action/pin`).
3. Never point default installs at a moving branch URL.

## Validate

CI uses [`krate-apps/fleet-bucket-action`](https://github.com/krate-apps/fleet-bucket-action). Locally (workspace):

```bash
FLEET_BUCKET_ROOT=. python3 ../../actions/fleet-bucket-action/scripts/validate-listings.py
```

## Excavator

Daily schedule (`06:20 UTC`) calls [`fleet-bucket-action/excavate`](https://github.com/krate-apps/fleet-bucket-action), which bumps listings and commits **one change per package**:

```text
org.fleet.example: Update to version 1.2.3
```

Set repo secrets `GIT_NAME` and `GIT_EMAIL` (passed as `git-name` / `git-email`).

## Related

| | |
| --- | --- |
| Host | [krate-apps/fleet](https://github.com/krate-apps/fleet) |
| Template | [fleet-template-bucket](https://github.com/krate-apps/fleet-template-bucket) |
| Bucket CI | [fleet-bucket-action](https://github.com/krate-apps/fleet-bucket-action) |
| Docs | [Create a bucket](https://github.com/krate-apps/fleet/blob/main/docs/developer/create-bucket.md) |

---

<p align="center">
  Developed by the <a href="https://runkrate.com">Krate</a> team.<br />
  Released under the MIT License.
</p>
