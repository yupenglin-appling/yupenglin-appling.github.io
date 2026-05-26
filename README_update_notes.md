# Website update notes

Upload these files to the same paths in `yupenglin-appling/yupenglin-appling.github.io`.

## Changed files

1. `_pages/about.md`
   - Keeps `Selected Publications` on the homepage.
   - Moves `Research synthesis and methodology` out of `Research Interests`.
   - Adds a separate `Research Skills` section.
   - Wraps the opening personal introduction in `yl-intro-card` so its font size can be controlled separately.

2. `_includes/author-profile.html`
   - Adds a sidebar homepage section menu.
   - The sidebar publication link is now labelled `Selected Publications` and points to `/#selected-publications`.
   - The top navigation `Publications` remains the full `/publications/` page.

3. `_data/navigation.yml`
   - Keeps the top `Publications` item directed to `/publications/`.

4. `assets/css/main.scss`
   - Makes the opening introduction card text smaller.
   - Slightly reduces the sidebar profile text size.
   - Adds styling for the new sidebar section links.
