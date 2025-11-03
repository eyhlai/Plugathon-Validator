# ext InstructionsForUse.RepeatPeriodCyclicalSchedule - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext InstructionsForUse.RepeatPeriodCyclicalSchedule**

## Extension: ext InstructionsForUse.RepeatPeriodCyclicalSchedule 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-InstructionsForUse.RepeatPeriodCyclicalSchedule | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtInstructionsForUseRepeatPeriodCyclicalSchedule |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

The repeated period in a cyclical schedule (of one or more dosing instructions). A cyclical schedule is noted in days, the corresponding dosing duration is also in days.

The dosage instructions are interpreted differently if RepeatPeriodCyclicalSchedule is present. Therefore this extension is labeled as a modifier extension.

This extension represents the RepeatPeriodCyclicalSchedule concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

This extension should be used together with the [mp-InstructionsForUse.DosageInstructions](http://nictiz.nl/fhir/StructureDefinition/mp-InstructionsForUse.DosageInstructions) data type profile and [ext-RenderedDosageInstruction](http://nictiz.nl/fhir/StructureDefinition/ext-RenderedDosageInstruction) extension to fully implement the zib InstructionsForUse.

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md), [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md), [mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md) and [mp VariableDosingRegimen](StructureDefinition-mp-VariableDosingRegimen.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-InstructionsForUse.RepeatPeriodCyclicalSchedule)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-InstructionsForUse.RepeatPeriodCyclicalSchedule.csv), [Excel](StructureDefinition-ext-InstructionsForUse.RepeatPeriodCyclicalSchedule.xlsx), [Schematron](StructureDefinition-ext-InstructionsForUse.RepeatPeriodCyclicalSchedule.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-InstructionsForUse.RepeatPeriodCyclicalSchedule",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-InstructionsForUse.RepeatPeriodCyclicalSchedule",
  "version" : "0.1.0",
  "name" : "ExtInstructionsForUseRepeatPeriodCyclicalSchedule",
  "title" : "ext InstructionsForUse.RepeatPeriodCyclicalSchedule",
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
  "description" : "The repeated period in a cyclical schedule (of one or more dosing instructions). A cyclical schedule is noted in days, the corresponding dosing duration is also in days.\r\n\r\nThe dosage instructions are interpreted differently if RepeatPeriodCyclicalSchedule is present. Therefore this extension is labeled as a modifier extension.",
  "purpose" : "This extension represents the RepeatPeriodCyclicalSchedule concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).\r\n\r\nThis extension should be used together with the [mp-InstructionsForUse.DosageInstructions](http://nictiz.nl/fhir/StructureDefinition/mp-InstructionsForUse.DosageInstructions) data type profile and [ext-RenderedDosageInstruction](http://nictiz.nl/fhir/StructureDefinition/ext-RenderedDosageInstruction) extension to fully implement the zib InstructionsForUse.",
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
      "expression" : "MedicationRequest"
    },
    {
      "type" : "element",
      "expression" : "MedicationDispense"
    },
    {
      "type" : "element",
      "expression" : "MedicationStatement"
    },
    {
      "type" : "element",
      "expression" : "Timing"
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
        "max" : "1",
        "isModifier" : true,
        "isModifierReason" : "The dosage instructions are interpreted differently if RepeatPeriodCyclicalSchedule is present. Therefore this extension is labeled as a modifier extension."
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-InstructionsForUse.RepeatPeriodCyclicalSchedule"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "RepeatPeriodCyclicalSchedule",
        "definition" : "The repeated period in a cyclical schedule (of one or more dosing instructions). A cyclical schedule is noted in days, the corresponding dosing duration is also in days.\r\n\r\nExamples of a cyclical schedule:  \r\ncontraceptive pill (21 days, 1 pill 1x a day, then skip for 7 days, repeat), repeat period here is 28 days",
        "alias" : ["HerhaalperiodeCyclischSchema"],
        "type" : [
          {
            "code" : "Duration"
          }
        ]
      }
    ]
  }
}

```
