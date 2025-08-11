---
layout: post
author: draw.io
slug: mindmaps-from-text
date: 2022-05-30 09:10:00
title: Create a mindmap from text with Mermaid
tags: [integrations,uml]
categories: [integrations,features,use-cases, import]
---

Mindmaps are useful to quickly capture ideas, and are easy to draw in draw.io and our draw.io branded apps. But some people prefer to work from text lists when brainstorming. Drop a text list into the Mermaid import tool and draw.io will generate your mindmap for you - no need to fuss with connectors or layouts.
<br /><img src="/assets/img/blog/mindmap-mermaid-examples.png" style="width=100%;max-width:500px;height:auto;" alt="Mindmaps are easy to create from text with draw.io and Mermaid">

## Create a mindmap in text

Mermaid allows you to create a wide range of diagrams from a human-readable text description, from various UML diagrams to general purpose [mindmaps](https://mermaid.js.org/syntax/mindmap.html), concept diagrams and flows, and even Gantt and pie charts for project management and reports. 

Mindmaps in Mermaid begin with the ``mindmap`` keyword which tells the renderer to use mindmap shapes and layout branches around a central topic. 

* In draw.io, when you choose to generate a _Diagram_ from Mermaid code (the default), your mindmap will use a round shape for the root node, and rounded rectangles for all the branch and leaf nodes. 

* If you choose to add the Mermaid diagram as an _image_ to the drawing canvas, it will use the Mermaid mindmap shapes. 

**Write a mindmap in Mermaid**
* enclose the root node title in double brackets - ``((UML diagrams))``
* use spaces to indicate a branch into leaf nodes
* break a long label into two or more lines using the HTML newline tag ``<br/>``

```
mindmap
  root((UML diagrams))
    Behaviour diagrams
      Activity diagrams
      Use case diagrams
      State machine diagrams
      Interaction diagrams
        Sequence diagrams
        Communication diagrams
        Interaction overview diagrams
        Timing diagrams
    Structure diagrams
      Class diagrams
      Package diagrams
      Object diagrams
      Composite structure diagrams
      Component diagrams
      Profile diagrams
      Deployment diagrams
```

**Note:** there can be only one root node in a Mermaid mindmap.

## Insert the Mermaid mindmap into draw.io

1. In the  draw.io editor, click _Arrange > Insert > Advanced > Mermaid_.
2. Add the text for your mindmap into the text field, and click _Insert_ to generate the diagram from the Mermaid description.
<br /><img src="/assets/img/blog/mindmap-mermaid-example1-insert.png" style="width=100%;max-width:400px;height:auto;" alt="Generate a mindmap from text in draw.io by inserting Mermaid text via Arrange > Insert > Advanced > Mermaid">

Your diagram will be generated and drawn on the canvas with draw.io shapes. Now you can continue to edit and add to your mindmap, style the nodes and connectors as you would any other type of draw.io diagram. 
<br /><img src="/assets/img/blog/mindmap-mermaid-example1.png" style="width=100%;max-width:400px;height:auto;" alt="Generate a mindmap from text in draw.io by inserting Mermaid text via Arrange > Insert > Advanced > Mermaid">

When you insert Mermaid as a diagram in draw.io, you can't re-edit the Mermaid code as your diagram has been converted to use draw.io shapes. 


### Insert Mermaid mindmap as an image

When you choose _Image_ from the drop down list when inserting your Mermaid code, the diagram will be generated and [inserted as an SVG image](/doc/faq/svg-insert.html) on the drawing canvas. 

Hover to see the Mermaid code as a tooltip, and double click on it to re-edit the Mermaid code and _Apply_ your changes to update the diagram. 
<br /><img src="/assets/img/blog/mindmap-mermaid-example1-image-hover.png" style="width=100%;max-width:600px;height:auto;" alt="Generate a mindmap from text in draw.io by inserting Mermaid text via Arrange > Insert > Advanced > Mermaid">

**Tip:** You may need to add a background to the image as Mermaid will automatically use black and white for the first two branches. Select the mindmap image, enable _Fill_ in the _Style_ tab of the format panel and select a fill colour. 

If there is an error in your Mermaid mindmap text, draw.io will display a parser error.
<br /><img src="/assets/img/blog/mindmap-mermaid-example1-error.png" style="width=100%;max-width:250px;height:auto;" alt="If you see this error when inserting Mermaid, check for errors around the lines that are indicated in the error message">

### Mindmaps with different shapes

You can use different shapes to more clearly differentiate between branches.

* [] - rectangle with sharp corners
* () - rounded rectangle
* (()) - circle
* ))(( - bang shape
* )( - cloud shape
* \{\{\}\} - hexagon

[<img src="/assets/img/blog/mindmap-mermaid-example2.png" style="width=100%;max-width:600px;height:auto;" alt="Mindmaps are easy to create from text with draw.io and Mermaid">
<br />_Open this example in our diagram viewer_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&page=2&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fmindmap-mermaid-example.drawio)

```
mindmap
  root)HR(
    ))Onboarding((
      Prior to first day
        Contract signed
        Employee handbook
        IT equipment reserved
      First day
        Office tour
        Team intros
        Account setup
      First week
        Shadow team members
        Software training
      First month
        Assign projects/tasks
        Set goals
        Get team feedback

    id2{ {Offboarding} }
      [Feedback and review]
      [Exit interview]
      [Tasks/projects reassigned]
        [Handover]
      [Account deactivation/deletion]
      [IT hardware return]
```


## Prefer to draw a mindmap?

Use an automated layout container shape from the _Advanced_ shape library and drop _Sub Topic_ and _Branch_ shapes inside to draw your mindmap quickly and easily. 

<img src="/assets/img/blog/automatic-layout-mindmap.gif" style="width=100%;max-width:400px;height:auto;" alt="Drag and drop shapes onto a directional arrow of a shape inside a container layout shape to connect the new shape and resize the container">

[See how to use the automated mindmap layout shape](/blog/automated-layout-shapes.html)

