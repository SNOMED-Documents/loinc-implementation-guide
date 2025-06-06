---
cover: .gitbook/assets/LOINC_SNOMED_web.jpg
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: false
  outline:
    visible: false
  pagination:
    visible: true
---

# Implementation Guide for the LOINC Ontology

***

<details>

<summary>Summary</summary>

The SNOMED CT Implementation Guide for the LOINC Ontology provides essential guidance for implementing and utilizing the LOINC Ontology, an extension to SNOMED CT that enables LOINC users to leverage SNOMED CT’s structured design while also allowing SNOMED CT users to utilize LOINC. Developed through a collaboration between SNOMED International and the Regenstrief Institute, this guide supports terminology implementers, system developers, and clinical informaticians in adopting the LOINC Ontology for interoperable, standardized, and computable healthcare data.

The LOINC Ontology was established to bridge the gap between structured clinical terminologies and laboratory/observation data, ensuring that LOINC-coded tests and observations can be used within SNOMED CT’s concept model. By aligning these terminologies, the extension enhances data interoperability, standardization, and semantic precision. This guide explains the structure and content of the LOINC Extension, offering practical guidance on its implementation, data integration, and clinical applications.

The guide provides an overview of LOINC’s structure, purpose, and integration into SNOMED CT, detailing how LOINC-coded observations are structured using hierarchical relationships, attributes, and classification models. It introduces the LOINC Extension, explaining how it enhances LOINC’s computability within SNOMED CT. Clinical use cases demonstrate how the LOINC Ontology supports standardized laboratory results, decision support, and structured clinical documentation. Examples include ordering and reporting laboratory tests, interoperability between laboratory and clinical data systems, and integration with decision support systems to improve diagnostics and treatment pathways.

A key section covers how LOINC terms are represented within SNOMED CT, using its concept model, attributes, and relationships. It outlines strategies for incorporating LOINC attributes, the templated approach for structuring LOINC concepts, and the management of orderable and observable LOINC terms within SNOMED CT. To ensure compatibility across electronic health records (EHRs), laboratory systems, and clinical applications, the guide discusses logical modeling, terminology binding best practices, and HL7 FHIR-based approaches for laboratory data representation, including FHIR resources for test ordering, result structuring, and interoperability frameworks.

From a technical perspective, the guide provides practical steps for deploying the LOINC Ontology within SNOMED CT-enabled systems. It explains methods for accessing the LOINC Ontology, such as through a FHIR Terminology Server or relational databases, and best practices for querying, retrieving, and maintaining LOINC data. It also addresses managing references to inactive concepts, version control considerations, and impact assessment to ensure alignment with SNOMED CT updates and national extensions.

By implementing the LOINC Ontology within SNOMED CT, organizations can achieve greater interoperability, enhance the accuracy of laboratory result standardization, improve data consistency and analytics, and support terminology-driven decision support for a more structured and precise representation of clinical data. This guide serves as a comprehensive resource for ensuring the effective implementation, maintenance, and utilization of the LOINC Ontology within SNOMED CT, supporting a more standardized and interoperable healthcare ecosystem.

</details>

***

## Contents

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>Introduction</td><td><a href="introduction/1.-introduction.md">1.-introduction.md</a></td></tr><tr><td>What is LOINC?</td><td><a href="what-is-loinc/2.-what-is-loinc.md">2.-what-is-loinc.md</a></td></tr><tr><td>Clinical Use Case</td><td><a href="clinical-use-case/3.-clinical-use-case.md">3.-clinical-use-case.md</a></td></tr><tr><td>Content Development Principles</td><td><a href="content-development-principles/4.-content-development-principles.md">4.-content-development-principles.md</a></td></tr><tr><td>Information Models &#x26; Terminology Binding</td><td><a href="information-models-and-terminology-binding/5.-information-models-and-terminology-binding.md">5.-information-models-and-terminology-binding.md</a></td></tr><tr><td>Technical Application</td><td><a href="technical-application/6.-technical-application.md">6.-technical-application.md</a></td></tr></tbody></table>

***

{% include "https://app.gitbook.com/s/KbECNHVpqdRmTn8m03ns/~/reusable/fPpkHYQG98V7O7BwsCeR/" %}
