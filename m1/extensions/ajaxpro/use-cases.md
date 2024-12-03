---
layout: default
title: AjaxPro Use Cases
description: magento ajax module use-cases
keywords: " magento ajax, magento ajax module, magento ajax call to block,
magento ajax shopping cart, magento ajax cart pro "
category: AjaxPro
---

# Ajax Pro Use Cases

### Add to Cart Popup

 -  [Insert custom content](#insert-custom-content-into-popup)
     +  [Window type - Extended Shopping Cart](#window-type---extended-shopping-cart)
     +  [Window type - SuggestPage Content](#window-type---suggestpage-content)
 -  [Make Shipping information always visible in AjaxCart popup](#make-shipping-information-always-visible-in-ajaxcart-popup)

#### Insert custom content into popup

##### Window type - Extended Shopping Cart

You have to apply custom layout update to insert custom content into add to cart popup.

1. If you use Argento theme then you have to create or modify `custom.xml`
    file (you can [read here](/m1/argento/theme-customization/small-changes/#custom-layout-update-file) how to do this).
 2. For other magento theme you have to creat or modify `local.xml`
    file (you can [read here](http://inchoo.net/magento/using-local-xml-for-overriding-or-updating-xml-structure/) how to do this)
 3. Add code below to XML file from previouse item:

    ```xml
    <tm_ajaxpro_checkout_cart_add_with_cart_extended>
        <reference name="ajaxpro_message">
            <action method="unsetChild">
                <name>checkout.cart</name>
            </action>
            <block type="cms/block" name="custom_block">
                <action method="setBlockId">
                    <block_id>ajax-pro-cart_text</block_id>
                </action>
            </block>
            <action method="insert">
                <name>checkout.cart</name>
            </action>
        </reference>
    </tm_ajaxpro_checkout_cart_add_with_cart_extended>
    ```

 4. Create CMS Static block with identifier `ajax-pro-cart_text` using Magento
    Admin interface. And place some content into it. For example, we add such
    text:

    ```
    <p>You can close this popup by clicking X button in top right corner.</p>
    ```

 5. Flush Magento cache and try to add anything to cart.

![custom content into add to cart popup](/images/m1/extensions/ajax-pro/custom-content-to-popup-extended-cart.png)

##### Window type - SuggestPage Content

You have to apply custom layout update to insert custom content into add to cart popup.

 1. If you use Argento theme then you have to create or modify `custom.xml`
    file (you can [read here](/m1/argento/theme-customization/small-changes/#custom-layout-update-file) how to do this).
 2. For other magento theme you have to creat or modify `local.xml`
    file (you can [read here](http://inchoo.net/magento/using-local-xml-for-overriding-or-updating-xml-structure/) how to do this)
 3. Add code below to XML file from previouse item:

    ```xml
    <tm_ajaxpro_checkout_cart_add_suggestpage>
        <reference name="content">
            <block type="cms/block" name="block.01" before="suggest.cart">
                <action method="setBlockId">
                    <block_id>ajax-pro-cart_text</block_id>
                </action>
            </block>
        </reference>
    </tm_ajaxpro_checkout_cart_add_suggestpage>
    ```

 4. Create CMS Static block with name `ajax-pro-cart_text` using Magento Admin
    interface. And place some content into it. For example, we add such text:

    ```
    <p>You can close this popup by clicking X button in top right corner.</p>
    ```

 5. Flush Magento cache and try to add anything to cart.

![custom content into add to cart popup](/images/m1/extensions/ajax-pro/custom-content-to-popup.png)



#### Make Shipping information always visible in AjaxCart popup

 1. Open your theme **css** file
 2. Add following code to the end:

    ```CSS
    #ajaxpro-notice-form .cart-collaterals { display: block !important; }
    #invader { display: none !important; }
    ```

    ![Ajax Cart expanded](/images/m1/extensions/ajax-pro/ajax-cart.png)

#### You can also check:

*   [Installation](../installation/)
*   [Changelog](../changelog/)
*   [Configuration](../configuration/)
*   [Support](https://swissuplabs.com/contacts/)
*   [Forum](https://swissuplabs.com/magento-forum/)