---
layout: default
title: Improved Admin Security Installation
description: How to install Improved Admin Security module
category: TFA
exclude_from_search: true
---

# Installation

{% include installation/m2/composer.html package="swissup/tfa" %}


![2018-05-25 17-15-34](https://user-images.githubusercontent.com/412612/40549149-65439a1a-603f-11e8-950c-106fbf7590b1.png)

* TFA must be enabled by the individual user by clicking 'Account Setting(user)' in the Magento 2 admin panel.
* Once there, the user is able to enable the two factor authentication and view the QR code for a Google Authenticator compatible application.
* Users with TFA enabled will not be able to log into the admin panel without a valid authentication code input on the Magento 2 admin login page.
* Users with TFA disabled can leave the 'Authenticator Code' field blank during login.

### Activating the extension

* Open your admin user account settins at `System > Permisions > All Users >
Your User > Tab "Two Factor Authentication"`

* Scan QR code with Google Authenticator application using your smartphone.

* Insert the key you've got on your mobile device into the verification key field.

* That's all. You've enabled the protection for that admin user. Try logout
and login with verification key. Please notice that key is got refreshed every
30 seconds. In case you have not enabled the protection for some users, the
verification key will be ignored for those users.

### Google Authenticator Apps:

To use the two factor authentication, your user will have to install a Google Authenticator compatible app, those are some of the currently available:

* [Authy for iOS, Android, Chrome, OS X](https://www.authy.com/)
* [FreeOTP for iOS, Android and Pebble](https://apps.getpebble.com/en_US/application/52f1a4c3c4117252f9000bb8)
* [Google Authenticator for iOS](https://itunes.apple.com/us/app/google-authenticator/id388497605?mt=8)
* [Google Authenticator for Android](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2)
* [Google Authenticator (port) on Windows Store](https://www.microsoft.com/en-us/store/p/google-authenticator/9wzdncrdnkrf)
* [Microsoft Authenticator for Windows Phone](https://www.microsoft.com/en-us/store/apps/authenticator/9wzdncrfj3rj)
* [LastPass Authenticator for iOS, Android, OS X, Windows](https://lastpass.com/auth/)
* [1Password for iOS, Android, OS X, Windows](https://1password.com)
