---
layout: post
author: draw.io
slug: diagrams-google
date: 2025-07-10 09:54:00
title: Use draw.io diagrams in Google Docs, Slides and Sheets
tags: [features, integrations]
categories: [features]
---

Diagrams help you convey complex information faster and more accurately, helping your audience understand your documents more easily. Export your draw.io diagrams to PNG image files and then import them into your Google Docs, Slides and Sheets - drag and drop the image file into your document. 
<br /><img src="/assets/img/blog/drawio-google-image.gif" style="width=100%;max-width:500px;height:auto;" alt="Export a draw.io diagram to a PNG image, then import it into your Google document">

1. Open your ``.drawio`` diagram file in the draw.io editor (either our [online editor](https://app.diagrams.net) or [draw.io Desktop](https://get.diagrams.net/))
2. In the draw.io menu, select _File > Export As > PNG_, then click _Export_ to save your diagram as an image. 
3. In your Google Document, Slide, or Sheet select _Insert Image_ from the menu, or drag and drop your image into your document. 

<img src="/assets/img/blog/drawio-google-slide.gif" style="width=100%;max-width:500px;height:auto;" alt="Export a draw.io diagram to a PNG image, then import it into your Google presentation slide">

You can work with the image of your diagram in your Google document (Docs, Slides or Sheets) as you would any other image - you can move, resize, rotate, and style it as needed.

## Reopen your diagram from a draw.io image file

If you export your diagram from draw.io to a PNG image with _Include a copy of my diagram_ enabled, you will be able to drop that image file onto the draw.io editor to load the diagram data embedded in that file and continue diagramming. 
<br /><img src="/assets/img/blog/export-png-options.png" style="width=100%;max-width:200px;height:auto;" alt="Choose the export settings for the PNG image">

**Note:** You cannot reopen images from within Google documents as diagrams as Google strips the embedded diagram data.

## Diagrams in Google Sheets

In Google Sheets, you can either import an image of your diagram into a cell or overlay the cells. 
<br /><img src="/assets/img/blog/drawio-google-sheet.gif" style="width=100%;max-width:500px;height:auto;" alt="Export a draw.io diagram to a PNG image, then import it into your Google spreadsheet">

## Deprecated: draw.io apps for Docs, Sheets and Slides

Previously, the [draw.io apps for Google Docs, Slides and Sheets](/doc/faq/google-docs-diagrams.html) allowed you to embed the diagrams directly into your documents. Unfortunately, Google has instituted [new security permissions limitations](https://github.com/jgraph/drawio/issues/4589#issuecomment-2857181827) that limit access to your files stored on Google Drive. This means that new installations of the draw.io apps for Docs, Slides or Sheets are unable to access the diagram data in those files. 

If you have older, installed versions of these apps, you may be able to continue to embed and work with diagram file in your documents. 

**Important:** We have not disabled the Google Store listings for these apps as that would immediately disable all existing installations. Currently, those older installed versions of these apps still work. 

We recommend you convert your embedded diagrams to images in those documents. 

The [draw.io apps for Google Workspace](https://gsuite.diagrams.net/) and the [draw.io Chrome app for Google Drive](/blog/drawio-chrome-app.html) are unaffected - you can continue to store your ``.drawio`` diagram files in Google Drive and work with them in our [free online editor](https://app.diagrams.net).  

<img src="/assets/img/blog/google-docs-examples.png" style="max-width:100%;height:auto;"  alt="It's easy to import images of diagrams in Google Docs">