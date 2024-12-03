---
layout: default
title: Argento Luxury Product Page
description: ArgentoLuxury product page
keywords: "ArgentoLuxury, luxury, product page, colorswatches, tabs, soldtogehter"
category: Argento
---

# Argento Luxury Product Page

### Configuration settings

There is specific section for product page configuration in Magento Admin. Go to `System` → `Configuration`. Find `TM Argento Themes` section there and choose `Luxury`.

![Product page settings](/images/argento/default/product-page-settings.png)

Here you can:

 -  change product image layout and set product image size (check [Product Images](#images) paragraph),
 -  stick product image and/or product details section.

### Layout

Luxury is using `page_one_column` layout for the product page. To
change it to another one, create [custom.xml][custom_xml] file and add the
following instruction:

```xml
<catalog_product_view>
    <update handle="page_two_columns_left"/>
</catalog_product_view>
```

Possible values for handle variable:

```
page_two_columns_left
page_two_columns_right
page_three_columns
page_one_column
```

### Content

#### Images

Product images can be presented in two ways.

 Default                    | Slider 
----------------------------|--------------------------------
 Main image with thumbnails | Horisontal scroll of all images
----------------------------|--------------------------------
![Product Image - default](/images/argento/luxury/product-page/images.png){:class="noborder"} | ![Product Image - slider](/images/argento/luxury/product-page/images-slider.png){:class="noborder"}

Product image and gallery is powered by [Lightbox Pro](/m1/extensions/lightboxpro/) module,
that has a lot of configuration options at `System > Configuration > Template-Master > LightboxPro`
section.

It allows you to configure the following options:

- Image dimensions
- Gallery controls
- Overlay settings
- Popup settings

#### Colorswatches

{::options parse_block_html="true" /}
<div class="mdl-grid"><div class="mdl-cell mdl-cell--3-col mdl-cell--2-col-tablet">

![Catalog Configurable Swatches](/images/argento/luxury/product-page/colorswatches.png)

</div><div class="mdl-cell mdl-cell--9-col mdl-cell--6-col-tablet">

Catalog Configurable Swatches - is a standard Magento feature since 1.9.1, which
is fully integrated with the following Argento modules:

- AjaxPro
- AjaxSearch
- LightboxPro

You can read this
[great tutorial][colorswatches] by [sherodesigns](http://sherodesigns.com) about
color swatches configuration.

</div></div>

#### Tabs

Argento tabs is powered by [EasyTabs](/m1/extensions/easytabs/) module.
You can add or remove additional tabs from `Templates-Master > Easy Tabs` page.

The following tabs are shown under add to cart box:

![Product Tabs](/images/argento/luxury/product-page/product-tabs.png)

- Product Description
- Reviews
- Free delivery and Returns

Additional tabs are shown in content area:

![Info Tabs](/images/argento/luxury/product-page/info-tabs.png)

- Customers also buy
- Questions
- Recently viewed

This tabs inserted as a widget into CMS block `product_page_additional_tabs`.
You can add there any other content you want. Or you can add few more tabs.

#### Soldtogether blocks

[Sold Together](/m1/extensions/soldtogether/) powered blocks. You can customize these blocks
from `System > Configuration > Tempaltes-Master > Sold Together` section.

Configuration provides the following options:

- Products count
- Columns count
- Amazon style for `Frequently bought together` block

##### Frequently bought together

`System > Configuration > Tempaltes-Master > SoldTogether > Frequently Bought Together`

![Frequently bought together](/images/argento/luxury/product-page/frequently_bought_together.png)

##### Customers who bought this item also bought

`System > Configuration > Tempaltes-Master > SoldTogether > Customer Bought Together`

![Customers who bought this item also bought](/images/argento/luxury/product-page/info-tabs.png)

[custom_xml]: /m1/argento/theme-customization/small-changes/#custom-layout-update-file "custom.xml layout"
[colorswatches]: http://sherodesigns.com/tutorial-configurable-swatches-in-magento/ "Catalog Configurable Swatches tutorial"
