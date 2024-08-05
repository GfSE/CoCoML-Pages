---
title: "UML Class Diagram"
layout: default
parent: "From UML/SysML"
nav_order: 01
---

# UML Class Diagram

{: .highlight }
_Note: This is the very beginning of the discussion and in no way settled or complete._

## Selecting native UML Metaclasses

The following entities are selected for transformation:

| UML | SpecIF <dcterms:type> | OWL/RDF |
| ---: | :--- | :--- |
| uml:Class | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-DC9wVTLyGWOOBEpHdGRXwrkGNWt" target="_blank">SpecIF:ModelElement</a> <uml:Class> |  |
| uml:Property | coming soon |  |
| uml:Operation | coming soon |  |

... and the following relations:

| UML | direction | SpecIF | OWL/RDF |
| ---: | :---: | :--- | :--- |
| uml:Generalization | inverted | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-8pUc6Vjp86KYxpBFwvbnduOoHKp" target="_blank">SpecIF:isSpecializationOf</a> |  |
| uml:Composition | same | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-5AP5qdMeBeBnURVia2BWtTlTL3r" target="_blank">dcterms:hasPart</a> |  |
| uml:Aggregation | same | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-hmCfLTnuYbWWsE4qqo8zb8CwaE2" target="_blank">dcterms:hasPart</a> |  |
| uml:Association | same | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-H8KY2yoKNmBqEgSojfGX9oBclMN" target="_blank">SpecIF:isAssociatedWith</a> |  |


### Details

A directed association in UML means that only one side knows (can navigate to) the other. In SpecIF like RDF every association is a statement with subject, predicate and object. When translating a UML/SysML class diagram to SpecIF and further on to OWL/RDF:
- In case of a composition and aggregation, the class with the rhombus is the subject and any arrow is ignored: It doesn't matter whether there is or isn't an arrowhead on either side. 
- In case of an association, the arrow is interpreted as the direction according to RDF. Thus, the arrow póints from subject to object. UML associations with zero or two arrow-heads will get an 'undirected' flag in SpecIF.


### Example

The following UML Class Diagram uses UML native metaclasses only:

![UML Class Diagram](../assets/images/UML-SysML/UML_Class_Diagram_(native).png)
_Figure: UML Class Diagram using native metaclasses_

#### Transform first to SpecIF

The UML Class Diagram is first transformed to SpecIF. The relations of the element _General_Class_ are shown next. The names at the edges are the vocabulary terms _SpecIF:shows_, _dcterms:hasPart_, _SpecIF:isAssociatedWith_ and _SpecIF:isSpecializationOf_ translated according to the browser language; English in this case.

![SpecIF Relations of element General_Class on UML Class Diagram](../assets/images/UML-SysML/SpecIF-Relations_of_UML_Class_Diagram_(native).png)
_Figure: SpecIF Relations of element General_Class on UML Class Diagram_

The files can be examined:
- The <a href="CoCoML-UML-Class Diagram](https://github.com/GfSE/CoCoML-Verification-and-Validation/blob/main/1_Source/CoCoML-UML-Class-Diagram.mdzip" target="_blank">Cameo model file</a>,
- the example <a href="https://specif.de/apps/edit#import=../examples/CoCoML-Class-Diagram.specif.zip;view=doc;project=eee_1045467100313_135436_1;node=N-8264661645" target="_blank">UML Class Diagram</a> transformed to SpecIF,
- the <a href="https://specif.de/apps/edit#import=../examples/CoCoML-Class-Diagram.specif.zip;view=statements;project=eee_1045467100313_135436_1;node=N-12061513685" target="_blank">relations of 'General_Class'</a>, 
- the corresponding <a href="https://github.com/GfSE/CoCoML-Verification-and-Validation/blob/main/3_SpecIF/CoCoML-Class-Diagram.specif.zip" target="_blank">SpecIF file</a> ... in case you want to take a closer look: Isn't it much cleaner than an XMI file?
- ... and the generated <a href="https://github.com/GfSE/CoCoML-Verification-and-Validation/blob/main/9_DOCX/CoCoML-Class-Diagram.docx" target="_blank">WORD(R) file</a>.
- Finally, here is the <a href="https://specif.de/apps-beta/edit.html" target="_blank">SpecIF Model-Integrator and Editor</a> to use it with your own Cameo *.mdzip files. _(Please note that only the UML class diagram, SysML Block Definition Diagram and SysML Internal Block Diagram are translated as of now.)_

#### Transform further to OWL/RDF

... _coming soon using OMG's MOF2RDF_


### Discussion

<a href="https://github.com/GfSE/CoCoML/discussions/5" target="_blank">Any questions or ideas?</a>


## Adding meaning using Terms of a Controlled Vocabulary

... _coming soon_

## Adding meaning using Other Terms

... _coming soon_

