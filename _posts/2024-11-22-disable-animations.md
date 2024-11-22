---
layout: post
author: draw.io
slug: disable-animations
date: 2024-11-22 10:13:00
title: Disable distracting animations in diagrams
tags: [features]
categories: [features,connectors]
---

Flow animations on connectors can make diagrams much easier to understand - they can clearly show in which direction a process flows or how control/data moves through a system. But such animations can distract you while you edit a diagram. You can now disable the visual animation via the draw.io menu, but keep the flow animation style on the connector.
<br /><img src="/assets/img/blog/view-animations-disable.gif" style="width=100%;max-width:500px;height:auto;" alt="You can disable the animation visual without disabling the flow animation style setting on connectors in draw.io">

While animations are useful to explain a diagram in training material or documentation, they can be distracting when you are trying to draw and edit it. Animations also consume additional device resources and if there are many in a diagram, they may slow down the editor.

When you turn off the visual animations but leave the _Flow Animation_ style set on the connector, when you share this diagram with colleagues, or view it in the lightbox, all connectors that have the Flow Animation style will be animated. 

## Disable/Enable the animation visual

Select _View > Animations_ from the Classic draw.io menu or _... > Settings > Animations_ from the toolbar if you are using the Simple Mode or Sketch editor theme. 
<br /><img src="/assets/img/blog/view-animations-disable.png" style="width=100%;max-width:500px;height:auto;" alt="You can disable the animation visual without disabling the flow animation style setting on connectors in draw.io">

**Note:** This does not disable the flow animation style on the connectors, only the visual effect in your browser window.

For example, if you export the diagram to a URL while you have disabled _Animations_ via the menu, opening the exported link will animate all connectors that have the _Flow Animation_ style.

## More animated connector styles 

You can use animated connectors to illustrate and explain process flows, electrical circuits, sequence diagrams, infographics, and any other diagram that uses connectors to indicate a direction.

**Flow Animation:** Select the connector(s) you want to animate and enable the _Flow Animation_ checkbox in the _Style_ tab of the format panel. 

**Animation Pattern:** Change the animation pattern by selecting a different one from the _Pattern_ drop down list.
<img src="/assets/img/blog/flow-animation-pattern.png" style="width=100%;max-width:500px;height:auto;" alt="Animate connectors and change the flow animation pattern via the Style tab of the format panel">



**Animation Styles:** Change the _Flow Duration_, _Flow Timing_ and _Flow Direction_ via the connector _Properties_ at the bottom of the _Style_ tab of the format panel. 
<br /><img src="/assets/img/blog/connector-flow-properties.png" style="width=100%;max-width:500px;height:auto;" alt="Enable Flow Animation on your connectors in draw.io via the shape Properties in the Style tab.">

[Learn more about styling animated connectors in draw.io diagrams](blog/connector-animation-styles.html)