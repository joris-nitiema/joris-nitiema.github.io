# joris-nitiema.github.io

Personal portfolio of Joris NITIEMA, built with [Quarto](https://quarto.org) and published with GitHub Pages.

## How it works

- `en/` – English site (published at the root `/`)
- `fr/` – French site (published at `/fr/`)
- `assets/` – shared files: CV PDFs, award scans, certificates, images
- `.github/workflows/publish.yml` – on every push to `main`, GitHub renders both sites and publishes them. No local Quarto install is needed.

Each page has the same file name in `en/` and `fr/`, so the EN | FR button opens the same page in the other language.

## To do

- [x] Photo (assets/img/photo.jpg, round version in photo-circle.jpg)
- [x] CV PDFs (assets/cv, sources in cv-source)
- [x] Award and certificate files (assets/docs)
- [x] Project and experience detail pages
- [ ] Check every text on the home page (`en/index.qmd`, `fr/index.qmd`)
- [ ] Delete the temporary design panel (see below) once the texts are final
- [ ] Publish EcoTrack's code as a clean public repository (README, screenshots, visitor link, no default secret key), then put the GitHub links back (navbar in both `_quarto.yml`, contact band in both `index.qmd`, header of both CVs). They were removed on 11 Nov 2026 because no public repository was worth showing yet.
- [ ] Add new projects on real data that interest French companies

## Temporary design panel

Open the site with `?design` at the end of the address (for example `https://joris-nitiema.github.io/?design`) to show a **Design** button in the bottom-right corner. It changes colours and fonts live, only in your own browser. Visitors never see it. Use `?design=off` or the "Turn panel off" button to hide it.

To remove it for good: delete `en/design-lab.html` and `fr/design-lab.html`, and the `design-lab.html` line in both `_quarto.yml`.

## Documents and CV

- `assets/docs/` holds the public copies of diplomas, transcripts, awards, certificates, the thesis and the internship report. Date of birth, student ID and serial numbers are masked in these copies.
- `assets/cv/cv-en.pdf` and `cv-fr.pdf` are built from `cv-source/*.tex` with `xelatex`. They contain no phone number.
