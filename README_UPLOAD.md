# Upload instructions — fixed static package

This package is intended for the GitHub Pages repository:

`yupenglin-appling/yupenglin-appling.github.io`

## What this package fixes

1. Adds `.nojekyll` so GitHub Pages serves this as a plain static website instead of trying to process the old Academic Pages/Jekyll template.
2. Keeps the top navigation to only three items: `HOMEPAGE`, `PUBLICATIONS`, and `ACADEMIC SERVICE`.
3. Keeps the sidebar consistent across homepage, Publications, and Academic Service pages.
4. Keeps sidebar links to homepage anchors, including `Selected Publications` and `Academic Service Summary`.
5. Removes the two long biography paragraphs from the homepage opening card.
6. Adds `deploy-check.html` so you can confirm whether GitHub Pages is serving this new upload.
7. Adds redirects for old direct URLs: `publications.html` and `academic-service.html`.

## Very important upload method

Do **not** upload this zip file itself, and do **not** upload the outer folder.

Open the unzipped folder and upload the files/folders inside it to the repository root on the `master` branch:

- `.nojekyll`
- `index.html`
- `publications/index.html`
- `academic-service/index.html`
- `service/index.html`
- `publications.html`
- `academic-service.html`
- `deploy-check.html`
- `_data/navigation.yml`
- `_includes/author-profile.html`

When GitHub asks for a commit message, use something like:

`Fix static homepage deployment`

## How to confirm the upload worked

After committing, open:

`https://yupenglin-appling.github.io/deploy-check.html`

If this page says `Deploy check passed`, GitHub Pages is reading the fixed upload.
Then open the homepage with a hard refresh / incognito window:

`https://yupenglin-appling.github.io/`

The homepage opening card should no longer show the two long biography paragraphs.

## If the page still does not change

1. Go to the repository's `Actions` tab and check whether the latest `pages build and deployment` workflow succeeded.
2. Go to `Settings` → `Pages` and confirm the source is the `master` branch and root folder.
3. Confirm the new files were uploaded to the repository root, not inside a nested folder such as `yupenglin_static_fixed_20260526/`.
