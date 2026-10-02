# GP Storage Solutions

Website for **GP Storage Solutions**: indoor heated storage and 20' & 40' C-Can rentals in Grande Prairie, Alberta.

- **Phone:** 780-518-3615
- **Email:** gpstoragesolutions@gmail.com
- **Office:** 9845 99 Ave #36, Grande Prairie, AB T8V 0R3
- **Storage units:** 10715 92 St, Grande Prairie, AB T8V 3W1 (separate location)

It's a single static page (plain HTML and CSS) with no build step and no dependencies.

## Project files

| File / folder | What it is |
|---|---|
| `index.html` | All page content: text, contact details, hours, SEO tags |
| `styles.css` | All styling. Brand colours are at the top (`--navy`, `--red`) |
| `images/` | Photos, logo, map and social share image |
| `images/icons/` | Browser tab and phone home-screen icons |
| `favicon.ico` | Fallback tab icon for older browsers |
| `robots.txt`, `sitemap.xml` | Help search engines find the site |
| `site.webmanifest` | App name and icons when saved to a phone home screen |
| `wrangler.jsonc`, `.assetsignore` | Cloudflare deployment settings |

## Previewing changes

Open `index.html` in any browser. No server is needed.

## Publishing

The site is hosted on **Cloudflare Workers** and connected to this GitHub repository. Every push to the `main` branch goes live automatically within a minute or two.

```bash
git add -A
git commit -m "Describe the change"
git push
```

`.assetsignore` keeps the README and config files from being published.

## Common updates

All of these are in `index.html`:

- **Phone, email or office hours:** search for the current value (e.g. `780-518-3615`) and replace every match. The phone number also appears in the `tel:` links and the structured data near the top of the file.
- **Office address:** in the "Our Office" section (text and the Directions to Office link).
- **Storage unit address:** in the "Storage Unit Location" section and the structured data.
- **Photos:** put the new image in `images/` and update the matching `src="images/..."`. Keep files under ~300 KB (JPG or WebP) so the page loads quickly.
- **C-Can sizes and descriptions:** in the "C-Can Rentals" section.

## Site address and link previews

The live site is **https://milosgarden.ca**. That address appears in several places because WhatsApp, Facebook, X and Google need full URLs:

- `index.html`: canonical link, Open Graph, Twitter and structured-data tags
- `robots.txt`
- `sitemap.xml`

If the address changes (for example, moving to a custom domain), replace it in all three files.

After publishing, check the results:

- **Facebook / WhatsApp preview:** https://developers.facebook.com/tools/debug/ (click **Scrape Again** to refresh)
- **Google structured data:** https://search.google.com/test/rich-results
