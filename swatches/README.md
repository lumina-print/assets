# Lumina Print — Color Swatches

Solid-color PNG swatches (80×80) for the Lumina Print catalog app.

## Naming
Each file is named by its 6-digit hex code, lowercase, no `#`:
`4298b5.png` = the color `#4298b5`.

## How the app uses these
In Glide, the `Master_Variants` table has a `Hex_Clean` column (hex with no `#`).
A Template column builds the image URL by dropping `Hex_Clean` into:

`https://cdn.jsdelivr.net/gh/<USER>/<REPO>/swatches/HEXVAL.png`

(jsDelivr serves these straight from GitHub via CDN — free, fast, Glide-friendly.)

## Regenerating
Source of truth: `Brand_Colors_MASTER.csv`. One PNG per distinct valid hex.
