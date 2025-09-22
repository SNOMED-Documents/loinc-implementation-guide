# LOINC Feature Transformation

LOINC Concepts feature a number of logical properties - beyond their text descriptions and parts - that required some creative way to surface in a SNOMED CT format.

Two examples of these are the ORD/OBS flag (which indicates if a LOINC Term should be used in the context of an Order, and Observation, or Both), and a status of "Discouraged" which indicates that a LOINC Term is still active, but its use should be avoided. &#x20;

Both of these flags exist as columns in the published LOINC distribution csv file and the method for exposing them in a SNOMED CT format is described in the following pages.  &#x20;
