---
title: Notice Module
post_excerpt: Show a dismissible announcement or promotional message above the website header.
taxonomy:
    category: module
    post_tag: module
custom_fields:
    module_version: 1.0.1
    module_updated: "19 July 2026"
---

### Overview

The Notice module adds a full-width message above the website header. Use it for demo-site reminders, opening hours, promotions, service alerts, or other information visitors should see immediately.

The notice can include a call-to-action link and a close button. When a visitor closes it, a cookie controls how long it stays hidden. Updating the Notice settings resets that cookie so the revised message is shown again.

### Content Fields

**Message**  
The announcement displayed in the notice.

**Button**  
Optional call-to-action label.

**Website Link**  
Destination for the call-to-action.

**Open in New Tab**  
Opens the call-to-action destination in a separate browser tab.

### Settings Fields

**Active**  
Shows or hides the Notice module.

**Order**  
Controls where Notice appears in the WordPress module menu. The public notice always displays above the website header.

**Hide After Closing**  
Number of days the notice remains hidden after a visitor closes it. A value of `0` hides it until the Notice settings are updated.

**Close Button**  
Allows visitors to dismiss the notice.

**Background Colour**, **Text Colour**, **Accent Colour**  
Controls the notice background, text, bottom border, and call-to-action colour.

**Text Align**  
Aligns the notice content left, centre, or right.

### Preview Helpers

Add `?digifox_notice_force=1` to preview the notice even when its dismissal cookie exists. Add `?digifox_notice_clear=1` to clear the current dismissal cookie.
