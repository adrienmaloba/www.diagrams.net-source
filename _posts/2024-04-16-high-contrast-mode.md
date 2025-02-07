---
layout: post
author: draw.io
slug: high-contrast-mode
date: 2024-04-16 09:24:00
title: High contrast mode in draw.io
tags: [features]
categories: [features]
---

The new high contrast mode is available in draw.io: _High Contrast_ makes the editor interface easier to read without adjusting your monitor's contrast settings, similar to the accessibility options in your operating system.
<br /><img src="/assets/img/blog/high-contrast.gif" style="width=100%;max-width:500px;height:auto;" alt="High contrast simplifies the draw.io editor interface so that it is easier to read, and improve contrast updates the colours in dark mode to make diagrams easier to see on a dark background">

High contrast mode simplifies and removes non-essential backgrounds and increases the definition between interface elements by adding clear outlines. You may find it is easier to read text and it can reduce eye strain. 

## High Contrast mode

Choose _Settings > Appearance > High Contrast_ from the draw.io menu.

When you enable high contrast modes or themes in your operating system, the range of colours in the interface is reduced and visual elements are simplified. Panels, tools, buttons, and toolbars have simpler backgrounds (white in light mode, black in dark mode), with a clear outline to better separate the various parts of the application's interface. 

In the draw.io editor, **High Contrast** mode works in the same way.
* Panel backgrounds are simplified to off-white (light mode) or nearly black (dark mode).
* Text labels, shapes, and tools that were previously grey are clearer - black (light mode) or white (dark mode).
* Strong contrasting outlines are added around buttons, between the shape libraries, around the format panel tabs and other elements in the editor interface: a crisp white outline in dark mode, and a black outline in light mode.

The default dark mode is on the left in the screenshot below, and High Contrast mode on the right.
<br /><img src="/assets/img/blog/high-contrast-dark-mode-comparison.png" style="width=100%;max-width:500px;height:auto;" alt="High contrast works on all of the draw.io editor themes and in both dark and light mode">

High contrast mode works with all draw.io themes in both dark and light mode, including the Sketch online whiteboard theme. 
<br /><img src="/assets/img/blog/sketch-theme-high-contrast.png" style="width=100%;max-width:400px;height:auto;" alt="High contrast works on all of the draw.io editor themes">

## Better colours for dark mode

Dark mode is often used to reduce eye strain - with draw.io you can diagram in dark mode using any of our editor themes (click the sun/moon icon in the top right and select the mode you want to use. Alternatively, select _Settings > Appearance > Dark Mode_ from the menu).

A while back, we updated [colours automatically change when working with draw.io in dark mode](/blog/dark-mode-diagrams.html), but continue to use the light mode palette as the default. When you switch to dark mode, by default, shapes, connectors and text change intensity to ensure an improved contrast that remains readable. 

* To disable adaptive colours for light and dark mode, make sure nothing is selected in your diagram, then in the document _Style_ tab of the format panel, set _Adaptive Colors_ to _None_. (Also available in the Classic mode menu via _Extras > Adaptive Colors_).
<br /><img src="/assets/img/blog/adaptive-colors-none.png" style="width=100%;max-width:400px;height:auto;" alt="Set Adaptive Colors to none if you don't want your diagram to automatically change colours in dark and light modes">

* If you want only the black and white parts of your diagram to invert in dark or light mode, set _Adaptive Colors_ to _Simple_.

* If you want to [choose specific dark mode colours](/blog/adaptive-colours.html) for shapes, connectors and text instead of using an automatic adaptive colour, add the dark mode colour for that shape in the colour palette under _Advanced_.

**Note:** draw.io Desktop uses the original simple adaptive colours. Set Adaptive colour
