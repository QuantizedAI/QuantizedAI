---
layout: default
title: Argento custom theme
description: How to create Argento-based custom theme
keywords: >
    argento theme, custom theme, argento customization
category: Argento
---

# Argento custom theme

Creating Argento sub-theme gives you unlimited possibilities in theme
customization. Unlike [css customization](/m2/argento/customization/custom-css/),
custom theme allows you to change much more things:

- Layout instructions
- Template files
- Javascripts
- Css styles

> Using Argento sub-theme, you guarantee that all Argento files left untouched and
> you can unpack new Argento version over the old one without losing your
> modifications

## Contents
{:.no_toc}

* TOC
{:toc}

### Create custom theme

#### Terminal command
{:.collapsible}

 1. Open terminal and navigate to magento home folder.
 2. Run the following command:

    > Please replace `[essence|flat|pure2|mall|stripes|luxury|force|home|marketplace]`
    > with theme name, you'd like to use.

    ```bash
    bin/magento swissup:theme:create Local/my-theme [essence|flat|pure2|mall|stripes|luxury|force|home|marketplace]
    ```

 3. Log in to Magento backend and navigate to Content > Themes. You should see
    new theme in the list.
 4. That's all. [Apply your new theme now](#apply-custom-theme)

#### Manual
{:.collapsible.collapsed}

Please replace `[essence|flat|pure2|mall|stripes|luxury|force|home|marketplace]` entries with
theme name, you'd like to use

 1. Create folder for your new theme:

    ```
    app/design/frontend/Local/my-theme
    ```

 2. Create following files inside new theme directory, to register your
    theme in Magento:

    1.  composer.json

        ```json
        {
            "name": "local/my-theme",
            "type": "magento2-theme",
            "version": "1.0.0",
            "require": {
                "swissup/theme-frontend-argento-[essence|flat|pure2|mall|stripes|luxury|force|home|marketplace]": "*"
            },
            "autoload": {
                "files": [ "registration.php" ]
            }
        }
        ```

    2.  theme.xml

        ```xml
        <theme xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xsi:noNamespaceSchemaLocation="urn:magento:framework:Config/etc/theme.xsd">
            <title>Local custom theme</title>
            <parent>Swissup/argento-[essence|flat|pure2|mall|stripes|luxury|force|home]</parent>
        </theme>
        ```

    3.  registration.php

        ```php
        <?php

        use Magento\Framework\Component\ComponentRegistrar;

        ComponentRegistrar::register(ComponentRegistrar::THEME, 'frontend/Local/my-theme', __DIR__);

        ```

 3. Log in to Magento backend and navigate to Content > Themes. You should see
    new theme in the list.
 4. That's all. [Apply your new theme now](#apply-custom-theme)

#### View Examples
{:.collapsible.collapsed}

If you have trouble when creating new theme, please take a look at our examples
at [github repository](https://github.com/swissup/theme-frontend-argento-custom).

### Apply custom theme

Navigate to _Content > Design > Configuration_, select the store you wish
to apply a theme, and select your theme in "Default Theme" section:

![Design Configuration](/images/m2/argento/customization/custom-theme/configuration.png)

Save configuration, clear cache, and check the frontend.

### Enable theme editor for custom theme

> Supported since theme-editor version 1.9.8

By default, custom theme doesn't inherit theme editor changes. If you want
to apply the changes to your custom theme (inherited from one of Argento themes)
you should explicitly indicate this in theme view.xml file:

 1. Open `etc/view.xml` file inside your custom theme. If it doesn't exist, create it:

    ```xml
    <?xml version="1.0"?>
    <view xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:noNamespaceSchemaLocation="urn:magento:framework:Config/etc/view.xsd">
    </view>
    ```

 2. Add the following code into the file (between `<view>` tags):

    ```xml
    <vars module="Swissup_ThemeEditor">
        <var name="code">THEME_EDITOR_CODE</var>
    </vars>
    ```

 3. Replace `THEME_EDITOR_CODE` with one of the following values:

    - swissup_absolute
    - swissup_argento_chic
    - swissup_argento_essence
    - swissup_argento_flat
    - swissup_argento_force
    - swissup_argento_home
    - swissup_argento_luxury
    - swissup_argento_mall
    - swissup_argento_marketplace
    - swissup_argento_pure
    - swissup_argento_pure2
    - swissup_argento_stripes

    > Make sure your theme is a child of selected theme.

 4. Save the file, clear cache, and check the frontend.

#### Next Up
{:.no_toc}

- [Customization](../)
- [Change page layout](../change-page-layout/)
