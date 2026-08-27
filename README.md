# ez-version

Public version catalog for Sakez `ez_*` resources.

**Format:** plain JSON map — resource name → version string. No logic.

```json
{
  "ez_mute": "1.0.0",
  "ez_vault": "1.0.1a"
}
```

## API

```
https://raw.githubusercontent.com/SakEasy/ez-version/main/versions.json
```

Local `fxmanifest.lua` `version` is the runtime source of truth (`ez.boot`). This repo mirrors it for remote/API checks only.
