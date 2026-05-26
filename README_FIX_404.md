# Emergency fix for 404 / navigation issue

Upload these files to the root of `yupenglin-appling/yupenglin-appling.github.io` and keep the same folder structure.

## What this package changes

1. `index.html`
   - Directly updates the live static homepage. The current site is serving the root `index.html`, so changing only `_pages/about.md` will not update the visible homepage.
   - Sidebar section link is now `Selected Publications`, pointing to `/#selected-publications`.
   - Top navigation still uses `Publications`, pointing to `/publications/`.
   - `Research synthesis and methodology` is moved out of Research Interests and placed under a separate `Research Skills` section.
   - The biography in the first card is slightly smaller.

2. `service/index.html`
   - Adds a redirect from `/service/` to `/academic-service/` to prevent 404 errors from old links.

3. `_data/navigation.yml`
   - Corrects the Jekyll navigation URL for Academic Service to `/academic-service/`.

4. `_includes/author-profile.html`
   - Keeps the Jekyll sidebar consistent if the Jekyll source pages are used again later.

## Upload instruction

Do not upload the folder `yupenglin_site_fix` itself as a nested folder. Open it and upload the contained files/folders into the repository root, so that the paths become:

- `index.html`
- `service/index.html`
- `_data/navigation.yml`
- `_includes/author-profile.html`
