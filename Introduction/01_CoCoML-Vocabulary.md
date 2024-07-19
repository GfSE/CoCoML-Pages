---
title: "CoCoML Vocabulary"
layout: default
parent: Introduction
nav_order: 01
---

# CoCoML - Controlled Vocabulary

Among the concepts offered by UML/SysML we will select those deemed relevant for overarching system modeling.
Different modeling languages use their own terminology - but share many concepts. 
The final goal is to put system information from difference sources into a common context.  
A common terminology is essential in all those cases.

Of course, established terms shall be re-used whenever possible, for example from the <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/" target="_blank">Dublin Core Metadata Initiative (DCMI)</a> or <a href="https://schema.org/" target="_blank">Schema.org</a>.

<a href="https://github.com/GfSE/CoCoML/discussions/6" target="_blank">Any questions or ideas?</a>

| Concept | Term Name | Type of Term | Description |
| :--- | :--- | :--- | :--- |
| Title | <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/terms/title/" target="_blank">dcterms:title</a> | Property | A name given to the resource. |
| Description | <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/elements11/description/" target="_blank">dcterms:description</a> | Property | Description may include but is not limited to: an abstract, a table of contents, a graphical representation, or a free-text account of the resource. |
| Type | <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/elements11/type/" target="_blank">dcterms:type</a> | Property | Recommended practice is to use a controlled vocabulary such as the DCMI Type Vocabulary [DCMI-TYPE]. |
| Composition | <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/terms/hasPart/" target="_blank">dcterms:hasPart</a> | Property | This property is intended to be used with non-literal values. This property is an inverse property of Is Part Of. |
