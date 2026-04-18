---
title: Cinema - Changelog
post_excerpt: Cinema module for Digifox One Page. Video lightbox, poster thumbnails, title overlay.
taxonomy:
    category: changelog
    post_tag: changelog

---

3.0.0.2 | 2026-04-18
* Test Repo Push

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
