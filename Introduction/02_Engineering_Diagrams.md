---
title: "Engineering Diagrams"
layout: default
parent: Introduction
nav_order: 02
---

# Engineering Diagrams

What is the difference between a diagram of an electronic circuit and, let's say, a SysML Block Definition Diagram (BDD)?

<img class="size-40 my-align-right" src="../assets/images/Schaltplan.gif" alt="Elektronik Schaltplan" />
<!-- <img class="size-40 my-align-right" src="../assets/images/uml-sysml-ibd-02.png" alt="SysML IBD" /> -->

Very simply put, the electronic diagram specifies a circuit sufficiently well, so that any person educated in the domain can audit or build it without further explanation. 
In contrast, UML, SysML v1 and many other notations are considered semi-formal<sup>[1]</sup>. There is semantic ambiguity in many cases. 
Consequently, such a diagram must be accompanied with additional information to get the idea across.

The goal of CoCoML is to define a formally sound language to describe the concept of mechatronic devices and software. 
UML and SysML elements shall be used as graphic notation. So any CoCoML diagram shall conform with UML, but obviously not vice-versa.

fUML<sup>[2]</sup> defines a subset of UML to allow model execution. It will be examined whether approach and results are viable for the goals of CoCoML. 

<!--
<a href="https://github.com/GfSE/CoCoML-Pages/discussions/4" target="_blank">Any questions or ideas?</a>
-->

## Literature

1. <a href="https://ris.utwente.nl/ws/portalfiles/portal/6140830/Kent_Evans_Rumpe_1999.pdf" target="_blank">UML Semantics FAQ</a>
1. <a href="http://www.omg.org/spec/FUML/" target="_blank">Semantics of a Foundational Subset for Executable UML Models (FUML™)</a>



