---
title: Cinema - Changelog
post_excerpt: Cinema module for Digifox One Page. Video lightbox, poster thumbnails, title overlay.
taxonomy:
    category: changelog
    post_tag: changelog

---

3.0.1.3 | 2026-04-20
* (Placeholder — replace or remove before release.)

3.0.1.2 | 2026-04-20
* (Placeholder — replace or remove before release.)

3.0.1.1 | 2026-04-20
* Add `cinema-module.md` (subscriber-facing module copy for documentation).
* Add GitHub Action `sync-module.yml` to copy `cinema-module.md` to `DIGIFOX-documentation` / `module` on push.

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
