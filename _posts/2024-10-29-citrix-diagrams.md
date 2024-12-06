---
layout: post
author: draw.io
slug: citrix-diagrams
date: 2024-10-29 09:43:00
title: Updated Citrix shape library for clean infrastructure diagrams
tags: [shape libraries]
categories: [use-cases, shape-libraries]
---

The new _Citrix_ shape library helps you to draw Citrix diagrams of complex infrastructures that are easier to read. The older 3D shapes are still available in the _Citrix (legacy)_ shape library. 
<br /><img src="/assets/img/blog/shape-library-citrix.png" style="width=100%;max-width:500px;height:auto;" alt="Enable the new Citrix shape library to draw Citrix infrastructure and network diagrams">

Citrix is a popular secure centralised platform for deploying applications, desktops and virtual solutions to devices in large enterprises with locations distributed worldwide, especially where high availability and scalability is required. 

[Learn more about drawing infrastructure and network diagrams](/blog/network-diagrams.html)

**Enable the new Citrix shape library in draw.io**

1. Click on _More Shapes_ at the bottom of the shapes panel in draw.io. 
2. Enable the checkbox next to the _SAP_ shape library in the _Networking_ section and click _Apply_. 
<br /><img src="/assets/img/blog/shape-library-citrix-enable.png" style="width=100%;max-width:300px;height:auto;" alt="Enable the new Citrix shape library to draw Citrix infrastructure diagrams">

## Citrix infrastructure diagram tips

* Use **regions** to visually group segments, security zones, and workloads. A simple rectangle [placed behind](/blog/move-shapes-forwards-backwards.html) a group of systems or services is the simplest option. You could also use [collapsible container shapes](/doc/faq/collapse-expand-enable-disable.html) or AWS groups.
<br />[<img src="/assets/img/blog/citrix-infrastructure-example.png" style="width=100%;max-width:500px;height:auto;" alt="Use rectangles with different fill colours and line styles">](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=0&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fcitrix-network2.drawio)

* Use [**shape fill colours and outline styles**](/doc/faq/shape-styles.html) consistently to visually indicate regions, types and grouping of services or tools, or show which teams are responsible for maintaining those infrastructure areas. 
  
* Use **application, device and platform logos** where possible. [Search for these by name](/doc/faq/shape-search.html) in the top left of the shapes panel in draw.io. Hover over any shape to see a larger preview.
<br /><img src="/assets/img/blog/citrix-shape-search.png" style="width=100%;max-width:300px;height:auto;" alt="Search for infrastructure shapes and tool logos using their names">

* Add a **legend** if necessary. This is especially important when working with external parties, as they may not be familiar with all the components in your infrastructure. 

* **Align shapes** using the [blue guidelines](/blog/snap-to-grid.html) that appear as you move them around the drawing canvas. 
<br /><img src="/assets/img/blog/citrix-guidelines.png" style="width=100%;max-width:300px;height:auto;" alt="Align shapes using the snap to grid and guideline tools for neat diagrams">

* To [**group shapes**](/doc/faq/group-shapes-connectors.html) once you have drawn a subsystem and placed it in a region, drag a selection box around all the shapes, right-click and select _Group_ from the context menu. Now you can move the group without losing its internal layout. 

## Draw multi-platform infrastructure diagrams

Enable the _AWS_, _Google Cloud Platform_ and _Azure_ shape libraries in draw.io to document your multi-environment infrastructure. 

You can use the [up-to-date shapes](/blog/gcp-aws-shapes-network-diagrams#updated-gcp-icons.html) in the _AWS groups_,  _GCP Zones_ and cards from the Google Cloud Platform libraries to indicate different regions. Alternatively, place an identifying shape in the top left corner of a basic rectangle shape, [move the shape label](/blog/text-alignment.html) to the right and position it neatly with custom spacing.
<br /><img src="/assets/img/blog/citrix-region-labels.png" style="width=100%;max-width:400px;height:auto;" alt="Align shapes using the snap to grid and guideline tools for neat diagrams"> 

This will let you show how sub-systems are isolated and confined to each region in your cloud platforms and how loads are distributed when using the Citrix Hybrid Multi-Cloud.
<br />[<img src="/assets/img/blog/citrix-hybrid-infrastructure-example.png" style="width=100%;max-width:500px;height:auto;" alt="Use rectangles with different fill colours and line styles">](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=0&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fcitrix-hybrid-infrastructure.drawio)
<br />[_Open this example in the diagram viewer_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&page=0&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fcitrix-hybrid-infrastructure.drawio)

## Related

Basic infrastructure templates are under _Cloud_ and _Network_ in the template library. Select _Arrange > Insert > Template_ from the menu or click _+ > Template_ in the toolbar.
<br /><img src="/assets/img/blog/templates-network-diagrams.png" style="width=100%;max-width:300px;height:auto;" alt="Example infrastructure diagrams using various platforms are available in the template library"> 

Additional examples are in the [drawio-diagrams repository on GitHub](https://github.com/jgraph/drawio-diagrams). Check for [cloud](https://github.com/jgraph/drawio-diagrams/tree/dev/templates/cloud) and [network](https://github.com/jgraph/drawio-diagrams/tree/dev/templates/network) templates, and more detailed [examples](https://github.com/jgraph/drawio-diagrams/tree/dev/examples). You can [import a diagram](/blog/example-diagrams-github.html) into draw.io as a template using its raw GitHub URL.

Some platforms can automatically generate AWS, GCP or Azure diagrams of your implemented infrastructure. [Cloudcraft](/blog/drawio-aws-cloudcraft.html) and [Cloudockit](/blog/cloudockit-to-drawio.html) can export to the ``.drawio`` or ``.vsd`` formats. Select _File > Import from_ or drag and drop this file onto the drawing canvas to [import the diagram](/doc/faq/import-diagram.html) of that sub-infrastructure.