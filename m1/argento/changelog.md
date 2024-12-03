---
layout: default
title: Argento changelog
description: Argento changelog
category: Argento
---

# Argento Changelog

### Version 1.15.1

> Dec 18, 2020

 -  Fixed js error when inline JS minification enabled in PageSpeed module.
 -  EasyBanners: fixed missing class name on the banner when its inserted as widget.
 -  SEO XML Sitemap: respect 'Exclude CMS' config; add homepage url to sitemap file.
 -  Sold Together: fixed DDL statements are not allowed in transactions error.
 -  Richsnippets: added option for Price Valid Until. Now it ca be dynamic date - offset from today.

### Version 1.15.0

> Oct 22, 2019

 -  Magento 1.9.4.3 compatibility.
 -  Fixed Highlight template to make it work with carousel with enabled cache.
 -  Luxury theme: added rel="nofollow" to wishlist link in header.

**Modules fixes & improvements**

 -  Ajax Pro
     + Fixed add to compare/wishlist actions in Magento 1.9.4.3

 -  AMP
     + Fixed add/remove item from wishlist when browsing CDN-cached version of the site (Magento 1.9.4.3 compatibility)
     + Added styles for table caption and tables inside tabs

 -  Ask It
    + Added config to sort questions by votes number

 -  Attribute Pages
     +  Page Title field is now used for H1 tag only (previously, it was used for meta title too)
     +  Added ability to set meta title using xml_layout_update field

 -  Easybanner
     +  Added compatibility with lazy image loading feature of PageSpeed module

 -  EasyTabs
     +  Added integration with AMP module

 -  GDPR
     +  Fixed php warning about addcslashes parameter

 -  Highlight
     +  Fixed broken carousel when Magento cache is enabled
     +  Added missing SlickCarousel dependency
     +  Fixed “Item with ID already exists” at stores with multiple stocks

 -  Pagespeed
     +  Fixed not working ‘ignore’ config option
     +  Improve offset logic for mobile devices

 -  Pro Labels
     +  Remove limit from label styles and label text length
     +  Do not show system labels for all stores when it’s enabled only for one

 -  Review Reminder
     +  Added store view column to grid
     +  Order number added in grid and info tab
     +  Added config to disable reminders for guests
     +  Fixed grouped products review link

 -  SEO Suite
     +  XML Sitemap - Improved image generating for big catalogs

 -  Testimonials
     +  Added config option to disable/enable customer profile picture
     +  Separate options for testimonials list and form
     +  Added config option - min length for testimonial at frontend

### Version 1.14.0

> May 22, 2019

 -  Fixed ghost scrolling to the top when sticky header is used.
 -  Prevent horizontal scrollbar when resizing window with sticky header.
 -  RTL styles improved.
 -  Minor improvements for AskIt and Testimonials.

**Modules fixes & improvements**

 -  AMP:
     +  New feature to remove tag or attribute for AMP variant of the page. Use 'data-tmamp-remove' attribute.
     +  Prevent duplicates in 'amphtml' url on configurable product pages.

 -  Email:
     +  Added config option to enable/disable history saving.

 -  Pagespeed:
     +  Remove chunk name (full action name) from merged file. It reduces disk space usage and reuses already generated files.
     +  Improve HTML parse to prevent messing up page.

 -  SEO Suite:
     +  Rich Snippets: solve latest Google warnings; new config option to map product structured data with product attributes.
     +  XML Sitemap: prevent duplicate alternate locales.

### Version 1.13.0

> Feb 26, 2019

 -  New option for Luxury design - enable/disable transparent header for homepage.
 -  Improved RTL styles for Luxury and Essence design.
 -  Optimize menu sticking for Flat design. Reduce JavaScript resource consumption.
 -  Improved compatibility with PHP 7.2.

**Modules fixes & improvements**

 -  Ajax Pro:
     + Improve handling of Magento messages after adding product to cart when Stock Inventory is enabled.

 -  Ask It:
     +  Add plain text section to email templates to improve emails quality.
     +  Few minor improvements to frontend templates (simplify layout and render elements only when it is necessary).

 -  Easybanner:
     +  Fixed slow scrolling performance in Chrome when fixed banners are shown.

 -  Navigation Pro:
     +  Fix page jumping on scroll at mobile devices when nowrap feature for menu is enabled.

 -  Pagespeed:
     +  Improved compatibility with AMP and others third-party extensions.

 -  Pro Labels:
     +  Fix Integrity constraint violation error for manual labels when Customer Groups filter is enabled.

 -  SEO Suite:
     +  Metadata templates - improve module stability during metadata generation.
     +  Rich Snippets - don’t add social links to organization snippet when there is no values in social links.
     +  HTML Sitemap - add canonical URL to sitemap page.


### Version 1.12.0

> Oct 30, 2018

 -  [PageSpeed](/m1/extensions/pagespeed/) extension included into Argento package.
 -  Overall themes and extension stability improvements (AjaxPro, EasyTabs, Highlight).

 -  AskIt:
     +  Fix empty customer new in email.

 -  EasyTabs:
     +  Fix missing conditions on 2nd level in product tabs.

 -  LightboxPro:
     +  Fix broken gallery widget.

 -  SEO Suite:
     +  Rich Snippets - fix validation error "id is null" at product page.
     +  HTML Sitemap - show only enabled CMS pages in sitemap.

 -  Testimonials:
     +  Fixed rating stars validation.

### Version 1.11.0

 -  We added fantastic option to stick product image and/or product details at product page for every theme . Read more at [Product Page configuration](../luxury/product-page/).
    ![Sticky product image example](/images/argento/luxury/product-page/sticky-image-example.gif)

 -  New feature to change produt image layout at product page. You can have default (old-school) layout or fancy mobile-friendly slider.

**Major modules changes**

 -  AMP:
     +  Update deprecated mustache library to the version 0.2.

 -  GDPR:
     +  Improved compatibility with old php versions.
     +  Added missing translations.

 -  Lightbox Pro:
     +  New option for product page image. You can select between default layout with thumbnails and slider with all images.
     +  Overall code improvements.

### Version 1.10.0

 -  New highly in demand **GDPR module** is included in Argento package. Read more about this module at [our documentaion site](/m1/extensions/gdpr/).
 -  Fix duplicated H1 element in header of Luxury theme.
 -  Luxury theme supports FontAwesom icons. Please apply [upgrade instruction](../upgrade-instructions/#version-195---1100).
 -  RTL support for Flat theme.
 -  Improved compatibility with Magento 1.7.x.
 -  Minor CSS improvements.
 -  Improved source code of included modules (use of unified image uploader from TM Core in admin interfaces).

**Major modules changes**

 -  Attribute Pages:
     +  Fixed error when page identifier is entered in invalid registry.

 -  Hover Gallery:
     +  Integration with ManaDev Layered Navigation.

 -  Navigation Pro:
     +  New awesome [*Nowrap* feature](/m1/extensions/navigationpro/use-cases/nowrap/). It always keep top level menu items in single row. And it is responsive.

 -  SEO Suite:
     +  Metadata Templates: improved attribute directive output for numeric attributes (truncate trailing zeros in decimal part).

 -  Sold Together:
     +  Fix ‘product ID already exists’ error on checkout success page.
     +  Respect “Reindex… via Cron” config options. Cron process ignored config settings in previous versions.


### Version 1.9.6

 -  Full RTL support for Argento Argento and Argento Luxury themes.
 -  New '404' page at Luxury theme so your customers don't be upset but interested in staying at your store.
 -  New expanded layout for product tabs.
 -  Fix issue with 'More Products' button on product listing (content not loading, incorrect image sizes, black image background).
 -  Fix not woking "Estimate shipping" and "Apply coupon" forms at checkout cart page on Magento version less than 1.9.2.0.
 -  Overall stability and source code improvements.

**Modules fixes & improvements**

 -  Ajax Pro:
     +  Fix JavaScript error on shopping cart page when AjaxPro is disabled for this page.

 -  Attribute Pages:
     +  Improve compatibility with Magento Enterprise Edition.

 -  Easy Catalog Images:
     +  Improve responsive styles for widget layouts with 3 and 5 columns.

 -  Easytabs:
     +  New tabs layout - expanded tabs. You can change tabs layout in extension system config or in widget options.
     +  New option "Sticky tabs header" - tabs header sticks to top of the screen while tabs conteiner is in user viewport. You can enable sticky option in extension system config or in widget options.
     +  Overall source code improvements.

 -  Highlight:
     +  New carousel template with ajax content loading.

 -  Hover Gallery:
     +  Compatibility with new Highlight carousel template.

 -  Lightbox Pro:
     +  Improve extension stability.

 -  Navigation Pro:
     +  Improve behavior on stores with Argento themes and RTL contant direction.

 -  SEO Suite:
     +  SEO Templates - improve 'products' directive for category templates. Works with attributes that are not filterable also.

 -  Sold Together:
     +  Cron option works only on global level of config. So it is removed on other config levels.

 -  Testimonials:
     +  Fix missing message after posting new testimonial.

### Version 1.9.5

 -  Added new breathtaking config sections for every Argento theme - 'Category page and other listing pages' and 'Product page'. There you can setup product image resize options for listing pages, widgets and product pages. Check how this config looks at [Luxury image size settings for category](../luxury/category/#image-size).
 -  Load Google fonts with javascript librery webfontloader to improve pagespeed score in Luxury, Pure2, Flat and Argento themes.
 -  Source code improvements.
 -  Reduced number of templates. Check [upgrade instruction](../upgrade-instructions/#version-194---195) to find out what templates you can get rid of.

**Modules fixes & improvements**

 -  AMP:
     +  Added ability to disable layered navigation output via configuration.
     +  Attributepages 1.4.0 support added.
     +  Magento’s Cookie Restriction Mode support added.
     +  Fixed possible "Content mismatch" error when using third-party layered navigation modules.
 -  Ask It:
     +  Fixed 'reached 100 match iterations' when URL end with `/`.
     +  Fixed customer email template in nl_NL locale.
 -  Easytabs:
     +  Scroll to "Review form" itself instead of top of Review section when visitor clicks "Add review" link on product page.
 -  Facebook Like Button:
     +  Added options to setup size of og:image that facebook uses in shared URLs.
 -  Prolabels:
     +  Added new position for label - 'hidden'. With help of this position you can hide label on product page or category page.
 -  SEO Suite:
     +  XML Sitemap - prevent memory leak during sitemap generation.
 -  Sold Together:
     +  Added new option to reindex orders with specific statuses only.
     +  Fixed javascript error at some environments "groupSymbol is undefined".
     +  Fixed crush of cron reindex on huge number of orders (10K+).

### Version 1.9.4

 -  Fixed scroll bar in IE when Hover Gallery enabled
 -  Fixed invisible images in Luxury theme in "More Views" section when
    lazy-load module is used

**Modules fixes & improvements**

 -  AMP
    - Fixed product page slider animation on rtl theme
    - Fixed bug when user can't read error message after adding product to the cart
    - Attribute "checked/" is not allowed error fixed
 -  Easyslide
    - Fixed possible js errors
 -  Prolabels
    - Fixed possible broken html markup
    - Prevent label wrapper from stretching out of parent container
    - Significant code cleanup and code improvement
 -  Testimonials
    - Added check if guest is allowed to write a review
    - Code cleanup
 -  Stability improvements in AjaxPro, Askit, Lightboxpro modules

### Version 1.9.3

 -  Fixed critical vulnerability in EasyBanner module
 -  Fixed Easyslider styles on AMP theme

### Version 1.9.2

 -  Fixed error on last step of default magento checkout with Luxury theme.
 -  Argento themes always load custom css/js files at the end.
 -  Fixed missing form action on checkout/cart page for Magento versions
    before 1.9.2.0.
 -  Improved styles for Luxury theme.

**Modules fixes & improvements**

 -  Ajax Pro:
     +  Fix missing JS resources on home page for ajax actions (add to cart,
        add to compare, add to wishlist).

 -  Easy Tabs:
     +  Add missing initialization for custom links on tabs.

 -  Highlight;
     +  Fixed empty setLocation method, when ajaxpro is used. It caused issues
        with add to cart functionality on homepage.


### Version 1.9.1

 -  Improved compatibility with Amasty_ShopBy module
 -  Improved suggestpage product listing styles
 -  Improved Askit styles on product page
 -  Fix onhover icons positioning when prolabels disabled
 -  Fixed missing frontend translation fopr the 'More' phrase
 -  Fixed W3C validator error with unset HEIGHT property at homepage
 -  Fixed php notice when saving theme editor changes
 -  PHP code cleanup

### Version 1.9.0.1

 -  Fixed missing icons at Luxury theme when CSS merge enabled.
 -  Removed deprecated render templates for checkout cart. Please follow
    upgrade instructions for [package version 1.9.0](../upgrade-instructions/#version-186---190).

### Version 1.9.0

 -  New vivid theme included into package - Luxury theme. Checkout
    [Luxury Theme Demo](http://magento1demo.argentotheme.com/luxury_en/).
 -  Updated templates for checkout cart page.
 -  Unified sizes of product images at product listing and widget grids. It
    reduces size of media cache.
 -  JavaScript and CSS improvements.

**Modules fixes & improvements**

 -  AjaxPro:
     +  Qty Switcher added on product reviews page.
     +  Minor CSS and JavaScript improvements for popups

 -  AMP:
     +  Fixed bugs with actions at google AMP cache pages (Add to Cart, Add to
        Compare, Add to Wishlist)

 -  AskIt:
     +  Remove duplicated `div.left` element at product questions block.

 -  Facebook Like Button:
     +  New "like button" layout - custom button. It renders on server side,
        consumes less browser resources and provides possibility of CSS
        customization.

 -  ProLabels:
     +  Do not render empty container for content labels if there are no
        labels.

 -  SEO Suite:
     +  Metadata templates: fix price directive (respect tax config -
        include/exclude tax; remove decimal trailing zeros).

### Version 1.8.9

 -  Advanced layout settings for Argento and Pure themes. Now every theme in
    package can have full width or boxed layouts. How to change theme pages
    width you can read in
    [this article](http://docs.swissuplabs.com/m1/argento/page-layout/) at our
    documentation site.
 -  New SEO extension included in package - SEO Templates. Read more about it
    at [our documentaion site](/m1/extensions/seo-templates/).
 -  Reduced inline JavaScript.
 -  Removed enquire.js and replaced with matchMedia. JavaScript polyfill for
    older browsers included.
 -  Minor styles and javascript improvements (include deferred loading of wow,
    photoswipe, matchMedia polyfill and sticky-kit libs).

**Modules fixes & improvements**

 -  Ajax Search:
     +  Fixed compatibility with layered navigation on search result page when
        custom collection enabled.

 -  AMP:
     +  Added ability to use ['data-amp-' attribute](/m1/extensions/amp/use-cases/#change-css-class-name)
    for any tag
     +  Fixed 'Add to Cart' functionality on google search pages
     +  Fixed AMP validation errors with the following attributes `noshade`,
        `align`, `border` and `size`.

 -  Easy Banner:
     +  Fix redirect for banners when URL start with slash.

 -  Easy Flags:
     +  New style for language and store switcher - popup.

 -  Easy Tabs:
     +  Minor SEO improvement - tab titles as second level headers (h2).

 -  Easyslide:
     +  New slider option in adnvanced section - 'Space between slides'.

 -  ProLabels:
     +  Fixed missing labels when enabled option 'Move to content on mobile'.


### Version 1.8.8

**New fatures**

 -  Full compatibility with Magento 1.9.3.3.
 -  New styles for product review form. Ratings stars react to mouse hover.
 -  Fix missing product images for Pure 2 theme on retina displays.
 -  Updated styles for add to cart section on product page.

**Modules fixes & improvements**

 -  Ajax Pro:
     +  Improved handling of Magento messages
     +  CSS arrows for quantity switcher
     +  Updated styles for Quantity switcher elements on product page,
        category page and shopping cart

 -  Ajax Search:
     +  correct placeholder behavior for search field

 -  AMP:
     +  Fixed non-working add to cart, in case secure url is used but not for
        the product page
     +  Added support for products lists at homepage
     +  Added support for buttons with onclick="setLocation" attribute
     +  Better compatibility with third-party product listings

 -  Attribute Pages:
     +  MassDelete action in backend grids

 -  Easy Banners:
     +  Condition to show lightbox/awesomebar banner once a day/week/month per
        customer

 -  Easy Tabs:
     +  Do not hook click on review link at product page if reviews block is
        not in tab
     +  Period (.) allowed for tab alias

 -  Prolabels:
     +  Fix notice "Undefined variable" when stock labels render
     +  Improved backend interfaces
     +  Include Mobile_Detect lib only if it is nessecery

 -  SEO Suite:
     +  Improved intagration of XML Sitemap with Fishpig extension

### Version 1.8.7

**New features**

 -  New animated checkboxes and radio buttons (chrome, safary and mobile
    browsers support with fallback to default styles for other browsers).
    Read [Argento FAQ](../faq/#how-to-change-checkboxradio-button-color) if you want to know how to customize them.
 -  Fancy stars instead of boring select boxes in Product Review forms.
 -  Significantly improved styles of web forms (according modern trends).
 -  Product tabs with conditions (customer group, product attributes).
 -  SEO Suite 0.5.0 included in package. Current version of SEO Suite has
    RichSnippets, HTML and XML Sitemap.

**Modules fixes & improvements**

 -  AMP:
     +  Fixed empty ‘ShopBy’ popup for categories without children and layered
        navigation
     +  Improvend allowed tags and attributes filter

 -  AskIt:
     +  Added canonical URLs to extension pages on store frontend
     +  Fixed javascript errors at some stores when resources merge and
        minification enabled

 -  Attribute Pages:
     +  Improved extension stability (at some stores image resize caused error)

 -  Easyslide
     +  New slider options to stop slider on mouse hover and enable lazy load
        feature
     +  Fixed issue with slider controls on pages with multiple sliders

 -  Easytabs
     +  Added conditions for prodcut and wdget tabs (customer group and product attributes)

 -  Sold Together
     +  Added option to reindex orders only for last N days and you can
        specify value for N in your store system config.

### Version 1.8.6.1

 -  Updated slider styles for each theme to match original styles
 -  Fixed jumbotron styles, when inner content is floated
 -  Improved `BlockToggler` script for complex block markup

### Version 1.8.6

After successfull source files update you have to run data update. You can
find more details about data update at
[Upgrade Instructions for 1.8.6](../upgrade-instructions/#version-186).

**New Features**

 -  Accelerated Mobile Pages (AMP) extension included in package. You can
    read more about AMP extension at our [docs](/m1/extensions/amp/). Disabled
    by default.
 -  Product image hover feature added to package. It shows different
    image when visitor hovers mouse on product image in product listing.
    Disabled by default.
 -  Easyslide 3.0 with swiper library. Now slider supports touch and work
    smoothly on mobile devices.

**Modules fixes and improvements**

 -  Ajax Pro:
     +  fix redirect to cart after adding product to cart when minimal order
        amount enabled
     +  fix issue with empty cart when customer logged in and persistent
        shopping cart enabled (cart does not have items that were added when
        customer was not logged in)
     +  improved ajax update of cart related blocks

 -  Ajax Search:
     +  fix missing layered navigation on search results page when custom
        collection enabled
     +  fix different placeholders in search field when field has input cursor
        and has not

 -  Easy Banners:
     +  great performance improvements for stores with long-lived banners
     +  new banner conditions

 -  Easy Tabs:
     +  fixed issues with permissions to extension interfaces in Magento Admin
     +  fixed issue with lost tabs after extension update
     +  allow inline translation of attribute group name on additional tab

 -  Facebook Like Button:
     +  use Facebook SDK JavaScript version 2.8
     +  improved system configuration section (added comments and dependencies)
     +  improved and unified extension templates
     +  all inline JavaScripts moved to js-file

 -  Navigation Pro:
     +  no inline javascript, js-file deferred

 -  Sold Together:
     +  fix js error and incorrect total price for bundle product if one of
        items is out of stock

 -  Testimonials:
     +  improved integration with edit review form in Magento Admin
     +  fixed fatal error on review edit form in some environments

### Version 1.8.5

[Upgrade Instructions](../upgrade-instructions/#version-184---185)

**New Features**

 *  New homepage and footer markup in ArgentoPure and ArgentoMall designs
    using Bootstrap grid system
 *  [Easy Flags extension](/m1/extensions/easyflags/) is included in Argento
    Theme Package

**Fixes and Improvements**

 *  Easy Tabs 3.0 and Easy Flags 3.0 integration
 *  Minor css fixes
 *  Load external fonts with one request in Argento Flat
 *  Video of the day moved to static block in Argento Mall

**Modules fixes and improvements**

 *  Ajax Pro
     -  Crosssell block integration added

 *  Ajax Search
     -  Improved frontend styles (fixed problem with "jumping" search Argento
        themes)

 *  AskIt
     -  Fixed product url generation for emails
     -  Mass answers status change action added in Magento Admin
     -  Corrected block type for askit_tabbed block in layout
     -  Fixed bug about showing answers with pending status on frontend
     -  Missing translations added
     -  Question grid item column sorting and filtering fixed
     -  Vote table customer foreign key bug was fixed
     -  Export action was fixed

 * Easytabs (major update)
    -  Product tabs and Widget tabs
    -  Extension has its own widget (now you can place tabs any where you want)
    -  Group attributes in "Additional Information" tab (optional)

### Version 1.8.4

[Upgrade Instructions](../upgrade-instructions/#version-183---184)

**New Features**

 *  new homepage and footer markup in ArgentoPure2 design using Bootstrap grid
    system
 *  new products grid design
 *  new extension added - Quantity Switcher. [View Docs](http://docs.swissuplabs.com/m1/extensions/qty-switcher/)

**Fixes and Improvements**

 *  minor translation fixes
 *  20 overriden templates removed
 *  testimonials integration improved
 *  visual accent added to downloadable product link
 *  backend css now merged with rest of css files

**Modules fixes and improvements**

 *  Ajax Pro:
     -  added +/- buttons for product quantity change on product page
     -  improved magento 1.9.3 integration
     -  fixed bug "$j undefined"

 *  Easy Banners:
     -  added columns "Store view", "Banner content" in banner backend grid to make easier banners management
     -  fixed grid search in banned conditions for pages (issue occures on latest magento versions)
     -  fixed redirect issue for SEO url (.html)


 *  Navigation Pro:
     *  fixed incorrectly escaped `&gt;`, `&lt;` entities

 *  Product Label
     *  minor improvments for labels rendering

 *  Rich Snippets
     *  added possibility to show prices with/without VAT (prices with VAT enabled by default)

 *  Review Reminder
     *  fixed incorrect product name translation
     *  added config to disable reminders for guests
     *  added order number and store view columns in grid

 *  Sold Together
     *  error 404 in config fixed
     *  css fixes

 *  Testimonials
     *  sidebar list widget rewritten
     *  added feature to save product review as testimonial from review edit page
     *  missing captcha in testimonials widget fixed
     *  added config to allow guests to submit testimonials

### Version 1.8.3

**New Features**

 -  Magento 1.9.3 compatible
 -  New extension added - Slick Carousel. [View Docs](http://docs.swissuplabs.com/m1/extensions/slick-carousel/), [View Examples](http://docs.swissuplabs.com/m1/extensions/slick-carousel/usage/#using-in-argento)
 -  You can now create Amazon style menu with Navigation Pro. [View Manual](http://docs.swissuplabs.com/m1/extensions/navigationpro/use-cases/amazon-menu/)

**Fixes and Improvements**

 -  Removed easyslider box-shadow in Flat theme
 -  Removed horizontal scrollbar in Chrome between 980px and 990px
 -  Fixed missing FontAwesome icons after homepage save
 -  Added products count limit for sidebar related block (ArgentoFlat and Pure2 themes)
 -  Small css and js fixes

**Modules fixes and improvements**

 -  ConfigurableSwatches
    - Improved image swapping method
    - 1.9.3 support added
 -  Easy Catalog Images:
    - 'more in...' translation added in csv
 -  Highlight
    - integration with Slick Carousel added
 -  Easy Tabs
    - Fixed scroll to review form
    - JS file now loaded and executed with defer attribute
    - no inline javascript
 -  Ajax Pro
    - Catalog category view js script improvements
    - Improved third-party theme's integration
    - Imporoved logic to activate `current_page` in toolbar
    - Updated translations
 -  Navigation Pro
    - Added ability to create [Amazon-style](http://docs.swissuplabs.com/m1/extensions/navigationpro/use-cases/amazon-menu/) menu
    - Added status exception rules into cache key to fix invalid
        menu on different devices;
    - Small css fixes

### Version 1.8.2

**New Features**

 -  New homepage and footer markup in ArgentoFlat design using Bootstrap grid
    system

**Fixes and Improvements**

 -  20 overriden templates removed from Flat theme
 -  Fixed catalog configurable swatches output in layered navigation

**Modules fixes and improvements**

 -  Ajax Pro
     -  Styles for cart popup after buying product fixed
     -  Core magento translations for login form
 -  Ajax Search
     -  Unified templates
     -  Improved suggestions popup rendering
 -  Easy Tabs
     -  Scroll to review bug fixed
     -  Fixed disabling extension from magento backend
 -  Easy Slide
     -  Slides overlay fixed (slides stacked one on other during loading
        than first slide jumps on top)
     -  Slider rendering bug when slider name starts with digit fixed
 -  Lightbox Pro
     -  Incorrect initial position of thumbnails in Firefox fixed
     -  JS error related to *lightbox.js* when JS merge enabled fixed
 -  Prolabels
     -  JS file loads and executes with defer attribute
     -  no inline javascript
     -  significantly reduced html content generated by extension
 -  Rich Snippets
     -  correct names of breadcrumbs
 -  Sold Together
     -  integration with Checkout Success 2.x extension from our team
     -  hide already ordered products as recommendation in email blocks

### Version 1.8.1

**Perfomance Improvements**

 -  AjaxSearch scripts refactored and inline js completely removed from templates
 -  Js improvents for currency and language dropdowns in all argento themes

**Bugfixes**

 -  Fixed custom.css sort order:
    Custom.css should be added after theme.css to allow to customize all theme
    styles
 -  Fixed highlight filters by stock status and quantity for the following
    product types:
     -  Bestsellers
     -  Popular
     -  Products
     -  Recent reviews

### Version 1.8.0

[Upgrade Instructions](../upgrade-instructions/#version-174---180)

**New Features**

 -  Bootstrap grid system added
    - New homepage and footer markup in ArgentoArgento design
    - Resized homepage images to match Bootstrap powered grid system sizing

**Fixes and Improvements**

 -  Fixed css resources sort order to improve CSS parallel loading
 -  Fixed catalog configurable swatches on non-anchored categories
 -  EasyTabs: fixed JS error on product page when it has no tabs
 -  Easyslide: overall performance improvements and optimization
 -  Highlight: widget interface improvements, new filters by inventory added
 -  Lightbox Pro: css optimizations
 -  Review Reminder:
    - Use proper settings according order store id
    - Fixed translations for mail sent via cron

### Version 1.7.4

 -  FontAwesome updated to version 4.6.3
 -  backend CSS loads depends on request - secured or unsecured
 -  Ask It
     -  new frontend responsive design
     -  question can be assigned to multiple products
     -  question create date fixed
 -  Lightbox Pro
     -  significant code refactoring
     -  JS files load with 'defer' attribute and do not block page rendering
     -  no more inline JS
 -  Navigation Pro
     -  fixed third level drop-downs on tablet devices
 -  ProLabels
     -  fixed label priority determination
 -  Testimonials
     -  stars for 'Rating' field at new testimonial form
     -  JS files load with 'defer' attribute
 -  Suggest Page
     -  avoided potential error with multiple calls of event
        'sales_quote_product_add_after'
