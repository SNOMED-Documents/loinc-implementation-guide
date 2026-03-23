# Template Based Content Creation

LOINC Terms are expressed as SNOMED CT concepts by following a [transformation algorithm detailed in pseudocode](https://docs.google.com/document/d/1rz2s3ga2dpdwI1WVfcQMuRXWi5RgpJOIdicgOz16Yzg). This has been implemented as a number of Java classes, freely available in [this package in the SNOMED International GitHub Reporting Engine project](https://github.com/IHTSDO/reporting-engine/tree/7.9.2/script-engine/src/main/java/org/ihtsdo/termserver/scripting/pipeline/loinc).

## Overview <a href="#id-4.2templatebasedcontentcreation-overview" id="id-4.2templatebasedcontentcreation-overview"></a>

The processing algorithm follows these high level steps

1. The Java class loads the Loinc.csv and Part.csv file from the LOINC release
2. A part detail file is also supplied, which specifies part identifiers ("LP") for each part used in each LOINC Term
3. The process works through the part detail file, selecting a template based on the 'Property' part of each LOINC Term
4. Each part is mapped to a SNOMED CT Attribute where:
   1. The Part Type maps to a SNOMED Attribute type as specified in the template and
   2. The Part Number maps to a SNOMED Attribute value as specified via the Part/Attribute Map (maintained in the Snap2Snomed tool)
5. The terms for each concept are then completed, using the preferred terms of the attribute values that have been modelled.
6. The entire set of modelled concepts is the compared against the LOINC Extension in the SI Authoring Platform
7. A delta archive is produced which details changes required from the previous state of the content.

In addition, LOINC Panels are created as primitive concepts, where the individual tests in each panel are available as transformed SNOMED CT concepts.

See [LOINC Presentation](https://docs.google.com/presentation/d/1NvcH06JWgC2ss_A_TQDz9SzQzVR2RNWgBGjG5uARGpw/edit#slide=id.g2871ae07855_0_0)

<a href="https://docs.google.com/forms/d/e/1FAIpQLScTmbZIf0UEQwYDkY27EEWBkaiYkHSbR0_9DmFrMLXoQLyL7Q/viewform?usp=pp_url&#x26;entry.1767247133=LOINC+Implementation+Guide&#x26;entry.670899847=Template%20Based%20Content%20Creation" class="button primary">Provide Feedback</a>
