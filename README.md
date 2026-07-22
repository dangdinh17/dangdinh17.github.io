# Dang Bui Dinh — Academic Homepage

Source code for my personal academic website:

**[https://dangdinh17.github.io](https://dangdinh17.github.io)**

The website presents my research interests, publications, patent, honors, and curriculum vitae in a compact one-column academic layout.

## Structure

- `index.html` — homepage content and metadata
- `stylesheet.css` — responsive academic layout and visual styling
- `assets/` — shared homepage assets
- `cv/` — curriculum vitae mini-site, published at `/cv/`
- `esrpcb/` — ESRPCB research project mini-site, published at `/esrpcb/`

Each mini-site lives at the repository root and owns its page-specific styles and images. The repository no longer uses the legacy `docs/` theme structure.

The site is static and does not require a build step. GitHub Pages publishes it directly from the root of the `main` branch.

## Acknowledgments

The layout follows the academic format used by [Thao Nguyen (Shibe)](https://thaoshibe.github.io/) and is inspired by [jemdoc+MathJax](https://github.com/wsshin/jemdoc_mathjax).

The previous version of this website was adapted from [Sen Li's academic website](https://github.com/senli1073/senli1073.github.io).

## License

See [LICENSE](LICENSE).
