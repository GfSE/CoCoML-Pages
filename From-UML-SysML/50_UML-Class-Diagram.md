---
title: "UML Class Diagram"
layout: default
parent: "From UML/SysML"
nav_order: 01
---

# UML Class Diagram

As a very first step, the following entities are defined:

| UML | SpecIF <dcterms:type> | OWL/RDF |
| ---: | :--- | :--- |
| uml:class | [SpecIF:ModelElement](https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-DC9wVTLyGWOOBEpHdGRXwrkGNWt) <uml:class> |  |

... and the following relations:

| UML | direction | SpecIF | OWL/RDF |
| ---: | :---: | :--- | :--- |
| uml:Generalization | inverted | [SpecIF:isSpecializationOf](https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-8pUc6Vjp86KYxpBFwvbnduOoHKp) |  |
| uml:Composition | same | [dcterms:hasPart](https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-5AP5qdMeBeBnURVia2BWtTlTL3r) |  |
| uml:Aggregation | same | [SpecIF:aggregates](https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-hmCfLTnuYbWWsE4qqo8zb8CwaE2) |  |
| uml:Association | same | [SpecIF:isAssociatedWith](https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-H8KY2yoKNmBqEgSojfGX9oBclMN) |  |

Next steps:
- Attributes
- Methods (Operations)

## Details

A directed association in UML means that only one side knows (can navigate to) the other. In SpecIF like RDF every association is a statement with subject, predicate and object. When translating a UML/SysML class diagram to SpecIF and further on to OWL/RDF:
- In case of a composition and aggregation, the class with the rhombus is the subject and the arrow is ignored. 
- In case of a general association, the arrow is interpreted as the direction according to RDF. Thus, the arrow póints from subject to object. UML associations with zero or two arrow-heads will get an arbitrary direction.

## Example

![UML Class Diagram](../assets/images/UML-SysML/Class_Diagram.png)
_Figure: UML Class Diagram_

The UML model transformed to SpecIF:
- [UML Class Diagram](https://specif.de/apps/edit#import=../examples/CoCoML.specif.zip;view=doc;project=eee_1045467100313_135436_1;node=N-8264661645).
- The [relations of 'General_Class'](https://specif.de/apps/edit#import=../examples/CoCoML.specif.zip;view=statements;project=eee_1045467100313_135436_1;node=N-12061513685). 
- Download the [SpecIF file](https://specif.de/examples/CoCoML.specif.zip) ... in case you want to take a closer look.
