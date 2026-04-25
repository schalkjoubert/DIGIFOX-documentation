---
title: Digifox - Changelog
post_status: publish
post_excerpt: Update description of changelog feed in dashboard.
taxonomy:
    category: changelog
    post_tag: theme-changelog

---

3.0.4-beta.7 | 2026-04-25
* Feature | Centralize “link to module” registry + stable-key resolver in theme so module links work even if Banner plugin is inactive (`assets/functions/function-module-links.php`)

3.0.4-beta.6 | 2026-04-25
* Fix | Prevent dev-generated CSS/sourcemaps from being committed (ignore `assets/css/style-dynamic.css` and `*.map`)

3.0.4-beta.5 | 2026-04-24
* test*

3.0.4-beta.4 | 2026-04-19
* test*

3.0.4-beta.2 | 2026-04-17
* Update | WordPress login branding now always uses Digifox logo (`assets/img/digifox-logo-login.png`) instead of the site’s Customizer logo
* Feature | Hide default login URL: login is now served at `/login`, and direct requests to `wp-login.php` or logged-out `/wp-admin` redirect to `/login` (`assets/functions/function-login.php`)

3.0.4-beta.1 | 2026-04-13
* Chore | Reorder changelog entries so newest versions appear first
* Chore | Start 3.0 beta version line

2.3.6.13 | 2026-04-04
* Update | Theme Font Awesome for module icons now loads **FA Free 7.x** from the official CDN (`use.fontawesome.com/.../css/all.css`, default version `7.0.0`) instead of bundled FA 5.2 under `assets/vendor/fontawesome/`. Filters: `digifox_fontawesome_css_url` (full URL), `digifox_fontawesome_cdn_version`, `digifox_fontawesome_style_ver`. Self-host the old bundle by returning the theme `all.css` URL via `digifox_fontawesome_css_url`.

2.3.6.12 | 2026-04-04
* Fix | Enqueue bundled Font Awesome when Product module is active and any product row uses icon artwork with a Font Awesome icon, so Product icons work without Service or Counter (`function-assets.php` — `digifox_should_enqueue_fontawesome()`).

2.3.6.11 | 2026-01-28
* New | SVG icon resources moved into theme: `assets/svg-fa/plain-contact/` (phone, mobile, email, location, whatsapp) and `assets/svg-fa/plain-social/` (Facebook, X/Twitter, Instagram, LinkedIn, TikTok, YouTube). Contact and Team plugins now look in the theme first so copying theme + plugins to a new install shows all icons without a project-level `resources/` folder.

2.3.6.10 | 2026-01-28
* Fix | Admin menu order: map slug `digifox-slider` to slideshow option prefix so Slideshow appears in correct sidebar position (`slideshow_setting_order` / `slideshow_setting_active`)

2.3.6.9 | 2025-07-29
* Feature | Add File Download to Hero Module

2.3.6.8 | 2025-04-16
* Feature | Add new Hero module

2.3.6.7.3 | 2024-06-04
* Fix | Add cutom module scroll option to slider and video

2.3.6.7.2 | 2024-06-04
* Update | Add cutom module scroll option to slider and video

2.3.6.7.1 | 2024-06-04
* Update | ACF subtitle field in Propjects Overview

2.3.6.6 | 2024-06-04
* Update | ACF subtitle field in Products 

2.3.6.5 | 2024-06-04
* Update | ACF pricing field in Products

2.3.6.4 | 2024-02-14
* Update | Conditionall diplay ACF update in functions.php

2.3.6.3 | 2024-02-12
* Feature | Update Style custom field | Projects

2.3.6.2 | 2024-02-12
* Feature | Update more custom fields | Video

2.3.6.1 | 2024-02-07
* Feature | Add custom style section | Video

2.3.6 | 2024-02-07
* Feature | Add custom style section | About Projects, Products, Services

2.3.5.10 | 2024-01-21
* Fix: Remove JS already added to header.php and move max-width to media quary in css.

2.3.5.9 | 2024-01-21
* Fix: javascript to make sure logo is nod wider than menu

2.3.5.8 | 2024-01-20
* Fix: Changed the max-width for logo to screensize minus menu toggle width - _style-header.scss

2.3.5.7 | 2024-01-15
* New: Add option to Delay Header. Useful when the logo is included in a slider or video.
* Feature: Build in support for custom styles

2.3.5.6 | 2024-01-13
* New: Add DigiPlus function support - functions.php
* New: Add DigiPlus navigation support - header.php

2.3.5.4 | 2023-10-19
* New: Add option under Setup to add a bottom border to the header

2.3.5.3 | 2023-10-19
* Fix: ACF sync - fix website link for Banner Module

2.3.5.2 | 2023-10-19
* Fix: ACF sync - fix email and website link for Services Module

2.3.5.1 | 2023-09-06
* New: ACF sync - add download option to Products Module

2.3.5 | 2023-09-06
* New: Add Email & Website link options to Team Module

2.3.4 | 2023-07-31
* Update: Added JS & PHP to handle screen size detection. Used in  particular for the responsive display of gallery thumbnails.

2.3.3 | 2023-07-14
* Update: Update to sync new custom field created for the slider module.

2.3.2 | 2023-07-09
* Update: Update description of changelog feed in dashboard

2.3.1.3 | 2023-04-27
* New: Add Subtitle field for individual sevices

2.3.1 | 2023-04-27
* Fix: Slow loading of header. Move wp_head above nav.

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
