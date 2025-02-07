---
title: Configure default adaptive colours
layout: page
faq: true
categories: [Shapes,Connectors,Text]
---

Colours of shapes, connectors, text and diagram backgrounds in draw.io automatically adapt when you change between light and [dark mode](/blog/dark-mode-diagrams.html). This is important when some members of your team work in light mode, and others prefer dark mode. 

There are three adaptive colour settings. 
* **Automatic:** Changes the intensity to enhance the contrast of all coloured elements in a diagram.
* **Simple:** Improves the contrast of only the black and white elements, and retains all other colours. Thus the same palette can be used in dark and light modes. 
* **None:** Disables adaptive colours in dark mode completely. Diagrams will appear as they would in light mode even if you enable dark mode in the draw.io editor. 

<img src="/assets/img/blog/style-tab-adaptive-colors.gif" style="width=100%;max-width:500px;height:auto;" alt="Change the adaptive colours settings on a diagram in draw.io via the Extras menu or the Style tab in the format panel when nothing is selected">


The default is _automatic_, but you can set _simple_ or _none_ as your custom default via the draw.io editor configuration. Select _Extras > Configuration_ or _...> Settings > Configuration_ to open the configuration settings. 

Enter either ``automatic``, ``simple``, or ``none`` as the value for ``defaultAdaptiveColors`` in the configuration, then click _Apply_
```
{
  "defaultAdaptiveColors": "simple"
}
```
<img src="/assets/img/blog/adaptive-colors-configuration-dialog.png" style="width=100%;max-width:300px;height:auto;" alt="Select one or more shapes and open the colour palette">

Reload the browser tab to load your configuration with a different default. This will be shown in brackets on the _Adaptive Colors_ setting in the diagram _Style_ tab.
<br /><img src="/assets/img/blog/adaptive-colors-configured-default.png" style="width=100%;max-width:200px;height:auto;" alt="Select one or more shapes and open the colour palette">

## Related

* [Using adaptive colours and dark mode in draw.io](/blog/adaptive-colours.html)
* [Configure the draw.io editor](/doc/faq/configure-diagram-editor.html)
* [Configure the draw.io app in Atlassian Confluence Cloud](/blog/configure-drawio-app.html)
