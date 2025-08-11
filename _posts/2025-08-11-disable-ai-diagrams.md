---
layout: post
author: draw.io
slug: disable-ai-diagrams
date: 2025-08-11 09:24:00
title: Configure draw.io online to disable AI diagrams 
tags: [features]
categories: [features]
---

Like many software apps, diagramming tools now have AI-powered features that 'help' you diagram. These can be premium features and may not be easily disabled. With the free online draw.io editor, you have access to the smart templates feature by default. It's easy to disable this in draw.io - configure the editor or use the fully offline draw.io Desktop app. 

<img src="/assets/img/blog/configure-drawio-example.png" style="width=100%;max-width:400px;height:auto;" alt="All version of draw.io are highly configurable, with options for custom colours and fonts, and to enable or disable specific features">

**Note:** [Smart templates](/blog/smart-diagram-generation.html) are disabled by default in the draw.io apps for Confluence - ask your instance administrator to [configure the draw.io editor](/doc/faq/configure-diagram-editor.html) if you want to (and are allowed to) use this feature. 

While draw.io only shares the [text you enter as the query](/blog/write-query-generate-diagram.html) to generate a diagram using a smart template, and only at the time of generation. draw.io does not share your diagram data.

However, other diagramming applications may have to share your diagram data so their AI features can suggest changes to your diagram. 

If you need to include sensitive data or draw confidential diagrams, your diagramming application must not share your diagram data.

## Use an offline tool like draw.io Desktop

Since version 10.7.5, draw.io Desktop has been a fully offline application. You do not need a connection to the internet to use all the built-in shape libraries and templates, or use your own custom shape libraries, fonts or templates stored on your device.

Smart templates are not available in [draw.io Desktop](/blog/diagrams-offline.html). 

<img src="/assets/img/blog/desktop.png" style="width=100%;max-width:500px;height:auto;" alt="The draw.io desktop app works on MacOS, Windows and Linux">

Choose your platform (Windows, macOS or Linux), and [download draw.io Desktop](https://get.diagrams.net/) to start diagramming securely and privately.

**Tip:** Many extra template and example diagrams are available in the [JGraph/drawio-diagrams](https://github.com/jgraph/drawio-diagrams) repository on GitHub. Download these in advance to use them in draw.io Desktop.


## Configure the draw.io web application

Alternatively, you can run the web app while offline as a [progressive web app](/doc/faq/offline.html), or configure the editor in your browser to disable the smart templates feature.

All versions of the draw.io application are highly configurable, including but not limited to:
* default palette colours and styles
* default and custom fonts
* custom templates and a customised template library
* default and custom shape libraries to automatically open by default 
* default page and grid size 

Here's a full list of the [draw.io editor configuration options](/doc/faq/configure-diagram-editor.html) for the web application, draw.io Desktop, and the draw.io apps for Confluence Cloud and DC.

By default, only the online draw.io web application has the experimental ChatGPT support enabled. To [disable the smart templates feature](/doc/faq/smart-templates-diasble.html), add a line to the editor configuration. 

### Disable smart templates in the draw.io configuration

This removes the Smart Templates section from the template library, as well as the _Generate_ option in the [search field](/blog/search-omnibox.html) and draw.io menus. 

1. Select _Extras > Configuration_ from the menu, or _... > Settings > Configuration_ from the toolbar. 
<br /><img src="/assets/img/blog/extras-configuration-menu.png" style="width=100%;max-width:400px;height:auto;" alt="Access the draw.io configuration via Extras > Configuration">
3. Add the following JSON string to the configuration: ``"enableChatGpt": false``
<br /><img src="/assets/img/blog/configuration-chatgpt-false.png" style="width=100%;max-width:300px;height:auto;" alt="Set the enableChatGpt option to false in the draw.io configuration to disable smart templates and the Generate option in search">
1. Click _Apply_ to save your changes. Reload the browser tab to load the new draw.io configuration and disable the smart templates feature. 

**Note:** If you set the [``lockdown`` option](/blog/data-governance-lockdown.html) to ``true`` in the draw.io configuration, this will also disable the smart templates feature. 

