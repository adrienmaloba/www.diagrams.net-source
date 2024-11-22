---
layout: post
author: draw.io
slug: ibm-technical-diagrams
date: 2024-11-15 09:43:00
title: New IBM Cloud shape library for technical diagrams
tags: [shape libraries]
categories: [use-cases, shape-libraries]
---

The new _IBM Cloud_ shape library in draw.io (right) reflects IBM's updated design language, and extends the existing _IBM_ shape library (left) with a wide range of additional groups, connectors and infrastructure components.
<br /><img src="/assets/img/blog/ibm-shape-libraries.png" style="width=100%;max-width:500px;height:auto;" alt="Enable the new IBM and IBM shape libraries to draw IBM infrastructure diagrams">

IBM has provided their updated shapes for the new IBM Cloud shape library in draw.io. Please refer to their documentation for their [design language style guide](https://www.ibm.com/design/language/infographics/technical-diagrams/design), where they explain how shapes and icons should be used in a wide variety of technical diagrams.

**Enable the IBM shape libraries in draw.io**

1. Click on _More Shapes_ at the bottom of the shapes panel in draw.io. 
2. Enable the checkbox next to the _SAP_ shape library in the _Networking_ section and click _Apply_. 
<br /><img src="/assets/img/blog/shape-library-ibm-enable.png" style="width=100%;max-width:300px;height:auto;" alt="Enable the IBM shape libraries to draw IBM infrastructure diagrams">

**Tip:** There are also several IBM infrastructures in the template library. Select _Arrange > Insert > Template_ from the menu or _+ > Template_ in the toolbar, and look in the _Cloud > IBM_ category.
<br /><img src="/assets/img/blog/ibm-template-library.png" style="width=100%;max-width:300px;height:auto;" alt="draw.io has several example IBM infrastructures in the template library">

## Using old and new IBM shapes in one diagram

The new IBM Cloud shapes are compound shapes - a coloured background shape and an icon on top in the centre. This gives you more flexibility in styling your diagram as you can change the two shapes' fill colours independently. 

The older shapes are round with a white icon and blue text label, while the new IBM Cloud shapes are square with a white icon and text (in light mode) or black icon and text (in dark mode). 

There is also a larger and more varied set of groups (region shapes) in the new _IBM Cloud_ shape library.
<br /><img src="/assets/img/blog/ibm-infrastructure-cloud-icons.png" style="width=100%;max-width:600px;height:auto;" alt="The new IBM Cloud shapes work well with the older IBM shape library in draw.io">
<br />The example above is one of the IBM templates available in draw.io with the new IBM Cloud shapes replacing some older components.

Both sets of shapes work well when diagramming in dark mode - the new shapes will switch icon and label colours automatically to remain readable.
<br /><img src="/assets/img/blog/ibm-dark-light-mode.png" style="width=100%;max-width:600px;height:auto;" alt="The new IBM Cloud shapes automatically swap colours to remain readable in dark and light mode in draw.io">

**Tip:** To make the labels look the same on all of your IBM and IBM Cloud shapes, you'll need to edit the text labels to ensure their case matches and the _Font Color_ in the _Text_ tab of the format panel. 

However, mixing shapes from the two shape libraries and using their default label styles shows which components of your infrastructure are more recent at a glance, such as for IBM's newer cloud and Watson AI services.

## Make your own IBM shapes

The shapes in both the _IBM_ and _IBM Cloud_ shape libraries represent only part of the constantly expanding IBM Design Language.

You can easily make your own IBM shapes in draw.io using the black IBM ``.svg`` icons.

1. Add one of the _IBM Cloud_ shapes that matches the colour you want to use to the drawing canvas to serve as a template for your new shape. 
2. Add a simple rectangle from the _General_ shape library.
3. Select the IBM Cloud shape on the drawing canvas and select then select _Copy Size_ in the _Arrange_ tab of the format panel. Select the rectangle and click on _Paste Size_.
4. Select the IBM Cloud shape again, then select _Copy Style_ in the _Style_ tab of the format panel. Select the rectangle again and click on _Paste Style_. 
<br /><img src="/assets/img/blog/ibm-make-new-shape1.gif" style="width=100%;max-width:300px;height:auto;" alt="Make your own IBM shape using an existing IBM Cloud shape as a template for style and size">
5. You may need to deselect the _Line_ checkbox in the _Style_ tab, but your shape background should now look correct. 
6. Add a label, and move its _Position_ to the _Bottom_ via the _Text_ tab of the format panel.
6. Now, make the compound icon. Drag the ``.svg`` file of the UI icon from the [UI Icons list in the IBM Design Language](https://www.ibm.com/design/language/iconography/ui-icons/library/) - either from the webpage directly, or from your device - onto the drawing canvas to import it. Then drag it over the centre of the background square.
7. Finally, drag a selection box around the new compound shape, right click and select _Group_ from the context menu.
<br /><img src="/assets/img/blog/ibm-make-new-shape2.gif" style="width=100%;max-width:300px;height:auto;" alt="Make your own IBM shape using an existing IBM Cloud shape as a template for style and size">

**Tip:** To use this new shape in multiple diagrams, drag the group onto the [Scratchpad](/doc/faq/scratchpad.html) in the shapes panel. 
<br /><img src="/assets/img/blog/ibm-scratchpad-shape.png" style="width=100%;max-width:200px;height:auto;" alt="Make your own IBM shape and save it in the draw.io scratchpad">

You can also save the Scratchpad with your custom shapes to share them with your colleagues.

1. Click on the pencil to the right of the _Scratchpad_ library.
<br /><img src="/assets/img/blog/ibm-scratchpad-edit.png" style="width=100%;max-width:150px;height:auto;" alt="Edit the draw.io scratchpad and export the shapes in it to a custom shape library">
2. Select _Export_ to save all the shapes in the Scratchpad to a custom shape library.
<br /><img src="/assets/img/blog/ibm-export-scratchpad.png" style="width=100%;max-width:300px;height:auto;" alt="Edit the draw.io scratchpad and export the shapes in it to a custom shape library">
3. Enter a filename, select where to save the custom shape library file and click _OK_.
<br /><img src="/assets/img/blog/ibm-save-custom-shape-library.png" style="width=100%;max-width:250px;height:auto;" alt="Edit the draw.io scratchpad and export the shapes in it to a custom shape library">

[Learn more about custom shape libraries](/blog/custom-libraries.html)