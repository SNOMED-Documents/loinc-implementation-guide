# Table of contents

* [Implementation Guide for the LOINC Ontology](README.md)

## Introduction

* [Executive Summary](introduction/executive-summary.md)
* [Introduction](introduction/1.-introduction.md)

## About LOINC

* [What is LOINC?](what-is-loinc/2.-what-is-loinc.md)
* [LOINC Features](what-is-loinc/2.1-loinc-features.md)
* [LOINC Extension to SNOMED CT](what-is-loinc/2.2-loinc-extension-to-snomed-ct.md)

## Use Case

* [Clinical Use Case](use-case/3.-clinical-use-case.md)
* [Clinical Workflow](use-case/3.1-clinical-workflow.md)
* [Use Case Scenarios](use-case/3.2-use-case-scenarios.md)

## Content Development

* [Content Development Principles](content-development/4.-content-development-principles.md)
* [Alternate Identifiers - Identifying LOINC concepts in SNOMED CT](content-development/4.1-alternate-identifiers-identifying-loinc-terms-in-snomed-ct.md)
* [Template Based Content Creation](content-development/4.2-template-based-content-creation/README.md)
  * [Quality Observable with Component](content-development/4.2-template-based-content-creation/4.2.1-quality-observable-with-component.md)
  * [Quality Observable with Inheres in (System, no Component)](content-development/4.2-template-based-content-creation/4.2.2-quality-observable-with-inheres-in-system-no-component.md)
  * [Quality Observable with Inheres In](content-development/4.2-template-based-content-creation/4.2.3-quality-observable-with-inheres-in.md)
  * [Quality Observable with Process](content-development/4.2-template-based-content-creation/4.2.4-quality-observable-with-process.md)
  * [Quality Observable with Ratio](content-development/4.2-template-based-content-creation/4.2.5-quality-observable-with-ratio.md)
  * [Quality Observable with Relative to](content-development/4.2-template-based-content-creation/4.2.6-quality-observable-with-relative-to.md)
  * [Quality observable with Component for LOINC Grouper](content-development/4.2-template-based-content-creation/quality-observable-with-component-for-loinc-grouper.md)
  * [Quality Observable with Susceptibility](content-development/4.2-template-based-content-creation/4.2.7-quality-observable-with-susceptibility.md)
  * [Quality Observable with Process (No Process output, With Time aspect)](content-development/4.2-template-based-content-creation/4.2.8-quality-observable-with-process-no-process-output-with-time-aspect.md)
* [LOINC Feature Transformation](content-development/loinc-feature-transformation/README.md)
  * [Orderable and Observable LOINC Concepts](content-development/loinc-feature-transformation/4.3-orderable-and-observable-loinc-terms.md)
  * [Discouraged LOINC Concepts](content-development/loinc-feature-transformation/discouraged-loinc-concepts.md)

## Information Models and Terminology Binding

* [Information Models and Terminology Binding](information-models-and-terminology-binding/5.-information-models-and-terminology-binding.md)
* [Logical Model](information-models-and-terminology-binding/5.1-logical-model.md)
* [Terminology Bindings](information-models-and-terminology-binding/5.2-terminology-bindings.md)
* [HL7 FHIR and Laboratory Data](information-models-and-terminology-binding/5.3-hl7-fhir-and-laboratory-data/README.md)
  * [FHIR Resources for Ordering Laboratory Tests](information-models-and-terminology-binding/5.3-hl7-fhir-and-laboratory-data/5.3.1-fhir-resources-for-ordering-laboratory-tests.md)
  * [FHIR Resources for Representing Laboratory Results](information-models-and-terminology-binding/5.3-hl7-fhir-and-laboratory-data/5.3.2-fhir-resources-for-representing-laboratory-results.md)

## Technical Application

* [Technical Application](technical-application/6.-technical-application.md)
* [Implementation Approaches and Considerations](technical-application/6.1.-implementation-approaches-and-considerations.md)
* [Accessing the LOINC Ontology](technical-application/6.2-accessing-the-loinc-ontology.md)
* [Deploying the LOINC Ontology](technical-application/6.3-deploying-the-loinc-ontology.md)
* [Using the LOINC Ontology](technical-application/6.4-using-the-loinc-ontology/README.md)
  * [Querying the LOINC Ontology](technical-application/6.4-using-the-loinc-ontology/6.4.1-querying-the-loinc-ontology.md)
  * [Accessing the LOINC Ontology from a FHIR Terminology Server](technical-application/6.4-using-the-loinc-ontology/6.4.2-accessing-the-loinc-ontology-from-a-fhir-terminology-server.md)
  * [Accessing the Reference Set in a Relational Database](technical-application/6.4-using-the-loinc-ontology/6.4.3-accessing-the-reference-set-in-a-relational-database.md)
