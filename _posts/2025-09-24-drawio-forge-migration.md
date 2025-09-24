---
layout: post
author: draw.io
slug: drawio-forge-migration
date: 2025-09-24 09:54:00
title: The draw.io app for Confluence Cloud transitions to Forge-only
tags: [features, Atlassian]
categories: [features,atlassian]
---

Atlassian has [encouraged all Connect apps to transition to Forge](https://www.atlassian.com/blog/developer/updates-to-marketplace-revenue-share-2026) where their modernised Forge architecture can provide increased data security, updated integrated tools and UIs and other useful features. Our hybrid Connect/Forge draw.io app is currently migrating to be fully Forge-only, allowing for enough time to troubleshoot before the first migration deadline in January 2026, should any problems arise.

You should see no difference in functionality - the diagram editor is not changing, and your existing diagrams and draw.io macros will not be changed through this transition. 

**No full-screen custom macro UI on Forge**

We, like many other app developers, delayed moving draw.io to Forge as Atlassian has not yet implemented the full-screen custom UI dialog that is widely used by many Marketplace apps. 

A reduced diagram editor size may impact productivity or cause distractions as it does not fully cover the page behind. Some have also reported related display issues with dialogs not appearing correctly on mobile devices in the Forge-only apps. 

While we reported this issue back in November 2021, it is currently scheduled by Atlassian to be implemented in FY26Q2 (although, it is not yet included in the [Connect-Forge capability equivalence roadmap](https://developer.atlassian.com/platform/adopting-forge-from-connect/connect-forge-equivalences/connect-forge-capabilities-notavailable/)). 

<img src="/assets/img/blog/drawio-no-fullscreen-forge.png" style="width=100%;max-width:500px;height:auto;" alt="The Forge-only draw.io app cannot run in full screen as Atlassian does not currently support full screen apps in their Forge UI suite - if this is an issue, please add a comment to Atlassian's FRGE-557 or ECO-195 bug reports">

If full-screen diagramming or mobile diagramming is a priority for your teams, or if you are an app developer that is affected by this bug, please do comment on the original [FRGE-557 issue](https://ecosystem.atlassian.net/browse/FRGE-557) and the more recent [ECO-195 issue](https://jira.atlassian.com/browse/ECO-195).

As soon as this issue has been implemented by Atlassian, the draw.io macros in your Confluence Cloud instance will once again work in full screen. 

## Updating your draw.io app

Atlassian may choose to rollout these updated Forge-only apps automatically, or your administrator may need to manually update the draw.io app. 

If your teams require the full-screen app functionality as described above, we recommend not updating the draw.io app until Atlassian has resolved this issue. 

**Note:** No diagrams or macros will be removed from any pages in which they are used or edited in any way. There is no danger of losing data on this update.

## Migrating from DC to Cloud?

Atlassian has also recently [announced the end of life for Data Center](https://www.atlassian.com/blog/announcements/atlassian-ascend), with a three-year staged transition period starting in March 2026.  

If you are migrating from Confluence DC to Cloud because of this, or to take advantage of the enhanced security features of Atlassian's modernised Forge architecture, [migrate your draw.io diagrams in Confluence using the ``PageID`` method](/doc/faq/migrate-drawio-confluence.html) that preserves in-diagram links and embedded diagrams. 

## Which draw.io app for Confluence Cloud?

The [draw.io for Confluence Cloud app](https://marketplace.atlassian.com/apps/1210933/draw-io-diagrams-uml-bpmn-aws-erd-flowcharts?hosting=cloud&tab=pricing) that is transitioning to Forge is available in two editions - Standard and Advanced. The diagramming features of these two editions are the same. 

The _Advanced edition_ of the draw.io app includes premium support, custom security reviews, and additional data security options. 

The [draw.io Zero Egress app](https://marketplace.atlassian.com/apps/1235446/draw-io-zero-egress-diagramming-secured-on-forge?hosting=cloud&tab=overview) is already Forge-only, and provides strict data security, ensuring no diagram data leaves your Confluence instance (zero egress). For customers with such strict data security requirements, Atlassian plans to offer a single tenant _Isolated Cloud_ and their _Atlassian Government Cloud_. The draw.io Zero Egress app is designed to work with Atlassian's new secure Cloud offerings.

[Read more about the differences between the draw.io apps for Confluence Cloud](/doc/faq/confluence-cloud-drawio-zero-egress-vs-app-editions.html) 