# How to update the GitHub academic homepage

This package contains replacement files for the repository `VictorLin2024/victorlin2024.github.io`.

## Files included

- `_config.yml` — site title, author profile, email, sidebar biography, repository settings.
- `_data/navigation.yml` — simplified top navigation: Home, Publications, Academic Service.
- `_pages/about.md` — English homepage with refined profile, research interests, education, selected publications, and academic service.
- `_pages/publications.md` — detailed publications page with empirical studies, review articles, and conference presentations.
- `_pages/service.md` — editorial positions and invited peer-review service page.

## Changes in this version

- Removed the Chinese sections from the homepage, Publications page, and Academic Service page.
- Made the homepage visual hierarchy softer by reducing the apparent weight of the main profile heading.
- Reworked the Education section so that the current Tsinghua status, department/unit, and period are visually distinguished.
- Made DOI-bearing publication cards clickable. Clicking a publication card opens the corresponding DOI page in a new tab.

- Converted Editorial Service into clickable journal cards, with the role displayed as a prominent tag.
- Linked the editorial-service cards to the official journal pages for Quality Assurance in Education and Social Education Research.

## Recommended upload steps on GitHub web interface

1. Open the GitHub repository.
2. For each file in this package, open the corresponding path in the repository.
3. Click the pencil icon to edit.
4. Replace the existing file content with the content from this package.
5. Commit changes directly to the `master` or `main` branch.
6. Wait for GitHub Pages to rebuild.

## Notes

- Avatar, CV, Google Scholar, ORCID, ResearchGate, GitHub, and other external profile links are intentionally hidden in this version.
- DOI links are retained on the Publications page because they are part of formal academic citations.
- Old template pages such as Teaching, Talks, Portfolio, Blog Posts, CV, and Guide may still exist in the repository, but they will not appear in the top navigation after replacing `_data/navigation.yml`.


## Version 3 updates

- The homepage opening statement is now paragraph-sized, bold, and italic rather than styled as a large title.
- In Education, the Tsinghua entry now uses a more prominent color for the Current badge, and “Unit” has been changed to “Aff.”.
- Academic Service now includes a detailed invited-reviewer journal list with journal index/rank labels.


## V4 visual refinements

- The homepage profile statement is styled as bold italic body text, not a large title.
- The current Tsinghua University affiliation uses a warm-gold Current badge, and the school name is colored consistently with that badge.
- The Education field label uses **Aff.** rather than **Unit**.
- Academic Service includes a detailed invited-review journal list.


## Version v7 refinements

- Reduced the corner radius of editorial-service cards and role tags by approximately 60%.
- Changed editorial role labels from all caps to Title Case.
- Bolded the journal titles inside editorial-service cards.


Latest adjustment in v7: editorial-service cards now display the role tag first, then a smaller date line, then the bold journal title.


## Notes for this version

This version adds `_includes/author-profile.html` to customize the left sidebar. It separates the sidebar information into four lines: PhD Candidate in Applied Linguistics; Tsinghua University; Beijing, China; and Educational technology · Positive psychology · Applied linguistics. Upload this file together with the other files so the sidebar renders correctly.


## Important fix in v9

This package fixes the left author sidebar issue where raw CSS text appeared before the profile information.

What changed:
- `_includes/author-profile.html` no longer contains any inline `<style>` block.
- Sidebar styling has been moved into `assets/css/main.scss`.
- The avatar output is disabled until an actual avatar image is added.
- The left sidebar now displays:
  - Yu-Peng Lin
  - PhD Candidate in Applied Linguistics
  - Tsinghua University
  - Beijing, China
  - Educational technology · Positive psychology · Applied linguistics
  - Email

Upload/replace these files especially:
- `_includes/author-profile.html`
- `assets/css/main.scss`
- `_config.yml`
- `_data/navigation.yml`
- `_pages/about.md`
- `_pages/publications.md`
- `_pages/service.md`

After uploading, wait for GitHub Pages to rebuild. If the old sidebar persists, hard refresh the page or open it in an incognito window.


## v10 fix
This version fixes abnormal publication-card rendering caused by block-level `<a>` cards being parsed incorrectly by Jekyll/Kramdown. Publication cards are now clickable `<div>` blocks with `onclick` handlers, so the rounded empty boxes and stray `</a>` text should disappear.


## v12 fix
This version uses no block-level `<a>` wrappers in publication cards. Cards are normal `<div>` elements with `onclick` and keyboard handlers, preventing Jekyll/Kramdown from creating empty rounded boxes or visible `</a>` text.


## v13 visual and duplication fix
This version:
- removes duplicate name displays on the homepage by hiding the masthead site title and the layout-generated page title;
- removes the extra name inside the homepage hero card;
- restyles the GitHub Pages sidebar and main cards to match the preview design more closely;
- adds the YL initials block to the left profile card;
- keeps publication cards clickable without block-level anchor wrappers.
