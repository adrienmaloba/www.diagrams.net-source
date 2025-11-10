---
layout: post
author: draw.io
slug: diagrams-in-plane
date: 2025-11-10 09:54:00
title: Diagram with draw.io in Plane.so pages
tags: [features]
categories: [features,integrations]
---
Plane.so, a project management platform, has developed a draw.io integration where you can add, edit and store draw.io diagrams in [Plane.so](https://plane.so) pages. Plane is a useful platform for technical documentation and project management for distributed teams. Both the simple draw.io [Board editor](/blog/sketch-online-whiteboard.html) and the full draw.io diagram editor are available, with all the standard built-in draw.io shape libraries and templates, as well as the [generated smart templates](/blog/smart-diagram-generation.html) and [Mermaid diagram](/blog/mermaid-diagrams.html) support.
<br /><img src="/assets/img/blog/plane-page-diagram-light.png" style="width=100%;max-width:500px;height:auto;" alt="draw.io diagrams can be embedded and stored in Plane.so pages">

[Plane.so is a collaborative workspace for teams](https://plane.so) that can be deployed in the cloud, self-hosted in your own infrastructure or air-gapped for regulated industries. The project management platform has a range of features for IT, software development, marketing and sales - any team that needs projects, knowledge and agents in one space. 

## Install draw.io in your Plane workspace

1. Click on the configuration icon to open your Plane _Settings_.
2. Select the _Workspace_ tab.
3. Select _Integrations_ from the left hand menu. 
4. Click on _Configure_ under the draw.io integration and follow the prompts to set it up.
<br /><img src="/assets/img/blog/plane-drawio-integration.png" style="width=100%;max-width:500px;height:auto;" alt="Install the draw.io integration in Plane.so to embed and store diagrams in your Plane pages">

To uninstall the draw.io integration from your Plane workspace, click on the three vertical dots next to the green _Installed_ flag and select _Uninstall_.

## Add a diagram to a Plane page

* Type ``/draw`` and select the _Draw.io diagram_ to add a diagram macro to the page. If you want a simpler whiteboard editor, select the _Draw.io board_ macro. 
    <br /><img src="/assets/img/blog/plane-add-diagram.png" style="width=100%;max-width:400px;height:auto;" alt="draw.io diagrams can be embedded and stored in Plane.so pages">
* Click on the macro to open the draw.io editor. 
 <br /><img src="/assets/img/blog/plane-edit-diagram.png" style="width=100%;max-width:400px;height:auto;" alt="draw.io diagrams can be embedded and stored in Plane.so pages">
* When you have finished diagramming, click on _Save_ to return to the Plane page. 
 <br /><img src="/assets/img/blog/plane-drawio-editor.png" style="width=100%;max-width:400px;height:auto;" alt="draw.io diagrams can be embedded and stored in Plane.so pages">

Your diagram will now be displayed inline. To edit it again, simply click on it. 

**Important:** Diagram changes are not included in the page version history - your document will always display the most recent version of the embedded diagram.
 <br /><img src="/assets/img/blog/plane-version-history.gif" style="width=100%;max-width:400px;height:auto;" alt="Embedded draw.io diagrams are not versioned along with the page content in Plane.so">

## Diagram in dark or light mode

You can use the draw.io editor in dark or light mode and the colours of shapes and text will adapt.

draw.io uses [adaptive colours](/blog/adaptive-colours.html) by default, so that team members who prefer to work in dark mode will still be able to read the diagrams added to a page in light mode. 
<br /><img src="/assets/img/blog/plane-page-diagram-dark.png" style="width=100%;max-width:500px;height:auto;" alt="draw.io diagrams in Plane pages will automatically change colours depending on whether you view them in dark or light mode">

## Add diagrams to Plane work items

While the work item description can only contain text, you can add a draw.io diagram two ways.
1. Attach a ``.drawio`` file to the work item. 
2. Link to a Plane page containing a draw.io diagram. 
 <br /><img src="/assets/img/blog/plane-diagram-attached.png" style="width=100%;max-width:400px;height:auto;" alt="draw.io diagrams can be attached as files to work items, or linked to the Plane page that includes the diagram">

## Do more with diagrams in Plane

As you have probably experienced, diagrams can take some time to draw. Where diagrams are a big part of your project documentation and need to be scheduled to certain team members, add a label to the work items that are diagrams. 
 <br /><img src="/assets/img/blog/plane-add-label.png" style="width=100%;max-width:500px;height:auto;" alt="Label work items that require diagramming documentation (or that contain diagrams) to View only those work items">

Then, add a view that filters for that tag, and displays the work items in a timeline for a handy Gantt chart to plan and track your team's diagram development schedule.
 <br /><img src="/assets/img/blog/plane-view-label.png" style="width=100%;max-width:500px;height:auto;" alt="Label work items that require diagramming documentation (or that contain diagrams) to View only those work items">

## Embedded editor limitations
As the draw.io editor is embedded in a Plane page macro, there are a few limitations. There is currently no support for:
* customise the [draw.io editor configuration](/doc/faq/configure-diagram-editor.html)
* [custom shape libraries](/blog/custom-libraries.html) and [custom templates](/blog/custom-template-libraries.html)
* displaying [multi-page diagrams](/blog/multiple-page-diagrams.html) - the page will display the last diagram page tab you had open in the draw.io editor.

For custom templates, store your template diagrams in GitHub or on a cloud platform or shared drive within your network and import this file into a new diagram on a Plane page - in the draw.io editor, click _File > Import from > URL_.

**Important note:** This is a third-party integration 

To use expanded or updated features that you have been used to in the draw.io editor also in the Plane.so integration, please contact Plane.so support and raise a request with them. We have not developed this integration so can not help you with any problems with it.


