---
title: Product - Changelog
post_excerpt: Product module for Digifox One Page. Icon and image artwork, optional buttons and links.
taxonomy:
    category: changelog
    post_tag: changelog

---

3.0.5.3 | 2026-04-25
* Fix | Use theme module-link resolver (no dependency on Banner plugin)

3.0.4 | 2026-04-06
* Fix: When product_setting_text_align is center, icon and image artwork align to the center as well (style-dynamic); left alignment keeps artwork left-aligned.
* Bump version so live sites detect updates after repo reconnection

3.0.3 | 2026-01-28
* New: Display product_price in slider and grid (ACF sub field product_price)
* Cleanup: Remove stray blank lines in display template

3.0.2 | 2026-01-28
* Reverted: Remove default/fallback product content; module shows nothing when product_content is empty (use Demo Importer or add content in WP admin)

3.0.1 | 2026-01-28
* New: Default content when no products are added: two placeholder products with title and subtitle (Consulting / Support) so the module displays something until content is added in WordPress admin

3.0 | 2026-01-28
* Removed unused style-dynamic-x.php (legacy duplicate)
* Security: sanitize_hex_color for slider arrow (setup_arrow); escape file URL at output
* style-dynamic.php: hardened numeric values (grid column 1–5, gap 0–40, padding 0–10); docblock
* Changelog: version order fixed; typo fixes (selction → selection, Bufg → bug, sevices → products)
* GH_UPDATE_TOKEN: only set authentication when constant is defined (align with Cinema)
* Version 3.0 set in plugin header and constant

2.0 | 2023-03-01
* First major rebuild
* Remove built-in demo
* Updated column selection interface
* Convert slug

2.1 | 2023-03-22
* Fix: Remove hardcoded heading for testing

2.2 | 2023-03-22
* Codespace: Update master to main branch

2.3 | 2023-03-29
* Feature: Add option to scroll to contact module

2.3.1 | 2023-03-30
* Fix: Typo on custom field for grid gap

2.3.2 | 2023-03-30
* Fix: Minor bug fix

2.3.3 | 2023-03-30
* Feature: Add scroll option to contact module
* Fix: Smooth scroll

2.4 | 2023-04-14
* New: Create "under construction" setup option.

2.4.1 | 2023-04-27
* New: Add Subtitle field for individual products

2.4.2 | 2023-10-19
* Fix: Broken scroll when menu value is more than one word

2.4.3 | 2023-10-20
* Fix: Same issue but related to the optional CTA

2.4.5 | 2024-02-07
* Feature: Add custom style section
