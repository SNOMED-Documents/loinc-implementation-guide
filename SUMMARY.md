# Table of contents

* [Implementation Guide for the LOINC Ontology](README.md)

## Introduction

* [Executive Summary](introduction/executive-summary.md)
* [1. Introduction](introduction/1.-introduction.md)

## What is LOINC?

* [2. What is LOINC?](what-is-loinc/2.-what-is-loinc.md)
* [2.1 LOINC Features](what-is-loinc/2.1-loinc-features.md)
* [2.2 LOINC Extension to SNOMED CT](what-is-loinc/2.2-loinc-extension-to-snomed-ct.md)

## Clinical Use Case

* [3. Clinical Use Case](clinical-use-case/3.-clinical-use-case.md)
* [3.1 Clinical Workflow](clinical-use-case/3.1-clinical-workflow.md)
* [3.2 Use Case Scenarios](clinical-use-case/3.2-use-case-scenarios.md)

## Content Development Principles

* [4. Content Development Principles](content-development-principles/4.-content-development-principles.md)
* [4.1 Alternate Identifiers - Identifying LOINC Terms in SNOMED CT](content-development-principles/4.1-alternate-identifiers-identifying-loinc-terms-in-snomed-ct.md)
* [4.2 Template Based Content Creation](content-development-principles/4.2-template-based-content-creation/README.md)
  * [4.2.1 Quality Observable with Component](content-development-principles/4.2-template-based-content-creation/4.2.1-quality-observable-with-component.md)
  * [4.2.2 Quality Observable with Inheres in (System, no Component)](content-development-principles/4.2-template-based-content-creation/4.2.2-quality-observable-with-inheres-in-system-no-component.md)
  * [4.2.3 Quality Observable with Inheres In](content-development-principles/4.2-template-based-content-creation/4.2.3-quality-observable-with-inheres-in.md)
  * [4.2.4 Quality Observable with Process](content-development-principles/4.2-template-based-content-creation/4.2.4-quality-observable-with-process.md)
  * [4.2.5 Quality Observable with Ratio](content-development-principles/4.2-template-based-content-creation/4.2.5-quality-observable-with-ratio.md)
  * [4.2.6 Quality Observable with Relative to](content-development-principles/4.2-template-based-content-creation/4.2.6-quality-observable-with-relative-to.md)
  * [4.2.7 Quality Observable with Susceptibility](content-development-principles/4.2-template-based-content-creation/4.2.7-quality-observable-with-susceptibility/README.md)
    * [4.2 Template Based Content Creation](content-development-principles/4.2-template-based-content-creation/4.2.7-quality-observable-with-susceptibility/4.2-template-based-content-creation.md)
  * [4.2.8 Quality Observable with Process (No Process output, With Time aspect)](content-development-principles/4.2-template-based-content-creation/4.2.8-quality-observable-with-process-no-process-output-with-time-aspect.md)
* [4.3 Orderable and Observable LOINC Terms](content-development-principles/4.3-orderable-and-observable-loinc-terms.md)

## Information Models and Terminology Binding

* [5. Information Models and Terminology Binding](information-models-and-terminology-binding/5.-information-models-and-terminology-binding.md)
* [5.1 Logical Model](information-models-and-terminology-binding/5.1-logical-model.md)
* [5.2 Terminology Bindings](information-models-and-terminology-binding/5.2-terminology-bindings.md)
* [5.3 HL7 FHIR and Laboratory Data](information-models-and-terminology-binding/5.3-hl7-fhir-and-laboratory-data/README.md)
  * [5.3.1 FHIR Resources for Ordering Laboratory Tests](information-models-and-terminology-binding/5.3-hl7-fhir-and-laboratory-data/5.3.1-fhir-resources-for-ordering-laboratory-tests.md)
  * [5.3.2 FHIR Resources for Representing Laboratory Results](information-models-and-terminology-binding/5.3-hl7-fhir-and-laboratory-data/5.3.2-fhir-resources-for-representing-laboratory-results.md)

## Technical Application

* [6. Technical Application](technical-application/6.-technical-application.md)
* [6.1. Implementation Approaches and Considerations](technical-application/6.1.-implementation-approaches-and-considerations.md)
* [6.2 Accessing the LOINC Ontology](technical-application/6.2-accessing-the-loinc-ontology.md)
* [6.3 Deploying the LOINC Ontology](technical-application/6.3-deploying-the-loinc-ontology.md)
* [6.4 Using the LOINC Ontology](technical-application/6.4-using-the-loinc-ontology/README.md)
  * [6.4.1 Querying the LOINC Ontology](technical-application/6.4-using-the-loinc-ontology/6.4.1-querying-the-loinc-ontology.md)
  * [6.4.2 Accessing the LOINC Ontology from a FHIR Terminology Server](technical-application/6.4-using-the-loinc-ontology/6.4.2-accessing-the-loinc-ontology-from-a-fhir-terminology-server.md)
  * [6.4.3 Accessing the Reference Set in a Relational Database](technical-application/6.4-using-the-loinc-ontology/6.4.3-accessing-the-reference-set-in-a-relational-database.md)
