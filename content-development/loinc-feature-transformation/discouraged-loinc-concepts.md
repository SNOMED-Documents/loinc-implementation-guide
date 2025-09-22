# Discouraged LOINC Concepts

In the LOINC distribution csv file, the column "status" can indicate a number of concept states:

* ACTIVE
* TRIAL
* DISCOURAGED
* DEPRECATED

&#x20;For example, [https://loinc.org/6487-3](https://loinc.org/6487-3) has a status of 'DISCOURAGED'.

The equivalent property in SNOMED CT concepts, is the "active" flag, but this can only take a 1 or 0 value, which maps to the ACTIVE and DEPRECATED LOINC statuses respectively.

TRAIL concepts are considered available for use, and so this status is not expressed in the SNOMED CT transformation of LOINC concepts.

DISCOURAGED, however, is represented using an Annotation (starting from Release 2.0 Effective Time 20250921).   These are expressed in the ComponentAnnotation file eg der2\_scsRefset\_ComponentAnnotationStringValueSnapshot\_LO1010000\_20250921.txt with the column for _referencedComponentId_ set to the SCTID of the relevant concept, and the annotation text "Discouraged" in the _value_ column.
