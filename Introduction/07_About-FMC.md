---
title: "About FMC"
layout: default
parent: Introduction
nav_order: 07
---

# About FMC

The Fundamental Modeling Concepts (FMC) are a modeling technique created especially to support the communication about information processing systems. 
FMC uses a simple notation which can be used easily for ad-hoc creation of models in meetings. 
FMC is not tied to any programming paradigm and can even be used for information processing systems which are implemented with a hardware / software mix.[^2]

FMC has been created and refined by <a href="https://www.linkedin.com/in/siegfried-wendt-2331445a/" target="_blank">Siegfried Wendt</a> and his group in many industrial projects. 
FMC is based on established concepts such as Petri nets and Entity/Relationship modeling, and has been consequently tailored to support communication.[^2]

Later on, <a href="https://www.linkedin.com/in/odungern/" target="_blank">Oskar von Dungern</a> and his colleagues have applied FMC 
also to mechatronic systems including production sites and logistic chains.

FMC has been developed over years and consequently there are several explanations from different perspectives. 
Most useful for integrating system information is the FMC abstraction to 3 fundamental model element classes, namely _FMC:Actor_, _FMC:State_ and _FMC:Event_.[^3]

_Please note that SpecIF entity names used in early publications have changed since to better conform with the <a href="https://www.dublincore.org/" target="_blank">DCMI</a> concepts, but the structure of the metamodel is unchanged._

<a href="https://github.com/GfSE/CoCoML/discussions/3" target="_blank">Any questions or ideas?</a>

## Meta-model

The 'official' metamodel is published here:[^1][^2]

<img src="../assets/images/FMC/FMC-Metamodel.gif" alt="FMC Metamodel" />.

The fundamental model-element classes are not shown. The shown entities are classified as follows:

| Fundamental class | Metamodel entity |
| ---: | :--- |
| FMC:Actor | FMC:Agent, FMC:Operation |
| FMC:State | FMC:Location, FMC:Channel, FMC:Storage |
| FMC:Event | FMC:Event, FMC:Point_in_Time |

## Literature

[^1]: Home: <a href="http://fmc-modeling.org/" target="_blank">Fundamental Modeling Concepts</a>
[^2]: Knöpfel, A.; Gröne, B.; Tabeling, P.: <a href="https://www.wiley.com/en-ie/Fundamental+Modeling+Concepts%3A+Effective+Communication+of+IT+Systems-p-9780470027103" target="_blank">Fundamental Modeling Concepts: Effective Communication of IT Systems</a>, Wiley 2006.
[^3]: Dungern, Oskar v.: <a href="https://www.researchgate.net/publication/310360106_Semantic_Model_Integration_for_System_Specification_Creating_a_Common_Context_for_Different_Model_Types" target="_blank">Semantic Model Integration for System Specification: Creating a Common Context for Different Model Types</a>, GfSE Tag des Systems Engineering 2016, Herzogenaurach, DOI: <a href="https://www.hanser-elibrary.com/doi/10.3139/9783446451414.038" target="_blank">10.3139/9783446451414.038</a>


