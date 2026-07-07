# Kuan-Yu (Wesley) Wey — Personal Website

Source for my personal site at **[kywey.github.io](https://kywey.github.io)**.

I'm a Physics PhD candidate at UCLA. The site introduces who I am, my research with
scanning tunneling microscopy (STM) and angle-resolved photoemission spectroscopy (ARPES),
my CV, and a growing "Fun Life" corner.

## Structure

| File | Page |
| --- | --- |
| `index.html` | Home / landing hero (`/`) |
| `main_page.md` | About Me (`/about/`) |
| `Instrument_intro.md` | Research: STM & ARPES (`/research/`) |
| `research-related.md` | Research → Related Topics (`/research/related/`) |
| `fun.md` | Fun Life hub (`/fun/`) |
| `fun-physics.md` | Interesting Life Physics (`/fun/physics/`) |
| `fun-pets.md` | Pet Life — Cooby (`/fun/pets/`) |
| `fun-sports.md` | Sport Life (`/fun/sports/`) |
| `fun-wine.md` | Wine (`/fun/wine/`) |
| `cv.md` | CV viewer page (`/cv/`) |
| `CV_Kuan-Yu-20260309.pdf` | CV PDF (embedded + downloadable) |
| `assets/css/custom.css` | Custom styling on top of the theme |

Navigation and links live in `_config.yml`.

## Adding photos & videos to the Fun Life pages

The Fun Life galleries build themselves from folders — just drop files in and they appear
automatically (no editing needed). Supported: `jpg/jpeg/png/gif/webp/avif/svg` and
`mp4/webm/mov/m4v/ogg`.

| Folder | Shows up on |
| --- | --- |
| `Photos/life-physics/` | Interesting Life Physics (`/fun/physics/`) |
| `Photos/pet-life/` | Pet Life (`/fun/pets/`) |
| `Photos/sport-life/` | Sport Life (`/fun/sports/`) |

The gallery logic lives in `_includes/gallery.html`.

## Built with

The [Contrast](https://github.com/niklasbuschmann/contrast) Jekyll theme (public domain),
served by GitHub Pages, with a custom stylesheet layered on top.

## Run locally

```
gem install bundler jekyll jekyll-feed
bundle exec jekyll serve
```

Then open <http://localhost:4000>.
