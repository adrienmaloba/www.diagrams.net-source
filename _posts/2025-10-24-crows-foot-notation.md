---
layout: post
author: draw.io
slug: crows-foot-notation
date: 2025-10-24 09:54:00
title: Crow's foot notation for ER diagrams
tags: [features,connectors]
categories: [features,use-cases,connectors]
---

Crow's foot notation is used in [entity relationship (ER) diagrams]() to show how data in different database tables relate to each other. 
<br /><img src="/assets/img/blog/er-example-library.png" style="width=100%;max-width:500px;height:auto;" alt="An ER model using crow's foot notation for a library">

Using Crow's feet on ER connectors instead of the Chen notation eliminates the need to label each connector end with numbers, and can make a diagram much easier to read. 

## Draw ERDs using crow's feet notation

**Enable the entity relation shape library**

Click _More Shapes_ at the bottom of the left panel. In the _Software_ section, select the _Entity Relation_ shape library, then click _Apply_.

This library includes pre-styled connectors with the various types of crow's feet used for relational databases. Hover over each shape to see a description of the relationship.
<br /><img src="/assets/img/blog/entity-relation-shape-library-hover.png" style="width=100%;max-width:250px;height:auto;" alt="Hover over connector shapes in the Entity Relation library to see them more clearly">

**Change connector ends in the Style tab of the format panel**

1. Drag a connector between two entities. You can either connect the two tables, or connect individual rows within the table.
2. Select the connector, and choose a new connector end from the source and target lists. 
<br /><img src="/assets/img/blog/er-connector-ends-change.png" style="width=100%;max-width:400px;height:auto;" alt="Change the connector ends to use crow's foot notation in the Style tab of the format panel">
<br />**Tip:** The crow's foot connector ends are at the bottom of the list. 

### Connector ends for crow's foot notation

The connector ends indicate the _cardinality_ of the relationship between two entities - how many of one entity relate to how many of a second entity. You can show the minimum and maximum of any relationship by combining two symbols at the connector end.
<br /><img src="/assets/img/blog/er-connector-ends-single.png" style="width=100%;max-width:400px;height:auto;" alt="Change the connector ends to use crow's foot notation in the Style tab of the format panel">

* **circle** = zero
* **line** = one
* **crow's foot** = many or infinite

<img src="/assets/img/blog/er-connector-ends-combination.png" style="width=100%;max-width:400px;height:auto;" alt="Change the connector ends to use crow's foot notation in the Style tab of the format panel">
<br />By combining these, you can indicate: 
* **circle + line** = zero to a maximum of one
* **line + line** = one and only one (mandatory)
* **circle + crow's foot** = zero to many
* **line + crow's foot** = a minimum of one to many

**Limitations:** As you can see in the library example below, this notation does not indicate where there are limits other than one or zero. You can't specify that each library has a minimum of five staff, or each member can borrow up to 20 books. You may find the [Chen or ISO min/max notations](https://en.wikipedia.org/wiki/Entity–relationship_model#) more useful in this case.

[<img src="/assets/img/blog/er-example-library.png" style="width=100%;max-width:600px;height:auto;" alt="An ER model using crow's foot notation for a library">](https://viewer.diagrams.net/?lightbox=1&highlight=0000ff&edit=_blank&nav=1&dark=1#R%3Cmxfile%3E%3Cdiagram%20name%3D%22Page-1%22%20id%3D%22lvN3VKu7OU2csA47GwTQ%22%3E7Z1dc6M2FIZ%2FTWbai3b4Nr5cO0mbNtnuJNtp91IG2WaLkQfLmzi%2FvhJINrbAFv4AHGkmMzFCxsB5jx4dHQlu7OHs7bcUzKdPKITxjWWEbzf27Y1lWYbrk3%2B0ZJWXmKbj5CWTNApZ2abgJXqHrNBgpcsohIutihihGEfz7cIAJQkM8FYZSFP0ul1tjOLtX52DCRQKXgIQi6X%2FRCGe8svw%2Bpsdv8NoMmU%2F7Vu9fMcM8MrsShZTEKLXQpF9d2MPU4Rw%2Fmn2NoQxvXv8vuTfu6%2FYuz6xFCZY5gt%2Ff%2F7jtyB4CPy7738Mnr2H95f74BfTzQ%2FzA8RLdsUDhP4jJT89wTACP7Nzxyt%2BQ8hlzOlHDEa0aLDAIMXMbrZBCoglMIgSmJICM9uOYzBfRFn1vGQaxeEjWKEl5gfiW4Nx9AbD59xstC6x4CM5GN2kBx%2BTg7%2Bwk6G7QRxNEvI5IDeB%2FuIghQtyLo9ggVmNKZ7F7OM4iuMhilGaXYkdutAPnewSUvQfLOzxrZHteWQPuzkwxfCt8raba2MSN4BoBnG6IlXYFzyD2Z95gNVjynktyMlndaYFJVk9VgiYhCfrY2%2BsTD4wQ9cxuicYfb%2BZn6luB1OURu%2FUuDEzRtH02fZrNItBQvwBhDtFA5S1AMaOFRKUQEEitFKYovlXkE4gZgVzFCU4uxHugPyRWzM0fnVvXHKuQ7JtbrbJH62e4iFKiGWJFOkxIFHEK6SqGGA0ZweN4ZgfP2U3nn4eIYzRjIlGSgJ7fEsUBhOCbcjpwL6YDHqCDL78WSkEcrk4AvEzaWRBMolzs2VtLtiYrcS2pXd7fYd3b%2F2ufyNy48dx1mxOozCExNcHr9MIw5c5CGilV8KdbS8%2FwWBeucEKFrJrGogdbHPXah8NxKRhSwAmLrRMwoVg9fV5niAEvxQCD7efl7MRaVXblQRv4vO6gwUxfJRMHvNvejuacbuimbdqJ3fPqiGpwzUhor6GihRUjEtCxWsbKry3KyODZtoP0o3lx2ueKH01icJvUEEFXyNMT7bbKOmEOJRDB28iNDraREe%2FdXTYGh27TqEgOhxBBZ%2BWmPi6ZoeEOtRjhziAqdnRODtMq3V41BjTVAAeFeb68PAoGdJcjuJoMe3%2BMFYnBKIeP8SxT82P5vnhts6PGsOXCvDDV5Mf%2FCcLKvgGgUaHjDaUQ0dPjFQ1OppHh982Ono1QtCPj47cK9RDR08MQO9ROgNYw0NCHerBQ4xUNTwah8d6mml78KgRfyoAj56i8BCjzyH5wQliCtP42K8P5fBhupbmRwf44bTND9PVWXPRL9QjiOmKoxEPL4PPGh8y6lCPHzzvUVAGDCeQz6MmTe8UTVAC4rtN6SCl5wM5FzZ1HlEmCmqc7xDjFeMJWGK0bbp8pQ1fSGVx%2FnyiC7VIwd3zDCThX5nOsh33UcxBBZNwU%2B0dpugregLJKt9TqJdfFr2WSm2wogVapgHcc5NsvuCMQ6wuJVIYAxz92D6TsyPAFidbvkxhPN7fH9hh%2F3Ut3Rr7AQyCtaAKe0a%2B67jSzN%2B%2FdMvm0SFfsWNLLt1ae%2Fn5ba27fXLdvtNAYVcIoytLt2yx06f20i1b0W6fLfb6srZfr9w6WjLK9QVtPYWyiaGEA0xpfeWWrWdQCk6hIFDEvNQjCkgUg5Ku06QT%2BlCPHnoCZQfo0friLVvMYKlMD0XnT%2FJ0iJjHjOBC80NCIcrxw3R1%2BNEBgLS%2Fgst0dQAi%2BoV6DDFdMQShjyPS%2FJCSh3IAcUoi1miUgj1Tp3QCTDIBxqHAp7tIMuJy%2BS9HR5tN5L%2Bcinl2Xcl%2FOWK0qXb%2By1E04HTFgJM1%2FtcyatlqDqxKNsp1Isw641dKg%2BW0KPQAWFpPgpklI1gttyCtBqG2og8wNJ2SSXUYjKsn1XUEJ92Qh3L8cEW5aHw0jo%2FWs2B1VuV8fHq4FaMLHx0eJUty6KS8HzoFJiUP5eBh1pl6pelxKXp0IAVWMvtKYX4wv1APIGbJpKonSGd0a4JICUQ5hJTkTA88Nfn6c2DNvL%2FL5yNCdd%2Ff1b9YkKFzYE3kwNyO58BcnQMr8wv1egt80Fxo%2Bx9uu95baDX5VaUX5ToPnh68bCL8PACU1nNfnh68FJxCQZqIg5d69qWsONRDxzEvXNCh53GhpyMbc1ws9PR06NlE6Ol1PPT0dOhZ5hfqdRZ6Yui5bv519HmUZJTrQvR09NlE9HmAKa1Hnz0dfQpOoSBQdPR5vDiUQ4cvdj%2F2T9K9%2FshzPIZe%2BcK%2FsNcfGdKM2C%2BhncBT9u1s6xk0Z6eDrzsJTQSeuVG7G3j6YidB7cDTV7Sf4JdMsaUtvw46j5KLej0H%2Fe6%2BJoLOAzxpPej09av7BKdQECbi9PudReQ6%2FpTRiXIUMQ0xANUYaRwjrS%2F7M40a4enH5whzC%2FVAYhpifDqkfh7gW4hBFGuOSOlEOZD0RY7k63320%2BTKRzLHVsVIpjfy3DPNodldvWFIsuJyjzDr66HMJoYy%2Bx0fyuzrocwyv1Cv09AXhzLztl%2BPZR6lF%2FU6D3oss4kg9ABQWh%2FL7OuxTMEpFKSJOJY5QPS9qTDUE2lkRaIeQmo8d0Qj5FIIaX0cs19jeYcCCKmYMfvhESKu7tCDmLVVohxDTEMMZDVEGodIB55iZtQISD8%2BRphfqMcR0xAj0vssmaD5ISEPBQFSOQ9nCAge0ISU7gXKzTXnw0IA%2FXFpPswLfDgay6ps%2F7CoxxNgdV%2Fp418OFzr4bCIhxtyruxkx0xDDT7VTYsw1VOw6lMSgOQN0Vuw4yajXnTD15Mwm4tFDXGk9MWaaenam6BcKQsW0BB3onJi0PBQEiH4tQxcA0npazDT1axlEv1ARIGKAmj9pWSNESiAKIkTnxLqAkA4kxUydFBMdQ0WGiEmx9SMTNUakNKIgRvTbqTuBEdkHYV0OIxxkGiMFx1AQI5Y4pjkkvzghHq8nWMhpRD2MWD1BGTCcQJ6sIi3wFE1QAuK7TekgpecDOR42dR5RJgpqnO8Q4xXDClhitG06%2BBbhfwufv9FD%2Feqyrds33o7QDY4cYtJ09e%2BmIt38Vty3%2BVq2xb%2BXAe4TXe9ACu6eZyAJ%2F8oUnO24j%2BJ4%2FbVwU42I%2FCt6Askq31Gols%2FF%2BIfZ0loLkd62ShmyogVapgHcYw%2F%2B0nDMsVlV0a6Y05HCGODox%2FaZXIA5%2FTZks2PKoo26aEzO4YPGrHrtVEPG5O1O99uAHQG8wxTJKWDj9U3a35W0f9WD35uyv3ml9pdsy7dk0qD919MNDgogHwE4QQDZV8kVg1WhAgu3Nkf%2BQgs23Rx%2FZ%2BIfWy56L1md91eq6nv9vfXJh%2FyEz9uhcdw2xWyc2ph1Wc78nfQH5Vy1Dr%2Bh9szxrlQCqNT4olElOzdntX1f0vZVz5NtyPZuqyyrY3vpHqok8i7r%2B05P0v5Ou30Zt5XA5LR4diua3QS3FfFsQTdsKGZbMCFYTLNrMdnGF4DpOEJWYhmWIBX7Rlh4MPYDWP4grpHvOu6ZGxfHl%2B0mVc1kbUhc3tUESscOltQSV%2F03IF64uy3bP6l67W5TMrqaeEtNGdmyYfupMjoqaiON4HZcZbr74zbhC3Z%2Ff%2BDWt%2FfWv1Dgxt813X2vEOX3fTmb8xMFaXCZ4O6MGufPBztM3Irs52Ul7u4I0OrtV%2FhufdtyThEs2UwRwsXqKZhPn1AIaY3%2FAQ%3D%3D%3C%2Fdiagram%3E%3C%2Fmxfile%3E)

### Beware chasm and fan traps

A **chasm trap** occurs when a model suggests a relationship (see the dotted red line in the diagram), but the link between the two entities is not explicitly defined. 

For example, a _Library_ has many _Shelves_ and _Books_ are placed on those shelves. You should be able to query how many books are in the library - but if you queried via the books on the shelves, that would not include books that are temporarily not on shelves but still listed in the catalogue (books that are borrowed, or in the back room awaiting repair).

A **fan trap** is when a query could be answered via more than one pathway in your model, but may return different values. 

For example, the _Shelves_ database contains a list of all the _Books_ on _Shelves_ in the _Library_, and the _Catalogue_ database contains a list of all the _Books_ the _Library_ owns (whether they are on the shelf or not). When you query how many books are in the library, it could return different numbers depending on whether it queried via the _Catalogue_ or the _Shelves_.

**Best practices**

* In your diagram, make sure all query pathways are clearly defined with relationship connectors. 
* Where a query may return a different value because there are multiple query pathways, it may make sense to make turn that function into a separate entity.
* Try to remove any redundant relationships to simplify query pathways. In the example, this would be the Catalogue database to the Author and Publisher entities, indicated with dashed green lines.

## Related

Use keyboard shortcuts to [work with entity relationship table shapes](/blog/entity-relationship-tables.html) faster. Select a row and press ``Ctrl+Enter`` to clone it, or ``Backspace`` to delete it. 

You can also drag and drop a table into another to combine two tables.

Document your existing databases quickly in draw.io by [inserting SQL code](/blog/insert-sql.html) to add entities or table shapes, to the drawing canvas. Then, draw connectors between the entities and select the crow's foot connector ends from the Style tab. 
<br /><img src="/assets/img/blog/insert-sql-dialog.png" style="width=100%;max-height:180px;width:auto;" alt="Insert SQL code then click Insert to create an ER diagram automatically"> &nbsp; <img src="/assets/img/blog/inserted-sql-example-erd.png" style="width=100%;max-height:120px;width:auto;" alt="Entity shapes are automatically created based on your SQL code">

**Crow's feet notation vs UML class diagrams** 

Crow's feet notation is similar to, but not the same as [UML notation in class diagrams](/blog/uml-class-diagrams.html). 

* In ER diagrams, crow's feet indicate cardinality - how many of each entity relate to how many of a second entity. 

* In UML class diagrams, connector end shapes indicate dependency, aggregation and composition of the classes, and numbered labels denote multiplicity (the allowed cardinality of a relationship between classes).
<br /><img src="/assets/img/blog/uml-class-shape-visibility-example.png" style="width=100%;max-width:300px;height:auto;" alt="Numbers at either end of the connectors in UML class diagrams indicate multiplicity">