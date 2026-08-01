---
title: Digifox Demo Importer - Changelog
taxonomy:
    category: changelog
    post_tag: changelog
---
1.3.27 | 2026-07-30
* Add | Psychologist demo (`demos/psychologist.json`) — Dr Amara Naidoo; calm teal palette

1.3.26 | 2026-07-27
* Update | Project download filename pattern is now `project-01-file.pdf` (was `project-file-01.pdf`)

1.3.25 | 2026-07-27
* Feature | Project card download files from demo assets: `project-01-file.pdf` → card 1 `project_link_file` (sets link type to **file**)

1.3.24 | 2026-07-23
* Add | Bread & Brew bakery demo (`demos/bread-and-brew.json`) — artisan sourdough + coffee shop; warm wheat / espresso palette

1.3.23 | 2026-07-23
* Feature | GitHub updates via plugin-update-checker (release zip `digifox-demo-importer.zip`); build-release + changelog sync workflows

1.3.22 | 2026-07-23
* Feature | Setup **Background Texture** from demo assets: `setup-pattern.png` → `setup_texture` (`digifox-demo-importer.php`)

1.3.21 | 2026-07-19
* Update | Demo slugs now correspond to their labels: `auto-workshop` and `solar-installer`; JSON filenames and asset folders use the same slugs

1.3.20 | 2026-07-19
* Fix | Gravity Form remap only runs when a form ID is already set; empty popup/subscribe form fields stay empty (e.g. Auto Workshop popup without a form)

1.3.19 | 2026-07-19
* Update | Export filename now matches the industry slug directly (for example, `solar` downloads as `solar.json`) so it is ready for the demos folder without renaming

1.3.18 | 2026-07-19
* Update | Load demo uses industry radio buttons (nothing selected by default) with industry-type labels: Accountant, Restaurant, Auto Workshop, Solar Installer

1.3.17 | 2026-07-19
* Fix | Export creates portable JSON automatically: clears top-level and nested ACF image, gallery and file values while preserving Cinema video URLs and `_posts` featured-image names
* Update | Manual cleanup of source-site attachment IDs and upload URLs is no longer required

1.3.16 | 2026-07-19
* Feature | All bundled demos activate the new Digifox Notice module with a dismissible demo-site message and Contact Digifox call-to-action

1.3.15 | 2026-07-18
* Fix | Cinema: export/import oEmbed as video URLs (not iframe HTML) so posters and lightbox work after Load demo
* Fix | Gallery: generate Digifox intermediate sizes (`digifox_gallery_thumb` 4:3 crop) on demo upload so thumbs stay uniform
* Fix | Popup/Subscribe: if exported Gravity Form ID is missing on this site, remap to the first available form

1.3.14 | 2026-07-18
* Fix | Demo export/reset now includes the theme **Setup** field group (title is `Setup`, not `Digifox` / `| Settings`) — so `setup_site_title`, logo, colours, etc. are included

1.3.13 | 2026-07-18
* Feature | Blog posts in demos: Export includes `_posts` (slug, title, excerpt, content, date, featured); Load creates/updates posts and sets featured images from `blog-01.jpg` etc.; tagged with `_digifox_demo` so Load/Reset can replace them cleanly when switching industries

1.3.12 | 2026-07-17
* Feature | Hero video assets: `hero-video.mp4` (also `.webm` / `.mov`) uploads to `hero_video` and sets `hero_type` to video; optional `hero-video-placeholder.jpg` for poster

1.3.11 | 2026-07-17
* Fix | After Load demo (and Reset): regenerate theme + module `style-dynamic.css`, sync logo/favicon/site title — fixes broken padding/layout without saving each module manually
* Update | Demo dropdown only lists industries that have a readable `demos/{slug}.json` (Solar ready once `demos/solar.json` is added)

1.3.10 | 2026-07-17
* Fix | Demo import timeout on shared hosting: skip Imagick intermediate thumbnail generation during bulk upload; store lightweight attachment metadata only; extend import time limit to 300s

1.3.9 | 2026-07-17
* Update | **Digifox Demos** is a top-level admin menu (no longer under Settings)
* Update | Administrators and Editors can load and reset demos (`edit_posts` menu cap; export JSON remains administrators only)
* Add | `DIGIFOX_DEMO_IMPORTER_VERSION` constant for theme menu ordering

1.3.8 | 2026-06-28
* Add | Louw & Mason accountant demo (`demos/accountant.json`) — header `#394656` with cool light nav text; products use icons; banner/slideshow/project assets wired

1.3.7 | 2026-06-14
* Update | Client updates install from trimmed GitHub release zip (excludes `.md`, `.github`, `_images`, `.gitignore`)



1.0.0 | 2026-01-28
* Initial release
* Standalone plugin: Settings → Digifox Demos
* Restaurant demo: content for all 14 modules (About, Banner, Carousel, Cinema, Contact, Counter, Embed, Gallery, Hero, Review, Service, Slideshow, Subscribe, Team)
* Image/file fields left empty; add images in WP admin after import

1.1.0 | 2026-01-28
* Demo images: place images in demo-assets/{industry}/ named modulename-demo-01.jpg, etc.
* On import, images are uploaded to the Media Library and linked to the correct module fields (slideshow, hero, banner, service, counter, gallery, cinema, carousel, review, team)
* Optional hero logo: hero-logo.png (or hero-logo.jpg) in the same folder
* README documents naming convention and folder structure

1.2.0 | 2026-01-28
* Restaurant demo: Sardine branding (site title, primary #2b3bb6), Hero order 1, Gallery order 15, Embed skipped, sliders with at least one more card than columns, 4 counters with icons, 4 services (cuisines), 4 products (cocktails), 3 cinema cards (YouTube how-to), 4 reviews, 4 team, Carousel for wine farm logos
* Product module: added to demo (product_content, product-demo-NN images)
* Setup assets: setup-logo.png and setup-icon.png in demo-assets/restaurant/ → setup_logo and setup_favicon (theme logo and site icon)
* README: Product and setup-logo/setup-icon naming

1.2.1 | 2026-01-28
* Fix: Support short filenames (e.g. service-01.jpg, slideshow-01.jpg) in addition to service-demo-01.jpg so images in demo-assets/restaurant/ are found and linked
* File discovery: case-insensitive image extensions; scan directory once
* Admin notice after import shows how many images were linked; hint if 0 images found

1.3.0 | 2026-05-09
* Auto mechanic demo (`demos/auto-mechanic.json`): Precision Auto Care copy; Projects, Blog, Question, Popup modules included; primary palette #1a365d
* `demo-assets/auto-mechanic/placeholder.jpg`: single grey placeholder; on import, fills empty image fields only (named `module-demo-NN` files still win)
* Asset merge: `project-demo-NN` → Projects cards; `popup-demo-01` → popup image
* Export JSON: include field groups titled `Something | Settings` or `Something | Content` (theme modules), not only titles containing "Digifox"

1.3.1 | 2026-05-09
* Auto mechanic JSON regenerated from full solar site export: same field coverage (~370 keys) — slideshow slide CTAs (`button_1`, `link_module_1`, …), cinema/grid/contact/embed extras, review settings, etc.; mechanic-themed copy; attachment IDs and external image URLs cleared; `setup_*` + `subscribe_form` added for theme/options parity
* `bin/build-auto-mechanic-from-solar.php`: repeatable generator from a fresh export JSON

1.3.2 | 2026-05-09
* Numbered demo assets `01.jpg`, `02.jpg`, … in `demo-assets/{industry}/`: ingested as a pool and distributed to empty image fields after named files (`hero-01`, `team-01`, …) and before `placeholder.jpg`

1.3.3 | 2026-05-09
* Auto mechanic demo (`auto-mechanic.json`): Apex Auto Works, primary `#104267`; services remain icon-based; sliders tuned so card count exceeds visible columns (projects slider 2 columns / 3 cards, products slider 3 columns / 5 cards, cinema 2 columns / 4 items, services 4 columns / 5 cards; extra slideshow slide and fourth review); three restoration projects (Lotus Excel, Delahaye 135S, Bentley T-Series) with modal copy and Historic Vehicles links; fifth product card

1.3.4 | 2026-05-09
* Asset filenames `project-1-01.jpg`, `project-1-02.jpg`, `project-2-01.jpg`, …: row number matches project card order (1-based); second number is image sequence — first file is the card image, additional files populate `project_modal_images`
* Auto mechanic setup in JSON: `setup_header` / button bg `#104267`, header border and button border `#003966`, header/nav text `#cccccc`, delayed header on (`setup_setting_header_delay` `yes`); `demo-assets/auto-mechanic/hero-logo.png` and `setup-logo.png` for Apex branding on import

1.3.6 | 2026-05-10
* After a successful demo load, bump Digifox Popup’s cookie buster when the Popup plugin is active — same effect as saving Popup settings once, so auto-trigger popups are not blocked by an older dismiss cookie.

1.3.5 | 2026-05-10
* Settings → Digifox Demos: **Reset all demo data** clears ACF option values for every Digifox-related field group (same discovery rules as JSON export). Does not remove files from the Media Library; confirm dialog before running
