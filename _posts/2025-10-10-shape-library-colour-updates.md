---
layout: post
author: draw.io
slug: shape-library-colour-updates
date: 2025-09-10 09:43:00
title: Shape library updates for multi-colour shapes
tags: [shape libraries]
categories: [use-cases, shape-libraries]
---

There are many shapes in the draw.io shape libraries that use more than one line or fill colour. These shapes are being updated so you can change each of the colours and style your diagram with more flexibility. 
<br /><img src="/assets/img/blog/aws-3d-colours-dark.png" style="width=100%;max-width:500px;height:auto;" alt="The updated AWS shapes allow you to customise all of the colours in the shapes">

As the collection of shape libraries is rather large in draw.io, it will take some time to update all of those that contain multi-coloured shapes. The first two libraries that have been updated are Mockups and the AWS 3D shapes. 

Each shape still contains a Fill and a Line (outline) colour that typically forms the background colour and the outer line colour of the shape. The additional colours are defined with new, customisable style settings. 

For example, the Mockup Map shape has a white background and black outline, but also internal areas with different fill colours and a different internal outline colour. 
<br /><img src="/assets/img/blog/shapes-extra-colours-map.png" style="width=100%;max-width:400px;height:auto;" alt="The updated Mockups Map shape has many customisable internal fill and outline colours">

The list of fill and outline colours will be different for each shape.
<br /><img src="/assets/img/blog/shapes-extra-colours.gif" style="width=100%;max-width:500px;height:auto;" alt="The updated Mockups and AWS 3D shape libraries allow you to customise multi-colour shapes">

**How it works**

A ``default`` attribute was introduced for the ``fillcolor`` and ``strokecolor`` attributes. 

Each shape has a list of ``defaultFillColors`` and ``defaultStrokeColors`` attributes which are used to show the customisable colours in multi-colour shapes. These are comma-separated lists that define the default colours in the ``fillColorStyles`` and ``strokeColorStyles`` attributes within a shape.

Right click on a shape, then edit the colour style attributes, then click _Apply_.
<br /><img src="/assets/img/blog/shapes-extra-colours-edit-style.png" style="width=100%;max-width:300px;height:auto;" alt="Right click on a shape and select Edit Style to change the colours of the shape directly">


**Which libraries have been updated?**

The updated AWS 3D and Mockups shape libraries are available now in the current version of the web-based draw.io editor. The Cloud and IT shape libraries are in the process of being updated to this new, more flexible system of colours. Multi-colour shapes in other shape libraries will be updated after the IT shapes are finished. 

Go to [app.diagrams.net/clear.html](https://app.diagrams.net/clear.html) to ensure you are using the most recent version of the online draw.io editor.


## Gradients with multi-coloured shapes

The gradient option in the _Style_ tab of the format panel will use the main background fill colour. The gradient does not apply to any of the other additional colour styles within the multi-colour shape.
<br /><img src="/assets/img/blog/shapes-extra-colours-gradient.png" style="width=100%;max-width:400px;height:auto;" alt="The updated Mockups Map shape has many customisable internal fill and outline colours">

## Reset to the original colour styles 

To revert to the original colour, the easiest is to copy the original style from an unstyled shape and apply it to the customised shape. 
1. Select the unstyled shape. In the Style tab, click _Copy Style_.
2. Select the customised shape. In the Style tab, click _Paste Style_. 
<br /><img src="/assets/img/blog/shapes-extra-colours-copy-style.gif" style="width=100%;max-width:500px;height:auto;" alt="The updated Mockups and AWS 3D shape libraries allow you to customise multi-colour shapes">

[Learn more about styling shapes](/doc/faq/shape-styles.html)