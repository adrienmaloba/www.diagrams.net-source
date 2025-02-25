---
layout: post
author: diagrams.net
slug: collaborative-editing-confluence-cloud
date: 2020-09-15 07:54:00
title: Collaborative editing in draw.io for Confluence Cloud
tags: [features, Atlassian]
categories: [features,atlassian]
---

Confluence allows you to collaboratively edit the content of its pages: You and other Confluence users will see each others' changes in real-time as you edit the page.

diagrams.net already supports collaborative editing online when storing in Google Drive or OneDrive, draw.io for Confluence Cloud now supports collaborative editing. Multiple users can edit a diagram at the same time and see all of the changes that everyone makes.

This is ideal for remote teams who need to brainstorm on mindmaps or vote on agile boards - team members can now all edit the same diagram and see what edits are made.

_In the examples, two browser windows are open and editing the same diagram as if they were two different Confluence Cloud users._

<img src="/assets/img/blog/confluence-cloud-collaborative-editing.gif" style="max-width:100%;height:auto;" alt="Two people editing the same diagram in draw.io for Confluence Cloud will see each others' changes as they are auto-saved">

## How collaborative editing works

The collaborative editing feature in draw.io uses the auto-save feature that is already built into the diagram editor. You don't need to worry about manually synchronising or merging changes.

1. Once you have made a change to a draw.io diagram - added, formatted or deleted shapes, text and connectors, the diagram will be automatically saved.
2. Then these changes will be loaded into the draw.io diagram editor for whoever is also editing your diagram automatically.

If several users add shapes to the same location on a diagram, draw.io will take both shapes and simply overlap them.

<img src="/assets/img/blog/confluence-cloud-collaborative-editing-overlap.gif" style="max-width:100%;height:auto;" alt="When multiple users add shapes in the same location, draw.io for Confluence Cloud will overlap them">

Drag the top shape into a new position to see the underlying shape.


### When a child shape is added to a parent shape that is deleted

Say you add and connect a shape to an existing shape on the drawing canvas and another Confluence user deletes the existing shape.

1. Your new shape will be added and synchronised automatically when your diagram is auto-saved.
2. The existing shape along with any connectors coming from it will be deleted when the other user's diagram is auto-saved.

<img src="/assets/img/blog/confluence-cloud-collaborative-editing-delete.gif" style="max-width:100%;height:auto;" alt="If a parent node is deleted by one user, but a child shape is connected to that parent node by another user, the connector from the parent to the child shape will be deleted when the diagram is auto-saved">
