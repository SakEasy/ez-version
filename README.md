# ez-version

Canonical fleet version manifest for `ez-developer` resources.

- **Primary runtime source:** `version '…'` in each resource `fxmanifest.lua` (read by `ez.boot` via `GetResourceMetadata`).
- **This repo:** synced copy for dashboards, CI, and cross-checks.

## Raw URL

```
https://raw.githubusercontent.com/SakEasy/ez-version/main/versions.json
```

## Bump workflow (preprod)

```bash
node resources/[local]/[core]/[sakez]/ez_lib/_tools/fleet-version.js bump --all
node resources/[local]/[core]/[sakez]/ez_lib/_tools/fleet-version.js sync-version-repo
node resources/[local]/[core]/[sakez]/ez_lib/_tools/fleet-version.js publish-version-repo
```

Pre-release letters: `1.0.1a`, `1.0.1b`, … · Release (owner says ปล่อย): `release --all`.

See [`ez_lib/docs/version.md`](../ez-developer/ez_lib/docs/version.md) in the fleet repo.
