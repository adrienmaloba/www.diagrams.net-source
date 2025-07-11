---
layout: post
author: draw.io
slug: search-omnibox
date: 2025-07-03 09:54:00
title: Search for shapes, in-diagram text, help and more with the new search omnibox
tags: [shapes, features]
categories: [features, shapes]
---

The search field in draw.io has been extended. In addition to shape search, you can now open various features from the menu via the search field, generate a smart template, apply styles to text, and more. The omnibox search field can speed up your diagramming workflow. 
<br /><img src="/assets/img/blog/search-omnibox.png" style="width=100%;max-width:400px;height:auto;" alt="The draw.io search feature is now an omnibox providing quick access to options and diagram tools, as well as searching the shape libraries">

**Note:** As this feature is currently under development, useful tools will be added to the search omnibox over time. If you have a suggestion, please [raise a feature request on the JGraph/drawio GitHub repository](https://github.com/jgraph/drawio/issues).

## Search for shapes

The default search using the new omnibox is to [search for shapes](/doc/faq/shape-search.html) in all the built-in shape libraries. 

1. Click in the search field.
2. Type the name of the shape or icon you are looking for and press _Enter_. 
3. Shapes that match your search term will appear below the search field. Click on _More_ to see additional shapes.
<br /><img src="/assets/img/blog/search-omnibox-shapes.png" style="width=100%;max-width:400px;height:auto;" alt="Type the name or type of shape in the drawio search and press enter to search for shapes">

## Find text in your diagram

You can now search for text that appears in shape and connector labels, tags, tooltips and custom shape properties via the new search omnibox. 

**Note:** This in-diagram search is not case sensitive. 

In the example below, one shape has the ``lambda`` tag, another has a tooltip ``lambda``, a third has a custom ``type`` shape property with the same text, and the third has ``lambda`` its shape label. 
<br /><img src="/assets/img/blog/search-omnibox-in-diagram.gif" style="width=100%;max-width:600px;height:auto;" alt="Search for text in labels, tags, tooltips, shape properties via the draw.io search omnibox">

1. Type the text you wish to find in your diagram.
2. Select _Find in Diagram_ to open the [Find/Replace dialog](/doc/faq/find-shapes.html). 
3. Click _Find_ to step through all shapes and connectors that contain the text you searched for. 
<br /><img src="/assets/img/blog/search-omnibox-in-diagram.png" style="width=100%;max-width:250px;height:auto;" alt="Click Find to step through all matching shapes and connectors that contain the text you entered as the search term">

**Tip:** Enable the options to search with a _Regular Expression_, or to find matching text on _All Pages_ within a multi-page diagram. 

## Generate a smart template

Type in a description of a diagram in the search field and select _Generate_.
<br /><img src="/assets/img/blog/search-omnibox-generate.png" style="width=100%;max-width:200px;height:auto;" alt="Describe a diagram and select Generate from the search omnibox to quickly generate a smart template in draw.io">

This will open the template library and generate a smart template. Click on the template to see a larger preview and click _Insert_ to add it to the drawing canvas. 
<br /><img src="/assets/img/blog/search-omnibox-generate2.png" style="width=100%;max-width:400px;height:auto;" alt="CHange your query and regenerate the smart template, and insert it onto the draw.io drawing canvas via the template library">

[_Learn more about smart templates_](/blog/smart-diagram-generation.html)

## Access draw.io features quickly

Some menu options are also available in the search omnibox. For example:

* Searching for ``import`` shows two options you can select from: open the _Import_ dialog or open the dialog to import an _Image_ file.
<br /><img src="/assets/img/blog/search-omnibox-features.png" style="width=100%;max-width:180px;height:auto;" alt="Search for draw.io features in the new search omnibox to avoid having to hunt through the menus">

* Select one or more shapes or connectors in your diagram, then type ``Bold`` or ``Italic`` in the search field. Select _Bold_ or _Italic_ from the omnibox list to apply that style to those selected diagram elements. 

* Search for ``Clear`` when you have selected a connector to see the _Clear Waypoints_ option.
<br /><img src="/assets/img/blog/search-omnibox-clear.png" style="width=100%;max-width:600px;height:auto;" alt="Search for draw.io features in the new search omnibox to avoid having to hunt through the menus">

* Search for the name of a diagram page that is not the one you are currently editing. Click on the name to open that diagram page in the editor. This is useful for diagram that contain a large number of diagram pages.
<br /><img src="/assets/img/blog/search-omnibox-page.png" style="width=100%;max-width:350px;height:auto;" alt="Search for the name of a draw.io diagram page and click on it to open that page in the editor">

This list remembers and shows you the last five search actions you selected - an ideal way to 'bookmark' the tools and menu options that you use often. 

**Note:** Only a limited number of tools are available in the new search field at the moment. Raise a feature request to suggest the features you'd like us to add to the search omnibox over on the [JGraph/drawio repository](https://github.com/jgraph/drawio/issues). 

