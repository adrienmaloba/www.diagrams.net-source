---
layout: post
author: draw.io
slug: consistent-diagrams
date: 2025-05-28 09:10:00
title: Consistency makes technical diagrams easier to read
tags: [use-cases]
categories: [features, use-cases]
---

Diagrams can convey a lot of information at a glance, but only if they follow the three C's - for drawing technical diagrams that means `concise`, `clear` and `consistent`. As the diagram author, you are responsible for _clarity_ and _conciseness_. For _consistency_ however, draw.io has many tools to help you draw diagrams that are easier to read.

Inconsistent diagrams can cause confusion and annoy your audience. But in the worst case, they could cause serious misunderstandings, processes followed incorrectly, or wrong implementations and a finished product that does not meet its requirements.

The [principles of grouping](https://en.wikipedia.org/wiki/Principles_of_grouping) explain how humans see objects organised into patterns. While there are some slight [cultural differences in perception](https://en.wikipedia.org/wiki/Global_precedence), consistent alignment, styles and shapes allow people to comprehend what they see more quickly and clearly.

## Consistent shapes

Use the same shape for the same type of element in your diagram. This is especially important when there are official or de facto standards for the type of diagram you are drawing. 

For example: 
* Use a rounded rectangle for all steps in a flow chart and a diamond for choices. 
* Click on _More Shapes_ in the shapes panel and enable the shape libraries for standard shapes - [BPMN](/blog/bpmn-2-0), [C4](/blog/c4-modelling.html), [AWS](/blog/aws-diagrams.html), etc.

In the example below, you can see a [Citrix](/blog/citrix-diagrams.html) Hybrid Multi-Cloud manages AWS and GCP clouds within the same infrastructure, where shapes from each of the platform's shape libraries have been used.
<br /><img src="/assets/img/blog/citrix-hybrid-infrastructure-example.png" style="width=100%;max-width:500px;height:auto;" alt="Use appropriate shapes for each infrastructure provider with the draw.io shape libraries">

**Create your own library**

If you have an internal diagram standard or corporate style, you can create your own [custom shape library](/blog/custom-libraries.html) and share it with your team. 

## Consistent shape sizes

Consistent sizes help us pattern match when reading a diagram. Make all the elements of your diagram of the same type also the same size in a couple of steps.

1. Select the source shape that is the size you want to use, then click _Copy Size_ in the _Arrange_ tab of the format panel.
2. Select the shape you want to resize, and click _Paste Size_.
<br /><img src="/assets/img/blog/shapes-copy-size-paste-size.gif" style="width=100%;max-width:350px;height:auto;" alt="Copy and paste a selected shape's size to quickly resize other shapes">

The height and width of the selected shapes will now match the one you copied, even if they are different shapes.



## Consistent shape colours and styles

Just as you used the same shapes for the same type of object or step, you should use the same [shape styles](/doc/faq/shape-styles.html). When using colour coding or shape outline styles to add meaning to your diagram, make sure the same meaning applies throughout your diagram. 

**Copy and paste styles**

1. Select the shape that has the style you want to use. 
2. In the _Style_ tab of the format panel, select _Copy Style_.
3. Select all the shapes you want to apply the style to. 
4. In the _Style_ tab of the format panel, select _Paste Style_ to make the selected consistent. 
<br /><img src="/assets/img/blog/styles-copy-paste.gif" style="width=100%;max-width:300px;height:auto;" alt="Copy and paste styles from one shape or connector to another in draw.io">

**Tip:** Select a shape or connector and then click _Set default style_ in the _Style_ tab of the format panel. Every subsequent shape or connector you add to the drawing canvas will use that default style. 

## Consistent connector styles and arrow heads

Use different connector colours or styles to indicate different groupings. For example, a dotted or dashed connector could indicate an optional step in a flow chart, or an externally provided service in an infrastructure diagram.

**Restyle multiple selected connectors**

1. Right click on the drawing canvas to show the context menu and _Select Edges_ to select all connectors. Alternatively, hold ``Shift`` and click on each connector you want to include. 
2. Select the arrow heads, line styles and thickness you want to use for all selected connectors. 
<br /><img src="/assets/img/blog/style-tab-line-start-line-end.png" style="width=100%;max-width:400px;height:auto;" alt="Style your connector using the options in the Style tab in the format panel on the right in draw.io">

[Learn more about styling connectors](/doc/faq/connector-styles.html)

## Consistent positioning

In general, humans innately prefer designs that are symmetrical and organised. The brain is wired to quickly recognise patterns - a consistently aligned diagram is easier for the brain to process.

For example, neatly aligned and equally spaced process steps ensures there is no confusion over the order in which they must be implemented. Space between grouped devices can visually indicate they are on different subnetworks. 

Enable the [drawing grid, snap-to-grid option and the guidelines](/blog/snap-to-grid.html) to help you align shapes and connectors as you move them around the drawing canvas. 

Select multiple shapes and use the alignment tools in the _Arrange_ tab of the format panel to [space and align shapes in just a couple of clicks](/blog/arrange-align-shapes.html)
<img src="/assets/img/blog/arrange-align-distribute-example.mp4" style="width=100%;max-width:600px;height:auto;" alt="draw.io has alignment and distribute tools that let you neaten diagrams quickly and easily">

## Consistent labelling

Use consistent fonts, font sizes, text styles (italic, bold), spacing, and label positions via the _Text_ tab of the format panel. Keep the text as concise and accurate as possible. 
<br /><img src="/assets/img/blog/text-tab.png" style="width=100%;max-width:500px;height:auto;" alt="Select a shape, then select the Text tab in the format panel to change its style">

Consistent naming conventions will also help your audience read your diagram. For all labels: 
* all plurals
* all singular words
* following a pattern like 'verb + noun'
* with consistent numbering
<br /><img src="/assets/img/blog/communication-diagram-example.png" style="width=100%;max-width:500px;height:auto;" alt="An example communication diagram of the sequence diagram">

[Learn more about styling text labels in draw.io](/doc/faq/text-styles.html)

## More tips for easy-to-read diagrams

If you have drawn a complex diagram or used many abbreviations, include a legend to reduce the risk of misunderstanding. 

Ensure your diagram elements are all at the same level of abstraction. Typically, a diagram should be low-level and detailed, or a high-level overview, and not both. 

