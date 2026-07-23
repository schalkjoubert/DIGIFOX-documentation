---
title: Contact - Changelog
post_excerpt: New major release. We removed the built-in demo feature in favour of speed and stability en user experience. Addressed minor bug fixes and enhanced the UI for the column selection
featured_image: _images/contact-module.jpg
taxonomy:
    category: changelog
    post_tag: changelog

---
3.0.10 | 2026-07-21
* Fix | Contact icon grid column count is calculated live on each page load (inline CSS), so 4 items spread correctly after a plugin update without re-saving Contact

3.0.9 | 2026-07-21
* Fix | Contact Intro (and other textareas) render Enter line breaks as real HTML `<br>`, not visible `&lt;br /&gt;` text
* Fix | Contact Custom Style is printed inline on the front end so icon colour rules (e.g. `.digifox-icon-foreground`) reliably override the default white glyph colour

3.0.8 | 2026-07-01
* Feature | Optional **header CTA button** in the main navigation (`contact_button`, `contact_link_module` ACF in theme; `nav_contact_cta()` on `digifox_nav_cta` hook in `digifox-contact.php`, `includes/contact-helpers.php`)
* Update | CTA scrolls to the selected active module anchor (defaults to Contact when the chosen module is inactive)

3.0.7 | 2026-06-16
* Fix | Phone, mobile, WhatsApp, and email label textareas render `<br>` line breaks on the front end (`includes/contact-helpers.php`, `public/partials/digifox-contact-display.php`)

3.0.6 | 2026-06-14
* Update | Client updates install from trimmed GitHub release zip (excludes `.md`, `.github`, `_images`, `.gitignore`)



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
