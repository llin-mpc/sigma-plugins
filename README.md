# sigma-plugins

Static hosting (GitHub Pages) for MPC's custom Sigma plugins. Code only — no data lives here.

| Plugin | Path | Registered in Sigma as |
|---|---|---|
| Issuer picker — single-line autocomplete for the basecamp Issuer Quick Search search slot (type, ↑↓, Enter) | `issuer-picker/index.html` → https://llin-mpc.github.io/sigma-plugins/issuer-picker/ | "MPC issuer picker" |

Source of truth for the spec that embeds it: `mpc-labs/sigma-dashboard` → `basecamp-combined/basecamplite-v2-spec.yaml`.
Sigma pins a plugin to its URL (set-once): moving this file means re-registering and repointing the `pluginId` in the spec.
