# The Biscuits & Gravy Show — static website

This is a plain HTML and CSS website prepared for Cloudflare Pages. It does not
use React, Next.js, Node.js, npm, a database, or a build process.

## Files

- `index.html` — all website content
- `styles.css` — all layout, colors, responsive behavior, and animations
- `assets/images/` — images used by the website
- `assets/images/crew/` — one replaceable image per crew member
- `assets/images/star-builder-program.png` — the Star Builder Program graphic used on the page
- `assets/originals/` — the original supplied PNG files, including the Star Builder Program graphic
- `_headers` — basic security and privacy response headers for Cloudflare Pages
- `robots.txt` — permits search engines to index the public website

## Preview locally

Open `index.html` in a browser. No installation or local server is required.

## Upload to GitHub

1. Create a new empty GitHub repository.
2. Extract this ZIP.
3. Upload the contents of this folder to the repository root.
4. Commit the files to the `main` branch.

`index.html` must remain at the repository root.

## Deploy with Cloudflare Pages

1. In Cloudflare, open **Workers & Pages**.
2. Select **Create application**, then **Pages**, then **Connect to Git**.
3. Authorize GitHub and select the repository.
4. Set the production branch to `main`.
5. Select no framework preset.
6. Set the build command to `exit 0`.
7. Use `/` as the build output directory.
8. Select **Save and Deploy**.

Cloudflare will redeploy the site whenever changes are pushed to `main`.

## Add the domain later

After the first deployment, open the Pages project and choose **Custom domains**
then **Set up a domain**. Because the domain will be managed by Cloudflare, its
required DNS record can normally be created automatically.

## Replace crew headshots

Replace the matching PNG in `assets/images/crew/` and keep the filename:

- `eric-reynolds.png`
- `maxwell-kilimczak.png`
- `bryton-dalglish.png`
- `will-journiette.png`
- `ronimus-robinson.png`
- `cole-tatum.png`
- `jay-cruse.png`
- `john-critter.png`

Portrait images with a 4:5 aspect ratio work best. Other dimensions are cropped
automatically by the CSS.

## Common edits

- Latest episode and episode links: edit `index.html`
- Instagram and TikTok links: search `index.html` for `social-link`
- Supported-by content: search `index.html` for `supported-section`
- Guest and sponsor form URL: search `index.html` for `docs.google.com/forms`
- Crew names and roles: search `index.html` for `crew-card`
- Colors and visual styling: edit the variables near the top of `styles.css`
