---
layout: post
author: draw.io
slug: plantuml-to-mermaid
date: 2025-06-05 09:43:00
title: Migrate diagrams from PlantUML to Mermaid and draw.io
tags: [shape libraries, uml]
categories: [use-cases, templates, shape-libraries]
---

Diagrams from text are oft faster for programmers to draw than to spend time manually styling and aligning the diagram elements. PlantUML support in draw.io is being phased out at the end of 2025, so here are some ways you can migrate your PlantUML diagrams to draw.io or rewrite them in [Mermaid syntax](https://mermaid.js.org/intro/syntax-reference.html).
<br /><img src="/assets/img/blog/plantuml-mermaid-comparison-hover.png" style="width=100%;max-width:500px;height:auto;" alt="Comparing a PlantUML state diagram with a Mermaid diagram of the same state">

**Why is PlantUML support being removed?**

PlantUML's lack of security reviews makes draw.io updates more difficult. Mermaid's breadth of diagram types, its popularity and its client-side architecture is more in line with the draw.io tool. See the [deprecation notice on the draw.io GitHub repository](https://github.com/jgraph/drawio/discussions/5074) for full details.  

Support for [PlantUML](https://plantuml.com) will be removed at the end of the year (2025) in our online version at [app.diagrams.net](https://app.diagrams.net), and in 2028 in the draw.io apps for Confluence and Jira Cloud. 

**Disclaimer:** We've linked several open-source projects and tools below. We don't endorse these tools specifically but want to highlight that PlantUML tools are readily available.

**Your PlantUML diagrams will still work**

This will not remove any PlantUML elements you have in your diagrams - the images and the underlying text description will still be there. You will still be able to copy the PlantUML text and paste it into another tool, such as the [PlantText](https://www.planttext.com) or [PlantUML](https://plantuml-editor.kkeisuke.com) online editors, or [PlantUML diagrams for Confluence](https://marketplace.atlassian.com/apps/1215115/plantuml-diagrams-for-confluence?hosting=cloud&tab=overview).

Until support is removed, when you try to insert PlantUML into a draw.io diagram via _ Advanced > PlantUML_ in the simple editor theme or _Arrange > Insert > Advanced > PlantUML_ in the classic editor theme, you will see a warning.
<br /><img src="/assets/img/blog/plantuml-deprecated-warning.png" style="width=100%;max-width:400px;height:auto;" alt="A warning about PlantUML support being phased out by the end of 2025 in the online draw.io editor">


## Convert your PlantUML to draw.io diagrams

There are several third-party tools that can convert your PlantUML text into draw.io diagrams. [plantuml2drawio](https://github.com/doubleSlashde/plantuml2drawio) and [plantuml_to_drawio](https://github.com/rglaue/plantuml_to_drawio) are both available on GitHub.  

The [pu2mm tool](https://opoto.github.io/pu2mm/) can convert PlantUML sequence diagrams to Mermaid. And there are many tools that can convert your code directly to a variety of Mermaid diagrams, such as [PythonToMarkdown](https://github.com/ctrlvee85/PythonToMermaid), [flomatic](https://github.com/romilly/flomatic), and [pymermaider](https://github.com/diceroll123/pymermaider).

**Disclaimer:** We don't endorse these tools specifically but want to highlight that PlantUML-to-Mermaid conversion tools and Mermaid-from-code generation tools are available.

Once you have the Mermaid code, insert it into draw.io and save it either as an image on the canvas (so you can edit the Mermaid code - click on the example below), or convert it to a diagram to style. 
<br />[<img src="/assets/img/blog/mermaid-sequence-example.png" style="width=100%;max-width:400px;height:auto;" alt="A simple sequence diagram inserted using the Mermaid syntax">](https://app.diagrams.net/?lightbox=0&highlight=0000ff&edit=_blank&layers=1&nav=1&page=3&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fmaster%2Fblog%2Fmermaid-examples.drawio)

[Learn more about working with Mermaid diagrams in draw.io](/blog/mermaid-diagrams.html).

**Write a Mermaid version of a PlantUML diagram** 

It is not difficult to rewrite PlantUML code as Mermaid code as the syntax for both diagrams is roughly the same. 

In the following example, the same state diagram has been written in both PlantUML and Mermaid and inserted on the canvas as an image. 
<br />[<img src="/assets/img/blog/plantuml-mermaid-state-comparison.png" style="width=100%;max-width:600px;height:auto;" alt="Comparing a PlantUML state diagram with a Mermaid diagram of the same state">](https://app.diagrams.net/?page=0&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fplantuml-to-mermaid-example.drawio)
<br />[_Open this example then double click on one of the state diagrams to edit the PlantUML or Mermaid_](https://app.diagrams.net/?page=0&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fplantuml-to-mermaid-example.drawio)

**State diagram in PlantUML**
```
@startuml
  [*] --> Reconnecting
  state Reconnecting {
    [*] --> EstablishingConnection
    EstablishingConnection --> EstablishingConnection : failed [no connection] /wait 5s then reconnect
    EstablishingConnection --> [*] : success [connection established]
    ||
    [*] --> Listening
    Listening --> VerifyingAccess : key presented [valid RFID code] /verify
    VerifyingAccess --> Listening
    state VerifyingAccess{
      [*] --> CheckingInternalRecords
      CheckingInternalRecords --> KeyAccessVerified : key allowed [valid key]
      KeyAccessVerified --> Unlocked : [valid key] /unlock
      Unlocked --> [*] : wait 5 seconds after door close [unlocked] /lock
      CheckingInternalRecords --> InvalidKey : not found [invalid key] /ignore
      InvalidKey --> [*] : /ignore
    }
  }
@enduml
```
**State diagram in Mermaid**
```
stateDiagram-v2
  [*] --> Reconnecting
  state Reconnecting {
      [*] --> EstablishingConnection
      EstablishingConnection --> EstablishingConnection : failed [no connection] /wait 5s then reconnect
      EstablishingConnection --> [*] : success [connection established]
  --
  [*] --> Listening
  Listening  --> VerifyingAccess : key presented [valid RFID code] /verify
  VerifyingAccess --> [*]
  VerifyingAccess --> Listening
    state VerifyingAccess{
      [*] --> CheckingInternalRecords
      CheckingInternalRecords --> KeyAccessVerified : key allowed [valid key]
      KeyAccessVerified --> Unlocked : [valid key] /unlock
      Unlocked --> [*] : wait 5 seconds after door close [unlocked] /lock
      CheckingInternalRecords --> InvalidKey : not found [invalid key] /ignore
      InvalidKey --> [*] : /ignore
    }
  }
  ```