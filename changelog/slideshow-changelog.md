---
title: Slideshow - Changelog
post_excerpt: Header-aware height (100% viewport) and global slider script.
featured_image: _images/slideshow-module.jpg
taxonomy:
    category: changelog
    post_tag: changelog

---
3.0.9 | 2026-07-21
* Fix | Slide backgrounds used WordPress **large** (max ~1024px), so 1920×1080 uploads looked soft; now use **digifox_slideshow** (1920×1080 soft) with fallback to **full** (`public/partials/digifox-slideshow-display.php`, `digifox-slideshow.php`)

3.0.8 | 2026-06-12
* Fix | Mobile full-screen slides (**Header offset** = Full screen, **Delay Header** = No): two-row grid vertically centres content in the area below the measured header (`--digifox-header-offset` via JS); left-aligned slides included
* Fix | Mobile **Delay Header**: header fully hidden until scroll (`transform: translateY(-100%)` in theme dynamic CSS); slideshow at 100% height fills the viewport and centres content in the full slide
* Fix | Mobile 4:3 / 16:9: aspect ratio kept; slide `min-height` grows when content + header clearance need more height (no empty band below the slide)
* Update | Left-aligned slide content padding `3em` top/bottom; responsive title/intro typography on mobile (`public/css/digifox-slideshow-public.css`, `public/js/digifox-slideshow-height.js`)

3.0.7 | 2026-07-03
* Fix | Mobile full-screen slides (4:3 / 16:9): slide text clears the fixed header when **Header offset** is Full screen and **Delay Header** is No — uses `data-slideshow-viewport` / `data-slideshow-header-delay`; fixes left-aligned content that was still vertically centred (`public/css/digifox-slideshow-public.css`)

3.0.6 | 2026-07-01
* Feature | Slide **Title** and **Intro** support basic HTML (e.g. `<span class="yellow">highlight</span>`) via `wp_kses_post()` (`public/partials/digifox-slideshow-display.php`, `acf-json/group_5e53c5cff26d0.json`)
* Update | Intro field changed to textarea; maxlength removed on title and intro for HTML markup
* Update | Built-in `.yellow` highlight colour on slide content (`public/css/digifox-slideshow-public.css`)

3.0.5 | 2026-07-01
* Feature | Per-slide **Style** and **Colour** for CTA buttons 1 and 2: fill / outline and default / white / black (`acf-json/group_5e53c5cff26d0.json`, `public/partials/digifox-slideshow-display.php`)
* Feature | **Content alignment** setting: left-align slide text and buttons within the site container (`slideshow_setting_content_align`, `acf-json/group_5e53c5b1cb6ec.json`, `public/css/digifox-slideshow-public.css`)
* Update | Slide buttons use theme `digifox_module_button_class()` and shared `module-buttons` styles

3.0.4 | 2026-07-01
* Feature | **Header offset** setting (`slideshow_setting_viewport`): Below header vs Full screen — same behaviour as Hero; natural-crop height driven by JS for all percentages (`acf-json/group_5e53c5b1cb6ec.json`, `public/partials/digifox-slideshow-display.php`, `public/js/digifox-slideshow-height.js`, `public/inc/style-dynamic.php`)
* Update | Full screen mode adds `module-viewport-full` class; removed fixed `vh` height for natural crop in favour of header-aware JS

3.0.3 | 2026-06-14
* Update | Rename plugin identity from `digifox-slider` to `digifox-slideshow` (GitHub repo, updater slug, admin menu slug, text domain)

3.0.2 | 2026-06-14
* Update | Client updates install from trimmed GitHub release zip (excludes `.md`, `.github`, `_images`, `.gitignore`)
* Add | Public module documentation page, featured image, and GitHub Actions sync workflow for the Digifox documentation site

3.0.1 | 2026-04-25
* Fix | Use theme module-link resolver (no dependency on Banner plugin)

3.0.0 | 2026-01-28
* Rebuild: use theme global slider script (remove Slick)
* Rename module to Slideshow; ACF field names slider_* → slideshow_*
* Image crop: Natural / 4:3 / 16:9 (height % only when Natural)
* Header-aware height when crop Natural and height 100%:
  * Scenario 1: Order 1 + Header delay Yes → 100% browser height
  * Scenario 2: Order 1 + Header delay No → 100% browser height minus large header
  * Scenario 3: Order 2+ → 100% browser height minus small header
* Fix: Admin sidebar position now respects order setting (theme maps menu slug `digifox-slider` to `slideshow_setting_order` / `slideshow_setting_active`)

2.4.9 | 2024-06-04
* Fix: Add Scroll to custom module option

2.4.7 | 2024-01-15
* Fix: Move Delay header feature to global settings

2.4.6 | 2024-01-13
* Fix: Overlay background not showing up since introduction if "logo option"
* New: Add option to hide the Header initially wehn thge logo is included in the slide.

2.4.5 | 2023-10-20
* Fix same issue as 2.4.4. but related to the optional CTA

2.4.4 | 2023-10-19
* Fix: broken the scroll when menu value is more than one word, thus includes a space.

2.4.3 | 2023-07-31
* Update access token

2.4.1 | 2023-07-14
* New: We added a new feature. You can now add an small logo / icon above the title as an overlay.

2.3 | 2023-04-14
* New: Create "under construction" setup option.

2.2 | 2023-03-30
* Feature: Add scroll option to contact module
* Fix: Smooth scroll

2.1.4 | 2023-03-27
* Fix: Minto bug fix

2.1.3 | 2023-03-26
* Fix: Minto bug fix

2.1.2 | 2023-03-25
* Fix: Update Callt oaction colour values

2.1.1 | 2023-03-23
* Fix: Update Height Control

2.1 | 2023-03-22
* Fix: Remove hardcoded heading for testing.

2.0 | 2023-03-01
* First major rebuild
* Remove built-in demo
* Updated column selction interface
* Convert slug.
