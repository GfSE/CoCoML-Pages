---
title: Introduction
layout: default
has_children: true
nav_order: 0
---

<!-- templates <a href="" target="_blank"></a> <img class="my-align-right size-60" src="./assets/images/Home/" alt="" /> -->

# CoCoML - The Purpose

A concise and consistent language for modeling (mechatronic) systems and software: 
- Communicate the structure and behavior between the participants in its lifecycle;
- Create a common context for artifacts created and consumed by participating (engineering) disciplines and organizations.

UML/SysML offers a plethora of possibilities, is considered semantically vague and thus cannot be mapped genuinely to any other technical realm. 
CoCoML shall define a practical and formally well defined subset of UML/SysML for bidirectional and lossless mapping with OWL/RDF and perhaps other formats (to be discussed). 
Other notations and languages such as FMC, BPMN and ArchiMate shall be considered in future.

CoCoML is one aspect of <a href="https://github.com/GfSE/CASCaDE-Layered-Ontology" target="_blank">CASCaDE</a>, 
an initiative to facilitate collaboration in the product lifecycle from conception to retirement - similarly to 
<a href="https://en.wikipedia.org/wiki/Building_information_modeling" target="_blank">Building Information Modeling (BIM)</a> in the construction industry. 
Goal is to submit a standard candidate at OMG - addressed at a Request for Proposals yet to be prepared and issued. 
While CASCaDE aims at the whole product lifecycle, CoCoML addresses the early phases of systems engineering and in particular UML/SysML.

<!--<details markdown="block">
<summary>... read more</summary>

This is content inside a `<details>` dropdown.

</details>-->

# CoCoML - The Way Forward

## Limit the Scope

UML has been devised to specify software products. It is also used to generate software and thus offers many language features towards that end.
SysML v1 is a UML Profile and as such shares many characteristics.
However, much less detail is needed to communicate the overarching concept of a system. 
So, the first step is to select the UML and SysML elements to use for that purpose. 

Three categories are proposed:
1. Well defined element to transform, e.g. _uml:Class_, _uml:Generalization_ or _uml:Composition_.
2. Weakly defined element to transform, where *the name* from a controlled vocabulary defines the meaning. 
For example, an association with type _uml:Association_ and a name _sysml:satisfies_ 
is understood as a relationship between a function or component and a requirement with a well defined meaning.
(Better than specifying meaning of a relation with a _name_ is to assign a _stereotype_ such as «sysml:Allocate». 
But how to define such stereotypes for CoCoML?)
3. Element not to transform. If used, a warning shall be issued. 

<a href="https://github.com/GfSE/CoCoML-Pages/discussions/7" target="_blank">Any questions or ideas?</a>

## Use an Intermediate Format

The transformation shall be done in two steps using an intermediate, neutral format. 
The model in the neutral format shall be 'formal' such that it can be expressed with a Domain-Specific language (DSL), for example.
First, it is intended to transform UML/SysML models, but later other MOF-based modeling notations like BPMN
and potentially others may follow.
Second, there is interesting innovation in the context of knowledge-graphs and related data formats. It will be easier 
to generate such data from an intermediate format.
Finally, it is a fairly common and well proven approach to separate transformation in pre- and post-processing.

<img src="./assets/images/CoCoML-Development.svg" alt="Transform UML/SysML to OWL/RDF" />

It is proposed to use the Specification Integration Facility ([SpecIF](https://specif.de)) as intermediate format.
It is a generic and simple information model to build a Knowledge Graph (aka Property Graph) with typed nodes, edges and properties.
[Schema and constraints](https://github.com/GfSE/SpecIF-Schema) are available to assure syntactical data quality. 
However, so far there is no checking at the semantic level.

While there have been numerous publications on UML to OWL/RDF transformation (see <a href="./literature" target="_blank">literature</a>), 
there has been little practical application to our knowledge. The mappings described in 
<a href="https://www.omg.org/spec/MOF2RDF/" target="_blank">OMG: MOF to RDF Mapping (MOF2RDF)</a> and
<a href="https://henrietteharmse.com/wp-content/uploads/2017/11/uml-class-diagram-to-owl-and-sroiq-reference.pdf" target="_blank">Harmse: UML Class Diagram to OWL and SROIQ Reference</a>
are most promising. 

Another approach is to use a subset of SysML v2 to define the CoCoML. 
To date there is no mapping of SysML v2 to OWL/RDF according to authoritative members of the submission group.
This track will be investigated, first.

There is a number of details to decide, for example which flavor of OWL to use (where anything beyond DL is considered impractical).

<a href="https://github.com/GfSE/CoCoML-Pages/discussions/4" target="_blank">Any questions or ideas?</a>

## Use a Controlled Vocabulary

Among the concepts offered by UML/SysML we will select those deemed relevant for overarching system modeling.
Different modeling languages use their own terminology - but share many concepts. 
The final goal is to put system information from difference sources into a common context.  
A common terminology is essential in all those cases.

An example: A _bpmn:Lane_ and a _uml:Actor_ both represent a role with responsibility for certain activities.
The resulting ontology (resp. knowledge graph) shall represent both in the same way. 
And if used with the same name, they can be considered the same and combined.

<a href="https://github.com/GfSE/CoCoML-Pages/discussions/6" target="_blank">Any questions or ideas?</a>

## Use FMC for Abstraction

Prof. Dr.-Ing. Siegfried Wendt, founding director of the Hasso-Plattner-Institute in Potsdam, and his collaborators have shown 
that it possible to successfully describe system structure and behavior using three fundamental model elements, namely _Actor_, _State_ and _Event_. 
The concept is extremely promising for integrating models of different notations and tools: Numerous practical examples in more than a decade have shown the power of the approach. 
Therefore we propose the <a href="http://fmc-modeling.org/" target="_blank">Fundamental Modeling Concepts (FMC)</a> 
as an abstraction layer for (preferably automatic) system model integration.

<!--<details markdown="block">
<summary>... read more</summary>

This is content inside a `<details>` dropdown.

</details>-->

<a href="https://github.com/GfSE/CoCoML-Pages/discussions/3" target="_blank">Any questions or ideas?</a>


## Joint Effort

Worldwide, there are many similar initiatives going on at moment. We do not want to re-invent the wheel: Do you know any other promising approach?

Let us join forces:
- <a href="https://github.com/GfSE/CoCoML/discussions" target="_blank">Discussions</a>
- <a href="https://github.com/GfSE/CoCoML/issues" target="_blank">Issues</a>

We will establish a 3-head technical committee to summarize the discussions and to take wise decisions.
The decision guideline will be consistency first, conciseness second. So-called "design by committee" incorporating any and every proposal shall be avoided.

Just now, in September 2024, we are at the very beginning. But we are sure that with your help and a joint effort we will succeed.

## Contact
- Dr.-Ing. Oskar von Dungern via <a href="https://github.com/odungern" target="_blank">GitHub</a>, <a href="https://www.linkedin.com/in/odungern/" target="_blank">linkedIn</a> or [e-mail](mailto:oskar.dungern@gfse.org).

