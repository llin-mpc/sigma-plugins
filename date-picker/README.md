# Date picker (Sigma plugin)

Single HTML file, `@sigmacomputing/plugin` SDK via CDN, no build step. Open the file standalone for a demo: the last five weekdays
are enabled.

A calendar of the previous and the current month. Days present in the source element can be clicked on and off; every other day is
greyed out. `mode: apply` (default): nothing is written until **Apply**. `mode: live`: no Apply button, the selection is written
0.7 s after the last click — for a modal with its own Done button (Sigma takes no spec-authored actions on a plugin's action
trigger, so the plugin cannot close a modal). **Clear** empties the selection.

Editor-panel contract: `source` (element: one row per available day) · `dayColumn` (text `YYYY-MM-DD`) · `countColumn` (optional
number shown under the day) · `dates` (variable: a text control; receives `YYYY-MM-DD,YYYY-MM-DD`, sorted, cleared when none) ·
`onApply` (action-trigger, optional) · `mode` (text, `apply` or `live`) · `months` (text, default `2`) · `color` (text, default `#2F4A6B`).

The plugin renders inside its element's box (a Sigma plugin cannot float over the page), so place it in a modal: two months side by
side need about 520 × 330 px; narrower boxes stack the months.
