---
layout: default
title: PDF Invoices Changelog
description: PDF Invoices for Magento 2 Changelog
keywords: magento pdf invoices changelog
category: PDF Invoices
---

# Changelog

### Version 1.4.6

> Jul 19, 2023

 -  Do not add PDF attachment to email when entityId is missing
 -  Fixed access to undefined constant

### Version 1.4.5

> Mar 22, 2023

 -  Replaced Zend namespace with Laminas

### Version 1.4.4

> Dec 12, 2022

 -  Fixed missing barcodes

### Version 1.4.3

> Nov 16, 2022

 -  PHP 8.1 compatibility fix: passing null to base64_decode

### Version 1.4.2

> Oct 18, 2022

 -  Replaced `header` tag with `div` to fix broken sales pdf style
 -  Fixed missing logo image in PDF templates
 -  Displaying order creation date without time by default. Use `created_at_formatted_full` variable to display it with time.

### Version 1.4.0

> Apr 18, 2022

 -  Fixed PDF templates in Magento 2.4.4. [More info here](/m2/extensions/pdf-invoices/known-issues/#magento-244-compatibility).
 -  Converted php schemes into xml format

### Version 1.3.5

> Apr 15, 2022

 -  PHP 8.1 compatibility fix

### Version 1.3.4

> Aug 27, 2021

 -  Added en_US translation csv file

### Version 1.3.3

> Feb 11, 2021

 -  Magento 2.4.2 compatibility: fixed undefined method error

### Version 1.3.2

> Jan 15, 2021

 -  Fixed product image display in items grid in Magento 2.4.1
 -  Fixed js error if codemirror has a toolbar

### Version 1.3.1

> Dec 14, 2020

 -  Added two new PDF template designs in the style of Argento Stripes and Luxury themes

### Version 1.3.0

> Nov 5, 2020

 -  Added two new PDF template designs
 -  Fixed download link in Magento 2.3.6/2.4.0
 -  Attachment name now includes increment id
 -  Added configuration option to select address template used in PDF

### Version 1.2.2

> Oct 19, 2020

-  Magento 2.4.1 compatibility

### Version 1.2.1

> Aug 1, 2020

 -  Fixed not working `Add New Template` button in templates grid (Magento 2.4 compatibility)

### Version 1.2.0

> Jul 22, 2020

 -  You can now send PDF as an attachment in sales email
 -  Fixed tracking information error in shipment PDF on Magento 2.3.3 and newer

### Version 1.1.1

> Jun 30, 2020

 -  Fixed insert variable in Magento 2.3.3
 -  Switch to using Codemirror module
 -  Catch possible errors when creating pdf

### Version 1.1.0

> Sep 03, 2019

 -  Added barcode and QR code support, check [manual](/m2/extensions/pdf-invoices/use-cases/#using-barcodes-and-qr-codes)
 -  Added product image to items table, check [manual](/m2/extensions/pdf-invoices/use-cases/#display-product-image-in-items-table)
 -  Added sku barcode to items table, check [manual](/m2/extensions/pdf-invoices/use-cases/#display-product-sku-barcode-or-qr-code-in-items-table)
 -  Added config for page size and orientation

### Version 1.0.0

> Jun 18, 2019

 -  Initial release
