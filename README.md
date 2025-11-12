# WCS Schema Push v3.2 — Underscore sitemap filenames

**Why:** Some GitHub Pages setups serve `*-index.xml` with the wrong MIME type. Using underscores helps ensure `application/xml`.

**Files to upload/replace:**
- robots.txt  → points to `/sitemap_index.xml`
- sitemap_index.xml → indexes `/sitemap_main.xml`
- sitemap_main.xml  → lists index.html, org.jsonld, faq.jsonld

**After uploading:**
1. Commit changes on GitHub.
2. In Google Search Console (property: https://westchestercleaning.github.io/wcs-schema/), submit `sitemap_index.xml`.
3. If needed, also submit `sitemap_main.xml`.
4. Wait a few minutes and refresh the Sitemaps status.
