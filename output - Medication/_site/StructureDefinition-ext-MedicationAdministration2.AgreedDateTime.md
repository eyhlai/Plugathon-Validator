# ext MedicationAdministration2.AgreedDateTime - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext MedicationAdministration2.AgreedDateTime**

## Extension: ext MedicationAdministration2.AgreedDateTime 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAdministration2.AgreedDateTime | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtMedicationAdministration2AgreedDateTime |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide the date and time in the medication or administration agreement to which this administration pertains.

This extension represents the AgreedDateTime concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp MedicationAdministration2](StructureDefinition-mp-MedicationAdministration2.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-MedicationAdministration2.AgreedDateTime)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-MedicationAdministration2.AgreedDateTime.csv), [Excel](StructureDefinition-ext-MedicationAdministration2.AgreedDateTime.xlsx), [Schematron](StructureDefinition-ext-MedicationAdministration2.AgreedDateTime.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-MedicationAdministration2.AgreedDateTime",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAdministration2.AgreedDateTime",
  "version" : "0.1.0",
  "name" : "ExtMedicationAdministration2AgreedDateTime",
  "title" : "ext MedicationAdministration2.AgreedDateTime",
  "status" : "active",
  "date" : "2025-10-30T10:56:51+00:00",
  "contact" : [
    {
      "name" : "Nictiz",
      "telecom" : [
        {
          "system" : "url",
          "value" : "https://www.nictiz.nl",
          "use" : "work"
        }
      ]
    }
  ],
  "description" : "An extension to provide the date and time in the medication or administration agreement to which this administration pertains.",
  "purpose" : "This extension represents the AgreedDateTime concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    }
  ],
  "kind" : "complex-type",
  "abstract" : false,
  "context" : [
    {
      "type" : "element",
      "expression" : "MedicationAdministration"
    }
  ],
  "type" : "Extension",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Extension",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Extension",
        "path" : "Extension",
        "max" : "1"
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAdministration2.AgreedDateTime"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "AgreedDateTime",
        "definition" : "Date and time in the medication or administration agreement to which this administration pertains. Since multiple times can be indicated in one medication/administration agreement, this can be used to identify the agreed time in the event of e.g. early administration or a late administration.",
        "alias" : ["AfgesprokenDatumTijd"],
        "type" : [
          {
            "code" : "dateTime"
          }
        ]
      }
    ]
  }
}

```
