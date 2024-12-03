---
layout: default
title: ChatGPT Assistant for Shopware
description: ChatGPT Assistant for Shopware Documentation
category: ChatGPT Assistant Shopware
---

# sw6-chat-gpt-assistant

## Installation (developer way)

```bash
cd <shopware_root>
composer config repositories.sw6-chat-gpt-assistant vcs git@github.com:swissup/sw6-chat-gpt-assistant.git
composer require swissup/sw6-chat-gpt-assistant:dev-master --prefer-source
symfony console plugin:refresh
symfony console plugin:install SwissupChatGptAssistant --activate
symfony console cache:clear
symfony run bin/build-administration.sh
```
## Features

Extension allows to generate content with the help of ChatGPT AI. You can create and use predefined prompts or write custom requests in chat popup.

OpenAI API key is required. You can get it here: [OpenAI API](https://platform.openai.com/account/api-keys)

Supported fields:

 -  Product Description
 -  Product Meta Title (SEO)
 -  Product Meta Description (SEO)
 -  Product Keywords (SEO)
 -  Category Description
 -  Category Meta Title (SEO)
 -  Category Meta Description (SEO)
 -  Category Keywords (SEO)

![Product Description](/images/shopware/chat-gpt-assistant/product.png)
![Product Seo](/images/shopware/chat-gpt-assistant/seo.png)

## Configuration  (Extensions -> My Extensions -> Chat GPT Assistant plugin)

Option  | Description
--------|--------------------------------------------------
Enable  | Allows to enable/disable plugin per sales channels
Api Key | Enter [OpenAI API](https://platform.openai.com/account/api-keys) key
Model   | Enter model used for generation, e.g. `gpt-3.5-turbo`, `gpt-4`, etc. Find more at [Models Documentation](https://platform.openai.com/docs/models) page.

![configuration](/images/shopware/chat-gpt-assistant/configuration.png)

## Usage

With our extension you can generate content in two ways.

### Black ChatGPT Icon ![black](/images/shopware/chat-gpt-assistant/black.png)

You can send a request to chatGPT by pressing the black chatgpt icon near the associated field  near product description for example.
Request will be sent using the default prompt and chatGPT response will be inserted into the field.
> Please note that any existing field content will be replaced.

You can then edit the content if needed and save the product and/or category.

### Green ChatGPT Popup Icon ![green](/images/shopware/chat-gpt-assistant/green.png)

If you need more control over the content generation process or want to send a custom prompt, press the chat button to open popup window.
Here you can edit existing prompt and run it.
> Please note that any existing field content will be replaced.

You can then edit the content if needed and save the product or category.


https://github.com/swissup/sw6-chat-gpt-assistant/assets/412612/e3fae459-f7c5-4f22-8718-f5da0bbdcade
