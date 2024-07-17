---
title: "UML Class Diagram"
layout: default
parent: "From UML/SysML"
nav_order: 01
---

# UML Class Diagram

As a very step, the following entities are defined:

| UML | SpecIF [dcterms:type] |
| ---: | :--- |
| uml:class | SpecIF:ModelElement [uml:class] |

... and the following relations:

| UML | direction | SpecIF |
| ---: | :---: | :--- |
| uml:Generalization | inverted | SpecIF:Specialization |
| uml:Composition | same | dcterms:hasPart |
| uml:Aggregation | same | uml:Aggregation |
| uml:Association | same | uml:Association |
