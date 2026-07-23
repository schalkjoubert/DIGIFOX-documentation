---
title: Cinema - Changelog
post_excerpt: Cinema module for Digifox One Page. Video lightbox, poster thumbnails, title overlay.
featured_image: _images/cinema-module.jpg
taxonomy:
    category: changelog
    post_tag: changelog

---
3.0.1.5.8 | 2026-07-15
* Feature | Card title and subtitle allow intentional line breaks via `<br>` (`wp_kses`)

3.0.1.5.7 | 2026-06-12
* Fix | YouTube auto posters: when maxresdefault is unavailable YouTube returns a tiny placeholder (not a 404), so posters now fall back to mqdefault on load if the image is narrower than 320px, as well as on error

3.0.1.5.6 | 2026-06-14
* Update | Client updates install from trimmed GitHub release zip (excludes `.md`, `.github`, `_images`, `.gitignore`)



3.0.2 | 2026-05-08
* Add public module documentation page, featured image, and GitHub Actions sync workflow for the Digifox documentation site.

3.0.1 | 2026-04-19
* Image crop (Natural / 4:3 / 1:1) applies to video poster cards as well as image-only cards; fixed ratios use `object-fit: cover` with poster area filling the frame (including absolute-filled lightbox trigger for YouTube/Vimeo thumbs).
* Dynamic styles: video posters no longer inherit “natural” contain rules that caused letterboxing; natural mode uses auto aspect on video posters with contain on the thumb only when appropriate.
* YouTube auto posters: prefer `maxresdefault.jpg`, fallback `mqdefault.jpg` on load error (`includes/cinema-helpers.php`); avoid `hqdefault` bitmaps that often embed black bars.

3.0 | 2026-01-28
* Video lightbox only: all videos open in lightbox (no inline embeds)
* Removed cinema_artwork, cinema_icon, cinema_button and all link/button fields and code
* Poster: cinema_image when set; otherwise YouTube/Vimeo thumbnail when no image
* Title overlay on video poster (above play icon); title hidden below for video items
* Play icon triangle uses setup_icon color (style-dynamic)
* Removed unused AJAX oEmbed endpoint and related hooks
* Security: sanitize_hex_color for arrow/icon colors; escaped outputs; hardened style-dynamic numeric values
* Cleanup: removed style-dynamic-x.php (legacy); cache-busted assets; no jQuery dependency
* Changelog and version set to 3.0
