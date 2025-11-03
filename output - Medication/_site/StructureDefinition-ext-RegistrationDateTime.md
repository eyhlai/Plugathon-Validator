# ext RegistrationDateTime - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext RegistrationDateTime**

## Extension: ext RegistrationDateTime 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-RegistrationDateTime | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtRegistrationDateTime |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide the date and time a certain medication agreement, variable-dosing regimen, administration agreement or medication administration was recorded.

For the medication administration this extension can be seen as a pre-adopt of the `MedicationAdministration.recorded` element that has been added in FHIR R5.

This extension represents the RegistrationDateTime concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md), [mp MedicationAdministration2](StructureDefinition-mp-MedicationAdministration2.md), [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md) and [mp VariableDosingRegimen](StructureDefinition-mp-VariableDosingRegimen.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-RegistrationDateTime)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-RegistrationDateTime.csv), [Excel](StructureDefinition-ext-RegistrationDateTime.xlsx), [Schematron](StructureDefinition-ext-RegistrationDateTime.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-RegistrationDateTime",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-RegistrationDateTime",
  "version" : "0.1.0",
  "name" : "ExtRegistrationDateTime",
  "title" : "ext RegistrationDateTime",
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
  "description" : "An extension to provide the date and time a certain medication agreement, variable-dosing regimen, administration agreement or medication administration was recorded.\r\n\r\nFor the medication administration this extension can be seen as a pre-adopt of the `MedicationAdministration.recorded` element that has been added in FHIR R5.",
  "purpose" : "This extension represents the RegistrationDateTime concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
    },
    {
      "type" : "element",
      "expression" : "MedicationDispense"
    },
    {
      "type" : "element",
      "expression" : "MedicationRequest"
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
        "id" : "Extension.extension",
        "path" : "Extension.extension",
        "max" : "0"
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-RegistrationDateTime"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "RegistrationDateTime",
        "definition" : "The date and time when a certain agreement, variable dosing regimen or administation was recorded. RegistrationDateTime is used to accurately determine the chronological order of agreements. Therefore, the date and time are mandatory. These values are immutable. When consulting or receiving this agreement, variable dosing regimen or administation, the original RegistrationDateTime remains unchanged. \r\n\r\nNote: This data element differs from the data element RegistrationDateTime in zib RegistratieGegevens-v1.1.1 (2024NL). In zib RegistratieGegevens-v1.1.1 (2024NL), RegistrationDateTime refers to the date and time when the data was recorded. This may be the initial registration or the date and time when data was transferred. The zib concept RegistrationDateTime is not applied in MP9.",
        "alias" : ["RegistratieDatumTijd"],
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
