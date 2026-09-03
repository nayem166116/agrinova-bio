# Investor logos

These files are rendered in the site's forest tone (`#12211E`) and trimmed to
their artwork edges, so the four marks sit evenly on one row.

## Replacing a logo

Drop a new file in with the **same filename** and rebuild. Nothing else needs editing.

| File | Investor |
| --- | --- |
| `nfx.svg` | NFX |
| `illumina-ventures.svg` | Illumina Ventures |
| `orbimed.png` | OrbiMed |
| `astanor.png` | Astanor |

Notes:

- Supply artwork trimmed of surrounding whitespace, otherwise it will look smaller than its neighbours.
- A single-colour (monochrome) version on a transparent background works best.
- Row height is set per logo in `.investor-strip__item` CSS if a replacement needs a different optical size.
- Original untouched files are kept outside the site in `/data/investor_src/`.
