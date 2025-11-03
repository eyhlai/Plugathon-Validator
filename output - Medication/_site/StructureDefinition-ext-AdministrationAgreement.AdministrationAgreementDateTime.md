# ext AdministrationAgreement.AdministrationAgreementDateTime - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext AdministrationAgreement.AdministrationAgreementDateTime**

## Extension: ext AdministrationAgreement.AdministrationAgreementDateTime 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-AdministrationAgreement.AdministrationAgreementDateTime | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtAdministrationAgreementAdministrationAgreementDateTime |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide the time at which the agreement was made.

This extension represents the AdministrationAgreementDateTime concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-AdministrationAgreement.AdministrationAgreementDateTime)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-AdministrationAgreement.AdministrationAgreementDateTime.csv), [Excel](StructureDefinition-ext-AdministrationAgreement.AdministrationAgreementDateTime.xlsx), [Schematron](StructureDefinition-ext-AdministrationAgreement.AdministrationAgreementDateTime.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-AdministrationAgreement.AdministrationAgreementDateTime",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-AdministrationAgreement.AdministrationAgreementDateTime",
  "version" : "0.1.0",
  "name" : "ExtAdministrationAgreementAdministrationAgreementDateTime",
  "title" : "ext AdministrationAgreement.AdministrationAgreementDateTime",
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
  "description" : "An extension to provide the time at which the agreement was made.",
  "purpose" : "This extension represents the AdministrationAgreementDateTime concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-AdministrationAgreement.AdministrationAgreementDateTime"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "AdministrationAgreementDateTime",
        "definition" : "The time at which the agreement was made.",
        "alias" : ["ToedieningsafspraakDatumTijd"],
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
