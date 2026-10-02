# GP Storage Solutions – Landing Page

A static one-page site: `index.html`, `styles.css` and `images/`. It has no build step.

## Deploy to Cloudflare Pages (free)
1. Cloudflare dashboard → Workers & Pages → Create → Pages → **Upload assets**
2. Name the project (e.g. `gp-storage-solutions`) and drag in this whole folder
3. Deploy → the site goes live at `gp-storage-solutions.pages.dev`
4. (Optional) Custom domains → add the client's domain

Or connect a GitHub repo with Framework preset **None**, build command empty, and output directory `/`.

## SEO / link previews
The full site address (`https://gp-storage-solutions.pages.dev`) appears in `index.html` (canonical, Open Graph, Twitter and structured-data tags), `robots.txt` and `sitemap.xml`. If the live address changes (e.g. a custom domain), replace it in those three files.

Check link previews after deploying:
- Facebook / WhatsApp: https://developers.facebook.com/tools/debug/
- Google structured data: https://search.google.com/test/rich-results
