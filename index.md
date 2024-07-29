---
title: Introduction
layout: default
has_children: true
nav_order: 0
---

<!-- templates <a href="" target="_blank"></a> <img class="my-align-right size-60" src="./assets/images/Home/" alt="" /> -->

# CoCoML - The Purpose

A concise and consistent language for modeling (mechatronic) systems and software. 

UML/SysML offers a plethora of possibilities and cannot be mapped genuinely to any other technical realm. 
CoCoML shall define a practical and formally well defined subset of UML/SysML for bidirectional and lossless mapping with OWL/RDF and perhaps other formats (to be discussed). 
Other notations and languages such as FMC, BPMN and ArchiMate shall be added in future.

<!--<details markdown="block">
<summary>... read more</summary>

This is content inside a `<details>` dropdown.

</details>-->

# CoCoML - The Way Forward

## Using an Intermediate Format

The transformation shall be done in two steps using an intermediate, neutral format. 
First, it is intended to not only transform UML/SysML models, but also other MOF-based modeling notations like BPMN
and potentially others.
Second, there is interesting innovation in the context of knowledge-graphs and related data formats. It will be easier 
to generate such data from an intermediate format.
Finally, it is a fairly common and well proven approach to separate transformation in pre- and post-processing.

<img class="my-align-right size-60" src="./assets/images/CoCoML-Development.svg" alt="" />

It is proposed to use the Specification Integration Facility ([SpecIF](https://specif.de)) as intermediate format.
It is a generic and simple information model to build a Knowledge Graph (aka Property Graph) with typed nodes, edges and properties.
[Schema and constraints](https://github.com/GfSE/SpecIF-Schema) are available to assure data quality.

<a href="https://github.com/GfSE/CoCoML/discussions/4" target="_blank">Any questions or ideas?</a>

## Using a Controlled Vocabulary

Among the concepts offered by UML/SysML we will select those deemed relevant for overarching system modeling.
Different modeling languages use their own terminology - but share many concepts. 
The final goal is to put system information from difference sources into a common context.  
A common terminology is essential in all those cases.

<a href="https://github.com/GfSE/CoCoML/discussions/6" target="_blank">Any questions or ideas?</a>

## Using FMC for Abstraction

Prof. Dr.-Ing. Siegfried Wendt, founding director of the Hasso-Plattner-Institute in Potsdam, and his collaborators have shown 
that it possible to successfully describe system structure and behavior using three fundamental model elements, namely _Actor_, _State_ and _Event_. 
The concept is extremely promising for integrating models of different notations and tools: Numerous practical examples in more than a decade have shown the power of the approach. 
Therefore we propose the <a href="http://fmc-modeling.org/" target="_blank">Fundamental Modeling Concepts (FMC)</a> as an abstracting layer for system model integration.

<!--<details markdown="block">
<summary>... read more</summary>

This is content inside a `<details>` dropdown.

</details>-->

<a href="https://github.com/GfSE/CoCoML/discussions/3" target="_blank">Any questions or ideas?</a>


## Joint Effort

Worldwide, there are many similar initiatives going on at moment. We do not want to re-invent the wheel: Do you know any other promising approach?

Let us join forces:
- <a href="https://github.com/GfSE/CoCoML/discussions" target="_blank">Discussions</a>
- <a href="https://github.com/GfSE/CoCoML/issues" target="_blank">Issues</a>

Just now, in July 2024, we are at the very beginning. But we are sure that with your help and a joint effort we will succeed.

## Contact
- Dr.-Ing. Oskar von Dungern via <a href="https://github.com/odungern" target="_blank">GitHub</a>, <a href="https://www.linkedin.com/in/odungern/" target="_blank">linkedIn</a> or [e-mail](mailto:oskar.dungern@gfse.org).

