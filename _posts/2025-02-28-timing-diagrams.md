---
layout: post
author: draw.io
slug: timing-diagrams
date: 2025-02-28 09:43:00
title: Timing diagrams for UML and embedded systems
tags: [uml]
categories: [use-cases, shapes, shape-libraries]
---

Timing diagrams are important for activities that need to be completed within a specific time frame. Such as the ringing of a doorbell after pressing a button, or a ticket gate opening after a ticket has been validated. 
<br /><img src="/assets/img/blog/uml-timing-example-invisible-waypoints.png" style="width=100%;max-width:500px;height:auto;" alt="An example timing diagram where the waypoint shapes have been made invisible to look neater">

While you can show these constraints in other diagrams, timing diagrams can visualise more clearly the time limits on activities, their triggers, and when their state changes occur. 

Timing diagrams can be used to document compliance with safety or service regulations where reaction times are important, and to analyse the performance of existing systems.

## Timing diagrams in draw.io

While timing diagrams are usually mocked up in other tools, you can also create them easily in draw.io, with a few helpful layout features.

The shapes you need are relatively simple:
* diagram or frame shape from the UML shape library
* horizontal line to separate sections inside the frame shape.
* vertical line to create the scale at the bottom of the frame.
* waypoint shape to join connectors for both the state and value lifelines. 
* partial rectangle for the actions in the value lifeline. 
* horizontal dimension shape to specify timing constraints.
* text shapes for the actions and states on the left of the timing diagram.
<br /><img src="/assets/img/blog/timing-diagram-scratchpad.png" style="width=100%;max-width:300px;height:auto;" alt="Create your own quick custom library for timing diagrams using the scratchpad in draw.io">

**Tip:** Drag one of each of these shapes from their shape libraries onto the drawing canvas before you start, then back onto the _Scratchpad_ in the shapes panel. Now you have a quick custom timing diagram shape library in the scratchpad. 

[See how to use the scratchpad to speed up diagramming](/doc/faq/scratchpad.html)

### Draw a custom scale 

While there are ruler shapes in draw.io, they are inside a rectangular outline. You can quickly make your own scale though. 

1. Add a small vertical line (from _Misc_ shape library), resize it, and place it over the bottom of the frame shape at the start of the scale.
2. Copy and paste this small vertical line and move it to the end of the scale.
3. Copy and paste as many vertical lines as you need to fill in the scale, placing them roughly between the start and end shapes. 
4. Drag a selection box around all the vertical lines. 
5. Go to the _Arrange_ tab of the format panel, click on _Align - Middle_ and then on _Horizontal_ to _Distribute_ the vertical lines evenly along the scale. 
<br /><img src="/assets/img/blog/timing-diagram-align-scale.gif" style="width=100%;max-width:500px;height:auto;" alt="Add a custom scale to any diagram easily with the Align and Distribute tools in the Arrange tab of the format panel in draw.io">

**Scale labels:** Add labels to the lines in the scale. Select the _Bottom_ from the _Position_ list in the _Text_ tab to reposition the labels under the scale.
<br /><img src="/assets/img/blog/timing-diagram-scale-labels.png" style="width=100%;max-width:350px;height:auto;" alt="Add labels to your custom scale positioning the labels on the Bottom of the shapes in the Text tab of the format panel in draw.io">

If you have multiple sections in your timing diagram that use the scale, select all the vertical lines before you add any labels, and group them together. Now you can copy and reposition that group over another section or add it to the scratchpad.
<br /><img src="/assets/img/blog/timing-diagram-copy-scale.png" style="width=100%;max-width:400px;height:auto;" alt="Group the finished scale together and drag it onto the scratchpad in draw.io so you can easily add it to other sections in your timing diagram">

### Waypoints and connectors for timing lines

Now that you have your scale in the correct position, you can use the [guidelines](/doc/faq/guides-hide-display.html) that appear as you drag shapes onto the canvas to position your waypoint shapes. 

1. Drag at least two waypoint shapes into position in your timing diagram. 
2. Hover over one waypoint shape and drag a connector from the direction arrows. Drop this onto the next waypoint shape in the timing diagram. 
3. Change the connector to have no arrows at either end, and set it to be a straight line. While it is still selected, click _Set as Default Style_.
4. Continue attaching connectors between waypoint shapes until your state timeline is complete. 
<br /><img src="/assets/img/blog/timing-diagram-waypoint-line.gif" style="width=100%;max-width:500px;height:auto;" alt="Use the draw.io waypoint shape and connectors to draw your timing line">

**Action triggers:** If you have drawn two related state lifelines, use connectors with an arrow at one end to show where an action in one lifeline triggers a state change in the other.
<br /><img src="/assets/img/blog/timing-diagram-trigger-connectors.png" style="width=100%;max-width:300px;height:auto;" alt="Draw connectors with an arrow to indicate when an action or state change in one state lifeline triggers a change of state in another in UML timing diagrams"> 

**Action labels:** Use the text shape in the _General_ shape library to add labels to the different states. Use the blue guidelines to align the labels with their waypoint shapes. 
<br /><img src="/assets/img/blog/timing-diagram-align-labels.png" style="width=100%;max-width:300px;height:auto;" alt="Use the guidelines to align labels with shapes in your diagrams in draw.io">

### Draw a value lifeline

While value lifelines are less common, they are used to clearly visualise the action steps and timing constraints for important use cases. 

Note that they do not need to line up with the timing diagrams exactly. If there is a constraint specified with a horizontal dimension shape, it is best to ensure at least these actions line up. 

1. Add and resize partial rectangle shapes for each action in the use case. 
  * Use the _Middle_ alignment in the _Arrange_ tab of the format panel to ensure they are at the same height. 
2. Add waypoint shapes between each action and align them evenly. 
3. Drag connectors (with no arrows) from the top right and bottom right corner of one partial rectangle to the waypoint. 
<br /><img src="/assets/img/blog/timing-diagram-value-lifeline.png" style="width=100%;max-width:500px;height:auto;" alt="Connect partial rectangles in your value lifelines with waypoint shapes">
<br />Make sure you attach them as [fixed connectors](/doc/faq/connector-fixed-vs-floating.html) to the fixed connection points on the partial rectangles (the green cross above). You can also [customise the connection points](doc/faq/shape-connection-points-customise.html) on the partial rectangle shape. 
4. Drag connectors from the waypoint shape to the top and bottom left connection points of the next action. 
5. Repeat until you have drawn the full value lifeline. 

**Tip:** While could use an 'x' shape to avoid the extra steps using connectors and waypoint shapes, but the partial rectangle makes it easier to add labels, resize actions and move them around.

## Simplify the timing diagram

You can make the waypoint shapes invisible when you have finished your diagram - select all the waypoint shapes and deselect _Line_ in the _Style_ tab of the format panel. Now, your timing diagram will look less cluttered.
<br />[<img src="/assets/img/blog/uml-timing-example-invisible-waypoints.png" style="width=100%;max-width:500px;height:auto;" alt="An example timing diagram where the waypoint shapes have been made invisible to look neater">](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=0&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fuml-timing-example.drawio)<br />[_Open this timing diagram example in the draw.io viewer_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=0&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fuml-timing-example.drawio)

## More UML diagrams

Timing diagrams are also part of the UML specification. There are many different types of UML diagrams that allow you to model the behaviour and data of systems and processes both as abstract overviews and in detail for accurate implementations. 

[<img src="/assets/img/blog/uml-2-5-diagram-overview.png" style="width=100%;max-width:500px;height:auto;" alt="Diagram types defined in UML 2.5">](https://app.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fconcept-map-uml-diagrams-overview.drawio)

Refer to the [UML diagram overview post](/blog/uml-overview.html) for the many other types of UML diagrams. 