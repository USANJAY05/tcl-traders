# TCL Traders website

Modern, responsive, static website for TCL Traders, a coconut manufacturer and exporter based in Thiruppuvanam, Tamil Nadu, India.

## Stack

- Semantic HTML5
- CSS (responsive layout, accessible focus states, reduced-motion support)
- Vanilla JavaScript (mobile navigation, product enquiry selection, reveal-on-scroll)
- Netlify Forms markup for the enquiry form

No package installation or build step is required.

## Run locally

Open `index.html` in a browser, or serve the folder with any static HTTP server, for example:

```bash
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Hosting

### Netlify
The included `netlify.toml` publishes the repository root. In Netlify, connect the `USANJAY05/tcl-traders` repository to the existing `tcl-traders` site and set the production branch to `main`. The currently deployed Netlify site was created using a manual deploy, so pushing to GitHub alone will not update that site until repository-based continuous deployment is connected.

The enquiry form uses Netlify Forms markup. Enable form detection for the site and submit a test enquiry after deploying before using it for business.

### GitHub Pages
The workflow in `.github/workflows/deploy-pages.yml` publishes the static site from `main`. If needed, set **Settings → Pages → Build and deployment → Source** to **GitHub Actions**. GitHub Pages will then publish the site at the repository's Pages URL.

## Content accuracy

The website uses business facts available from the public TCL Traders profile: manufacturer/exporter, coconuts and coconut products, establishment in 2019, and the Thiruppuvanam address. No phone number or email address was added because a verified business contact address was not available during this rebuild. Product photography is served from Unsplash and requires an internet connection.

## Before launch

- Verify business contact details and product descriptions.
- Confirm product photo suitability and replace images if the company has its own photography.
- Submit a test enquiry and verify delivery in the hosting dashboard.
- Check the live deployment at desktop and mobile sizes.
