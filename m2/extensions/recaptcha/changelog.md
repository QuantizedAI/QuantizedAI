---
layout: default
title: Changelog
description: magento2 recaptcha module changelog
keywords: " magento2 recaptcha, recaptcha extension, changelog "
category: reCAPTCHA
---

# Changelog

### Version 1.4.10

> Jul 6, 2023

 -  JS improvements for Breeze-powered store front to reduce number of initially loaded assets.
 -  Fixed dynamic property creation error in PHP 8.2.

### Version 1.4.8

> May 30, 2023

 -  Update integration with Amazon Pay at checkout.

### Version 1.4.7

> Mar 31, 2023

 -  Few more fixes for PHP 8.2.
 -  Meeting Magento Coding Standarts. Avoid using closing slash with void tags.

### Version 1.4.5

> Mar 14, 2023

 -  PHP 8.2 compatibility.

### Version 1.4.3

> Apr 15, 2022

 -  Magento 2.4.4 and PHP 8.1 compatibility.

### Version 1.4.2

> Feb 21, 2022

 -  Recaptcha on checkout. Fixed grecaptcha js error when applied 100% order discount and no payment required. Error said that Google reCAPTCHA already rendered for this element.
 -  Fixed weirdest bug ever with Magento Paypal on checkout. Bug description: after passing recaptcha button for "In context paypal" doesn't react on clicks.

### Version 1.4.1

> Jan 28, 2022

 -  Fixed deprecation error in PHP 7.4

### Version 1.4.0

> Oct 18, 2021

  - [Breeze](/m2/extensions/breeze/) integration.
  - Fixed missing recaptcha at checkout when third-party paymnent doesn't render `checkout-agreements-block`.
  - Overall improvements for recaptcha at checkout.

### Version 1.3.18

> Sep 13, 2021

  - Compatibility with FireCheckout when terms and conditions block moved.
  - Fixed missing recaptcha at checkout for some payments methods (e.g., CreditKey_B2BGateway).

### Version 1.3.17

> Aug 6, 2021

  - Fixed not working racaptcha at checkout when stored card is used for payment.
  - Compatibility with EsteSolutions_ManualCCPayment, ZipMoney_ZipMoneyPayment and Ravedigital_CoreUpdate.

### Version 1.3.16

> May 7, 2021

  - Newsletter recaptcha - lazy init. Initialize it on click at newsleter form.
  - Prevent JS error "Cannot read property 'method' of undefined" at checkout with Ebizmarts_SagePaySuite payment.
  - Compatibility with Mageants_FrontOrderComment abd VLCSolutions_OrderComments modules.

### Version 1.3.15

> Mar 23, 2021

 - Reset recaptcha on frontent when token expired. Prevent sending of submitting invalid token.
 -  Improve compatibility with Magento 2.1.x.
 -  Improve compatibility with third-party modules.

### Version 1.3.14

> Feb 17, 2021

  - Added ACL.
  - Better compatibility with Mageplaza One Step Checkout.
  - Fixed not working JS validator for checkout agrements. Caused by module version 1.3.11.
  - Fixes for PayPal payment method when checkout is protected with recaptcha.
  - Few minor JS fixes for recaptcha at checkout.
  - JS code cleanup and improve potential for JS minification. 

### Version 1.3.12

> Oct 20, 2020

  - Fixed recaptcha validation on checkout when payment does mulptiple server requests to place an order.

### Version 1.3.11

> Oct 1, 2020

 -  Recaptcha validation on client side. Validate if checkmark is checked right before placing order.

### Version 1.3.10

> Aug 5, 2020

 -  Make friends with braintree payment method.

### Version 1.3.9

> Jun 10, 2020

  - Checkout: prevent "Invalid recaptcha" message for next "Place Order" when first attempt failed due to some incorrect data.

### Version 1.3.8

> May 22, 2020

  -  Fixed missing [OrderAttachements](/m2/extensions/order-attachments/) block when recaptcha is enabled

### Version 1.3.7

> May 15, 2020

  -  Magento 2.3.5 CSP compatibility.

### Version 1.3.6

> Apr 13, 2020

 -  Fixed unable to place order when recaptcha protects checkout and paypalflow method is selected.

### Version 1.3.5

> Mar 20, 2020

 -  Integrate with latest version of Swissup AskiIt module (version 1.7.0+).

### Version 1.3.4

> Mar 11, 2020

 -  Improve recaptcha behavior at checkout. Fixed missing recaptcha when customer uses stored with braintree payment card.

### Version 1.3.3

> Mar 6, 2020

 -  Fixed defaultCaptcha.js error when recaptcha disabled on frontend.
 -  Make Recaptcha and Amazon Payment friends (integrate with amzn/amazon-pay-module).
 -  Add Recaptcha to login form at checkout when only virtual product is in cart.

### Version 1.3.2

> Mar 2, 2020

 -  Show missing recaptcha at checkout shipping address section when user input email address of existed customer and store asks him to login. Works when captcha at signin form enabled.

### Version 1.3.0

> Feb 6, 2020

 -  Protect checkout with recaptcha.
 -  Config recaptcha look for any form with ["Design Exceptions"](../configuration/).

### Version 1.2.3

> Dec 6, 2019

 -  Remove 'jquery/ui' dependency to prevent message about slow performance in browser console at Magento 2.3.

### Version 1.2.2

> Jul 29, 2019

 -  Fixed error - No property exists by the name 'formId' in Magento 2.1.x.
 -  Slightly improve recaptcha styles for newsletter. Prevent recaptcha from streching newsletter form on small screens.

### Version 1.2.1

> Jun 12, 2019

 -  Fixed missing recaptcha at some pages for newsletter form. Forgot password page is one of them.
 -  Added comment to general section of Recaptcha settings at Magento Configuration.

### Version 1.2.0

> May 13, 2019

 -  New feature - protect "Subscribe to newsletter" with recaptcha.

### Version 1.1.3

> Mar 29, 2019

 -  Magento 2.3.1 compatibility (Fixed frontend js error)

### Version 1.1.2

> Dec 4th, 2018

 -  Updated google/recaptcha requirement to get latest stable version.
    (Magento 2.3.0 compatibility)

### Version 1.1.1

> Nov 8th, 2018

 -  Use curl to request recaptcha validation. It makes request slightly quicker.
 -  Improve module stability.

### Version 1.1.0

Internal module naming convention was updated. We applied this changes to reach full compatibility with Magento Marketplace policy.

### Version 1.0.1

 -  Add reCAPTCHA in authentication popup.
 -  Do not load JS ans CSS for default Magento Captcha when reCAPTCHA enabled.

### Version 1.0.0

Initial release.

Extension replaces default Magento Captcha with Google reCAPTCHA.
