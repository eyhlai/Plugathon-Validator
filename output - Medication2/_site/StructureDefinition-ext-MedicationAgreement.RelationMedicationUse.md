# ext MedicationAgreement.RelationMedicationUse - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext MedicationAgreement.RelationMedicationUse**

## Extension: ext MedicationAgreement.RelationMedicationUse 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAgreement.RelationMedicationUse | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtMedicationAgreementRelationMedicationUse |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide a relation to a MedicationUse2 on which the MedicationAgreement is based.

This extension represents the RelationMedicationUse concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-MedicationAgreement.RelationMedicationUse)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-MedicationAgreement.RelationMedicationUse.csv), [Excel](StructureDefinition-ext-MedicationAgreement.RelationMedicationUse.xlsx), [Schematron](StructureDefinition-ext-MedicationAgreement.RelationMedicationUse.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-MedicationAgreement.RelationMedicationUse",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAgreement.RelationMedicationUse",
  "version" : "0.1.0",
  "name" : "ExtMedicationAgreementRelationMedicationUse",
  "title" : "ext MedicationAgreement.RelationMedicationUse",
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
  "description" : "An extension to provide a relation to a MedicationUse2 on which the MedicationAgreement is based.",
  "purpose" : "This extension represents the RelationMedicationUse concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
      "expression" : "MedicationRequest.basedOn"
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAgreement.RelationMedicationUse"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "RelationMedicationUse",
        "definition" : "A reference to a MedicationUse2 on which the MedicationAgreement is based.",
        "alias" : ["RelatieMedicatiegebruik"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationUse2"
            ]
          }
        ]
      }
    ]
  }
}

```
