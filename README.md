# Digital Services Tax (DST) Global Map

Interactive color-coded world map of Digital Services Taxes and related digital revenue levies. Static site — no build step required.

Works on **GitHub Pages**, **Netlify**, or any static host.

## Local preview

```bash
git clone <your-repo-url>
cd dst-map
python3 -m http.server 8080
```

Open [http://localhost:8080](http://localhost:8080).

> Use a local server rather than opening `index.html` directly (`file://`). The map loads GeoJSON from a CDN, which some browsers restrict on `file://` pages.

## GitHub Pages

### Option A — GitHub Actions (recommended)

1. Push this repo to GitHub.
2. **Settings → Pages → Build and deployment**
   - Source: **GitHub Actions**
3. Push to `main` (or `master`). The workflow in `.github/workflows/pages.yml` deploys automatically.

**Project site URL:** `https://<username>.github.io/<repo-name>/`  
**User/org site:** If the repo is named `<username>.github.io`, Pages serves from the repo root at `https://<username>.github.io/`.

### Option B — Deploy from branch

1. **Settings → Pages**
2. Source: branch `main`, folder **`/ (root)`**
3. Save. GitHub publishes `index.html` at your Pages URL.

`.nojekyll` is included so GitHub skips Jekyll processing.

## Netlify

Drag the folder onto [Netlify Drop](https://app.netlify.com/drop), or connect the repo. `netlify.toml` is already configured.

## Data

Country data is embedded in `index.html`, aligned with the [VATCalc DST tracker](https://www.vatcalc.com/global/digital-services-taxes-dst-global-tracker/) and public sources. For informational use only — not tax advice.

## License

Licensed under the MIT License. See [LICENSE](LICENSE).
