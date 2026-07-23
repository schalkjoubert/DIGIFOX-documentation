---
title: Counter - Changelog
post_excerpt: New major release. We removed the built-in demo feature in favour of speed and stability en user experience. Addressed minor bug fixes and enhanced the UI for the column selection
featured_image: _images/counter-module.jpg
taxonomy:
    category: changelog
    post_tag: changelog

---
3.0.5 | 2026-07-15
* Feature | Card title allows intentional line breaks via `<br>` (`wp_kses`)

3.0.4 | 2026-07-03
* Feature | Content ACF: optional **Suffix** text after the counter value (`counter_suffix` in `acf-json/group_601d960c252d1.json`)
* Update | **Number** is optional — cards can show title, description, and suffix without an animated count (`public/partials/digifox-counter-display.php`)
* Update | Counter value markup: `.counter-value` wraps animated number and suffix (`.counter-suffix`) (`public/css/digifox-counter-public.css`)

3.0.3 | 2026-07-02
* Feature | Settings ACF: grid layout controls — **Columns**, **Gap**, **Padding**, **Card Max Width**, **Image Radius**, **Image Crop**, **Layout**, **Text Align**, **Equal Heights** (`acf-json/group_601d960487080.json` in theme)
* Update | Dynamic grid styles ported from Service module (`public/inc/style-dynamic.php`, `public/css/digifox-counter-public.css`)
* Update | Equal heights toggle via `counter_setting_height` (`public/js/digifox-counter-public.js`, `public/class-digifox-counter-public.php`)
* Update | Legacy fallback when **Columns** is unset: desktop column count matches the number of counter cards (capped at 5) via `digifox_counter_grid_columns()` (`digifox-counter.php`)

3.0.2 | 2026-06-14
* Update | Client updates install from trimmed GitHub release zip (excludes `.md`, `.github`, `_images`, `.gitignore`)



3.0.1 | 2026-05-08
* Add public module documentation page, featured image, and GitHub Actions sync workflow for the Digifox documentation site.

3.0 | 2026-01-29
* Cleanup: Removed legacy templates and inline scripts.
* Update: Kept Font Awesome icons with conditional loading.
* Improvement: Refreshed template output and assets.

2.4 | 2023-10-19
* Fix broken the scroll when menu value is more than one word, thus includes a space.

2.3 | 2023-07-31
* New: Upadte Access Token

2.2 | 2023-04-14
* New: Create "under construction" setup option.

2.1 | 2023-03-14
* Fix: Create universal containers for head, heart and feet

2.0 | 2023-03-01
* First major rebuild
* Remove built-in demo
* Updated column selction interface
* Convert slug.
