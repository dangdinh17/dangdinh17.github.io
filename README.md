# Dang Bui Dinh — Academic Homepage

Source code for my personal academic website:

**[https://dangdinh17.github.io](https://dangdinh17.github.io)**

The website presents my research interests, publications, patent, honors, and curriculum vitae in a compact one-column academic layout.

## Structure

- `index.html` — homepage content and metadata
- `stylesheet.css` — responsive academic layout and visual styling
- `assets/` — shared homepage assets
- `cv/` — curriculum vitae mini-site, published at `/cv/`
- `research/` — research project mini-sites, organized by year, venue, and project name
- `research/2025_EAAI_esrpcb/` — ESRPCB project, published at `/research/2025_EAAI_esrpcb/`

Research mini-sites live under `research/` and own their page-specific styles and images. The CV mini-site lives under `cv/`. The repository no longer uses the legacy `docs/` theme structure.

The site is static and does not require a build step. GitHub Pages publishes it directly from the root of the `main` branch.

## Acknowledgments

The layout follows the academic format used by [Thao Nguyen (Shibe)](https://thaoshibe.github.io/) and is inspired by [jemdoc+MathJax](https://github.com/wsshin/jemdoc_mathjax).

The previous version of this website was adapted from [Sen Li's academic website](https://github.com/senli1073/senli1073.github.io).

## License

See [LICENSE](LICENSE).

## Publications and project pages

The homepage lists six papers. The default `selected` view shows MDFI and ESRPCB; `all` shows the complete list. Filter counts are computed from the publication entries in the HTML.

Each project remains at `research/<year>_<venue>_<project>/` and contains its own `index.html` and `style.css`. Venue text follows the confirmed publication information, even when an original manuscript filename refers to a different submission.

- `figures/` contains original paper figures. MDFI retains its existing `figure/` directory. These originals stay local, are ignored by Git, and are not loaded directly by the website.
- `images/` contains the selected, optimized WebP images for the project page and a lightweight `thumbnail.webp` for the homepage. Figures link to their full-size web versions.
- Paper PDFs remain local in their existing project folders and are ignored by Git. Public pages use DOI/arXiv links where available and omit local manuscript download links. The CV PDF remains tracked.

To add a paper, create its project page, prepare its web images, and add a publication entry with `data-selected-publication="true"` or `"false"`. Keep the static filter labels consistent as a fallback when JavaScript is unavailable.
