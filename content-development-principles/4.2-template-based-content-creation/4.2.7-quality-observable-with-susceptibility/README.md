# 4.2.7 Quality Observable with Susceptibility

## Quality Observable with Susceptibility <a href="#id-4.2.7qualityobservablewithsusceptibility-qualityobservablewithsusceptibility" id="id-4.2.7qualityobservablewithsusceptibility-qualityobservablewithsusceptibility"></a>

This template is utilized for LOINC terms representing susceptibility observations, such as microbial susceptibility tests.

This template is documented in Confluence here:  [Susceptibility observable for LOINC (observable entity) - v1.0](https://confluence.ihtsdotools.org/display/SCTEMPLATES/Susceptibility+observable+for+LOINC+\(observable+entity\)+-+v1.0)

The java implementation of this template can be found: [https://github.com/IHTSDO/reporting-engine/blob/develop/script-engine/src/main/java/org/ihtsdo/termserver/scripting/pipeline/loinc/LoincTemplatedConceptWithSusceptibility.java](https://github.com/IHTSDO/reporting-engine/blob/develop/script-engine/src/main/java/org/ihtsdo/termserver/scripting/pipeline/loinc/LoincTemplatedConceptWithSusceptibility.java)

### Attributes <a href="#id-4.2.7qualityobservablewithsusceptibility-attributes" id="id-4.2.7qualityobservablewithsusceptibility-attributes"></a>

* **LOINC Property**: Represents the property of the observation, such as mass concentration or presence.
* **LOINC Scale**: Describes the scale type, like quantitative or qualitative.
* **LOINC Time**: Indicates the time aspect of the observation, e.g., single point in time.
* **LOINC System**: Specifies the direct site of the observation.
* **LOINC Method**: Describes the technique used for the observation.
* **LOINC Component**: Specifies the target organism or substance towards which the susceptibility is observed

LOINC Properties currently supported:  "Susc"

### Template <a href="#id-4.2.7qualityobservablewithsusceptibility-template" id="id-4.2.7qualityobservablewithsusceptibility-template"></a>

#### Model <a href="#id-4.2.7qualityobservablewithsusceptibility-model" id="id-4.2.7qualityobservablewithsusceptibility-model"></a>

```
<<< 363787002 |Observable entity (observable entity)| : 
	{
		370130000 |Property (attribute)| -> 118588007 |Susceptibility (property) (qualifier value)|, 
 		370132008 |Scale type (attribute)| -> 117365007 |Ordinal OR quantitative value (qualifier value)|, 
 		370134009 |Time aspect (attribute)| -> 123029007 |Single point in time (qualifier value)|, 
 		704319004 |Inheres in (attribute)| -> 410607006 |Organism (organism)|, 
 		704320005 |Towards (attribute)| -> 372840008 |Ciprofloxacin (substance)| 
	}
```

\


Note the three angle brackets at the start of this concept expression, indicating that the concept is primitive.

This will be because no attribute mapping was available for the "system" part.&#x20;

This is also reflected in the terms below, where the LOINC system "Isolate.meningitis" has been used directly.

#### Terming <a href="#id-4.2.7qualityobservablewithsusceptibility-terming" id="id-4.2.7qualityobservablewithsusceptibility-terming"></a>

Template slots are filled by taking the preferred term of the relevant value from the model and making the initial character lower case, if allowed by the case significance setting of the preferred term.

\[PROPERTY] of \[COMPONENT] in \[SYSTEM] at \[TIME] by \[METHOD] using \[DEVICE] \[CHALLENGE]

Some slots are optional, and are then tidied up along with any linking words (eg 'using')

The LOINC Long Common Name is specified as the Preferred Term and the LOINC Short Common Name is also included unchanged as an acceptable synonym.  Finally a terse form of the LOINC Parts is added, with all part names specified, separated by colons.

In the case of the example below, this results in the following terms:

* 2213311010000110 \[481741010000108] US: P Susceptibility to ciprofloxacin in isolate.meningitis at point in time (observable entity) \[ci],
* 2213301010000112 \[481741010000108] US: P Ciprofloxacin \[Susceptibility] for meningitis \[CS],
* 2213331010000118 \[481741010000108] US: A Ciprofloxacin:Susc:Pt:Isolate.meningitis:OrdQn \[CS],
* 2213321010000116 \[481741010000108] US: A Ciprofloxacin (Isolate.meningitis) \[Susc] \[CS],
* 2213291010000111 \[481741010000108] US: A Susceptibility to diprofloxacin in isolate.meningitis at point in time \[ci]

### Examples <a href="#id-4.2.7qualityobservablewithsusceptibility-examples" id="id-4.2.7qualityobservablewithsusceptibility-examples"></a>

LOINC Term [103653-2](https://loinc.org/103653-2)

#### Loinc Parts mapped to SNOMED Attributes <a href="#id-4.2.7qualityobservablewithsusceptibility-loincpartsmappedtosnomedattributes" id="id-4.2.7qualityobservablewithsusceptibility-loincpartsmappedtosnomedattributes"></a>

| Part Type | LOINC Part Name | LOINC Part Num | Mapped to Attribute Type / Value                                                                      |
| --------- | --------------- | -------------- | ----------------------------------------------------------------------------------------------------- |
| Component | Ciprofloxacin   | LP15380-6      | 704320005 \|Towards (attribute)\| -> 372840008 \|Ciprofloxacin (substance)\|                          |
| Property  | Susc            | LP6870-2       | 370130000 \|Property (attribute)\| -> 118588007 \|Susceptibility (property) (qualifier value)\|       |
| Time      | Pt              | LP6960-1       | 370134009 \|Time aspect (attribute)\| -> 123029007 \|Single point in time (qualifier value)\|         |
| Scale     | OrdQn           | LP7752-1       | 370132008 \|Scale type (attribute)\| -> 117365007 \|Ordinal OR quantitative value (qualifier value)\| |
