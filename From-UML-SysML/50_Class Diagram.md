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
| uml:Generalization | inverted | SpecIF:specializes |
| uml:Composition | same | dcterms:hasPart |
| uml:Aggregation | same | SpecIF:aggregates |
| uml:Association | same | SpecIF:associates |

## Details

A directed association in UML means that only one side knows (can navigate to) the other. In SpecIF every association is a statement with subject, predicate and object, hence directed like RDF statements. When translating a UML/SysML class diagram to SpecIF and further on to OWL/RDF:
- In case of a composition and aggregation, the class with the rhombus is the subject and the arrow is ignored. 
- In case of a general association, the arrow is interpreted as the direction according to RDF. Thus, the arrow póints from subject to object. Associations with zero or two arrow-heads will get an arbitrary direction.

## Example

![UML Class Diagram](./assets/UML-SysML/Class_Diagram.png)
