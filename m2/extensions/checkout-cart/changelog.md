---
layout: default
title: Checkout Cart Changelog
description: Checkout Cart changelog
keywords: Checkout Cart changelog
category: Checkout Cart
---

# Changelog

### Version 1.5.9

> May 23, 2023

 -  [Breeze Theme](https://breezefront.com/) integration improved.
 -  Improve user experience when changing products count at checkout page.
 -  Accessebility fix: addded missing label for quantity input field.


### Version 1.5.6

> Jan 13, 2021

  - Checkout modules dropdown over module config at System Configuration.
  - Convert section "Swissup Checkout" into item "Checkout" under section "Swissup" at System Config page.

### Version 1.5.5

> Oct 30, 2020

 -  Added ability to show product SKU below product name.
 -  Added ability to disable qty editor.
 -  Fixed js error when module is disabled.
 -  Performance improvements.

### Version 1.5.3

> Jul 31, 2020

 -  Added additional checkoutConfig checks to prevent js error

### Version 1.5.2

> May 13, 2020

 -  Convert quantity value to number when incrementing to prevent string concatenation
 -  Removed default argument value in JS code (IE compatibility)

### Version 1.5.0

> Apr 27, 2020

 -  Added translations
 -  Added support for Quantity Increments configuration

### Version 1.4.2

> Sep 9, 2019

 -  New, better looking product qty buttons.

### Version 1.4.1

 -  Fixed missing shipping rates when GiftRegistry address is used
 -  Fixed error when grouped product added to cart (When simple products are
    not visible in catalog)

### Version 1.3.0

 -  Allow to use html entities (Like these: ® ©) in product names

### Version 1.2.1

 -  Translation file added

### Version 1.2.0

 -  Added ability to show product name as a link

### Version 1.1.4

 -  Fixed styles compatibility with firecheckout 1.10.0

### Version 1.1.3

 -  Order totals moved below cart items by default

### Version 1.1.2

 -  Fixed vertical alignment of button and input fields
 -  Fixed visible scrollbar on tablet devices

### Version 1.1.1

 -  Fixed styles small screen sizes

### Version 1.1.0

 -  LumaIcons replaced with css styled arrows
 -  Added ability to use plus/minus symbols instead of arrows with less variable:

    ```scss
    @checkout-cart__toggler-style: 'sign'; // [sign|arrow]
    ```

### Version 1.0.0

 -  Initial Release
