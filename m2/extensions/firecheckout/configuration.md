---
layout: default
title: Firecheckout Configuration
description: Firecheckout Configuration
keywords: firecheckout, options, configuration
category: Firecheckout
---

# Configuration

* TOC
{:toc}

### General section

You can access Fire Checkout configuration at Configuration > Swissup > Checkout > Firecheckout page.

![General section](/images/m2/firecheckout/configuration/general.png)

Option      | Description
------------|------------
Enabled     | Allows to enable/disable firecheckout per store view
Url Path    | Set custom url to the firecheckout page
After Adding a Product Redirect to Firecheckout | Allows to redirect to firecheckout page after Add to Cart action

> If `After Adding a Product Redirect to Firecheckout` is not working on your
> site, try to enable `After Adding a Product Redirect to Shopping Cart` at
> _Stores > Configuration > Checkout > Shopping Cart_ section

### Design section

![Design section](/images/m2/firecheckout/configuration/design.png)

Option      | Description
------------|------------
Page Layout | [Select page layout](#page-layout) to use at firecheckout page
Layout      | [Select layout](#layout) to use at firecheckout page
Place Order Button Position | [Ability to place](#place-order-button-position) "Purchase" button under payment section. This config is visible for "1 Column" layouts only.
Theme       | [Select theme](#theme) to use at firecheckout page
Form Styles | [Select form styles](#form-styles) to use at firecheckout page

#### Page Layout

There are 4 page layouts available to use:

 -  [Default Checkout Layout](#&gid=1&pid=1) (Depends on your active theme)
 -  [Empty](#&gid=1&pid=2) (No Header and Footer)
 -  [Minimal](#&gid=1&pid=3) (Header with Store Logo only)
 -  [Full](#&gid=1&pid=4) (Full 1column layout with header, navigation and footer)

Page layout screenshots:

{% include gallery.html images=site.data.gallery.m2.firecheckout.configuration.page-layout class="scroll phone-up-1 tablet-up-4 photoswipe" %}

#### Layout

There are 5 layouts available to use:

 -  [1 Column (Multistep Wizard)](#&gid=2&pid=1)
 -  [1 Column (Expanded)](#&gid=2&pid=2)
 -  [2 Columns (Wide Payment and Shipping sections)](#&gid=2&pid=3)
 -  [2 Columns (Place Payment and Shipping sections side by side)](#&gid=2&pid=4)
 -  [3 Columns](#&gid=2&pid=5)

Layout screenshots:

{% include gallery.html images=site.data.gallery.m2.firecheckout.configuration.layout class="scroll phone-up-1 tablet-up-3 photoswipe" %}

#### Move Email to the Separate Step

> Available since v1.26.0

Ability to move email field to the separate "Email" step. This option is available
when using 1-column Multistep layout only.

{% include gallery.html images=site.data.gallery.m2.firecheckout.configuration.move-email class="scroll phone-up-1 tablet-up-3 photoswipe" %}

#### Place Order Button Position

Ability change "Purchase" button position:

 - Default Position (Order Summary Section - For All Layouts)
 - Below Payment methods Section (For "1 Column" Layouts only)

{% include gallery.html images=site.data.gallery.m2.firecheckout.configuration.place-order-position class="scroll phone-up-1 tablet-up-3 photoswipe" %}

#### Theme

There are 4 themes available to use:

 -  [Default](#&gid=5&pid=1)
 -  [Light](#&gid=5&pid=2)
 -  [Midnight](#&gid=5&pid=3)
 -  [Round](#&gid=5&pid=4)

Themes screenshots:

{% include gallery.html images=site.data.gallery.m2.firecheckout.configuration.theme class="scroll phone-up-1 tablet-up-3 photoswipe" %}

#### Form Styles

There are 3 form **modes** available:

 -  [Horizontal](#&gid=6&pid=1) (Label aside of the field)
 -  [Basic](#&gid=6&pid=2) (Same as horizontal, except label above the field)
 -  [Compact](#&gid=6&pid=3) (Multiple fields per row. [How to change field size?](/m2/extensions/firecheckout/customization/use-cases/field-size/))

{% include gallery.html images=site.data.gallery.m2.firecheckout.configuration.form-styles class="scroll phone-up-1 tablet-up-3 photoswipe" %}

**Use field placeholders instead of labels** - You can hide labels and use field
placeholders instead. This option works together with **Basic** and **Compact**
modes only:

{% include gallery.html images=site.data.gallery.m2.firecheckout.configuration.hidden-labels class="scroll phone-up-1 tablet-up-3 photoswipe" %}

**Show field errors and notices in the Tooltips** - Allows you to switch between
awesome Tooltips mode and Magento's old-school notices and errors below the fields:

{% include gallery.html images=site.data.gallery.m2.firecheckout.configuration.tooltips class="scroll phone-up-1 tablet-up-3 photoswipe" %}

### Additional content section

![Additional content section](/images/m2/firecheckout/configuration/additional-content.png)

Option                  | Description
------------------------|------------
Above Firecheckout Form | Additional content above firecheckout form
Below Firecheckout Form | Additional content below firecheckout form
Above place order button| Additional content above place order button
Below place order button| Additional content below place order button
**Intro Popup**         | See [ready-to-use examples](/m2/extensions/firecheckout/customization/use-cases/intro-popup/)
Content for Guest Customers | Content to show for guest customers only
Content for Registered Customers | Content to show for logged in customers

### Analytics section

![Analytics section](/images/m2/firecheckout/configuration/analytics.png)

Option | Description
-------|------------
Enable Google Analytics Integration | Enable/Disable Analytics Integration
Account Number | Google Analytis Account Number. If you use Magento's built-in GA module, this field will be filled automatically. See [Analytics](analytics/) page for more information.

Please follow [Analytics integration docs](analytics/) to setup Analytics inside
Firecheckout.

### Shiping settings section

![Shipping settings section](/images/m2/firecheckout/configuration/shipping.png)

Option                  | Description
------------------------|------------
Default Method          | Default shipping method to use
Default Method Code     | Same setting as above. Use this field if you can't find the method you are looking for in the previous option
Hide methods if single method is available only | Useful if you use single method for all customers
Sort shipping methods by price | Allows to sort shipping methods by their price. From lower to higher.

### Payment settings section

![Payment settings section](/images/m2/firecheckout/configuration/payment.png)

Option                  | Description
------------------------|------------
Default Method          | Default payment method to use
Show Billing Address Title | Show/Hide title above billing address form
Display Billing Address On | Select billing address form placement: [Inside Payment Method](#&gid=9&pid=1), [Above Payment Methods](#&gid=9&pid=2), [Below Payment Methods](#&gid=9&pid=3), [Above Shipping Address](#&gid=9&pid=4), [Below Shipping Address](#&gid=9&pid=5)
Save Mode | Choose "Default" or "Instant" modes. Default uses "Update" button to save billing form. Instant saves address without "Update" button.

Billing address placement screenshots:

{% include gallery.html images=site.data.gallery.m2.firecheckout.configuration.billing-address-position class="scroll phone-up-1 tablet-up-3 photoswipe" %}

### Terms and Conditions settings section

> Available since version [1.22.0](/m2/extensions/firecheckout/changelog/#version-1220)

![Terms and Conditions section](/images/m2/firecheckout/configuration/terms-and-conditions.png)

Option                  | Description
------------------------|------------
Enabled                 | Enable/Disable agreements at checkout page
Position                | Ability to show agreements at default position (Payment Method) or "Above Place Order Button"
Title                   | Optionally set the title above agreements

### Order summary settings section

![Order summary settings section](/images/m2/firecheckout/configuration/order-summary.png)

Option                  | Description
------------------------|------------
Show Order Review       | Show order review information (Shipping Address and Shiping Method) above the cart items.
Title                   | Set the title for order summary section

### Custom CSS and JS settings section

![Custom CSS and JS settings section](/images/m2/firecheckout/configuration/custom_css_js.png)

Option  | Description
--------|------------
CSS     | CSS styles. LESS is not supported.
LESS    | CSS styles with LESS syntax support.
JS      | JS code

View JS code examples at [Checkout Customizations](/m2/extensions/firecheckout/customization/) pages.

### Performance settings section

![Performance section](/images/m2/firecheckout/configuration/performance.png)

Option  | Description
--------|------------
Use jsBuild | Combine checkout-related js files into single jsbuild to reduce number of requests and improve page load time.
jsBuild include paths| List of modules to process
Prefetch jsBuild | When enabled, checkout page and jsBuild will be prefetched when customer will add a product to the cart.

#### Next up
{:.no_toc}

 -  [Back to Main Page](../)
