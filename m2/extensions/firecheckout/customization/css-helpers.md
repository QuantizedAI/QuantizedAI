---
layout: default
title: CSS Helpers
description: Various CSS classes to customize firecheckout page
category: Firecheckout
---

# CSS Helpers

> This feature supported since v.1.12.0

* TOC
{:toc}

### Grid system

CSS class                   | Description
----------------------------|--------------------------
`fc-col-1` .. `fc-col-12`   | Helps to resize the field. Use just like any other 12-columns grid system
`fc-hidden`                 | Hides content on all screen sizes
**Using together with container size selectors** |
`fc-size-l:fc-col-4`        | `fc-col-4` will work, when parent container has `fc-size-l` class

### Container size selectors

These classes are added automatically by firecheckout to the main checkout steps.

Please note, that they do not describe screen size like media query, but they
actually indicate how large the container is.

CSS class   | Description
------------|-----------
`fc-size-l` | Added to the section, when its width > 550px
`fc-size-m` | Added to the section, when its width > 420px
`fc-size-s` | Added to the section, when its width > 275px
`fc-size-xs`| Added to the section, when its width > 0px

##### Next up
{:.no_toc}

 -  [Back to customization page](/m2/extensions/firecheckout/customization/)
 -  [Back to home](/m2/extensions/firecheckout)
