---
layout: post
author: draw.io
slug: network-library-shadow
date: 2025-04-15 09:43:00
title: New networking shape library with customisable shadows
tags: [shape libraries]
categories: [use-cases, shape-libraries]
---

The new _Network_ shape library in draw.io has extra styling options built in. When you enable the background colour, the shapes will have a bold long shadow. You can colour each part of these shapes individually - shape outline, shape fill colour (and neutral colour for internal details), background colour and gradient.
<br /><img src="/assets/img/blog/network-shadow-colours.png" style="width=100%;max-width:600px;height:auto;" alt="The new Network shape library includes a long shadow with additional colour styling options">

**Open the new _Network_ shape library:** Click on _More Shapes_ in the shapes panel, enable the new (second) _Network_ shape library, and click _Apply_.
<br /><img src="/assets/img/blog/network-shape-library-new.png" style="width=100%;max-width:400px;height:auto;" alt="The new Network shape library includes a long shadow with additional colour styling options">

Networks are getting more complex. Even a simple home network has many devices connected to it. This is only becoming more complicated as wi-fi is built into more and more household appliances. A quick [network diagram](/blog/network-diagrams.html) will help you stay on top of what device is connected where.

Of course, you can make much more detailed diagrams for a home hub filled with smart devices, servers and additional networking equipment. An example of such a complex smart home system will be in a future post.

## Draw your home network

In this example, the home has three hubs connected to a router, which is connected to a modem that has a firewall to provide some protection from bad actors on the internet. A wired hub connects to the home office equipment, one wi-fi hub connects the TV and game consoles, and the other wi-fi hub connects various mobile devices and a wi-fi printer.
<br /><img src="/assets/img/blog/network-home-example.png" style="width=100%;max-width:500px;height:auto;" alt="A simple home network drawn using the new Network shape library in draw.io"> 

Wi-fi connections use a dashed connector, and wired connections a solid connector. All connectors have no arrows to make the diagram neater as network traffic is both ways.

**Enable the shape's Background to see the long shadow**

1. Right click on a blank area of the drawing canvas and choose _Select Vertices_ from the context menu. 
2. Click on _Background_ in the _Style_ tab of the format panel.
<br /><img src="/assets/img/blog/network-background-enable.gif" style="width=100%;max-width:600px;height:auto;" alt="The new Network shape library includes a long shadow with additional colour styling options">


### Indicate network zones with colours

It's much easier to see the hub-based zones when you add colour to the network diagram. The new network shapes have additional style options for background colours and the long shadow.

* **Fill:** the colour inside the shape.
* **Gradient:** the second colour in a gradient background and direction.
* **Background Color:** the background colour (behind the shadow) - enable this to see the shape's long shadow.
* **Neutral Fill:** the colour of any 'open' details in a shape, such as the little circles in the router and modem. 
* **Line:** the shape's line colour and style.
<br /><img src="/assets/img/blog/network-style-colours.png" style="width=100%;max-width:500px;height:auto;" alt="The new Network shapes have additional style options for shape and background colour, and a long shadow"> 

**Disable the long shadow**

If you don't like the long shadows, you can disable it and keep the background colours and gradients. 

1. Select the shapes you want to have no shadow on. 
2. Deselect the _Long Shadow_ checkbox in the _Style_ tab of the format panel. 
<br /><img src="/assets/img/blog/network-long-shadow-disable.png" style="width=100%;max-width:500px;height:auto;" alt="Disable the Long Shadow and keep the background colours of the new Network shapes via the Style tab of the format panel"> 

**Note:** Long shadows are currently only available on these shapes in the new _Network_ shape library. 

### Dark mode network shapes

The new Network shapes also look great in [dark mode](/blog/dark-mode-diagram-editor.html) using the automatic [adaptive colours](/blog/adaptive-colours.html). To switch to dark mode, select _Settings > Appearance > Dark_ or _Extras > Appearance > Dark_ from the draw.io menu. 
<br /><img src="/assets/img/blog/network-dark-mode.gif" style="width=100%;max-width:500px;height:auto;" alt="The new Network shape library includes a long shadow with additional colour styling options">


## Network diagrams in draw.io

Learn more about [network and infrastructure diagrams](/blog/network-diagrams.html) with multiple examples from the draw.io template library. 

There are a large number of network and infrastructure shape libraries, including [AWS and GCP](/blog/gcp-aws-shapes-network-diagrams.html), [Citrix](/blog/citrix-diagrams.html), [Veeam](/blog/veeam-stencils.html), [IBM](/blog/ibm-technical-diagrams.html) and [many more cloud infrastructure platforms](/blog/more-cloud-shapes.html).

Complex networks with many dedicated servers can be documented with a [rack diagram](/blog/rack-diagrams.html) so you can trace cabling problems more easily.  

