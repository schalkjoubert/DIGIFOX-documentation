---
title: Popup - Changelog
post_excerpt: Popup module for Digifox One Page.
featured_image: _images/popup-module.jpg
taxonomy:
    category: changelog
    post_tag: changelog

---
1.0.11 | 2026-07-23
* Fix | Popup footer HTML no longer double-wrapped with `nl2br()`; WYSIWYG markup renders via `wp_kses_post` only (`public/partials/digifox-popup-display.php`)

1.0.10 | 2026-06-14
* Update | Client updates install from trimmed GitHub release zip (excludes `.md`, `.github`, `_images`, `.gitignore`)



1.0.9 | 2026-06-14
* Update | Version bump to confirm client updates install from the trimmed GitHub release zip (requires 1.0.8+ updater)

1.0.8 | 2026-06-12
* Update | GitHub release deploy zip excludes dev-only files (`.md`, `.github`, `_images`, `.gitignore`) from client plugin updates

1.0.4 | 2026-05-08
* Add public module documentation page, featured image, and GitHub Actions sync workflow for the Digifox documentation site.

1.0.5 | 2026-05-08
* Update | Versioned the “closed” cookie so updating the plugin resets popup state for all users

1.0.6 | 2026-05-08
* Update | Cookie buster now auto-updates when saving Popup options, resetting popup state for all users

1.0.7 | 2026-05-08
* Fix | `popup_setting_overlay` now overlays the hero background image when layout is set to Hero

1.0.3 | 2026-04-29
* Fix | Respect auto-popup expiry cookie even when logged-in (use `?digifox_popup_force=1` to test)
* New | Debug helpers: clear cookie with `?digifox_popup_clear=1`, force open with `?digifox_popup_force=1`

1.0.2 | 2026-04-25
* Update | Add plugin-update-checker support for GitHub updates

1.0.1 | 2026-04-25
* New | Popup module with auto/button triggers, cookie expiry, hero layout, and Gravity Forms selector
