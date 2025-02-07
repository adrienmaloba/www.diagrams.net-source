---
layout: post
author: draw.io
slug: adaptive-colours
date: 2025-02-07 10:13:00
title: Using adaptive colours to diagram in light and dark modes
tags: [features]
categories: [features,shapes,text,connectors]
---

When you change from light to dark mode in draw.io, the colours automatically switch intensity so that your diagram and its labels are easy to read. You can set now specific colours for shapes, connectors, text and the diagram page background for both light and dark modes via the updated colour palette. 
<br /><img src="/assets/img/blog/style-colour-palette-custom.png" style="width=100%;max-width:500px;height:auto;" alt="An additional custom colour scheme has been added to the style palette in draw.io">

Adaptive colours are important when part of your team prefers to work in [dark mode](/blog/dark-mode-diagrams.html), and the rest prefers light mode. 

## Colour style - use a specific dark and light colour

1. Select one or more shapes, connectors, text labels, or the diagram background, then click on a colour block to open the colour palette, for example, the _Fill_ colour of a shape.
<br /><img src="/assets/img/blog/adaptive-colors-open-palette.png" style="width=100%;max-width:200px;height:auto;" alt="Select one or more shapes and open the colour palette">
1. Click _Advanced_ to see the dark mode colour settings in the palette.
<br /><img src="/assets/img/blog/adaptive-colors-advanced.png" style="width=100%;max-width:150px;height:auto;" alt="Select one or more shapes and open the colour palette">
1. Enter a colour value in the Light mode field (sun). The dark mode value will update automatically to its inverse if you are using the _Automatic_ adaptive colour setting.
2. To use a specific dark mode colour instead, enter a different colour value in the Dark mode field (moon). This colour is now _User-defined_.
<br /><img src="/assets/img/blog/adaptive-colors-set-both.png" style="width=100%;max-width:150px;height:auto;" alt="Select one or more shapes and open the colour palette">
1. Click _Apply_ to save the colour style to your selected shapes, connectors, text or diagram page background. 

You'll notice that the colour block now has two triangles, in both dark and light mode. 
<br /><img src="/assets/img/blog/adaptive-colors-user-defined.png" style="width=100%;max-width:400px;height:auto;" alt="Change the adaptive colours settings on a diagram in draw.io via the Extras menu or the Style tab in the format panel when nothing is selected">

**Tip:** To use the same colour in dark and light modes, enter the same value in both fields. 


## Adaptive colour settings

Each page in a multi-page diagram has its own adaptive colour setting. 

With nothing selected in your diagram page, click on the diagram _Style_ tab. Change the _Adaptive Colors_ setting. Alternatively, select _Extras > Adaptive Colors_ from the menu. 
<br /><img src="/assets/img/blog/style-tab-adaptive-colors.png" style="width=100%;max-width:300px;height:auto;" alt="Change the adaptive colours settings on a diagram in draw.io via the Extras menu or the Style tab in the format panel when nothing is selected">

* **Automatic:** Changes the intensity to enhance the contrast of all coloured elements in a diagram. This is set by default.
* **Simple:** Improves the contrast of only the black and white elements, and retains all other colours. Thus the same palette can be used in dark and light modes. 
* **None:** Disables adaptive colours in dark mode completely. Diagrams will appear as they would in light mode even if you enable dark mode in the draw.io editor. 

<img src="/assets/img/blog/style-tab-adaptive-colors.gif" style="width=100%;max-width:500px;height:auto;" alt="Change the adaptive colours settings on a diagram in draw.io via the Extras menu or the Style tab in the format panel when nothing is selected">

Set ``defaultAdaptiveColors`` in the draw.io configuration to ``simple`` or ``none`` when you want your diagram colours to stay the same in light and dark modes. 
<br /><img src="/assets/img/blog/adaptive-colors-configured-default.png" style="width=100%;max-width:150px;height:auto;" alt="Select one or more shapes and open the colour palette">

**Step by step:** [Configure default adaptive colours](/doc/faq/adaptive-colors-configure-default.html)

### Sharing diagrams with adaptive colours

The adaptive colour settings are saved in the diagram file. When you share your diagram file, a URL link with the diagram or HTML code with the diagram embedded, when it is reopened in the editor, the diagram will display with the adaptive colour settings it was saved with.

## Related

[Diagrams pose a particular challenge](https://github.com/jgraph/drawio/discussions/4773) when automatically adjusting colours for readability in dark mode.

If you want to reset a diagram to automatically adapt to dark mode, you can [remove all the user-defined dark-mode colours](/doc/faq/adaptive-colors-remove-user-defined.html).

See how to [set custom dark-mode colours in the style and colour palettes](/doc/faq/custom-colours-confluence-cloud.html) with the light-dark function for each color definition.

Learn more about how adaptive colours work when you [export to an SVG image](/doc/faq/export-to-svg.html).