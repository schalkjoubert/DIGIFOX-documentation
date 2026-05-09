---
title: Contact - Changelog
post_excerpt: New major release. We removed the built-in demo feature in favour of speed and stability en user experience. Addressed minor bug fixes and enhanced the UI for the column selection
featured_image: _images/contact-module.jpg
taxonomy:
    category: changelog
    post_tag: changelog

---

3.0.5 | 2026-05-09
* Remove `contact_setting_text_align` and alignment-specific CSS; heading and intro follow theme `.module .head` (center) styles only.

3.0.4 | 2026-05-09
* Honour `contact_setting_text_align` so the heading and intro respect Left/Center; alignment classes and public CSS.

3.0.3 | 2026-05-08
* Add public module documentation page, featured image, and GitHub Actions sync workflow for the Digifox documentation site.

3.0.2 | 2026-04-17
* Fix: Prevent missing Contact icons when file-based SVG assets are unavailable by falling back to built-in SVG paths (so the icon stack never renders “background only”)

3.0.1 | 2026-01-28
* Fix: Contact SVG icons (phone, mobile, email, location) now load on new installs when only plugins/theme are copied. Icons are bundled in the plugin (`svg/plain-contact/`) so the block no longer depends on project `resources/svg-fa/plain-contact/`.
* Update: SVG lookup now checks the active theme first (`assets/svg-fa/plain-contact`, `assets/svg-fa/plain-social`). Use the digifox theme to keep all icon assets in one place.

3.0 | 2026-01-28
* Cleanup: Removed legacy comments and unused assets.
* Update: Added TikTok social link support.
* Improvement: Sanitised output and refreshed dynamic styles.

2.4 | 2023-10-19
* Fix broken the scroll when menu value is more than one word, thus includes a space.

2.3 | 2023-10-15
* Fix: Missing colon in email link

2.2 | 2023-07-31
* New: Upadte Access Token

2.1 | 2023-04-14
* New: Create "under construction" setup option..

2.0 | 2023-03-01
* First major rebuild
* Remove built-in demo
* Updated column selection interface
* Convert slug
