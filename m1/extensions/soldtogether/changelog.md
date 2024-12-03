---
layout: default
title: Sold Together Changelog
description: Sold Together Changelog
keywords: sold together updates
category: Sold Together
---

# Changelog

### Version 1.5.2

 -  Fix 'product ID already exists' error on checkout success page.
 -  Improved caching for blocks of module.
 -  Respect "Reindex... via Cron" config options. Cron process ignored config settings in previous versions.

### Version 1.5.1

 -  Cron option works only on global level of config. So it is removed on other config levels.

### Version 1.5.0

 -  Added new option to reindex orders with specific statuses only.
 -  Fixed JavaScript error at some environments “groupSymbol is undefined”.
 -  Fixed crush of cron reindex on huge number of orders (10K+).

### Version 1.4.8

 -  Responsive product images for amazon style of Sold Together block on
    Ultimo themes.

### Version 1.4.7

 -  Add ability to show soldtogether like a widget
 -  Get products from current cart (quote)

### Version 1.4.5

 -  Added option to reindex orders only for last N days (user can specify
    value for N in store system config).
 -  Fix javascript error and incorrect total price for bundle product if some
    items are out of stock.

### Version 1.4.3

 -  Overall styles and templates improvements.
 -  Load and execute Java Scrip with *defer* attribute.
 -  Fixed rendering of blocks for emails. They caused empty emails in some
    environments.
 -  Compatibility with *Amasty_Cart* extension when Amazon style enabled. Sold
    Together adds all selected products but in default Magento way (no Ajax).
 -  Admin interfaces improved. Added product ID columns in Sold Together grids.

### Version 1.4.1

 -  Integration with [Checkout Success](http://docs.swissuplabs.com/m1/extensions/checkout-success/) 2.x extension
 -  Hide already ordered products as recommendation in email blocks
 -  Minor style improvements

### Version 1.4.0

 -  Added soldtogether customer and order blocks to order email
