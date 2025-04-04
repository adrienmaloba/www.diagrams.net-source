---
layout: post
author: draw.io
slug: arrange-align-shapes
date: 2025-04-04 10:13:00
title: Align and space shapes for neater diagrams in draw.io
tags: [features]
categories: [features,shapes]
---

Diagrams look neater and are easier to read when the shapes are aligned and evenly spaced. It can be time consuming to line everything up using the grid by hand - there is an easier way. In the _Arrange_ tab of the format panel, the _Align_ and _Distribute_ tools let you align and space multiple shapes quickly and easily. 
<br /><img src="/assets/img/blog/arrange-align-distribute-tools.png" style="width=100%;max-width:600px;height:auto;" alt="draw.io has alignment and distribute tools that let you neaten diagrams quickly and easily">

**An example automated factory layout**

This example is of an extensible manifold layout for a construction line that takes iron ore from a miner, smelts iron into ingots, and constructs iron plates, and iron rods, and screws from the iron rods. 

* Plates, rods and screws are stored in their own dedicated containers. 
* Conveyer belts connect each machine in the automated fabrication process. 
 
You could build this production line with fewer merge and split nodes. However, using a split node before and a merge node after each factory component allows for a compact and neat build. These also let you extend the system neatly to produce larger quantities. 

**Tip:** A split node _before_ each storage container lets you store some of the base components and forward the rest for advanced construction. 

## Arranging shapes quickly

Instead of using the guidelines in the draw.io editor to arrange every single shape separately in this production line, you can use the tools in the _Arrange_ tab of the format panel. 

These tools will appear in the _Arrange_ tab when you have selected two or more shapes. 

* **Align shapes horizontally:** Use the _Left_, _Center_, and _Right_ tools. In the example, _Left_ neatly aligns these shapes.
<br /><img src="/assets/img/blog/arrange-align-horizontal.png" style="width=100%;max-width:400px;height:auto;" alt="Align selected shapes horizontally in the Arrange tab in draw.io to the Left, Center or Right">

* **Align shapes vertically:** Use the _Top_, _Middle_, and _Bottom_ tools. In the example below, _Middle_ aligns them the best.
<br /><img src="/assets/img/blog/arrange-align-vertical.png" style="width=100%;max-width:530px;height:auto;" alt="Align selected shapes vertically in the Arrange tab in draw.io to the Top, Middle, or Bottom">

* **Distribute shapes evenly between the two outermost selected shapes:** Enable the _Spacing_ checkbox to distribute the selected shapes with an even amount of space between them then click on _Horizontal_ or _Vertical_. 
<br /><img src="/assets/img/blog/arrange-distribute.png" style="width=100%;max-width:500px;height:auto;" alt="Distribute shapes horizontally with even spacing between the shapes via the Arrange tab in draw.io">
<br />Without _Spacing_ selected, the centre of each shape is distributed evenly between the two outermost. The example below shows this difference more clearly - the middle distributes the rectangles using the shapes' centres, and the bottom makes the space between their outlines even. 
<br /><img src="/assets/img/blog/arrange-distribute-spacing.png" style="width=100%;max-width:500px;height:auto;" alt="Distribute shapes horizontally with and without the Spacing checkbox enabled in the Arrange tab in draw.io">


**Note:** Grouped shapes like the storage containers in the example, and custom shapes like the screw and plate can be tricker to align. You may need to manually reposition these in your diagram, as you can see in the example animation below.
<img src="/assets/img/blog/arrange-align-distribute-example.mp4" style="width=100%;max-width:600px;height:auto;" alt="draw.io has alignment and distribute tools that let you neaten diagrams quickly and easily">
<br />[_Open the finished diagram in draw.io_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=0&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fautomated-factory-example.drawio)

_Now, if only the game also had such useful alignment tools for aligning multiple components._

## Related

Learn more about the [_Snap to Grid_ tool and the alignment guidelines](/blog/snap-to-grid.html) that appear when you move shapes around the drawing canvas. 

If you were more mathematically inclined, you may find [dependency graphs](/blog/dependency-graphs.html) useful to visualise production timings. 

New to draw.io and diagramming, but want to streamline your factory? Here's how to [draw a basic flowchart](/doc/getting-started-basic-flow-chart.html). 