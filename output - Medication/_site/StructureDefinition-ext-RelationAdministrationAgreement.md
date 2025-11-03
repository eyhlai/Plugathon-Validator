# ext RelationAdministrationAgreement - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext RelationAdministrationAgreement**

## Extension: ext RelationAdministrationAgreement 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-RelationAdministrationAgreement | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtRelationAdministrationAgreement |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide a relation to an AdministrationAgreement on which the MedicationAgreement or AdministrationAgreement is based.

This extension represents the RelationAdministrationAgreement concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md) and [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-RelationAdministrationAgreement)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-RelationAdministrationAgreement.csv), [Excel](StructureDefinition-ext-RelationAdministrationAgreement.xlsx), [Schematron](StructureDefinition-ext-RelationAdministrationAgreement.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-RelationAdministrationAgreement",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-RelationAdministrationAgreement",
  "version" : "0.1.0",
  "name" : "ExtRelationAdministrationAgreement",
  "title" : "ext RelationAdministrationAgreement",
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
  "description" : "An extension to provide a relation to an AdministrationAgreement on which the MedicationAgreement or AdministrationAgreement is based.",
  "purpose" : "This extension represents the RelationAdministrationAgreement concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
    },
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-RelationAdministrationAgreement"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "RelationAdministrationAgreement",
        "definition" : "A reference to an AdministrationAgreement on which the MedicationAgreement or AdministrationAgreement is based.",
        "alias" : ["RelatieToedieningsafspraak"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-AdministrationAgreement"
            ]
          }
        ]
      }
    ]
  }
}

```
