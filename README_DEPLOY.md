# Crum IP website update

This folder contains drop-in replacement files for the GitHub Pages repository at `https://github.com/isaacscrum/blog`.

## What changed

- Replaces the old personal landing page with a law-firm homepage for Crum IP.
- Adds a Services page for IP litigation, trademark, trade secret, technology disputes, counseling, and transactions.
- Updates the About page to position Isaac S. Crum as the founder of Crum IP.
- Updates the Contact page with intake instructions and warnings not to submit confidential information before conflict review.
- Replaces the Legal Disclaimer page with the law-firm disclaimer language.
- Adds a Privacy Policy page and a `/privacy/` redirect.
- Adds `robots.txt`, `sitemap.xml`, `.nojekyll`, `CNAME`, and a single self-contained stylesheet: `crumip.css`.

## Deployment options

### Option 1: Manual upload in GitHub

1. Download and unzip `crumip_site_update.zip`.
2. Go to the GitHub repository.
3. Upload these files/folders to the root of the repository, replacing existing files when prompted.
4. Commit directly to `main` or open a pull request.
5. GitHub Pages should publish the changes automatically.

### Option 2: Local git workflow

```bash
git clone https://github.com/isaacscrum/blog.git
cd blog
cp -R /path/to/crumip_site_update/. .
git status
git add index.html 404.html about contact services legal-disclaimer privacy-policy privacy crumip.css robots.txt sitemap.xml CNAME .nojekyll README_DEPLOY.md
git commit -m "Update Crum IP law firm website"
git push origin main
```

## Before publishing

- Confirm the entity name. The pages currently use `Crum IP, LLC`.
- Confirm the public phone number and email. The pages currently use `(602) 888-3383` and `info@crumip.com`.
- Add a physical mailing address if you want one displayed.
- Review the legal disclaimer and privacy policy before launch.
- If the firm is not yet formed, consider using `Crum IP` rather than `Crum IP, LLC` until the entity is active.

## Existing assets referenced

The pages reference existing repository assets:

- `/favicon_main.svg`
- `/mainpage-Isaac.jpg`
- `/Headshot-2.png`

If any of those filenames change, update the corresponding references in the HTML.


## Blog / insights notes

This update keeps the old blog posts but reformats them as an "Insights" archive under `/posts/` and removes the old Messner contact footer content from the visible post pages. Each post includes an archived-article notice explaining that the post is general information only and may not reflect current law.

If you decide you do not want any legacy posts on the firm website, remove the `/posts/` folder and remove the `Insights` navigation link from the header/footer templates in the HTML pages.


## v4 article-page consistency pass

This package updates the individual Insights article pages with a revised article header, improved archive notice, polished article body styling, contact call-to-action, and article navigation cards.
