---
layout: default
title: Highlight Widgets
description: >
    Highlight widgets for magento 2 - convenient way to show promoted products on your store
keywords: >
    magento2 featured products, magento2 new products, magento2 popular products,
    magento2 bestsellers, magento2 onsale products
category: Highlight
---

# Highlight Widgets

Following widget types are available:

![Highlight Widgets](/images/m2/highlight/widgets_dropdown.png)

Type                                                | Description
----------------------------------------------------|------------
Swissup\Highlight\Block\ProductList\NewList         | New Products, ordered by `news_from_date` attribute
Swissup\Highlight\Block\ProductList\Featured        | Products with enabled `featured` attribute
Swissup\Highlight\Block\ProductList\Onsale          | Products with non-empty `special_price` attribute, ordered by `special_from_date`
Swissup\Highlight\Block\ProductList\Popular         | Most viewed products. Calculation is based on `Magento Reports` data
Swissup\Highlight\Block\ProductList\Bestsellers     | Most sold products ordered by orders count. Calculation is based on `Magento Sales` data
Swissup\Highlight\Block\ProductList\Bulksellers     | Most sold products ordered by quantity sold count. Calculation is based on `Magento Sales` data
Swissup\Highlight\Block\ProductList\All             | All visible products. Usefull to manually filter products
Swissup\Highlight\Block\ProductList\Attribute\Date  | Products filtered by any `date` attribute. Attribute value is compared with current date. Attribute used for this widget requires to have option **"Use in Product Listing" enabled** (tab "Storefront Properties" in edit attribuye interface).
Swissup\Highlight\Block\ProductList\Attribute\Yesno | Products filtered by any `yes/no` attribute. Products with enabled attribute are returned. Attribute used for this widget requires to have option **"Use in Product Listing" enabled** (tab "Storefront Properties" in edit attribuye interface).

### Contents

1. [Widget Usage](usage/)
    - [WYSIWYG Editor](usage/#wysiwyg-editor)
    - [Widgets Page](usage/#widgets-page)
    - [XML Layout Update](usage/#xml-layout-update)
    - [PHP Inline Code](usage/#php-inline-code)
2. [Widget Settings](settings/)

##### Next up

Great! Now you might want to see next:

- [Highlight Pages](/m2/extensions/highlight/pages/)
