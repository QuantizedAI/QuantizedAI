---
layout: default
title: GDPR Changelog
description: GDPR changelog
keywords: gdpr changelog
category: GDPR
---

# Changelog

### Version 1.7.8

> Oct 25, 2024

 -  Accessibility improvements.
 -  Improve GoogleConsent integration. Now, we update consents right after default
    values was set. This makes much better compatibility with third-party GTM modules.
 -  Fixed blink of default cookie bar for a moment.
 -  Fixed conflict with built-in cookie restriction mode.
 -  Fixed not working GDPR consents validation in UI forms.

### Version 1.7.3

> Jul 15, 2024

 -  Magento 2.4.7-p1 compatibility: Fixed not working Google consents and GDPR
    cookie consent toolbar at the checkout page.
 -  Do not pass GA session params in URL when consent is declined or not yet accepted.

### Version 1.7.0

> Apr 30, 2024

 -  Added ability to change and create region-specific [default Google consent values](/m2/extensions/gdpr/configuration/#cookie-consent-section).
 -  Added "Deny" and "Allow Selection" buttons to [minimal cookie bar mode](/m2/extensions/gdpr/configuration/#cookie-bar-display-modes).
 -  Fixed not working default Google consent values.
 -  Do not set Google consent values until customer presses "Accept" or "Deny" buttons.
 -  Allow using `url_passthrough` variable when consent is declined.
 -  Default cookie wall color changed to dark.

### Version 1.6.3

> Apr 1, 2024

 -  Breeze: fixed missing focus styles.
 -  Improve styles for cookie togglers.

### Version 1.6.2

> Mar 15, 2024

 -  Do not store `!notfound` cookie group in cookies.

### Version 1.6.1

> Mar 12, 2024

 -  Fixed possible undefined 'swissupGdprCookieSettings' when using js bundling.
 -  Fixed not working Magento_GoogleTag because of
    [window.gtag function checking by Magento](https://github.com/magento/magento2/blob/2.4-develop/app/code/Magento/GoogleGtag/view/frontend/web/js/google-analytics.js#L39).

### Version 1.6.0

> Mar 5, 2024

![Google Consent Mode](/images/m2/gdpr/google-consent.png){:width="772" height="440"}

 - Added integration with [Google Consent Mode v2](https://developers.google.com/tag-platform/security/guides/consent?consentmode=advanced).
   It's enabled by default. Still, you can disable it from the [module configuration](/m2/extensions/gdpr/configuration/#cookie-consent-section).
 - Cookies reorganized into better groups. Preferences cookie group added.
   Advertisement group merged into Marketing group.
 - Removed useless customers section update after cookie consent settings were changed.

### Version 1.5.23

> Feb 2, 2024

 - Breeze integration updated. Dynamic JS support added.
 - Locale files cleanup.

### Version 1.5.20

> Nov 28, 2023

 -  Code cleanup.

### Version 1.5.19

> Sep 14, 2023

 -  Performance: improved LCP when cookie bar is enabled.

### Version 1.5.18

> Jul 27, 2023

 -  [Breeze](https://breezefront.com) integration fixes.
 -  Stability improvements.

### Version 1.5.14

> May 23, 2023

 -  Fixed missing validation message when form uses `data-errors-message-box` (Swissup_Askit)

### Version 1.5.13

> Mar 27, 2023

 -  When new cookie group is added by store administrator, show cookie consent 
    again to all visitors.
 -  Fixed possible initially invisible consents in all forms except newsletter.
 -  Remove outdated PHP code.

### Version 1.5.10

> Mar 14, 2023

 -  PHP 8.2 compatibility.
 -  Stability improvements.

### Version 1.5.9

> Nov 15, 2022

 -  Improve Breeze integration

### Version 1.5.8

> Aug 5, 2022

 -  GA4 cookies added to the known cookies list.

### Version 1.5.2

> Apr 15, 2022

 -  Magento 2.4.4 and PHP 8.1 compatibility.

### Version 1.5.0

> Apr 9, 2022

 -  Added ability to [make a pre-checked cookie consent](/m2/extensions/gdpr/backend/#cookie-registry)
    for optional cookie group. Previously only required cookie groups
    were pre-checked.

### Version 1.4.11

> Jan 28, 2022

 -  Magento Coding Standard fixes
 -  [Breeze Theme](https://breezefront.com) integration added

### Version 1.4.10

> Dec 13, 2021

 -  Breeze theme integration added.

### Version 1.4.9

> Sep 24, 2021

 -  Facebook pixel cookie added to known cookies list.

### Version 1.4.8

> Sep 14, 2021

 -  Updated breeze integration.

### Version 1.4.7

> Jul 22, 2021

 -  [Breeze](/m2/extensions/breeze/) integration updated. Fixed not working
    'Delete My Data' button.

### Version 1.4.6

> Jul 15, 2021

 -  [Breeze](/m2/extensions/breeze/) integration updated. Prevent js error when
    Magento_GoogleAnalytics is disabled.

### Version 1.4.5

> Jun 14, 2021

 -  Fixed not working 'Add Cookie Group' button in backend (Magento 2.4)
 -  "Accept All" button replaced with "Accept All & Save" in cookie bar component.

### Version 1.4.3

> May 14, 2021

 -  [Breeze](/m2/extensions/breeze/) integration added.

### Version 1.4.2

> Mar 30, 2021

 -  Show accepted cookie group titles instead of group ids at account page.
 -  Fixed invalid 'updated_at' value when client consents gets updated.
 -  Better compatibility with Athlete theme.

### Version 1.4.1

> Mar 23, 2021

 -  Fixed overlay blink while styles are loading

### Version 1.4.0

> Jan 25, 2021

 -  [Cookie Wall](/m2/extensions/gdpr/configuration/#cookie-consent-section) feature added.

### Version 1.3.18

> Jan 22, 2021

 -  Fixed translation for "Agree & save" phrase.
 -  Updated integration with our [Pagebuilder module](/m2/extensions/pagebuilder/)

### Version 1.3.17

> Nov 26, 2020

  - Do not send email notifications (order status update, newsletter, review reminders)
    to anonymized email addresses.
  - Fixed possible disappeared message after add to cart. It prevents Magento from updating customer sections after registering unknown cookie.
  - Decrease number of ajax requests if some module write cookies multiple times.
  - Fixed margin for newsletter consent at RTL locales.

### Version 1.3.14

> Oct 27, 2020

 -  Improved frontend performance when a bunch of cookies are blocked. Previously
    GDPR module sent a request per each cookie. Now, all cookie names will be
    merged into a single request.
 -  Fixed blocked google analytics cookies when Magento_GoogleAnalytics module is
    enabled in runtime via third-party plugin.
 -  Fixed missing GDPR checkboxes on customer registration page when
    [Swissup_CustomerFields](/m2/extensions/customer-field-manager/) is enabled.

### Version 1.3.11

> Oct 19, 2020

 -  Fixed php error when using "Login as Customer" feature.

### Version 1.3.10

> Oct 13, 2020

 -  [Pagebuilder](/m2/extensions/pagebuilder/) integration added

### Version 1.3.9

> Aug 25, 2020

 -  Fixed cookie bar flickering when critical css is enabled in theme.

### Version 1.3.8

> Aug 7, 2020

 -  Fixed ability to translate `I accept following cookies: ...` phrase via
    admin configuration _Stores > Configuration > Swissup > GDPR > Personal Data Consents > Cookie Consents_
 -  Do not show empty "Cookie Settings" on "Privacy Tools" page when it's disabled.

### Version 1.3.7

> Aug 5, 2020

 -  PHP 7.4 compatibility.
 -  Allow to translate cookie title and description via i18n files.
 -  Do not show cookie bar until scripts are ready.
 -  Fixed newsletter signup styles in Magento 2.4.
 -  Place consents before captcha/recaptcha field.

### Version 1.3.3

> Jun 18, 2020

 -  Fixed DB error when customer logging in.

### Version 1.3.2

> May 7, 2020

 -  16 locales added to translate backend and frontend phrases:
    - Arabic
    - Chinese
    - Dutch
    - French
    - Hebrew
    - Italian
    - German
    - Japanese
    - Norwegian
    - Korean
    - Polish
    - Portuguese
    - Russian
    - Spanish
    - Swedish
    - Ukrainian

### Version 1.3.1

> Apr 27, 2020

 -  Fixed error during static content deploy when theme buttons use gradient for background.
 -  Fixed cookie bar positioning when theme uses margins on page-wrapper.

### Version 1.3.0

> Apr 17, 2020

{% include gallery.html images=site.data.gallery.m2.gdpr.changelog.v140 class="phone-up-2 tablet-up-3 photoswipe scroll" %}

**Cookie consent feature added. Here is some highlights of the new feature:**

 -  Cookie bar banner in minimalistic and full display modes.
 -  Separate page to control cookie settings.
 -  Cookie settings at customer account page.
 -  When the user creates an account, guest cookie consent automatically links
    with this account.
 -  Module blocks all optional cookies until visitor accept consent.
 -  Accepted cookie consent is saved into DB.
 -  All _unknown_ blocked cookies automatically added to the backend list, so
    you can regulary check if all cookies that are used on the site are
    in the consent list.
 -  Store owner can register unlimited count of additional cookies and groups.
 -  All magento cookies are known by the module out of the box.

### Version 1.2.3

> Feb 17, 2020

 -  RTL fixes for newsletter consent

### Version 1.2.2

> Jan 31, 2020

 -  Fixed broken ACL resources page in Magento older than 2.3.4
 -  Fixed too large margin in newsletter checkbox in Magento 2.3.4

### Version 1.2.0

> Jun 4, 2019

 -  Added consent text to the "Newsletter Subscriptions Management" page.
 -  Added ability to withdraw newletter consent for registered customers.
    (Available at "Newsletter Subscriptions Management" page inside
    customer account.)
 -  Fixed not working form autocomplete when gdpr is initialized on the form.

> **Upgrade Instruction**
>
> Navigate to module configuration and check "Show in Forms" option for
> Newsletter consents config. Two forms should be selected:
>
> - Magento: Newsletter Subscription
> - Magento: Newsletter Subscription Management

### Version 1.1.4

> May 29, 2019

 -  Fixed missing consents at account privacy page when cache is enabled
 -  Fixed not working customer link in requests grid at the backend

### Version 1.1.2

 > May 24, 2019

 -  Deprecated code removed

### Version 1.1.1

> Mar 29, 2019

 -  Added missing localization file
 -  Fixed mysql error on client consents page when table prefixes are used

### Version 1.0.0

 -  Initial Release
 -  Consents in the following forms:
    - Newsletter
    - Contacts
    - Registration
    - Product Reviews
 -  Ability to request account deletion from Privacy Tools page
