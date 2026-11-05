# Digital Pets

Free tools and a starter pet for ChatGPT and Codex desktop pets.

![Mochi](preview.gif)

## Mochi, a free starter pet

The repo root holds a small purple bunny: a 1536 x 2288 transparent PNG sheet (8 columns by 11 rows, 192 x 208 cells) and a `pet.json`.

- **ChatGPT on the web (tested):** needs a ChatGPT Plus account. Go to Settings > Pets > Upload and choose `spritesheet.png`.
- **Desktop app (Windows and Mac):** make a folder named `mochi` containing `pet.json` and `spritesheet.png`, and put it in `~/.codex/pets/` (on Windows, `%USERPROFILE%\.codex\pets\`), then refresh Settings > Pets. This is not tested yet. The `pet.json` fields come from a third-party copy of the hatch-pet skill.

## Validate your own pet

Use it online: https://bzucker4.github.io/digital-pets/

Or open `index.html` in a browser. Drop in your spritesheet and read the results. Nothing is uploaded; it runs in your browser.

It checks size on disk, exact dimensions, transparency, leftover magenta background, frame counts per row, empty cells, edge bleed and an optional `pet.json`. A preview plays any row.

Sheet layout it expects (from a real hatch-pet export):

| Row | State | Frames |
| --- | --- | --- |
| 1 | idle | 6 |
| 2 | running-right | 8 |
| 3 | running-left | 8 |
| 4 | waving | 4 |
| 5 | jumping | 5 |
| 6 | failed | 8 |
| 7 | waiting | 6 |
| 8 | running | 6 |
| 9 | review | 6 |
| 10 | look 0 to 157.5 degrees | 8 |
| 11 | look 180 to 337.5 degrees | 8 |

The 9-row standard sheet (1536 x 1872) is also supported.

## Custom pets

I make finished, checked pets for developer brands and creators. [Link to Gumroad]

Third-party project. Not affiliated with or endorsed by OpenAI.
