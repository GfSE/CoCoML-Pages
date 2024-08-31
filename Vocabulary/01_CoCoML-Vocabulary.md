---
title: "CoCoML Vocabulary"
layout: default
nav_order: 03
---

# CoCoML - Controlled Vocabulary

{: .highlight }
_Note: This vocabulary is the very beginning and will be complemented step by step following the discussion in the interested community._

Among the concepts offered by UML/SysML those deemed relevant for overarching system modeling will be selected.
Different modeling languages use their own terminology - but share many concepts. 
The final goal is to put system information from difference sources into a common context.  
A common terminology is essential in all those cases.

Of course, established terms shall be re-used whenever possible, for example from the <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/" target="_blank">Dublin Core Metadata Initiative (DCMI)</a> or <a href="https://schema.org/" target="_blank">Schema.org</a>.

<a href="https://github.com/GfSE/CoCoML-Pages/discussions/6" target="_blank">Any questions or ideas?</a>

| Concept | Term Name | Type of Term | Description |
| :--- | :--- | :--- | :--- |
| Model Diagram | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-CVAvZ6kJv8gOO8VxKdOz985VoPw" target="_blank">uml:Diagram</a> | Entity |  |
| Model Diagram | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-rtsxeVw90JsJmIPM9LSO7Z9cE1D" target="_blank">SpecIF:View</a> | Entity |  |
| Class | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-kb7b8eclxar8zXHrOhn3fc4L5Yt" target="_blank">uml:Class</a> | Entity |  |
| Model Element | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-DC9wVTLyGWOOBEpHdGRXwrkGNWt" target="_blank">SpecIF:ModelElement</a> | Entity |  |
| Requirement | RFLP:Requirement | Entity |  |
| Function | RFLP:Function | Entity |  |
| Logical (Element) | RFLP:Logical | Entity |  |
| Physical (Element) | RFLP:Physical | Entity |  |
| Requirement | IREB:Requirement | Entity |  |
| Active Entity | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-4NoXVcSzSs07Htg4959SJnDEm0D" target="_blank">FMC:Actor</a> | Entity | An 'Actor' is a fundamental model element type representing an active entity, be it an activity, a process step, a function, a system component or a role.<br/> The particular use of FMC:Actor is specified with a dcterms:type property. A value of that property should be a vocabulary-term itself. |
| Passive Entity | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-yeUw4dc3iTxk7PHLdQo7efxLvBc" target="_blank">FMC:State</a> | Entity | A 'State' is a fundamental model element type representing a passive entity, be it a value, a condition, an information storage or even a physical shape.<br/> The particular use of FMC:State is specified with a dcterms:type property. A value of that property should be a vocabulary-term itself. |
| Event | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-8HwdIxFap0pTQ5JiE31I1BQJ15z" target="_blank">FMC:Event</a> | Entity | An 'Event' is a fundamental model element type representing a time reference, a change in condition/value or more generally a synchronization primitive.<br/> The particular use of FMC:Event is specified with a dcterms:type property. A value of that property should be a vocabulary-term itself. |
| Composition | <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/terms/hasPart/" target="_blank">dcterms:hasPart</a> | Relation | This property is intended to be used with non-literal values. This property is an inverse property of Is Part Of. |
| Title | <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/terms/title/" target="_blank">dcterms:title</a> | Property | A name given to the resource. |
| Description | <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/elements11/description/" target="_blank">dcterms:description</a> | Property | Description may include but is not limited to: an abstract, a table of contents, a graphical representation, or a free-text account of the resource. |
| Type | <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/elements11/type/" target="_blank">dcterms:type</a> | Property | Recommended practice is to use a controlled vocabulary such as the DCMI Type Vocabulary [DCMI-TYPE]. |
| Occurence | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-KySdnxpGEFIs3FWCaOlzbpLVEq4" target="_blank">SpecIF:shows</a> | Relation |  |
| Satisfaction | <a href="https://specif.de/apps/edit#import=../v1.1/Ontology.specif;view=doc;project=P-SpecIF-Ontology;node=N-YShAhKHuxcyBV85xnVLD1iXE53o" target="_blank">oslc_rm:satisfy</a> | Relation |  |
