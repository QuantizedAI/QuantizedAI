---
layout: default
title: Facebook Like Button installation
description: Facebook Like Button installation instructions
keywords: "Facebook Like Button installation"
category: Facebook Like Button
exclude_from_search: true
---

# Manual Installation

{% include installation/m2/manual.html package="swissup/fblike" %}

## Add Like Button To Catalog

add code to any place in catalog list.phtml:

```php
<?php echo $this->helper('Swissup\Fblike\Helper\Like')->getProductLike($_product); ?>
```

That's all. Now you need [Create a New Facebook App][facebook_app] and configure extension in admin panel [Configuration][configuration]

#### After installing the extension you can go to:

* [Create a New Facebook App][facebook_app]
* [Configuration][configuration]

[facebook_app]: /m2/extensions/facebooklikebutton/app/
[configuration]: /m2/extensions/facebooklikebutton/configuration/
