# Date picker (Sigma plugin)

Single HTML file, `@sigmacomputing/plugin` SDK via CDN, no build step. Open the file standalone for a demo: the last five weekdays
are enabled.

A calendar of the previous and the current month. Days present in the source element can be clicked on and off; every other day is
greyed out. Nothing is written until **Apply**; **Clear** empties the selection (Apply then clears the control).

Editor-panel contract: `source` (element: one row per available day) · `dayColumn` (text `YYYY-MM-DD`) · `countColumn` (optional
number shown under the day) · `dates` (variable: a text control; receives `YYYY-MM-DD,YYYY-MM-DD`, sorted, cleared when none) ·
`onApply` (action-trigger, fired after the control is written) · `months` (text, default `2`) · `color` (text, default `#2F4A6B`).

The plugin renders inside its element's box (a Sigma plugin cannot float over the page), so place it in a modal: two months side by
side need about 520 × 330 px; narrower boxes stack the months.
