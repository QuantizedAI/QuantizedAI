---
layout: default
title: Easy Slider Installation
description: magento slider module installation
keywords: >
  magento slider on homepage, magento slider extension, magento image
  slider, magento slider on product page "
category: Easy Slider
---

# Easy Slider installation instructions

Please follow next steps to complete the installation:

1. Go to store backend, navigate to `Admin > Tools > Compilation` and deactivate the compilation mode.
2. Go to your magento store root directory (via FTP or CPanel).
3. Create file `maintenance.flag` in root directory.
4. Open your store in browser. You have to see page `Service Temporarily Unavailable`. If you can not see this page, then probably you try to install extension at wrong magento instance. So, please, stop installation and try to find out where is your magento instance.
5. Unpack all files from extension archive into your magento store root directory.
6. Remove file `maintenance.flag` when copy process completed.
7. Login your store admin, refresh your magento store cache and start to configure extension.

You can read how to create slider at
[Easy Slide Admin Interface](../backend/#admin-interfaces) page.

### Update extension from 2.3.2 to 2.4.0

After updating extension you can delete deprecated files and directories
to keep your magento instance clean and tidy:

```
app/code/local/TM/Easyslide/etc/system.xml
app/design/frontend/base/default/template/tm/easyslide/load.phtml
app/design/frontend/base/default/template/tm/easyslide/slider.phtml
skin/frontend/base/default/tm/easyslide/images
skin/frontend/base/default/tm/easyslide/js/jquery-1.8.2.min.js
skin/frontend/base/default/tm/easyslide/nivo
```

### Update extension from 2.5.0 to 3.0.0

After updating extension you can delete deprecated files and directories
to keep your magento instance clean and tidy:

```
app/code/local/TM/Easyslide/controllers/IndexController.php
app/design/frontend/base/default/template/tm/easyslide/easyslider.phtml
app/design/frontend/base/default/template/tm/easyslide/nivoslider.phtml
app/design/frontend/tmamp/default/template/tm/easyslide/easyslider.phtml
app/design/frontend/tmamp/default/template/tm/easyslide/nivoslider.phtml
js/tm/lib/easyslider
js/tm/lib/nivo
```


Please, feel free to contact us about any additional questions:

* [Support](https://swissuplabs.com/contacts/)
* [Forum](https://swissuplabs.com/magento-forum/)