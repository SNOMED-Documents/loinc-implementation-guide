# Quality observable with Component for LOINC Grouper

This template is used for LOINC Concepts that do not have all their parts specified and which, as such, act as groupers for all child concepts which also have the same parts.  These grouper concepts are all expected to be orderable.

This template is documented here:  [Quality observable with Component for LOINC Grouper (observable entity) - v1.0](https://conf.spaces.snomed.org/wiki/spaces/SCTEMPLATES/pages/134002439/Quality+observable+with+Component+for+LOINC+Grouper+observable+entity+-+v1.0)

The java implementation of this template can be found [here](https://github.com/IHTSDO/reporting-engine/tree/7.9.2/script-engine/src/main/java/org/ihtsdo/termserver/scripting/pipeline/loinc/template/LoincTemplatedConceptForGrouper.java).

## Attributes <a href="#id-4.2.5qualityobservablewithratio-attributes" id="id-4.2.5qualityobservablewithratio-attributes"></a>

* **LOINC Property**: Represents the property of the observation, such as mass concentration or presence.
* **LOINC System**: Specifies the direct site of the observation.
* **LOINC Component**: Represents the specific component being measured or observed.

{% hint style="info" %}
LOINC Properties currently supported: {Measurement}
{% endhint %}

## Template <a href="#id-4.2.5qualityobservablewithratio-template" id="id-4.2.5qualityobservablewithratio-template"></a>

### Model <a href="#id-4.2.5qualityobservablewithratio-model" id="id-4.2.5qualityobservablewithratio-model"></a>

{% code overflow="wrap" %}
```
=== 363787002 |Observable entity (observable entity)| : {  
  [S1] 246093002 |Component (attribute)| -> 304053000 |Phosphate electrolyte (substance)|,
  [S1] 370130000 |Property (attribute)| -> 685451010000100 |Measurement property (qualifier value)|,
  [S1] 704327008 |Direct site (attribute)| -> 122575003 |Urine specimen (specimen)| 
}
```
{% endcode %}

### Terming <a href="#id-4.2.5qualityobservablewithratio-terming" id="id-4.2.5qualityobservablewithratio-terming"></a>

Template slots are filled by taking the preferred term of the relevant value from the model and making the initial character lower case, if allowed by the case significance setting of the preferred term.

{% code overflow="wrap" %}
```
[PROPERTY] of [COMPONENT] in [SYSTEM] 
```
{% endcode %}

The LOINC Long Common Name is specified as the Preferred Term and the LOINC Short Common Name is also included unchanged as an acceptable synonym. Finally a terse form of the LOINC Parts is added, with all part names specified, separated by colons.

In the case of the example below, this results in the following terms:

<table><thead><tr><th>Concept Id</th><th>Description Id</th><th width="99.43487548828125">Acceptability</th><th width="292.2630615234375">Term</th><th>Case</th></tr></thead><tbody><tr><td>711831010000101</td><td>4079581010000116</td><td>US: P</td><td>Measurement of phosphate electrolyte in urine (observable entity)</td><td>ci</td></tr><tr><td>711831010000101</td><td>4079571010000119</td><td>US: P</td><td>Phosphate [Measurement] in Urine</td><td>CS</td></tr><tr><td>711831010000101</td><td>4079561010000112</td><td>US: A</td><td>Measurement of phosphate electrolyte in urine</td><td>ci</td></tr><tr><td>711831010000101</td><td>4079591010000118</td><td>US: A</td><td>Phosphate (U) [Measurement]</td><td>CS</td></tr><tr><td>711831010000101</td><td>4079601010000112</td><td>US: A</td><td>Phosphate:{Measurement}:-:Urine:-</td><td>CS</td></tr></tbody></table>

### Examples <a href="#id-4.2.5qualityobservablewithratio-examples" id="id-4.2.5qualityobservablewithratio-examples"></a>

**LOINC Term** 108011-8

#### Loinc Parts <a href="#id-4.2.5qualityobservablewithratio-loincparts" id="id-4.2.5qualityobservablewithratio-loincparts"></a>

<table data-full-width="true"><thead><tr><th width="163.52734375">Part Type</th><th width="166.0859375">LOINC Part Name</th><th width="163.55859375">LOINC Part Num</th><th>Mapped to Attribute Type / Value</th></tr></thead><tbody><tr><td>Component</td><td>Phosphate</td><td>LP14912-7</td><td>246093002 |Component (attribute)| -> 304053000 |Phosphate electrolyte (substance)|</td></tr><tr><td>Property</td><td>{Measurement}</td><td>LP447904-6</td><td>370130000 |Property (attribute)| -> 685451010000100 |Measurement property (qualifier value)|</td></tr><tr><td>System</td><td>Urine</td><td>LP7681-2</td><td>704327008 |Direct site (attribute)| -> 122575003 |Urine specimen (specimen)|</td></tr></tbody></table>
