# GitHub Pages skeleton for papers

This repository is a minimal static site scaffold for hosting papers on GitHub Pages.

Site URL (user site): https://davidtswanson903.github.io/

See `RELATIONS.md` for the PDF ↔ landing page ↔ BibTeX mapping.

## What is included

- `index.html` homepage
- `style.css` minimal styling
- `papers/` one page per paper
- `pdfs/` folder for PDF files
- `bib/swanson-canon.bib` bibliography file
- `papers/template-paper.html` reusable paper-page template
- `.nojekyll` to keep GitHub Pages simple

## How to use it

1. Create a GitHub repository named `YOUR-USERNAME.github.io`.
2. Upload these files to that repository.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and the `/(root)` folder.
6. Save.
7. Wait for the site URL to appear.

## What to edit first

- Replace the placeholder abstract text on paper pages.
- Upload your PDFs into `pdfs/`.
- Update the PDF links if filenames differ.
- Add PhilArchive / SSRN / other links where relevant.
- Add more paper pages by copying `papers/template-paper.html`.

## Google Scholar indexing checklist

Google Scholar typically indexes *a landing page per paper* (HTML) that links to a crawlable PDF and includes Scholar-compatible `citation_*` metadata.

- Each paper page in `papers/` should include at least:
	- `citation_title`
	- `citation_author` (repeat this tag for each author if multiple)
	- `citation_publication_date` (YYYY or YYYY-MM-DD)
	- `citation_pdf_url` (prefer an absolute URL)
- The PDF URL should be publicly accessible (no login) and linked in the page body.
- `robots.txt` should not block crawling; this repo allows all and advertises `sitemap.xml`.

Quick self-check: open a paper page in the browser, View Source, and verify the `citation_pdf_url` points to `https://davidtswanson903.github.io/pdfs/...`.

## Suggested next additions

- A dedicated `about.html`
- A CV page
- A longer publications page with categories
- A custom domain later if desired
