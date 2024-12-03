---
layout: default
title: Helpmate Changelog
description: Helpmate Changelog
keywords: Helpmate chanlog
category: Helpmate
---

# Changelog

### Version 1.7.18

> Jan 8, 2021

**Fixes**
 - Add light status,proirity etc. changes
 - If the file does not exist, it will be created


### Version 1.7.13-17

> Sep 4, 2020

**Fixes**
 - Comment timeout undisable submit button
 - Add dom:loaded wrapper
 - Prevent many submiting
 - Debounce ticket submiting
 - add form_key param
 - Add getFormKey in new ticket block

### Version 1.7.12

> May 24, 2019

**Fixes**
 - Fixed missing page title at contacts page (overriden) when layout cache is enabled
 - Add patch for issue #68 (Problem with Referrer-Policy strict-origin header)
 - Get configured email template by store id

### Version 1.7.11

**Fixes**
 - Improve markup for ticket/new/attached template.
 - Add proper referer Url to Ticket_Theard_New block.
 - Improve close ticket checkbox for Ticket_Theard_New block.
 - Set active link in for navigation at view ticket page on storefront.

### Version 1.7.10

**Fixes**
 - Fix \$\$('#global_search').present() is undefined
 - Fix require_once HTMLPurifier
 - Fix potential xss

### Version 1.7.9

**Fixes**
 - Improve JavaScript code stability for admin interface
 - Workaround to show SELECT elements hidden with materialized
 - Fix frontend rating functionality
 - Revert 'show/hide editor button'
 - Fix cron task methods locations

### Version 1.7.8

**Fixes**
 - Fix 'User get empty email when private message is posted' close #65

**Improvments**
 - Rename helpmate_send_ticket_answer => helpmate_notify_customer_ticket_change
 - Split big class Observer.php

### Version 1.7.7

**Fixes**
 - Fix 'User get empty email when private message is posted' close #65

**Improvments**
 - Rename helpmate_send_ticket_answer => helpmate_notify_customer_ticket_change
 - Split big class Observer.php

### Version 1.7.7

**Fixes**

 -  Fix line breaks bug on the frontend

**Added**

 -  Added Materialize design to tickets view

### Version 1.7.6
 - Fix getTimeAgo
 - Fix getFileUrl without default store id

### Version 1.7.5

 - Update translates
 - Move archive email to bbc header
 - Fix double event call bug (helpmate_notify_customer_ticket_create)
 - etc.

### Version 1.7.4

 - Set default priority value for usePriorityOnFrontend == false case
 - Disable unsupported dashboard tickets grid functionality
 - Fix encoding bug

### Version 1.7.3

 - Fixed incorrect ticket identification by In-Reply-To header
 - etc.

### Version 1.7.2

 - Remove code dublication
 - Fix xss
 - Fix empty letter bug (change status)
 - Improve MEQP
 - etc.

### Version 1.7.1

 - Fix MEQP
 - Blacklist email logic was improved

### Version 1.7.0

 - Fix lost guest email bug
 - Improved attachments rendering

### Version 1.6.9

 - Fix not show attachments bug
 - Improved attachments rendering on backend

### Version 1.6.8

 - Add opened tickets count in admin header
 - Check if user is logged in when showing file
 - Fixed error when break time is empty
 - Add check before dapartment remove
 - Add decorate name for ticket grid
 - Don't send email for blacklist emails
 - fetch_enable conf option was added
 - Last replier column was 'added'
 - Improve __addNewTheard logic
 - Fix bug double send email when ticket create from backend
 - Trim email
 - Add ticket from backend call helpmate_notify_customer_ticket_create
 - Code cleanup
 - Unix encoding


#### You can also check:

*   [Installation](../installation/)
*   [Configuration](../configuration/)
*   [Use Cases](../use-cases/)
*   [Support](https://swissuplabs.com/contacts/)
*   [Forum](https://swissuplabs.com/magento-forum/)
