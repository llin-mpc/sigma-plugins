# sigma-plugins

Static hosting (GitHub Pages) for MPC's custom Sigma plugins. Code only — no data lives here.

| Plugin | Path | Registered in Sigma as |
|---|---|---|
| Issuer picker — single-line autocomplete for the basecamp Issuer Quick Search search slot (type, ↑↓, Enter) | `issuer-picker/index.html` → https://llin-mpc.github.io/sigma-plugins/issuer-picker/ | "MPC issuer picker" |
| Range slider — bare two-handle slider with no labels (drag a handle or the band, double-click resets); writes a number-range control | `range-slider/index.html` → https://llin-mpc.github.io/sigma-plugins/range-slider/ | "MPC range slider" |

Source of truth for the spec that embeds it: `mpc-labs/sigma-dashboard` → `basecamp-combined/basecamplite-v2-spec.yaml`.
Sigma pins a plugin to its URL (set-once): moving this file means re-registering and repointing the `pluginId` in the spec.
