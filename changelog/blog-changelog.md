---
title: Blog - Changelog
post_excerpt: Blog module for Digifox One Page (pulls default WordPress Posts).
featured_image: _images/blog-module.jpg
taxonomy:
    category: changelog
    post_tag: changelog

---
3.0.9 | 2026-07-22
* Fix | **Padding** applies to card text (`.item-txt`) like Service/Product, not the outer grid (`public/css/digifox-blog.css`, `public/partials/digifox-blog-display.php`)

3.0.8 | 2026-07-22
* Fix | **Excerpt** Yes/No and **Meta** Top/Bottom/None now applied on module cards (`public/partials/digifox-blog-display.php`)

3.0.7 | 2026-07-22
* Fix | Landscape card images use natural height (`height: auto`) instead of stretching to match the text column (`public/css/digifox-blog.css`)

3.0.6 | 2026-07-22
* Fix | Layout = Landscape places image and text side-by-side from 480px up; stays portrait stacked on small mobile (`public/partials/digifox-blog-display.php`, `public/css/digifox-blog.css`)

3.0.5 | 2026-07-22
* Fix | Card **Border** and **Background** settings now apply (were unused); Custom Style also wired via inline CSS (`public/inc/style-dynamic.php`)

3.0.4 | 2026-07-18
* Feature | When the Blog plugin is active, Editors can use the standard WordPress Posts menu (All Posts, Add New, Categories and Tags)
* Feature | Posts list notice explains that articles feed the Digifox Blog module, with links to Blog settings and Add New Post

3.0.3 | 2026-06-25
* Fix | Front-page module and nav order respect `blog_setting_order` (was hardcoded to priority 999)

3.0.2 | 2026-06-14
* Update | Client updates install from trimmed GitHub release zip (excludes `.md`, `.github`, `_images`, `.gitignore`)



3.0.2 | 2026-05-08
* Add public module documentation page, featured image, and GitHub Actions sync workflow for the Digifox documentation site.

3.0.1 | 2026-04-29
* Update | Add `blog_setting_card_radius` override (-1 inherits theme), improve slider gap handling, and align card typography/layout for grid/slider + single post support (excerpt/meta toggles; crop + radius inheritance)

3.0.0 | 2026-04-28
* New | Rebuild Blog module from scratch: grid/slider display pulling WordPress Posts
