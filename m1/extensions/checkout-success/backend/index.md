---
layout: default
title: Backend Confiruration
description: magento checkout success backend settings
keywords: "checkout success backend settings, checkout success backend configuration, Google Adwords"
category: Checkout Success
---

# Extension configuration

In order to change general extension settings, go to `System` ➔ `Configuration`
➔ `TM Checkout` section ➔ `Success Page`.

Checkout Success Page settings have three sections.

### General

![Checkout Success system config general](/images/m1/extensions/checkout-success/backend/general.png)

You can enable or disable extension in this section.

Field `Additional content at the bottom of success page` allows you to insert
on checkout success page any HTML or JS code. This field can be very usefull
if you have to add Google Adwords conversion code. This field allows to use
variables:

| Variable                                  | Description                     |
|-------------------------------------------|---------------------------------|
| `{% raw %}{{orderId}}{% endraw %}`        | Order number                    |
| `{% raw %}{{orderAmount}}{% endraw %}`    | Order grand total               |
| `{% raw %}{{currency}}{% endraw %}`       | Order currency                  |
| `{% raw %}{{currencySymbol}}{% endraw %}` | Order currency symbol           |
| `{% raw %}{{customerEmail}}{% endraw %}`  | Email of customer who placed an order |
| `{% raw %}{{customerId}}{% endraw %}`     | Id of customer who placed an order |
| `{% raw %}{{paymentCode}}{% endraw %}`    | Code of payment method for an order |
| `{% raw %}{{paymentTitle}}{% endraw %}`   | Name of payment method for an order |
| `{% raw %}{{shippingCode}}{% endraw %}`   | Code of shipping method for an order |
| `{% raw %}{{shippingTitle}}{% endraw %}`  | Name of shipping method for an order |
| `{% raw %}{{orderShippingAddress}}{% endraw %}` | JSON encoded shipping address for an order. _Since 2.0.9_  |
| `{% raw %}{{orderBillingAddress}}{% endraw %}`  | JSON encoded billing address for an order. _Since 2.0.9_ |

### Mockup

![Checkout Success system config mockup](/images/m1/extensions/checkout-success/backend/mockup.png)

Section `Mockup` provides easy to use drag-and-drop interface to modify
checkout success page layout. Success page constructed with predefinded blocks that can be arranged in any way you want.

`Blocks available on Success Page` is a list of available blocks. It can not be edited. You can only grab one of that blocks and drop it on success page mockup.

`Mockup of Success Page` is a schematic representation of success page. Extension divides page content on four segments - top, bottom, middle-left and
middle-right. You can move blocks from one segment to other. You can delete block by clicking red cross in right side of block.

In "Mockup" section you can find very useful feature - preview success page.
Input order number in `Order # to preview` and press button
`Save and Start Preview`.

### Additional mockup settings

![Checkout Success system config additional mockup settings](/images/m1/extensions/checkout-success/backend/additional-mockup.png)

In this section you can assign CMS block to respective block on checkout success page.
