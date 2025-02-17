---
title: Generate code to embed a diagram in a webpage
layout: page
faq: true
categories: [Integrations, Features]
---

You can easily save your diagram as an image or a [SVG file](/doc/faq/embed-svg.html), which you can embed in your website. Or you can embed HTML or an IFrame into your web page as described below.

Select _File > Embed_.
<br /><img src="/assets/img/blog/file-embed.png" style="max-width:100%;height:auto;" alt="Click File > Embed and select HTML to export your diagram as HTML code">

## Embed a diagram using HTML

1. Select _File > Embed > HTML_ to open the HTML options dialog.
2. Select from the following [embed HTML options](/doc/faq/embed-html-options.html), then click on _Create_.
  * Include a copy of your diagram in the HTML or use the public link to your original diagram file.
  * Choose whether you want _Links_ to open in the current window or in a new window, and change the _Border Color_ to change the link highlight colour.
  * Set your diagram to open in dark or light mode (default _Appearance_ is _Automatic_).
  * Choose whether to zoom in or out.
  * Select you want to include all pages, layers, and/or tags.
  * If you want to display the diagram in a lightbox, choose what should happen when a user clicks on the edit icon.
  <br /><img src="/assets/img/blog/embed-html.png" style="width=100%;max-width:300px;height:auto;" alt="Generate a HTML code version of your diagram">
1. Copy the generated HTML code and paste it into your webpage.
<br /><img src="/assets/img/blog/diagram-html.png" style="width=100%;max-width:300px;height:auto;" alt="Copy the generated HTML code">

When you load the webpage in your browser, the diagram will appear with a toolbar, if you have used the default settings.
<br /><img src="/assets/img/blog/embedded-html-diagram.png" style="width=100%;max-width:300px;height:auto;" alt="A diagram embedded using HTML">

## Embed a diagram using an IFrame

An IFrame (Inline Frame) is an HTML document embedded inside another HTML document on a website. This means that your diagram file must be stored as a public file - for example on Google Drive.

1. Select _File > Embed > IFrame_ to open the IFrame options dialog.
2. Set the options you want to use within the IFrame. They are similar to the HTML options described above. Once you are done, click _Create_.
<br /><img src="/assets/img/blog/embed-iframe.png" style="width=100%;max-width:300px;height:auto;" alt="Generate a HTML code version of your diagram containing an iFrame">
   * By default, when you open the link it will create a copy of the diagram in the users' browser. If you have saved your diagram on a cloud platform, you can change this to _Authorisation required_, or to share the _Public URL of the diagram_.
   * Set the _Width_ and _Height_ to change the size of the diagram iFrame. 
  * Choose whether you want _Links_ to open in the current window or in a new window, and change the _Border Color_ to change the link highlight colour.
  * Set a transparent background. 
  * If you want to display the diagram in a _Lightbox_, choose what should happen when a user clicks on the _Edit_ icon.
  * Select you want to include layers and/or tags.
1. draw.io will generate the HTML code that contains the IFrame. Copy this HTML code containing the IFrame, and paste it into your web page.
<br /><img src="/assets/img/blog/iframe-code.png" style="width=100%;max-width:300px;height:auto;" alt="Copy the generated IFrame HTML code">

IFrames use the draw.io lightbox and centre the diagram in the page. If you have used the default settings, a toolbar will appear at the bottom of your diagram when you hover over the HTML page.
<br /><img src="/assets/img/blog/embedded-iframe.png" style="width=100%;max-width:300px;height:auto;" alt="An embedded IFrame is displayed in the draw.io lightbox">

## Related
* [Use diagrams in Google Docs](/blog/diagrams-google-docs.html)
* [Embed a diagram into Google Sites](/doc/faq/embed-diagrams-google-sites.html)
* [Embed diagrams from Google Drive into Confluence](/doc/faq/embed-diagram-googledrive-confluence-cloud.html)
* [Embed diagrams from OneDrive into Confluence](/doc/faq/embed-diagram-onedrive-confluence-cloud.html)
* [Embed a diagram as an SVG image](/doc/faq/embed-svg.html)
* [Embed diagrams into GitHub pages](/blog/embed-diagrams-github-markdown.html)
* [Simple draw.io embedding walk-through][/blog/embedding-walkthrough.html]
