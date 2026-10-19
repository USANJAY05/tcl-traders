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
The workflow in `.github/workflows/deploy-pages.yml` can publish the static site from `main`, but GitHub's repository settings must be enabled once by an owner: open **Settings → Pages → Build and deployment → Source**, choose **GitHub Actions**, and save. The connected workflow token cannot create the Pages site before that setting is enabled. After saving, rerun the workflow from the **Actions** tab. Note: GitHub Pages is static hosting and does not process Netlify Forms submissions; use Netlify hosting for the enquiry form unless you configure another form backend.

## SEO implemented

- Unique page title and meta description focused on coconut supply/manufacturing in Tamil Nadu
- Canonical URL, robots directives, Open Graph metadata and Twitter card metadata
- JSON-LD Organization structured data with verified available business details
- SVG favicon and refreshed TCL globe logo
- `robots.txt` and `sitemap.xml`

After the final production domain is confirmed, update the canonical URL, Open Graph URL, structured-data URLs, and sitemap URL in the site files if it differs from `https://tcltraders.netlify.app/`. Then verify the domain in Google Search Console, submit `https://tcltraders.netlify.app/sitemap.xml`, and use URL Inspection to request indexing. SEO changes do not guarantee rankings or immediate indexing.

The logo update keeps the TCL-inside-a-globe idea and removes unrelated import/export and truck elements. The original deployed site's source/logo asset could not be retrieved for pixel-by-pixel comparison, so verify the logo against the platform's original artwork before treating it as an exact reproduction.

## Content accuracy

The website uses business facts available from the public TCL Traders profile: manufacturer/exporter, coconuts and coconut products, establishment in 2019, and the Thiruppuvanam address. No phone number or email address was added because a verified business contact address was not available during this rebuild. Product photography is served from Unsplash and requires an internet connection.

## Before launch

- Verify business contact details and product descriptions.
- Confirm product photo suitability and replace images if the company has its own photography.
- Submit a test enquiry and verify delivery in the hosting dashboard.
- Check the live deployment at desktop and mobile sizes.
