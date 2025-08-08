---
layout: post
author: draw.io
slug: uml-package-diagrams
date: 2025-07-30 09:43:00
title: How to draw UML package diagrams
tags: [shape libraries, uml]
categories: [use-cases, templates, shape-libraries]
---

UML package diagrams document the structure of grouped components in a system along with their dependencies, especially for multi-layered web and application architectures. Package diagrams fall in between the detailed [class diagrams](/blog/uml-class-diagrams.html) and the high-level more abstract [profile diagrams](/blog/uml-profile-diagrams.html) and model diagrams. 
<br /><img src="/assets/img/blog/uml-package-example.png" style="width=100%;max-width:600px;height:auto;" alt="A simple UML package diagram to show ">

Packages of 'third-party' code are often used in software projects, reducing the need to develop the entire system in-house. While [UML diagrams](/blog/uml-overview.html) are commonly used for documenting software code in detail, several abstract types of UML diagrams can provide a clear overview of any type of medium to large system or complex service. 

By drawing the system structured into packages, it is easier to identify where components could be externally sourced or re-used in other projects. 

**Tip:** UML diagrams aren't limited to programming - you can document any system or service by grouping subsystems, service bundles, departments, and components into packages for a structured overview.

**Enable the UML 2.5 shape library in draw.io**

Type ``package`` into the search field and press ``Enter`` to see all package shapes. 
<br /><img src="/assets/img/blog/uml-package-search.png" style="width=100%;max-width:350px;height:auto;" alt="Search for package shapes to quickly draw a package diagram in draw.io without enabling shape libraries">

You may find the other shapes and connectors in the UML shape libraries useful.

1. Click on _More Shapes_ at the bottom of the shapes panel. 
2. In the _Software_ section, click on the checkboxes next to the _UML2.5_ and _UML_ shape libraries and click _Apply_.
3. In the shapes panel, you can now see the libraries. Hover over any shape to see its name and a larger preview. 
<br /><img src="/assets/img/blog/uml-package-library-shapes.png" style="width=100%;max-width:500px;height:auto;" alt="The UML 2.5 shape library contains most of the useful package shapes in draw.io">

The _SysML_ shape library in the _Business_ section also contains a number of package shapes.
<br /><img src="/assets/img/blog/uml-package-sysml-library.png" style="width=100%;max-width:500px;height:auto;" alt="The SysML shape library also contains a number of package shapes you can use in your UML diagrams">

**Can I generate this diagram?**

[Mermaid syntax](https://mermaid.js.org/intro/) - the format that most diagram generators use - doesn't currently define package diagrams, but it does support UML class, sequence, and state diagrams.

The [smart templates feature](/blog/smart-diagram-generation.html) in draw.io can provide inspiration for a package diagram as a class diagram, which may be useful when designing a new, large system from scratch. 

Keep in mind that the generator doesn't currently understand the package diagram syntax or shapes and cannot know anything about existing components in your system or third-party offerings that could be used as a 'package', so you will need to edit a generated diagram heavily. 

[_How to write good queries for smart templates_](/blog/write-query-generate-diagram.html)

## Components of a package diagram

**Package:** a container for classes and interfaces. The label can be either in the package tab when the package shape contains other elements, or in the middle of the shape if its elements or contained packages are not drawn. 

<img src="/assets/img/blog/uml-package-shapes.png" style="width=100%;max-width:600px;height:auto;" alt="A simple UML package diagram to show ">

**Dashed connectors:** a dependency between packages. You can add an optional label inside angle brackets to signify various types of dependency: ``<<needs>>``, ``<<use>>``, ``<<import>>``, ``<<access>>`` or ``<<merge>>``. Make sure there are no cycles in merge dependencies.

**Element:** a single element within a package. An element may be a fully contained package, a class, an interface or a subsystem. While package diagrams are generally a simple representation of the static system structure, highlighting an internal element can be useful to show its importance. 

**Combining package and class diagrams:** detail classes inside their package shapes. However, this would only be practical for small systems or to highlight a few specific elements within a system.

## UML package diagram examples

In this simple example of an online shop, the system's elements are separated into one package containing the web and mobile app interface, packages for the shopping cart and payment systems, and one package containing all the databases. 
<br />[<img src="/assets/img/blog/package-diagram-example.png" style="width=100%;max-width:300px;height:auto;" alt="A simple UML package diagram to show ">](https://app.diagrams.net/?page=0&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fuml-package-example.drawio)

This example can be extended into a medium-level overview of a larger company that develops products and sells them both in their physical stores and online in their web app and mobile app. This company employs third-party services for photography, video creation and shipping. 

While this is likely more detailed than most package diagrams as it shows business and application package 'layers' as well the store-related packages, it does illustrate how elements of a more complex business system can be grouped into logical packages. 
<br />[<img src="/assets/img/blog/uml-package-example.png" style="width=100%;max-width:600px;height:auto;" alt="A simple UML package diagram to show ">](https://app.diagrams.net/?page=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fuml-package-example.drawio)



## Other types of UML diagrams

The UML specification allows you to draw many different types of diagrams to model the behaviour and data of a system in different ways.

Refer to the [UML diagram overview post](/blog/uml-overview.html) for details of the many other types of UML diagrams. 

[<img src="/assets/img/blog/uml-2-5-diagram-overview.png" style="width=100%;max-width:500px;height:auto;" alt="Diagram types defined in UML 2.5">](https://app.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&layers=1&nav=1&title=#Uhttps%3A%2F%2Fraw.githubusercontent.com%2Fjgraph%2Fdrawio-diagrams%2Fdev%2Fexamples%2Fconcept-map-uml-diagrams-overview.drawio)