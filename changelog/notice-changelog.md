---
title: Notice - Changelog
post_excerpt: Dismissible website notice module for Digifox One Page.
taxonomy:
    category: changelog
    post_tag: changelog
---

1.0.2 | 2026-07-23
* Fix | Notice message HTML no longer double-wrapped with `nl2br()`; WYSIWYG markup renders via `wp_kses_post` only (`public/partials/digifox-notice-display.php`)

1.0.1 | 2026-07-19
* Update | Version bump to confirm client updates install from the GitHub release zip

1.0.0 | 2026-07-19
* New | Full-width notice above the website header with editable message and call-to-action
* New | Optional close button and configurable dismissal cookie expiry
* New | Background, text, accent and alignment controls
* New | Saving Notice settings or loading a demo resets the versioned dismissal cookie
* New | Responsive header offset automatically follows the notice height
* Update | ACF field groups live in the Digifox theme (`acf-json`), matching other modules
