# ext RenderedDosageInstruction - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext RenderedDosageInstruction**

## Extension: ext RenderedDosageInstruction 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-RenderedDosageInstruction | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtRenderedDosageInstruction |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

Pre-adopt of the `.renderedDosageInstructions` concept from the FHIR R5 medication resources. It provides a full representation of the dose of the medication included in all dosage instructions. To be used when multiple dosage instructions are included to represent complex dosing such as increasing or tapering doses.

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md), [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md), [mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md) and [mp VariableDosingRegimen](StructureDefinition-mp-VariableDosingRegimen.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-RenderedDosageInstruction)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-RenderedDosageInstruction.csv), [Excel](StructureDefinition-ext-RenderedDosageInstruction.xlsx), [Schematron](StructureDefinition-ext-RenderedDosageInstruction.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-RenderedDosageInstruction",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-RenderedDosageInstruction",
  "version" : "0.1.0",
  "name" : "ExtRenderedDosageInstruction",
  "title" : "ext RenderedDosageInstruction",
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
  "description" : "Pre-adopt of the `.renderedDosageInstructions` concept from the FHIR R5 medication resources. It provides a full representation of the dose of the medication included in all dosage instructions. To be used when multiple dosage instructions are included to represent complex dosing such as increasing or tapering doses.",
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
        "definition" : "Pre-adopt from FHIR R5 of the `.renderedDosageInstruction` element found in various medication resources.",
        "max" : "1"
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-RenderedDosageInstruction"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "definition" : "The full representation of the dose of the medication included in all dosage instructions. To be used when multiple dosage instructions are included to represent complex dosing such as increasing or tapering doses.",
        "comment" : "The content of the rendered dosage instruction must not be different from the dose represented in the dosage instructions content.",
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
