---
layout: post
author: draw.io
slug: uml-interaction-overview
date: 2025-02-17 09:43:00
title: UML interaction overview diagrams
tags: [shape libraries, uml]
categories: [use-cases, templates, shape-libraries]
---

Interaction overview diagrams show a high-level overview of how components of the system interact with each other. General flowchart shapes show the interaction flow between activities, and sometimes entire sequence diagrams or activity diagrams are embedded for  detailed documentation.
<img src="/assets/img/blog/interaction-overview-example.png" style="width=100%;max-width:500px;height:auto;" alt="An example interaction overview diagram with an embedded sequence diagram for using a library in various ways">

[_Open this example in the draw.io viewer_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=1&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fuml-interaction-overview-example.drawio)

Interaction overviews are useful when you want to gain stakeholder approval for new systems or changes to existing systems - they don't need to know the implementation specifics but do need see what interactions are important and the overall interaction flow. 

You can also use these diagrams to analyse and optimise complex multi-component systems, especially where the flow of control impacts dependencies when changing only part of the system. 

**When to draw interaction overview diagrams?**

[Activity](/blog/uml-activity-diagrams.html) and [sequence diagrams](/blog/sequence-diagrams.html) are typically drawn after [use case diagrams](/blog/uml-use-case-diagrams.html), showing how those use cases will be achieved. 

To tie the entire system together, interaction overview diagrams are best drawn after the lower-level detailed interactions. 

## Enable the UML 2.5, UML and General shape libraries

The basic flowchart shapes are in the _General_ shape library (enabled by default), while the other shapes are in the two UML libraries. 
<br /><img src="/assets/img/blog/uml-shapes.png" style="max-width:100%;height:auto;" alt="The UML and UML2.5 shape libraries in draw.io let you draw all types of UML diagrams">

In draw.io, click on _More Shapes_ in the shapes panel on the left, then enable the _General_, [_UML_ and _UML 2.5_ shape libraries](/blog/uml-2-5.html) and click _Apply_. 
<br /><img src="/assets/img/blog/uml-2-5-shape-library-enable.png" style="width=100%;max-width:400px;height:auto;" alt="Enable the UML 2.5 shape library, and the older UML library if you wish to use those shapes">

## UML interaction overview shapes

* **Start:** A filled circle, usually black. 
* **Stop:** A filled circle inside a larger second circle.
* **Interaction:** A frame shape with the name of the activity or sequence.   
* **Activity diagram or sequence diagram:** An embedded diagram in the overview enclosed in a frame shape, using either sequence or activity diagram shapes. 
* **Decisions or condition checks:** A diamond with one or more connectors coming in, and labelled connectors coming out. These are the same as in flow charts. 
* **Connectors:** Show the interaction flow in the running system. These may be labelled with condition results. 

<img src="/assets/img/blog/uml-interaction-shapes.png" style="max-width:100%;height:auto;" alt="The UML and UML2.5 shape libraries plus a few shapes from the General shape library in draw.io contain all the shapes you need for interaction overview diagrams">

### Using frame shapes

When a frame shape contains just the name of the activity or sequence and no details, use ``Ref`` as the frame name - this means it is a _reference_ to a more detailed diagram.

**Embedding sequence or activity diagrams**

To highlight a specific sequence or activity in your interaction overview, you can draw it in full detail inside a frame shape. Keep in mind that too many of these will make your interaction overview become hard to read.

Most of the frame shapes in the two UML libraries are not compound shapes. Instead, [group the frame shape with its sequence or activity](/doc/faq/group-shapes-connectors.html) to keep your diagram neat. 

1. Once you have drawn your embedded sequence or activity diagram add a **frame shape** and send it to the back behind the other shapes (_Arrange_ tab of the format panel > _To Back_). 
<br /><img src="/assets/img/blog/uml-interaction-overview-to-back.png" style="width=100%;max-width:400px;height:auto;" alt="Send the frame shape to the back behind the embedded sequence or activity diagram">
2. Drag a selection box around all the sequence or activity diagram shapes and connectors and its surrounding frame shape, right click and select _Group_, or press ``Ctrl+G`` (or ``Cmd+G``)
<br /><img src="/assets/img/blog/uml-interaction-overview-group-shapes.png" style="max-width:100%;height:auto;" alt="Group the embedded sequence and activity diagrams together with their frame so you can more easily move it around the diagram canvas">

Now, you can move the group around more easily and attach floating connectors neatly to the grouped interaction. 


### Save all interactions in a multi-page diagram

Use a [multi-page diagram](/blog/multiple-page-diagrams.html) to keep the interaction overview and all the sequence and/or activity diagrams organised in one file. 

[Add a link](/doc/faq/insert-text-link.html) from each interaction's 'frame' shape on the overview to its detailed diagram on another page. 
   * Right click on a shape and select _Edit > Edit Link_, or select a shape and press ``Alt+Shift+L``.
  <br /><img src="/assets/img/blog/uml-interaction-overview-add-link.png" style="width=100%;max-width:300px;height:auto;" alt="Add a link to the ref interaction shapes to be able to navigate to their diagram page">
   * Select the page from the drop down list, and click _OK_.
  <br /><img src="/assets/img/blog/uml-interaction-overview-link-page.png" style="width=100%;max-width:250px;height:auto;" alt="Add a link to the ref interaction shapes to be able to navigate to their diagram page">

**Tip:** Add a link on the detailed diagram pages back to the first overview page. 
<br /><img src="/assets/img/blog/uml-interaction-overview-links-navigate.gif" style="width=100%;max-width:500px;height:auto;" alt="Diagram types defined in UML 2.5">

Now, anyone who views your diagram can click on the shapes to navigate between the high-level diagrams and low-level interaction details. Links make it easy to navigate your diagram in the viewer, whether you use our online app, or when the diagram is on a Confluence page or Jira issue. 

[Open this example in the draw.io online viewer](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=1&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fuml-interaction-overview-example.drawio)

### Other types of UML diagrams

The UML specification allows you to draw many different types of diagrams to model the behaviour and data of a system in different ways.

[<img src="/assets/img/blog/uml-2-5-diagram-overview.png" style="width=100%;max-width:500px;height:auto;" alt="Diagram types defined in UML 2.5">](https://app.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fconcept-map-uml-diagrams-overview.drawio)

Refer to the [UML diagram overview post](/blog/uml-overview.html) for details of the many other types of UML diagrams. 