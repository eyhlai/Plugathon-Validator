# ext MedicationUse2.Prescriber - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext MedicationUse2.Prescriber**

## Extension: ext MedicationUse2.Prescriber 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-MedicationUse2.Prescriber | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtMedicationUse2Prescriber |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to reference the health professional that entered the medication agreement with the patient.

This extension represents the Prescriber concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-MedicationUse2.Prescriber)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-MedicationUse2.Prescriber.csv), [Excel](StructureDefinition-ext-MedicationUse2.Prescriber.xlsx), [Schematron](StructureDefinition-ext-MedicationUse2.Prescriber.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-MedicationUse2.Prescriber",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationUse2.Prescriber",
  "version" : "0.1.0",
  "name" : "ExtMedicationUse2Prescriber",
  "title" : "ext MedicationUse2.Prescriber",
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
  "description" : "An extension to reference the health professional that entered the medication agreement with the patient.",
  "purpose" : "This extension represents the Prescriber concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
      "expression" : "MedicationStatement"
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationUse2.Prescriber"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "Prescriber",
        "definition" : "The health professional that entered the medication agreement with the patient.",
        "alias" : ["Voorschrijver"],
        "type" : [
          {
            "code" : "Reference",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-NlCoreHealthProfessionalReference"
            ],
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthProfessional-PractitionerRole"
            ]
          }
        ]
      }
    ]
  }
}

```
