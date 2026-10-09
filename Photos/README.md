# Photos

Media for the website's **Fun Life** galleries. Each subfolder feeds one page — just drop
new photos or videos in and they appear on the site automatically (no code changes needed).

| Subfolder | Appears on |
| --- | --- |
| `life-physics/` | Interesting Life Physics — `/fun/physics/` |
| `pet-life/` | Pet Life (Cooby) — `/fun/pets/` |
| `sport-life/` | Sport Life (table tennis, climbing, hiking) — `/fun/sports/` |
| `Wine/` | Wine — `/fun/wine/` |
| `research/stm/` | Research → STM section — `/research/` (hand-arranged in `Instrument_intro.md`; new files need adding there) |
| `research/arpes/` | Research → ARPES section — `/research/` |
| `research/overview/` | Research → "What I'm working on" — `/research/` (one photo per project, hand-placed in `Instrument_intro.md`) |
| `research/qPlus/` | Research → Current work → qPlus AFM sensors — `/research/` |
| `research/Deposition_Gun/` | Research → Current work → Deposition gun — `/research/` |

Two single photos are picked up by name: `main_page.*` (homepage portrait) and
`research/research_page.*` (top of the Research page). Full-resolution originals of those two
live in `_originals/`, which is not published or committed.

Supported file types: images (`jpg`, `jpeg`, `png`, `gif`, `webp`, `avif`, `svg`) and
videos (`mp4`, `webm`, `mov`, `m4v`, `ogg`). Files are shown in filename order, so prefix names
like `01-...`, `02-...` if you want a specific order.

To caption a photo, add a line `File_Name.jpg: "caption text"` to `_data/captions.yml`.
