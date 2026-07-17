---
title: Digifox - Changelog
post_status: publish
post_excerpt: Update description of changelog feed in dashboard.
taxonomy:
    category: changelog
    post_tag: theme-changelog

---
3.0.4-beta.44 | 2026-07-17
* Fix | **Digifox Demos** admin menu no longer sorted as an inactive module — appears after Setup / Entries, above Active or Inactive Modules headings (`digifox_admin_utility_menu_slugs()` in `function-setup.php`)

3.0.4-beta.43 | 2026-07-17
* Update | Admin menu order: **Digifox Demos** appears after Setup / Entries when Demo Importer plugin is active (`digifox-demo-importer`)

3.0.4-beta.42 | 2026-07-16
* Fix | Module Custom Style: bare properties, `#module-id`, `&`, and `{ … }` correctly apply to the module root (e.g. custom background), while nested selectors like `.box` stay scoped inside the module (`digifox_scope_module_custom_css` in `assets/functions/function-helpers.php`)

3.0.4-beta.41 | 2026-07-15
* Feature | Card module title fields: ACF instructions document optional `<br>` line breaks (Services, Products, Projects, Cinema, Counter, Team, Review, Question)
* Update | Card title fields remain optional / not required where previously adjusted in ACF JSON

3.0.4-beta.40 | 2026-06-12
* Fix | **Delay Header**: header fully hidden off-screen on home until scroll (`transform: translateY(-100%)`); fixes mobile peek when header is taller than the old fixed `-50px` offset (`assets/inc/style-dynamic.php`, `assets/css/style-dynamic.css`)
* Fix | Mobile full-screen Hero: content vertically centred below the measured header (`assets/css/style.css`, hero plugin CSS)
* Update | Slideshow Image Crop ACF note: 4:3 / 16:9 kept on mobile; slide grows taller when content needs more height (`acf-json/group_5e53c5b1cb6ec.json`)

3.0.4-beta.36 | 2026-07-03
* Fix | Mobile full-screen Slideshow/Hero header clearance: left-aligned slide content no longer vertically centres under the logo; selectors use module `data-*-viewport` attributes (`assets/css/style.css`, `assets/scss/_style-header.scss`)

3.0.4-beta.35 | 2026-07-03
* Fix | Mobile full-screen Hero/Slideshow: text content clears the fixed header when **Delay Header** is No — padding-top matches `--digifox-header-large` (70px on ≤480px, 120px otherwise); applies to Slideshow 4:3/16:9 crop and Hero (`assets/css/style.css`, `assets/scss/_style-header.scss`)
* Feature | Body class `has-header-delay` when Setup → Delay Header is Yes (`assets/functions/function-setup.php`)

3.0.4-beta.34 | 2026-07-03
* Feature | Counter | Content ACF: optional **Suffix** after the counter value; **Number** optional (`counter_suffix`, `counter_number` in `acf-json/group_601d960c252d1.json`)
* Feature | Counter | Settings ACF: grid layout controls — **Columns**, **Gap**, **Padding**, **Card Max Width**, **Image Radius**, **Image Crop**, **Layout**, **Text Align**, **Equal Heights** (`acf-json/group_601d960487080.json`)

3.0.4-beta.33 | 2026-07-02
* Feature | One-page nav scroll spy marks the active section (`is-current` on `#menu li`; `assets/js/digifox-menu.js`, enqueued from `assets/functions/function-assets.php` on the front page when menu underline is enabled)
* Feature | Setup ACF: **Show Home in Menu** (`setup_setting_header_home`; `digifox_show_header_home_menu()` in `assets/functions/function-setup.php`, `header.php`)
* Feature | Setup ACF: **Menu underline** (`setup_setting_header_menu_underline`; `digifox_header_menu_underline_enabled()`, body class `has-header-menu-underline` in `assets/functions/function-setup.php`; `acf-json/group_5d5be147db736.json`)
* Update | Desktop header nav: active and hover underline via border-bottom (CTA excluded); CTA padding `5px 8px`; underline bottom-aligned with CTA (`assets/css/style.css`)

3.0.4-beta.32 | 2026-07-01
* Feature | Slideshow | Content ACF: per-slide button **Style** / **Colour** for buttons 1 and 2; slide **Title** and **Intro** support basic HTML (`acf-json/group_5e53c5cff26d0.json`)
* Feature | Slideshow | Settings ACF: **Content alignment** (`slideshow_setting_content_align`) (`acf-json/group_5e53c5b1cb6ec.json`)

3.0.4-beta.31 | 2026-07-01
* Feature | Shared **module button** variants for CTAs: fill / outline × default / white / black (`assets/functions/function-buttons.php`, `assets/css/module-buttons.css`, enqueued from `assets/functions/function-assets.php`)
* Feature | Hero | Content ACF: `hero_button_style`, `hero_button_colour`, `hero_button_2_style`, `hero_button_2_colour` (`acf-json/group_669763fe67215.json`)
* Feature | Hero | Settings ACF: **Content alignment** (`hero_setting_content_align`) and **Header offset** label/instructions (`acf-json/group_6697640dc1d5a.json`)
* Update | Outline + default buttons use Setup **border** colour for text (not button text colour) (`assets/css/module-buttons.css`)
* Update | Fill white / fill black hover inverts background and text; border keeps its colour; 2px border; subtle lift on hover (`assets/css/module-buttons.css`)

3.0.4-beta.30 | 2026-07-01
* Feature | **Header offset** support for Hero and Slideshow: when the first module uses full screen (`hero_setting_viewport` / `slideshow_setting_viewport` = No), `.site-content-contain` starts at `top: 0` so content sits under the fixed header (`has-first-module-full-viewport` body class, `assets/css/style.css`, `assets/functions/function-setup.php`)
* Update | ACF **Header offset** field labels and instructions on Hero and Slideshow settings (`acf-json/group_6697640dc1d5a.json`, `acf-json/group_5e53c5b1cb6ec.json`)
* Update | Header offset field hidden in Hero/Slideshow admin when Setup → Delay Header is Yes (`acf/prepare_field` in `assets/functions/function-setup.php`)

3.0.4-beta.29 | 2026-06-28
* Fix | `#menu` background colour applies on mobile hamburger dropdown only (≤1079px), so desktop nav shows header colour and texture consistently (`assets/inc/style-dynamic.php`)

3.0.4-beta.28 | 2026-06-28
* Fix | Background Texture no longer overrides header `position: fixed`, so delayed header behaviour works again on the home page (`assets/inc/style-dynamic.php`)

3.0.4-beta.27 | 2026-06-28
* Feature | Setup **Background Texture** (`setup_texture`): optional seamless pattern tiled over module, header and footer background colours, underneath text and content (`acf-json/group_5d5be147db736.json`, `assets/inc/style-dynamic.php`, `assets/functions/function-setup.php`)

3.0.4-beta.26 | 2026-06-16
* Update | Contact ACF: `contact_phone_text`, `contact_mobile_text`, `contact_whatsapp_text`, and `contact_email_text` are textareas with Automatically add `<br>` (`acf-json/group_5e9825d07ca19.json`)

3.0.4-beta.25 | 2026-06-16
* Fix | Dashboard Notices and News widgets are hidden when the digifox.media category feed has no published posts (avoids empty widgets and “feed is down” errors when posts are draft-only) (`assets/functions/function-widget.php`)

3.0.4-beta.24 | 2026-06-15
* Feature | New branded login screen for all sites: full-viewport background video or image, two-column card (Digifox logo + welcome copy, login form), served at `/login` (`assets/functions/function-login.php`, `assets/css/login-screen.css`)
* Feature | Login background defaults: `assets/img/login-background.mp4`, or `assets/img/login-background.jpg` when no video; optional overrides via Setup (`setup_login_video`, `setup_login_video_poster`, `setup_login_signup_url`, `setup_login_signup_text` in `acf-json/`)
* Update | Login screen always shows Digifox logo (`assets/img/digifox-logo-login.png`); welcome text uses site title and introduction from Setup
* Update | Removed legacy black login styles from `function-setup.php`

3.0.4-beta.23 | 2026-06-14
* Fix | Include `acf-json/` in GitHub release deploy zip so ACF field groups load on client sites after theme update

3.0.4-beta.22 | 2026-06-14
* Update | Further Slideshow ACF field group sync (`acf-json/`)

3.0.4-beta.21 | 2026-06-14
* Update | ACF JSON and admin menu mapping for Slideshow rename (`digifox-slider` → `digifox-slideshow` in `acf-json/`, `function-setup.php`)

3.0.4-beta.20 | 2026-06-14
* Update | Client updates install from trimmed GitHub release zip (excludes `.md`, `.github`, `_images`, `.gitignore`)



3.0.4-beta.19 | 2026-06-12
* Feature | Add `product_setting_card_width`, `service_setting_card_width`, and `project_setting_card_width` ACF range fields (300–600px, portrait layout) (`acf-json/`)

3.0.4-beta.18 | 2026-05-06
* Fix | Improve Facebook/OG image reliability by adding support for `og:image:type`, `og:image:width`, and `og:image:height` when the OG image is a WordPress attachment (`assets/functions/function-og.php`)

3.0.4-beta.17 | 2026-05-06
* Fix | Output canonical URL for Open Graph (`og:url`) and add `<link rel="canonical">` to prevent Facebook preview inconsistencies between `www` and non-`www` host variants (`assets/functions/function-og.php`)

3.0.4-beta.16 | 2026-04-29
* Update | Remove global heading `text-align: center` from `_style-general.scss` so heading alignment is controlled by modules and WYSIWYG editor content

3.0.4-beta.15 | 2026-04-29
* Fix | Prevent global centered headings from affecting post WYSIWYG content; left-align headings and add list padding inside single post content (`assets/scss/_style-single-post.scss`)

3.0.4-beta.14 | 2026-04-29
* Fix | Prevent global `header { ... }` styles from affecting post `<header class="entry-header">` by scoping header CSS to `.header` (SCSS source updated)
* Feature | Improve single post layout (1/3 featured image + 2/3 summary; content full width) and keep it stable across SCSS recompiles (`assets/scss/_style-single-post.scss`)
* Feature | Single post featured image respects Blog settings for crop (`blog_setting_image_crop`) and radius (`blog_setting_image_radius`, -1 inherits `setup_image_radius`)
* Feature | Add single post excerpt + meta positioning toggles (`blog_setting_excerpt`, `blog_setting_meta`) and only show “Updated on …” when modified date is at least one day after publish

3.0.4-beta.13 | 2026-04-27
* Fix | Track “Book a Visit” popup opens reliably by observing Digifox Popup open state (MutationObserver) instead of delegated click (blocked by popup plugin’s capture + stopImmediatePropagation) (`assets/js/site-custom.js`)

3.0.4-beta.12 | 2026-04-27
* Feature | Add optional site-specific script loader for `assets/js/site-custom.js` (enqueued only if present; footer; after jQuery; cache-busted via `filemtime()`) (`assets/functions/_function-core-custom-scripts.php`)

3.0.4-beta.11 | 2026-04-26
* Fix | Remove duplicate WordPress core SEO output (disable core canonical tag + core robots max-image-preview) so Digifox Core SEO remains the single source (`assets/functions/_function-core-seo.php`)

3.0.4-beta.10 | 2026-04-26
* Feature | Add built-in one-page SEO output (meta description, robots, canonical, Open Graph, Twitter, JSON-LD WebSite + Organization) + optional GA4/GTM tracking + simple `/sitemap.xml` endpoint driven by Setup ACF options (`assets/functions/_function-core-seo.php`, `functions.php`, `header.php`, `front-page.php`)

3.0.4-beta.9 | 2026-04-26
* Fix | Make `/login` work without WPS Hide Login by routing login requests even if rewrite rules weren’t flushed, and prevent redirect loops (`assets/functions/function-login.php`, `assets/functions/function-setup.php`)

3.0.4-beta.8 | 2026-04-25
* Feature | Add Setup fields for GTM/GA snippets and output them in `header.php` (`setup_gtm_head`, `setup_gtm_body`, `setup_ga`)

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
