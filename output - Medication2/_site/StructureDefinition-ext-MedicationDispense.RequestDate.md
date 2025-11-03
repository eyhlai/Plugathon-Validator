# ext MedicationDispense.RequestDate - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext MedicationDispense.RequestDate**

## Extension: ext MedicationDispense.RequestDate 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-MedicationDispense.RequestDate | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtMedicationDispenseRequestDate |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide the time at which a pharmacist records an intended dispense.

This extension represents the RequestDate concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp MedicationDispense](StructureDefinition-mp-MedicationDispense.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-MedicationDispense.RequestDate)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-MedicationDispense.RequestDate.csv), [Excel](StructureDefinition-ext-MedicationDispense.RequestDate.xlsx), [Schematron](StructureDefinition-ext-MedicationDispense.RequestDate.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-MedicationDispense.RequestDate",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationDispense.RequestDate",
  "version" : "0.1.0",
  "name" : "ExtMedicationDispenseRequestDate",
  "title" : "ext MedicationDispense.RequestDate",
  "status" : "active",
  "date" : "2025-10-30T15:05:26+00:00",
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
  "description" : "An extension to provide the time at which a pharmacist records an intended dispense.",
  "purpose" : "This extension represents the RequestDate concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
      "expression" : "MedicationDispense"
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationDispense.RequestDate"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "RequestDate",
        "definition" : "The request date is the time at which a pharmacist records an intended dispense.",
        "alias" : ["AanschrijfDatum"],
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
