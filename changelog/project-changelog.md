---
title: Project - Changelog
post_excerpt: Add new option to allow upload/download PDF for each project.
featured_image: _images/project-module.jpg
taxonomy:
    category: changelog
    post_tag: changelog

---
3.0.10 | 2026-07-15
* Feature | Card and modal title/subtitle allow intentional line breaks via `<br>` (`wp_kses`)

3.0.9 | 2026-07-02
* Update | Landscape card layout uses `grid-template-columns: 1fr 2fr` (`public/inc/style-dynamic.php`)

3.0.7 | 2026-06-14
* Update | Client updates install from trimmed GitHub release zip (excludes `.md`, `.github`, `_images`, `.gitignore`)



3.0.6 | 2026-06-12
* Fix | Grid gap setting aligned with Product module in style-dynamic
* Feature | Portrait card width driven by `project_setting_card_width` ACF field (300–600px) in style-dynamic

3.0.5 | 2026-05-09
* Fix | Project modal now opens correctly in slider display (render modals outside transformed slider track)
* Fix | Ensure dynamic CSS regenerates reliably (ACF class check + regenerate on options save); grid gap uses `gap` with `!important`

3.0.4 | 2026-05-08
* Add public module documentation page, featured image, and GitHub Actions sync workflow for the Digifox documentation site.

3.0.3 | 2026-04-25
* Fix | Use theme module-link resolver (no dependency on Banner plugin)

3.0.1 | 2026-04-06
* Add modal link type with text + gallery support
* Lock page scroll while project modal is open
* Show image captions in project modal gallery

3.0.0 | 2026-04-06
* Fork Project module from Projects base (ACF fields renamed to project_*)
* Align Project module settings and output with Project base

0.8 | 2024-06-04
* Fix | Issue with layout

0.7 | 2024-06-04
* Fix | Add Project Overview

0.6 | 2024-06-02
* Fix | Remove anchor from fearured image

0.5 | 2024-02-07
* Feature | Add custom style section

0.4 | 2023-10-20
* Fix scroll issue when nav item contains a space

0.3 | 2023-10-15
* Fix | Initialise Git, repo pushed to private GitHub

0.2 | 2023-10-13
* Fix broken the scroll when menu value is more than one word, thus includes a space.

0.1 | 2023-10-01
* First Beta Release
