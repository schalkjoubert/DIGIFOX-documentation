---
title: Team - Changelog
post_excerpt: New major release. We removed the built-in demo feature in favour of speed and stability en user experience. Addressed minor bug fixes and enhanced the UI for the column selection
featured_image: _images/team-module.jpg
taxonomy:
    category: changelog
    post_tag: changelog

---
3.0.8 | 2026-07-22
* Fix | **Landscape** layout stacks as portrait below 480px (photo above text) so cards stay readable on small phones (`public/inc/style-dynamic.php`)
* Fix | A single team card is centered in grid and slider layouts (`public/partials/digifox-team-display.php`, `public/inc/style-dynamic.php`)

3.0.7 | 2026-07-15
* Feature | Member name and title allow intentional line breaks via `<br>` (`wp_kses`)

3.0.6 | 2026-06-25
* Fix | Team social SVG icons use global Setup → Icons colour (`setup_icon`) instead of white fill

3.0.5 | 2026-06-14
* Update | Client updates install from trimmed GitHub release zip (excludes `.md`, `.github`, `_images`, `.gitignore`)



3.0.4 | 2026-05-10
* Fix updates overwriting appearance: `style-dynamic.css` is regenerated from **your** Team options when the plugin version changes (and after WP plugin updates), instead of keeping a bundled snapshot that forced portrait layout / wrong crop / stray colours.
* Removed injecting **Setup → Icon** colour onto social buttons (`!important`) — use theme `style-dynamic.php` or module CSS so Digifox Setup colours stay authoritative.
* Public CSS: social link tiles default to **transparent** background (was `#555`) so theme styles apply.

3.0.3 | 2026-05-10
* Documentation: public module docs page, featured image, GitHub Actions sync workflow for the Digifox documentation site.
* When **Text align** is **Center**, the social icon row now centers too (`justify-content: center` on `.teamInner .social`; flex layout ignored `text-align` before).

3.0.2 | 2026-04-06
* Center grid team inner content when padding is applied

3.0.1 | 2026-01-28
* Update: Social SVG icons now load from the active theme first (`assets/svg-fa/plain-social`). Use the digifox theme so all icon assets stay in the theme.

3.0 | 2026-01-28
* Replace Slick slider with Digifox slider
* Added dots/arrows pagination options
* Added cache-busting versions for public CSS
* Cleaned unused assets and old debug code

2.6.1 | 2024-02-25
* Feature | Update GH Access token for writing and syncing changelog

2.6 | 2024-01-15
* Fix: Slider Delay validation

2.5 | 2023-10-22
* New: Add Phone number option for each team member

2.4 | 2023-10-19
* Fix broken the scroll when menu value is more than one word, thus includes a space.

2.3.1 | 2023-09-06
* New: Add Email & Website link options.

2.3 | 2023-04-14
* New: Create "under construction" setup option.

2.2 | 2023-03-22
* Codespace: Update master to main branch

2.1 | 2023-03-22
* Fix: Remove hardcoded heading for testing.

2.0 | 2023-03-01
* First major rebuild
* Remove built-in demo
* Updated column selction interface
* Convert slug.
