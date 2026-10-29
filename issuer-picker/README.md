# Issuer picker (Sigma plugin)

Single HTML file, `@sigmacomputing/plugin` SDK via CDN, no build step. Open the file standalone for a demo with eight sample issuers.

Editor-panel contract: `source` (element: the issuer list, pre-sorted held-first then name) · `idColumn` · `labelColumn` · `searchColumn`
(optional lower-case haystack) · `issuer` (variable: the issuer control) · `onPick` (action-trigger, fired after the control is set) ·
`placeholder` (text).

Behaviour: idle = the current issuer's label; type to replace it; the best candidate shows inline with an "n / N" badge; ↑ ↓ cycle;
Enter picks (sets the control, fires On pick); Escape restores. All tokens typed must appear in the haystack (order-free).
