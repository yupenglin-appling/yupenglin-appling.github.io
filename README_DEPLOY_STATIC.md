# Static deployment package

This package is designed to make the GitHub Pages site visually match the preview.

Upload/replace these files in the root of the repository:

- index.html
- .nojekyll
- robots.txt
- sitemap.xml
- 404.html
- publications/index.html
- academic-service/index.html

Important:
The `.nojekyll` file disables Jekyll processing. This prevents the Academic Pages theme from overriding the preview design.
After uploading, wait for GitHub Pages to rebuild and refresh https://yupenglin-appling.github.io/ with Ctrl+F5.
