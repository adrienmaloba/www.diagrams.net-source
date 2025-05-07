---
layout: post
author: draw.io
slug: home-lab-diagrams
date: 2025-05-06 09:43:00
title: Home lab and smart home diagrams
tags: [shape libraries]
categories: [features, use-cases, shape-libraries]
---

Over on the _home lab_, _home networking_ and _smart home_ subreddits, it has been fantastic to see diagrams of increasingly complex home computing and network setups being shared.  Diagrams help home you understand the physical and logical connections between networked devices, and are useful for setting up security zones, upgrading hardware and debugging connection problems.
<br /><img src="/assets/img/blog/home-lab-example-dark.png" style="width=100%;max-width:500px;height:auto;" alt="A home network example with many smart home components">

_Home lab_, _home hub_, _home network_ and _smart home_ diagrams are the common terms used interchangeably to refer to a range of infrastructure diagrams. These diagrams may organise devices and components by physical location, by security and access, by cabled connections, or in another logical grouping. 

## Draw custom smart home shapes

Many Internet of Things (IoT) devices and services are used in smart homes. These are rapidly developed and shape libraries in technical diagramming apps can't keep up. In draw.io, you can create your own custom shapes for these devices.

The example above uses the new [Network 2025 shape library](/blog/network-library-shadow.html), with many custom shapes for smart devices and home appliances. 

1. Use _Search Shapes_ to find and add multiple shapes from the draw.io libraries.
2. Drag a selection box around all the shapes that make up your custom shape, right click and _Group_ them together. 

For example, this custom wall heater shape uses four overlapping _hairpin exchanger_ shapes, grouped together. 
<br /><img src="/assets/img/blog/home-lab-custom-shapes.png" style="width=100%;max-width:400px;height:auto;" alt="Make a new custom shape by combining and group multiple shapes from the draw.io shape libraries">

The custom hub shapes below combine _rounded rectangles_, _circles_, _ethernet_ port shapes, and a _delay_ shape as an antenna.
<br /><img src="/assets/img/blog/home-lab-make-custom-shape.png" style="width=100%;max-width:600px;height:auto;" alt="Make a new custom shape by combining and group multiple shapes from the draw.io shape libraries">
<br />A custom hub shape lets you:
* label each port
* attach connectors to the ethernet port shapes within the custom shape

### More ways to create custom shapes

**Edit an existing shape:** [Change the attachment points](/doc/faq/shape-connection-points-customise.html) of the _Network_ library's switch shape so connectors sit more neatly on each port. The mesh and router shapes have been edited to have four fixed connection points.
<br /><img src="/assets/img/blog/home-lab-edit-connection-points.gif" style="width=100%;max-width:350px;height:auto;" alt="Edit an existing shape's connection points to attach connectors precisely where you want them to go">

**Draw a freehand shape:** Click on the _Freehand_ tool in the toolbar or select _Arrange > Insert > Freehand_ from the menu. Disable the brush checkbox before drawing so you can style the outline and fill colours of your [freehand shape](/doc/faq/insert-freehand-shapes.html). 
<br /><img src="/assets/img/blog/home-lab-freehand.png" style="width=100%;max-width:300px;height:auto;" alt="Draw a new shape freehand - deselect the Brush option to style it with outline and fill colours">

**Add a logo image:** Drag and drop the file onto the drawing canvas. 
<br /><img src="/assets/img/blog/home-lab-import-logo.gif" style="width=100%;max-width:500px;height:auto;" alt="You can import logo image files into a draw.io smart home diagram with drag and drop">

**Experienced users:** [Draw a new complex custom shape](/doc/faq/shape-complex-create-edit.html) by describing its geometry and style in XML.

## Create home lab zones with containers

While you can show/hide parts of your diagram with [tags](/blog/tags-in-diagrams.html) and [layers](/doc/layers.html), for home lab or smart home diagrams, container zones are more practical.

1. Place a rectangular shape on the drawing canvas. While it is selected, click on _To Back_ in the Arrange tab. 
<br /><img src="/assets/img/blog/home-lab-zone-to-back.png" style="width=100%;max-width:300px;height:auto;" alt="Send a zone shape to the back behind the devices in that zone.">
2. Select the rectangle zone shape, expand the _Properties_ in the _Style_ tab of the format panel and enable the _Container_ checkbox. Ensure the _Collapsible_ checkbox is not enabled to always keep it expanded. 
<br /><img src="/assets/img/blog/home-lab-zone-container.png" style="width=100%;max-width:300px;height:auto;" alt="Turn a shape into a non-collapsible container by editing the shape Properties in the Style tab">
1. Drag the devices that belong in that zone over the rectangle and drop them when its outline is purple in light mode, or green in dark mode. 
<br /><img src="/assets/img/blog/home-lab-container-zone.gif" style="width=100%;max-width:300px;height:auto;" alt="Drag and drop device shapes into the zone container shape">

Now you can move and resize the container and its devices inside will move and resize with it.

### Use placeholders for smart IP labels

You can use a [shape property](/blog/shape-properties.html) on the container zone that assigns a subnet address, then use a [placeholder](/blog/placeholders.html) in the device label. When you move a device from one zone to another, its label will automatically update. 

1. Right click on the container shape and select _Edit Shape_. 
2. Enter the name of a shape property and click _Add Property_ and enable the _Placeholders_ checkbox. 
<br /><img src="/assets/img/blog/home-lab-add-property-placeholder.png" style="width=100%;max-width:300px;height:auto;" alt="Add a shape property to a container shape and enable the placeholders checkbox to turn it into a variable that can be displayed by other shapes inside the parent container shape">
1. Enter a value for the shape property (in this case, the subnet address) and click _Apply_.
<br /><img src="/assets/img/blog/home-lab-add-placeholder-value.png" style="width=100%;max-width:300px;height:auto;" alt="Add a value for the shape property so it can be displayed in its child shapes' labels">
1. For each shape in the zone, right click and select _Edit Shape_, enable the _Placeholders_ checkbox and click _Apply_. 
2. Click on a shape and type the container zone's property name surrounded by percentage characters (``%``) in the label to add the placeholder. You can add other text before or after the placeholder. In this example the label is written as ``%subnet%.4`` which will display as ``192.168.1.4``.
<br /><img src="/assets/img/blog/home-lab-placeholder-labels.gif" style="width=100%;max-width:400px;height:auto;" alt="Enter the name of the container shape's property in the label surrounded by percentage characters">

**Tip:** Change the container's property and the labels of all its devices will update automatically.

[Learn more about placeholders in draw.io](/blog/placeholders.html)

[<img src="/assets/img/blog/home-lab-example.png" style="width=100%;max-width:600px;height:auto;" alt="Home lab and smart home diagrams help you stay on top of your growing Internet of Things and home network">](https://viewer.diagrams.net/?lightbox=1&page=0&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fhome-lab-example.drawio)
<br />[_Open this example in draw.io_](https://viewer.diagrams.net/?lightbox=1&page=0&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fhome-lab-example.drawio)

## Rack diagrams for complex smart homes

[Rack diagrams](/blog/rack-diagrams.html), just like their physical counterparts, hold servers, switches and other components neatly together. 

1. Click on _More Shapes_ and enable the _Rack_ shape library. 
<br /><img src="/assets/img/blog/home-lab-rack-library.png" style="width=100%;max-width:250px;height:auto;" alt="Enable the rack library in draw.io">
1. Add one of the rack container shapes to your diagram. 
<br /><img src="/assets/img/blog/home-lab-rack-shape.png" style="width=100%;max-width:280px;height:auto;" alt="Add a rack shape to your diagram">
1. Drop each element of your rack just under the one above and it will fall into position. 
<br /><img src="/assets/img/blog/home-lab-rack-diagram.gif" style="width=100%;max-width:500px;height:auto;" alt="Drop rack elements into your diagram for neater home hub servers">

[_Open this rack diagram example in draw.io_ ](https://viewer.diagrams.net/?lightbox=1&page=0&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fhome-lab-example.drawio)

## Save your custom shape library

1. Drag each of your custom shapes from the drawing canvas onto the _Scratchpad_. 
2. Edit the _Scratchpad_ (click on the pen icon). Name each custom shape if you want to.
3. _Export_ and save your custom shape library to an ``.xml`` file. 
<br /><img src="/assets/img/blog/home-lab-export-shape-library.gif" style="width=100%;max-width:500px;height:auto;" alt="Export your custom home lab shape library from the Scratchpad">

[Learn more about working with custom shape libraries](/blog/custom-libraries.html)