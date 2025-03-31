---
layout: post
author: draw.io
slug: uml-profile-diagrams
date: 2025-03-28 09:43:00
title: How to draw UML profile diagrams
tags: [shape libraries, uml]
categories: [use-cases, templates, shape-libraries]
---

Profile diagrams are one of the newer UML diagram types, providing a broad overview of a system showing how the system can be implemented in different domains. Stereotypes and constraints indicate which sub-systems and components, languages and processes are modified in different use cases.
<img src="/assets/img/blog/profile-diagram-example.png" style="width=100%;max-width:500px;height:auto;" alt="A class diagram based on the basic class diagram template in draw.io"><br />
[_Open this example in draw.io_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=0&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fuml-profile-example.drawio)

Profile diagrams provide a high-level abstract view of a system and were originally part of SysML, recently brought into the [UML standard](https://www.omg.org/spec/UML/2.5.1/About-UML/). 

They are often drawn for software applications within complex systems where components need to be specialised to run on different platforms, use different database systems, or be programmed in different languages.

UML profile diagrams can help non-technical stakeholders understand which aspects of a system need to be changed to apply to a new domain. 

**Tip:** Profile diagrams may also show ownership and responsibility, as well as management or configuration options. 

## What are profile diagrams?

It may be easier to understand why profile diagrams are useful with a physical example.

Take a company that manufactures garden hoses. They use UML diagrams to document their production processes which specify how the materials they use need to be procured, stored, processed, and the final product packaged. These diagrams would include the data that should be gathered, constraints on the machines during the production process, and how the final product should be quality tested. 
<br /><img src="/assets/img/blog/uml-profile-hose-production-flow.png" style="width=100%;max-width:600px;height:auto;" alt="A flow diagram example for manufacturing a hose">

All the processes, data structures, machine setups, controlling and monitoring software applications, and testing procedures would be visualised in a [variety of UML diagrams](/blog/uml-overview.html). Together, they comprise the UML model of the hose production system. 

This company wants to start producing flexible tubes for a new domain - medical. The overall process for producing flexible medical tubes and garden hoses is similar - purchase the raw materials, mix them appropriately, extrude the hoses with production machines, cut to length, test, package, and send to vendors or customers. 
<br /><img src="/assets/img/blog/uml-profile-hose-medical-production-flow.png" style="width=100%;max-width:600px;height:auto;" alt="A flow diagram example for manufacturing a hose">

However, medical applications have more stringent requirements including constant testing. Materials must be safe for prolonged human contact. A clean room environment may be needed for production. There may be mandated software and hardware components for monitoring safety throughout the production process. And quality testing of the final product would be more rigorous - perhaps through an accredited third party. 

The UML model for producing garden hoses can be abstracted into a metamodel that visualises the production of any type of flexible hose or tube, where profiles are used to specify what is needed for each domain - in this case, _Garden_ and _Medical_.
* Metaclasses are the most basic elements of the hose production system - they show in a very general abstract way how a hose is manufactured. 
* Stereotypes specialise metaclasses and show which packages, processes and/or data structures are modified to meet either the Garden or Medical hose production requirements.
* In the lower-level, more detailed UML diagrams, tagged values, constraints and ``<<stereotype>>`` labels show which elements of each diagram have a stereotype applied.

For the hose production company example described above, the following UML profile diagram abstracts their garden hose production line model and customises it for a medical domain. 
<br />[<img src="/assets/img/blog/uml-profile-hose-example.png" style="width=100%;max-width:600px;height:auto;" alt="A profile diagram for manufacturing both garden hoses and medical hoses">](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=0&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fuml-profile-hose-production-example.drawio)
<br />[_Open this example in draw.io_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=0&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fuml-profile-hose-production-example.drawio)

## Elements of a UML profile diagram

**Enable the UML and SysML shape libraries**

Click on _More Shapes_ and enable the UML, UML2.5 and SysML shape libraries to see the profile diagram shapes and connectors in draw.io. Alternatively, use the search bar to quickly find ``stereotype``, ``profile`` and ``metaclass`` shapes. Hover over any shape to see a larger preview.
<br /><img src="/assets/img/blog/uml-profile-search-stereotype.png" style="width=100%;max-width:350px;height:auto;" alt="Search for shapes to quickly find stereotypes, profiles and metaclasses in draw.io">


### Profiles

**Profiles** are drawn with a package shape and the ``<<profile>>`` label. An open-ended arrow on a dashed connector goes from the profile to the package or metaclass with the label ``<<apply>>``. You can apply more than one profile to a package or class.
<br /><img src="/assets/img/blog/uml-profile-shapes.png" style="width=100%;max-width:500px;height:auto;" alt="Use the package shape with the profile label in angle brackets to draw a UML profile diagram">

### Metaclasses and stereotypes

**Metaclasses** are the foundational elements that need to be customised for each domain. In the high-level abstract, these may be simple rectangles or package shapes with a ``<<metaclass>>`` or ``stereotype`` label.  

**Stereotypes** are classes or packages that are used to customise entities, data structures, processes, and services (meta-attributes) so they can be used in another domain. Stereotypes define tagged values and constraints that show how your system is implemented in lower level UML diagrams, 'extending' metaclasses.
<br /><img src="/assets/img/blog/uml-profile-stereotype-shapes.png" style="width=100%;max-width:250px;height:auto;" alt="Classes or packages in a profile diagram contain the label stereotype when modified for a specific domain">

Stereotyped classes contain the ``<<stereotype>>`` label in addition to the entity's name but may simply write the name of the entity surrounded by angle brackets: ``<<Garden>>`` or ``<<Medical>>`` when a class or package belongs solely to one profile.

### Tagged values in stereotype classes

**Tagged values** are metaproperties in that provide additional information about the domain-specific processes and attributes, indicating how that component is used or instanced in a specific domain, or who is responsible for it. Tagged values are surrounded by curly brackets.
<br /><img src="/assets/img/blog/uml-profile-tagged-values.png" style="width=100%;max-width:150px;height:auto;" alt="Write the tagged values in the header of stereotype classes, surrounded with curly brackets">
  
### Constraints 

**Constraints** define conditions or rules that apply to profiles, or to elements within a stereotype. These are written in a note shape and attached to the stereotype or profile with a dashed line.
<br /><img src="/assets/img/blog/uml-profile-constraints.png" style="width=100%;max-width:300px;height:auto;" alt="Write the tagged values in the header of stereotype classes, surrounded with curly brackets">


## Combining profile and class diagrams

It is common to combine the profile overview with stereotype class definitions for one or more of the profiles, as in the diagram below.
<br />[<img src="/assets/img/blog/uml-profile-hose-example-class.png" style="width=100%;max-width:600px;height:auto;" alt="UML profile and stereotyped class diagrams are often combined into one diagram">](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=1&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fuml-profile-hose-production-example.drawio)
<br />[_Open this example in draw.io_](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&page=1&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fblog%2Fuml-profile-hose-production-example.drawio)


## Other types of UML diagrams

The UML specification allows you to draw many different types of diagrams to model the behaviour and data of a system in different ways.

[<img src="/assets/img/blog/uml-2-5-diagram-overview.png" style="width=100%;max-width:500px;height:auto;" alt="Diagram types defined in UML 2.5">](https://app.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fconcept-map-uml-diagrams-overview.drawio)

Refer to the [UML diagram overview post](/blog/uml-overview.html) for details of the many other types of UML diagrams. 