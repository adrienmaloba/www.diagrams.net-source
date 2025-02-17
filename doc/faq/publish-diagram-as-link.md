---
title: Publicly publish a diagram as a link
layout: page
faq: true
categories: [Features,Export]
---

You can encode a diagram created in draw.io within a URL. When someone clicks on that URL, they will see a static copy of your diagram, at the time you published it, in the draw.io viewer.

As different browsers have varying URL size limitations, very large diagrams may not be able to be loaded from a overly long URL. To get around this, use Google Drive to store your diagram - when you [publish a diagram publicly from Google Drive](/doc/faq/google-drive-publicly-publish-diagram.html), the URL will be shorter and neater.

1. Select _File > Publish > Link_.
<br /><img src="/assets/img/blog/file-publish-link.png" style="width=100%;max-width:300px;height:auto;" alt="Select File > Publish > Link to publicly publish your diagram as a link">
2. Select the link options you want to use, then click _Create_.
<br /><img src="/assets/img/blog/publish-link-options.png" style="width=100%;max-width:300px;height:auto;" alt="Set the options you want to encode along with the diagram in the URL">
   * By default, when you open the link it will create a copy of the diagram in the users' browser. If you have saved your diagram on a cloud platform, you can change this to _Authorisation required_, or to share the _Public URL of the diagram_.
   * By default _Links_ will open following the viewer's browser preferences. Select a different behaviour if you want links to always open in a new tab or a new browser window. If you want, set a different link _Border Color_.
   * If you want to force your diagram to appear in dark or light mode on a dark background, select it from the _Appearance_ drop down list. 
   * To open your diagram directly in the draw.io editor, deselect the _Lightbox_ checkbox. 
   * By default, viewers can edit a copy of the diagram from the draw.io lightbox - change the behaviour or deselect the _Edit_ checkbox.
   * Deselect the _Layers_ and/or _Tags_ checkboxes if you don't want viewers to interact with the layers in your diagram.
3. Copy the link that is generated (press ``Ctrl+C`` on Windows or ``Cmd+C`` on macOS). Click _Close_ to return to your diagram.
<br /><img src="/assets/img/blog/published-link.png" style="width=100%;max-width:300px;height:auto;" alt="Copy the generated link and share it with your intended diagram viewers">

**Note:** The diagram data is embedded in the URL you just created - your diagram is not hosted anywhere. This link is therefore always valid, and you can't _revoke_ access to your diagram.
