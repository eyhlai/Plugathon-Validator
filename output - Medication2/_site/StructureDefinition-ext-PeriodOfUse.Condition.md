# ext-PeriodOfUse.Condition - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext-PeriodOfUse.Condition**

## Extension: ext-PeriodOfUse.Condition 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-PeriodOfUse.Condition | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtPeriodOfUseCondition |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide a Condition to a PeriodOfUse.

This extension represents the PeriodOfUse.Condition concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md) and [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-PeriodOfUse.Condition)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-PeriodOfUse.Condition.csv), [Excel](StructureDefinition-ext-PeriodOfUse.Condition.xlsx), [Schematron](StructureDefinition-ext-PeriodOfUse.Condition.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-PeriodOfUse.Condition",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-PeriodOfUse.Condition",
  "version" : "0.1.0",
  "name" : "ExtPeriodOfUseCondition",
  "title" : "ext-PeriodOfUse.Condition",
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
  "description" : "An extension to provide a Condition to a PeriodOfUse.",
  "purpose" : "This extension represents the PeriodOfUse.Condition concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
      "expression" : "Period"
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-PeriodOfUse.Condition"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "Condition",
        "definition" : "Element to indicate that the start or end date is uncertain.\r\n\r\nIn certain situations the start or end date can depend on another piece of information. This is, for example, the case when a patient has to start or stop medication a few days before hospital admission. In that case this element is used to indicate (in free text): ‘start X days before hospital admission’ or ‘stop X days before hospital admission’. By doing this, it is clear that the entered start or end date is uncertain when the MedicationAgreement or AdministrationAgreement is being exchanged.",
        "alias" : ["Criterium"],
        "type" : [
          {
            "code" : "string"
          }
        ]
      }
    ]
  }
}

```
