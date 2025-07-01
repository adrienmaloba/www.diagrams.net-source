---
layout: post
author: draw.io
slug: generated-diagrams
date: 2025-06-16 09:24:00
title: When does it make sense to generate a diagram?
tags: [features]
categories: [features, import, templates]
---

In draw.io, the smart templates feature allows you to generate a diagram from a text description. It's easy to get hyped up about quickly generating visual documentation, but when _should_ you generate a technical diagram? What types of diagrams can't be generated? 
<br /><img src="/assets/img/blog/generated-diagrams-when.svg" style="width=100%;max-width:500px;height:auto;" alt="When should you use a diagram generator to draw technical diagrams?">

[_Open this diagram in draw.io_](https://viewer.diagrams.net/?lightbox=1&target=blank&highlight=0000ff&edit=_blank&nav=1&title=generate%20a%20diagram&dark=auto#R%3Cmxfile%3E%3Cdiagram%20id%3D%22wyUT3EkfGjSy6rjJWVdl%22%20name%3D%22When%20to%20generate%20a%20diagram%22%3E7Vxpj9u4Gf41xn6agU4fH%2BfMBtgWQdN2234paImyuJFEh6LG4%2Fz68tQtmxNbM5a3AZJYFG%2B%2Bx%2FMe1Mx9SF8%2FEbCN%2F4JDmMwcK3yduY8zx7E9z2L%2F8ZK9LFksVMGGoFBVqgq%2Boh9QFepqBQph3qhIMU4o2jYLA5xlMKCNMkAI3jWrRThpjroFG9gp%2BBqApFv6OwpprErt%2Bap68StEm1gNvXQW8kUKdGW1kjwGId7VitynmftAMKbyV%2Fr6ABO%2BeXpfZLvngbflxAjMqEmD%2F%2F5n%2F7fH19%2B97%2Bsf%2F3z4Fw3ul%2FPNjeolp3u9YBiy9atHTGiMNzgDyVNVek9wkYWQ92qxp6rObxhvWaHNCv%2BAlO7VYYKCYlYU0zRRb%2BWYfKDBpeh54YIE8MD8PUUSgGwgPVDP8codZ6QKcQop2bOGBCaAopfmRICimU1Zr9pW9kPt7Bt22ZH9voCkUCP9m9F0387%2FBtaMgRq7BRK0ydjvgG0OJKzgBRKKGIXeqRcpCkN5MDBHP8Ba9MePZotRRsVa%2FPuZ%2F1juPO8Avs562Ec1roi2fibDBNTdV9X7jXXryo4U%2B6vzMt521fMXvpJat06j0xu%2F2QGOopxRQ%2FvUyun9%2FEG6nYP8K%2F6TcJDtjsNBeP0Hl9uOlUjS580eMT9cXHD5zw%2FSWrPdYLTPR8uLhNG0Y%2B0Qk69spIyfWcqlOFssBCRgUve5oShkn3cvmB0tq7OFWYiyDft591lU%2BgYz3iGKBrpzLMyHhq8op7IhfAXpNuFVEG%2B5wZj3DDNcbOJbOfZBMqoLI0V2NfqpqIMf9S5GFH7dAnGIO6Zkm5QQoSR5wAmbIW%2FrhlYAIev7PqeELUy%2FCWEE2L7x%2Bjijiqxs%2B5BE6NDSIJPb9spqMrlW%2BruaxtQSJa4py7n1ZnJhj4pi3sC2%2FsR5dGXKo4sTeVQ0vSME7GsVlBoZlMbzRev47RYQade3D9ZnP%2BQMziq559ergv1jKnjhuk0t7JymhcfXs4s%2FCcM6q49g2MVhBuzWP8zg4zDs0hRqTY5fB4T0ZfJrHzy7I7DEZwKerDEgClMB9jeDO35M%2B5zCdOY88D0hOIB5rqEU4scSCUjTB9UeIQUoEbWjJvCSfeYCqIVVv1ySs1FhKHoSeJFXCYKCAApvNdTbwAyyAkxEB2IREUhxwR8jMbEYJEkRoAzw8UyQXJ1%2Fp4%2Fk5m6T0V3nwoCcFlwGanw6ysJ2TbWFc6K2OMmJYU%2FdV2S%2BzwOIalytbHsttTz3juDo1cH646hlu%2BvLuha9bB%2F1Za3s8ypm7b9yzuDA6lPUD8KdIRV1CPOAoLXS3FzZhQhsCEj5liUQkGRfqlUIciQeEW%2F%2FvYB8zD5N%2FQSEf4SitEIEBEYoqw0jmyvFjFKmsl%2F4WxrD%2Bhw4SkBUHF8u%2FDvSL8N19%2Beo7DsA2S%2B0MeHaskRzMeMdJmEu%2BwwJ2Ol3fEI5TCLeqYFub3i8pq%2Fcbde%2FcDeN7ZnKlgkpnYWp0jnVFDxNuU%2FdRWa%2Bzx%2Bi3Ns%2Br8vU7VfsJLOPesmWC%2FvE6NS51fcjFoat0mtsU4GooSIfpSW94UburBYR4euqRysSmEKxwb1xkY5lvEOCVDLMB%2FuW4V2lrZuGudgnYXSXdvlDiSFYC4YEsLCyA4FDZIdKIYsSbaFXQMDE5m54uaevl%2F2LV8vLiesGDdOP6gbvVAN7wLLrOFwXLcAvZ6aand%2Bdbq9MgdX05PrymFx3%2Fcbe69yBU1MQWkeqUwPGj42U%2BURXz47ugOB8p6Qd%2B3rRUC0BrbGz53VraF%2FR%2BXHRTDsE6k7%2FIhdJG1sYoAgFM5Fxt4Vl0EGcmcBTyilS94EMQ6PKS9IASTgT7gc55hrkYsAowbsgBoTWB5dwSB0Va2wCcZy6Ipo%2BxLH9tgK8NIzjuFMXqsaZkB%2Fj3Hb8CRjATtcB9Q%2FB4O2MsDlIOZdl63wrjnEuOCdEL%2BznhkqhrvLUhOzRNXh0NGZmkeh7%2Fr3gub%2BMIChPZr7ji3Oed7vdLbeREL4NMBM7zyrZ7EYJorxqqAfj1W8RFlafqJvr8VhzoGsNzZrVqU28Zy1ACs18i5j0QzgbatjiHyEA2U%2B272ibQxNB9Qp1Bjh%2F3kKC2Ily7ak7%2BVIV3Ycgj0sZyB%2B%2BAJ4kyHUrVzyW7XSFXxQFwWrVEX7sjTt3V244kvizWwkUvu91xd%2F8POLPkNL9DqU%2FSsNcWPpH6bvUij9JUynICpBwFfomWooZgTMR2yIOVVoSh%2FN2WuuhkyA4SCfyjb4T4IwUkPec26b5Ml92NefK71LOcjTKMXcSTkd7unND7XnqNYIzegwNj2vqqXSOcS7dhwCbdm7cZeKa602mc45m0y1tb5Sg%2FarZ4lzG7WcR%2FI7FxQKgrU5uXRrrZG7LDmvVpoVbH0BCVbBmmk0GGirTN5SRCOnBR1mQFKHIsMtkCL4RFVCWdd0ON8gENLKKryvbruMVvjSj2J26p9HVN0YvU3fY%2FhSUh9v1gz7EMPimbYWTjNsQMwHxHIHv7F9mYjJ2umGiYpuIoOCwnVvVsRK0JoDs%2By1e6Xw7KjlhJhSPXhDYMim1JUgOcMry1gnesP%2BE%2BXIjZ4pgjwUv7Ru9GDRowP%2Ff7n6T3e35TeOpz%2B523Pe0u12nw0wTl7GeqYyVNtbZg6vLVs66t2idnVxBJ7balcZWOxDf7mnkKK3OLb1ClO46%2FWdfofQzgfJWixFvgnsT51tjl8fJn074OWxktbCOv%2FTeAet03aJXw4IDx1ix4Ny13NO4cODzDDqvcBRTWWTHAbEzacqDEzWzle45EjLLepP3wTQOxNJUDYsANkzkMsKrct1SlIUpYBDQeaYE1hLZqshvDr8XMAvq7wwT0Bsac%2Fr2rm21VfXFGbyLa0Nnxt5T79Rcm7HRme19MDrr%2BlCvJh3IPepEbUr084C198Nqq4lzsbGN9TF%2BrJU7ATeWFh9Xyb8Dd4dqNxetlT0CC%2BuvR435hQGG6yLGfgqZCfeauNagYiRsc9hBFAkgGvCpOMTB1L7anUJ1wyGW9xzwrLyioAbo61NgP9b8F0F3a%2FklgVx%2BokqivlTefKjdcKCxvPMgYiZN%2FGmIBxs6evp4cNn%2BrMj7wcE%2BmvskTwNKc%2BINGTDizZqYuGlbn7kYvpErclS5VaNvz4oC6Z7%2BmsoM079XTvAIAloIghP1lKPclKycg2Rl7EcGPOTHj0g4lLs0dr96su78g07gd0mqsRf6PkT5PRu%2FS3h2D%2BGVhWMbIt6HpKPW99o6M4IxTU%2F1zoJgetxJTlPYLK33vYKjN6DuWYKVxpGMn3LNpvXVT0v21ikeCLkMBGkGsU3OBmVTvMeU4rQBc090DLQOZ2GVaW91luyL1Lhv50jDA%2Bu6Ak8PdHYjf5%2FE9y1zRn3yJqW6xFmGOvvCgC3q0AE%2FpcuO0UdTxooSSS3WreW3%2FvSQkyYOAZK%2F4ByJlOAakQwj4wYVAxLU5XrS6q4E2h3k%2FXZ65kt4Bin%2FpIX7%2BCtMXiCfoHrRhTpjUXn7M5njUjl7rL4tLaVY9YVu9%2Bl%2F%3C%2Fdiagram%3E%3Cdiagram%20name%3D%22Smart%20Template%22%20id%3D%22Te9pV2B9E-FbejOiF9xA%22%3EzVrLdps6FP0aD5MFiOfQSdM0gz5z70o6VEA2NICoELHdr68EEgZEsugKr5HNQQ%2B09z5H0pE24Do53hKYhZ9xgOKNoQXHDfiwMQzdNDX2wy2nyuI4wrAnUSAKnQ330R8kjLJYEQUobxWkGMc0ytpGH6cp8mnLBgnBh3axHY7bvWZwjxTDvQ9j1foQBTQUVt32zi8%2BoWgfiq5dw6leJFAWFiPJQxjgQ8MEbjbgmmBMq3%2FJ8RrFHDyJS1Xv4ytv6w8jKKVDKnih%2B%2FRVg48H7%2BoXuv0Gtid8dwFEMy8wLsSI7ykkrMEts35BKCgB50SgFBFIEceV8xnBPYHJBnwUo6MnCdkhjCi6z6DPnw9MFhtwlVOCn2sE2divRL%2BIUHR8dUR6jRMTGMIJouTEiogKNhDQCm1JpA9nogxb2MIGR44r9CG0sa9bPsPH%2FggE%2FwVNQ0HzLmCDiXb8q2nIwcsKkuEcKaiRECdPRd6LVR%2BiY%2BBnt%2FHTTVcFUOsBsDaOjyBQEcx5JVo6LxHq83GSxWzcpd%2F7KKN9OlwAUdM1W4iafZK0jB5EpXF8RM1%2BRCs1SviYQ0MKLwISvaB0JWACYLXAdExLBdP0esCUxvHBtBQwP8O0gLziBxERDe2aIEgjnC4XGT2r69mG14Ndj2tb5lTQ2Qp0W4IqIZa%2FGUEB2kVpNeUg5uBstslXokXdttuAarajAionlpYYp5ttHAXR%2F%2FnEom3v6mBZSfGFW29ilLDR5gvO12ZXlXoPiPPO2K6qSo6eD9OyuzzKafl97POYtcgpTqI%2FC3u3sT4Yvbek2F0%2F7gjmYTL32bMfLocjAKsDUnpIA8ibNKhW4xLRCwll0FiHr8eprb5pel4Q1U1NYxkOY4pIKqNijuOCe%2FOCYVE31hcXTXUnowDkF%2BQF8Ub0Ehm2a9zyDTczpDhlZa5QGkjLU4z9Z246RvSRPWuXlnj6KRpgYJFT4xV%2F5O809kBwkQZlV1oNOQqUjXsHcE5uQXz0VtySKQVI9oi%2BVdDop5CguFJSs9s%2BNsqqDA14ahTIcCQn5CZZdfvv4E%2FdR%2F1EqsbfRWGDQO3Ssxbj0BjKIZiWQ9HyN25oxEe97dxAbBHPhFctjku%2Fuukbnf5LzVyFC4Oh9JtL0G92ciyO5s1Av7pN%2FYJHZV9vOb%2FtvsX%2BpaavQwDWEgLQNWcJBai77QkCgLGKAGAO5d9egn%2BgtbNYuiYWHdPyr%2BYGJo0Ajr1kBBisAGcJBTidADCTAtTMxgQRwB4aAaaWgD1UAu4ik0A3HwvcOSSgZmVGDgJs3T94EbgaBXhrWAfOowBLTSeNzH9rG19RfFZAm3%2B2UJuSf3cg%2F6a2BP9KBLDax%2FUT8a9mwpbjX7cn5d9bNf%2BK%2F8%2FD%2F7xpvC7%2FM88AzkoUMHYyz1KTeTOyqHe82JqUQ2slHA7czM%2Fkxmo6b9p8zqJuPDSfa75yrDKxBICzQELXUjN6y4WAaRdy8vRurSGgy%2F%2FoIWB%2F1H7%2F%2BJF9T%2F%2BD7q%2FiFjw84tuLvoWcHTN4rp7Ynz3%2Fc76A1DwgFlcX8oTf6mxerGEd8jsOAYGHywjL1tjH1Q1KWxC9dE1PpGthFXvK9VWVhu8F4pBs3%2Bp6cKt5Vt7YOLuD%2FbvgN2urC0EXeXWOy4%2FRM4KqeqJAo6WNwVaRrc6rZusCospDiEroMKrvJibwuTxORml5Sl9eeShevwLRvELb%2FJLeQXf8nKIjt4c0iYVvwjjap%2Bx%2FjHb8DT%2BNjnwYb4U5iYKAV%2B69HNX24x1OqbiErZt15%2B863u5ufOR5WONs23R7zra9f79jyh7P96krzzvfSgc3fwE%3D%3C%2Fdiagram%3E%3C%2Fmxfile%3E)

First, let's see how smart templates work in draw.io.

**Generate a diagram with a smart template**

1. Select _Arrange > Insert > Generate_ to go directly to the smart templates section in the draw.io template library. 
  * Alternatively, start a new diagram and select the _Smart Templates_ section.
  * If you are using draw.io with the Simple, Minimal or Sketch editor themes, select ``+`` in the toolbar then _Generate_
2. Select your _Diagram type_ from the list. 
3. Write a simple and accurate text description of your diagram, then click _Generate_
4. Click on the diagram preview to expand it. 
   * If you like what you see, click _Insert_. 
   * If not, click _Generate_ again to generate a different diagram for the same query, or edit your query and regenerate the preview. 
<br /><img src="/assets/img/blog/generated-diagrams-flowchart.gif" style="width=100%;max-width:600px;height:auto;" alt="Generate a diagram with Smart Templates in draw.io">

Now, you can edit, add to and style your generated diagram freely using the draw.io shape libraries and format panel. 

Learn more about [smart templates in draw.io](/blog/smart-diagram-generation.html) and [how to write a good query](/blog/write-query-generate-diagram.html). 

## When should you draw your diagram manually?

It's probably easier to explain when _not_ to generate a diagram.

**Draw a diagram following a standard manually**

Diagram generators output mostly simple shapes - rectangles, lifelines, circles, connectors and so on. If you need [BPMN](/blog/bpmn-2-0.html) process flows, [C4 models](/blog/c4-modelling.html), [AWS](/blog/aws-diagrams.html) or [GCP](/blog/gcp-aws-shapes-network-diagrams.html) network diagrams, and so on, enable the appropriate shape libraries in draw.io, and draw your diagram manually so it follows that technical standard. 

**Note:** UML sequence and state diagrams may be an exception here - there are enough examples in most generator's training set that they can produce reasonable _generic_ diagrams.
<br /><img src="/assets/img/blog/diagram-generator-sequence.png" style="width=100%;max-width:300px;height:auto;" alt="Generate a UML sequence diagram from a text description via the template library in draw.io"> <img src="/assets/img/blog/diagram-generator-state.png" style="width=100%;max-width:300px;height:auto;" alt="Generate a state diagram from a text description via the template library in draw.io">

**Document existing systems or processes manually** 

The smart templates feature in draw.io can only work from your short text description - it does not know any information about your existing infrastructure or processes. Therefore, it can't draw accurate technical diagrams to document existing code, systems, workflows or networks, or interfaces to other systems and external processes. 

**Draw unsupported diagram types manually**

There are many types of technical and business oriented diagrams that are not supported by generators - fishbone cause/effect diagrams, rack diagrams, interface mockups, Kanban boards, infographics and other marketing diagrams (5C, SWOT, PEST), timelines and roadmaps, and many more [technical diagram use cases](/blog/use-cases.html) that you can use draw.io for.

**Tip:** Most of the diagram types supported by Mermaid syntax are supported by diagram generators. If you have a preferred diagram generator outside of draw.io, ask it to export Mermaid code - you can then [insert the Mermaid code into draw.io](/blog/mermaid-diagrams.html) and then edit and style your generated diagram afterwards. 


## When should you generate a diagram?

Generated diagrams can be useful to brainstorm _generic components_ of a system, or outline a _common workflow_, or draw a _mindmap of a concept_, perhaps to plan for an event or structure a document or presentation. 

For example, you could ask it to generate a flowchart of a "``browser-based file storage system using a serverless AWS pattern``". 
<br /><img src="/assets/img/blog/generated-diagrams-generic-example.png" style="width=100%;max-width:400px;height:auto;" alt="Generate a state diagram from a text description via the template library in draw.io">

It won't be correct, or have precise details of the system, but it gives you a general starting point that you can then use to draw your actual system. 

## Limitations of generated diagrams

Keep in mind that diagram generators do not sanity check anything in your diagram - there may be completely illogical elements. For example, when asked to generate a flowchart or decision tree for the query "``When does it make sense to use AI to generate a diagram``", there are a few problematic sections. 
  * Immediately after the decision to use _Manual Diagram Creation_, it instructs you to _Use AI-generated diagram_. 
  * The _Start_ task or decision in the flow is also unclear - _Need to generate a diagram?_.
  <br /><img src="/assets/img/blog/generated-diagrams-flowchart.png" style="width=100%;max-width:400px;height:auto;" alt="There are some logical problems with this generated flowchart">

The biggest limitation for technical diagrams for documentation purposes is that diagram generators do not know about your existing system and processes, and therefore any diagram you try to generate will not be accurate.

Generators also won't use your corporate style, specific layouts preferred by your team, or a diagramming standard that needs specific shapes, labels and connectors. 

Most generators, including the draw.io smart templates feature, don't have any memory of previous attempts, so they can't refine an already generated diagram. Regenerating starts over from scratch every time.

Generating multiple iterations and hoping for a usable diagram that you can then clean up may be slower than manually drawing your diagram from scratch. 

## Related

New to diagramming or to draw.io? The [getting started guide](/doc/) and [simple flowchart tutorial](/doc/getting-started-basic-flow-chart.html) will get you up and running. 

For example diagrams, check the [diagram gallery](/example-diagrams.html), the [use cases](/blog/use-cases.html) on this blog, or the [template library](/doc/faq/insert-template.html) in draw.io. There are many more templates and examples in the [jgraph/drawio-diagrams repository on GitHub](https://github.com/jgraph/drawio-diagrams).
