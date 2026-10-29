# SEO guidance

This is a static site published through GitHub Pages at
`https://kleinimhain.de/`. Apply these checks when changing public pages.

## Indexing

- Keep the homepage indexable. Do not add `noindex` to pages intended to
  appear in search results, either in a robots meta tag or an
  `X-Robots-Tag` response header.
- When promoting a preview or copied page to production, remove any preview
  `noindex` restriction before publishing.
- `impressum.html` currently has `noindex, follow`. Preserve this exclusion
  unless explicitly asked to change it.
- Keep `robots.txt` crawlable and allow crawling of pages intended for search.
  Allowing crawling does not override a page's `noindex` rule.

## Sitemap and URLs

- After significant changes to an indexed page, update its `<lastmod>` in
  `sitemap.xml` to the actual date of that change. Do not refresh dates for
  unrelated edits or every deployment.
- Include only canonical URLs intended for indexing in the sitemap. Do not
  add preview pages, fragment links, or intentionally excluded pages.
- Use absolute HTTPS canonical URLs and keep the sitemap URL in `robots.txt`
  correct. Preserve GitHub Pages HTTPS enforcement.

## Page content

- Use concise, descriptive page titles. For the homepage, clearly identify
  the childcare service, Berlin-Friedrichshain location, and Klein im Hain.
- Keep descriptions accurate and useful; avoid keyword stuffing. Keep the
  name, address, phone, and opening hours consistent between visible content
  and structured data.
- Preserve descriptive image alt text, explicit image dimensions, and
  appropriate lazy loading. Keep the main hero image eager to load.
- Keep structured data valid and consistent with the visible page.

## Verification

- Run `git diff --check` and review the diff for unintended SEO changes.
- After deployment, check the live HTML and response headers for accidental
  indexing restrictions, and verify the title, canonical URL, and sitemap.
- Check that HTTP redirects to HTTPS and that canonical pages return HTTP 200.
- For indexing fixes, request indexing or validation in Search Console when
  access is available. Report a submitted request separately from confirmed
  indexing; neither deployment nor a sitemap guarantees indexing or rankings.
