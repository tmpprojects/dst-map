# Digital Services Tax (DST) Global Map

Interactive color-coded world map of Digital Services Taxes and related digital revenue levies. Static site — no build step required.

**Live site:** [https://tmpprojects.github.io/dst-map/](https://tmpprojects.github.io/dst-map/)

## Local preview

```bash
git clone https://github.com/tmpprojects/dst-map.git
cd dst-map
python3 -m http.server 8080
```

Open [http://localhost:8080](http://localhost:8080).

> Use a local server rather than opening `index.html` directly (`file://`). The map loads GeoJSON from a CDN, which some browsers restrict on `file://` pages.

## GitHub Pages

Deployed automatically on push to `main` via [`.github/workflows/pages.yml`](.github/workflows/pages.yml).

Site: [https://tmpprojects.github.io/dst-map/](https://tmpprojects.github.io/dst-map/)

## Data

Country data is embedded in `index.html`, aligned with the [VATCalc DST tracker](https://www.vatcalc.com/global/digital-services-taxes-dst-global-tracker/) and public sources. For informational use only — not tax advice.

## License

Licensed under the MIT License. See [LICENSE](LICENSE).
