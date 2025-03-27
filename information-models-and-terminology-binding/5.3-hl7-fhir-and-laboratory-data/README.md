# 5.3 HL7 FHIR and Laboratory Data

## What is FHIR? <a href="#id-5.3hl7fhirandlaboratorydata-whatisfhir" id="id-5.3hl7fhirandlaboratorydata-whatisfhir"></a>

HL7 FHIR is a modern standard designed to facilitate the exchange of healthcare information electronically.

* **Consistency**: With standardized resources and robust semantics, FHIR ensures uniformity in healthcare data representation. This consistency supports accurate data exchange and enables healthcare providers to make informed decisions based on reliable information, ultimately enhancing patient care quality.
* **Modularity**: FHIR’s flexible architecture allows its resources to be used independently or in combination to meet specific healthcare needs. This modular approach supports adaptability across diverse healthcare contexts, enabling tailored solutions without overhauling entire systems.
* **Interoperability**: FHIR facilitates seamless data exchange between different healthcare systems and applications, enhancing communication and collaboration among healthcare providers. By standardizing data formats and protocols such as RESTful APIs and JSON/XML, FHIR promotes interoperability, improving patient care coordination and information sharing.
* **Standardization**: FHIR leverages contemporary web standards to ensure compatibility with existing IT infrastructures. By defining well-structured resources like Patient, Observation, and Medication with clear semantics, FHIR fosters consistency in how healthcare data is represented and interpreted across various systems.
* **Scalability**: Designed to accommodate evolving healthcare requirements and technological advancements, FHIR is scalable for both current and future healthcare needs. Its flexible architecture and support for extensibility allow healthcare systems to grow and adapt without compromising interoperability or data integrity.

HL7 FHIR plays a crucial role in linking healthcare data with standard terminologies, including SNOMED CT. By integrating FHIR with terminologies like SNOMED CT, more precise and standardized documentation and communication of clinical information can be achieved. This linkage enhances interoperability by enabling seamless exchange of structured clinical data, supporting accurate clinical decision-making, and promoting continuity of care for patients across various healthcare settings.

## FHIR Resources <a href="#id-5.3hl7fhirandlaboratorydata-fhirresources" id="id-5.3hl7fhirandlaboratorydata-fhirresources"></a>

For the purpose of representing the laboratory data workflow, we can use the following FHIR resources:

* **ServiceRequest**: Represents laboratory orders or requests for specific diagnostic tests or procedures.
* **DiagnosticReport**: Captures the overall results or findings of the laboratory tests as a summarized report.
* **Observation**: Provides detailed data points or specific results associated with the laboratory tests.

Examples:

* 5.3.1 FHIR Resources for Ordering Laboratory Tests
* 5.3.2 FHIR Resources for Representing Laboratory Results

## Map between the Generalized Logical Model FHIR Resources <a href="#id-5.3hl7fhirandlaboratorydata-mapbetweenthegeneralizedlogicalmodelfhirresources" id="id-5.3hl7fhirandlaboratorydata-mapbetweenthegeneralizedlogicalmodelfhirresources"></a>

The image below illustrates how FHIR resources can be used to represent the generalized logical model for laboratory data. It outlines the relationships between key FHIR resources (highlighted in red) and logical model entities (depicted in gray), offering a structured approach to representing laboratory orders, individual results, and specimen information.

* **Laboratory Order**: Mapped to the **FHIR ServiceRequest** resource, representing the clinical request for laboratory testing. It includes details such as test code, priority, status, and the specimen to be tested.
* **Result**: Mapped to the **FHIR DiagnosticReport** resource, summarizing the findings of the laboratory tests based on the order. The DiagnosticReport serves as a container for individual results.
* **Individual Results**: Represented by the **FHIR Observation** resource, where each Observation provides specific result details such as:
  * Result values
  * Units of measurement
  * Clinical interpretation (e.g., normal, abnormal)
  * Reference ranges
  * Link to the associated specimen
* **Specimen**: Mapped to the **FHIR Specimen** resource, which defines the type and method of specimen collection. This resource connects all entities within the generalized logical model.

| <table data-header-hidden><thead><tr><th></th></tr></thead><tbody><tr><td></td></tr></tbody></table> |
| ---------------------------------------------------------------------------------------------------- |
|                                                                                                      |

**Relationships**

* The **FHIR ServiceRequest** initiates the laboratory process and forms the basis for the **FHIR DiagnosticReport**.
* The **FHIR DiagnosticReport** includes one or more **FHIR Observations**, each representing an individual result.
* The **FHIR Specimen** resource is central to the model, linking the order, results, and observations to the biological material tested.

\
