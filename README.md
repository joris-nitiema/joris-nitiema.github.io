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
- [ ] CV PDFs (no phone number) → `assets/cv/cv-en.pdf`, `assets/cv/cv-fr.pdf`, then uncomment the links in both `cv.qmd`
- [ ] Award and certificate files (personal data hidden) → `assets/awards/`, `assets/certificates/`
- [ ] Write the 3 project pages, then remove `draft: true`
- [ ] Check every text on the home page (`en/index.qmd`, `fr/index.qmd`)

## Temporary design panel

Open the site with `?design` at the end of the address (for example `https://joris-nitiema.github.io/?design`) to show a **Design** button in the bottom-right corner. It changes colours and fonts live, only in your own browser. Visitors never see it. Use `?design=off` or the "Turn panel off" button to hide it.

To remove it for good: delete `en/design-lab.html` and `fr/design-lab.html`, and the `design-lab.html` line in both `_quarto.yml`.
