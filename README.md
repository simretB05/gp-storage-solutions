# GP Storage Solutions – Landing Page

A static one-page site: `index.html`, `styles.css` and `images/`. It has no build step.

## Images still needed
- `images/office.jpg` – photo of the storage office

Until this file is added, that spot shows a striped placeholder.

## Deploy to Cloudflare Pages (free)
1. Cloudflare dashboard → Workers & Pages → Create → Pages → **Upload assets**
2. Name the project (e.g. `gp-storage-solutions`) and drag in this whole folder
3. Deploy → the site goes live at `gp-storage-solutions.pages.dev`
4. (Optional) Custom domains → add the client's domain

Or connect a GitHub repo with Framework preset **None**, build command empty, and output directory `/`.
