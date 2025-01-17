---
layout: post
author: draw.io
slug: placeholders
date: 2019-12-17 09:54:00
title: Work with placeholders in labels and tooltips
tags: [features, shapes, properties, placeholders]
categories: [features, shapes]
---

Each shape in a diagram can contain metadata or custom properties - extra information about those shapes.

These custom properties can also be used to define placeholder values, acting like variables in a computer program. Placeholders can be used in shape labels and tooltips to show the value of the custom property of that shape, the container shape it is inside, or an ancestor in a multi-group shape.

When you move a shape that contains a placeholder into a container shape with a matching property, the label that contains the placeholder (or tooltip) will be updated automatically.

**Note:** As an advanced feature, placeholders are not enabled by default - you need to explicitly tell draw.io you want to use them.

But first, you need to add a property to the shape or container shape you want to reference.

## Add a custom property

You can add custom properties to any shape, connector, container shape, swim lane, etc.

1. Select a shape, and in the _Arrange_ tab of the format panel, click on _Edit Data_. Alternatively, right-click on the shape and select _Edit Data_ from the context menu, or select the shape and press the keyboard shortcut ``Ctrl+M`` on Windows or ``Cmd+M`` on MacOs.
2. The dialog lists the custom properties you have added. To add a new one, enter a name for the custom property, then click _Add Property_.
<br /><img src="/assets/img/blog/add-property-to-shape-1.png" style="width=100%;max-width:400px;height:auto;" alt="Add a property name to your shape">
3. Now enter a value for the custom property in the text field next to the name you just entered, and click _Apply_.
<br /><img src="/assets/img/blog/add-property-to-shape-2.png" style="width=100%;max-width:400px;height:auto;" alt="Enter the property value for the new property you just added">

When you hover over that shape, the custom properties that you added and their values are displayed in a tooltip, unless you have added a custom ``tooltip`` property - then only the tooltip value is displayed. To see how to define a tooltip, and use custom properties as placeholders within the tooltip, keep reading.

<img src="/assets/img/blog/custom-properties-hover.png" style="width=100%;max-width:300px;height:auto;" alt="Custom properties are displayed by default in a tooltip when you hover over the shape">

**Tip:** Properties can be set globally, working similar to global variables in a programming language. Make sure nothing is selected, then click on _Edit Data_ in the format panel to see the global custom properties.

## Use a property as a placeholder

Once you have added a custom property to your shape, you can use it as a placeholder in the shape's label or tooltip text.

**Tip:** You can see placeholders in action in the [simple kanban board template](/blog/kanban-boards.html), where the colour and status text of each card changes depending on which column it is in.

### Turn a shape into a container

If you want to use the properties defined in a parent shape as a placeholder, you need to turn the parent into a container shape.

1. Select the parent shape, and expand the shape _Properties_ in the format panel on the right.
2. Make sure the _Container_ checkbox is enabled.

### Add a placeholder to a shape label

To display the value of a shape's property in a label, write the property name surrounded by % signs. For example, if you have added a property called _group_ to the shape, write ``%group%``.

1. Right-click on a shape and select _Edit Data_ from the context menu, make sure the _Placeholders_ checkbox is selected, then click _Apply_.
<br /><img src="/assets/img/blog/use-placeholders-example.png" style="width=100%;max-width:400px;height:auto;" alt="Edit the shape's data, and enable the Placeholders checkbox">
2. Edit the text label of the shape to include the property name surrounded by % signs.
<br /><img src="/assets/img/blog/placeholder-example-label.png" style="max-width:100%;height:auto;" alt="Add a placeholder to a shape label, for example %group%">

There are a number of [predefined placeholders](/doc/faq/predefined-placeholders.html) where you can add the date and time in a variety of time formats, page number or title, and more to labels and tooltips.

**Troubleshooting tips**

If the property name does not exist for that shape, the value of the matching property name of the nearest ancestor (container shape or group) is used. If not found, the text is printed as is.

If a property isn't found and the placeholder text appears with the % signs, edit the shape data (``Ctrl+M`` or ``Cmd+M``) of both the shape and its ancestor, double check the property name is correct and make sure that the _Placeholders_ checkbox is enabled.

Note that the diagram itself can have custom properties that can be referenced by placeholders. Make sure nothing in you diagram is selected, then click _Edit Data_ in the format panel on the right to see these 'global' custom properties.

Note that there are a few _special_ shape property names:
- **tooltip**: If you define a tooltip property, only this text will be displayed when you hover over a shape (and no other custom properties).
- **placeholder**: This turns the entire shape label into a placeholder, without needing to add a property name to the shape's label manually. [See how to use the ``placeholder`` custom property](/blog/placeholder-scope.html)

### Add a placeholder to a tooltip on a shape

Select a shape and you can add a tooltip to it via _Edit > Edit Tooltip_ or by using the keyboard shortcut ``Alt+Shift+T``. By entering a tooltip this way, it simply adds it to the list of custom properties.

You can define a tooltip with a placeholder directly:
1. Right-click on a shape and select _Edit Data_ from the context menu, make sure the _Placeholders_ checkbox is selected.
2. Add a new property with the name: ``tooltip``.
3. In the blank field next to the tooltip property, add your tooltip text, putting % symbols around the placeholder you want to use in it. Then click _Apply_.
<br /><img src="/assets/img/blog/placeholder-tooltip-value.png" style="width=100%;max-width:400px;height:auto;" alt="Add a tooltip property, and write the tooltip text - include a placeholder by surrounding the property name with % signs">

Now, when you hover over the shape, the tooltip text will appear, and the placeholder will be replaced with the value of the property it references.

<img src="/assets/img/blog/placeholder-tooltip-hover.png" style="width=100%;max-width:400px;height:auto;" alt="How the example tooltip with a placeholder appears when you hover over the shape">

## Use placeholders to automate your diagramming

Looking at a somewhat more practical example - you can use placeholders in labels in your infrastructure diagrams. Then, when you change the address of the subnet group, the individual node IP addresses will update automatically.

In the example below, the labels on the individual nodes inside the subnet use a placeholder which references the custom ``subnet`` property of the containing oval shape. This makes it easy to update the IP addresses in that subnet.

<img src="/assets/img/blog/placeholder-subnet-example.gif" style="width=100%;max-width:400px;height:auto;" alt="Placeholders in the the labels of nodes in an infrastructure diagram">

[Open this example in our online version of draw.io](https://app.diagrams.net/?lightbox=0&highlight=0000ff&edit=_blank&layers=1&page=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fnetwork-with-placeholders.drawio)
