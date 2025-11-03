# ext Dosage AsNeededFor - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext Dosage AsNeededFor**

## Extension: ext Dosage AsNeededFor 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-Dosage-AsNeededFor | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtDosageAsNeededFor |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

Pre-adopt of the `Dosage.asNeededFor` concept from the FHIR R5 Dosage data type. In R4, `Dosage.asNeededCodeableConcept` has a maximum cardinality of 1. Additional 'asNeeded' data can be represented by adding this extension to Dosage.

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp InstructionsForUse.DosageInstructions](StructureDefinition-mp-InstructionsForUse.DosageInstructions.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-Dosage-AsNeededFor)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-Dosage-AsNeededFor.csv), [Excel](StructureDefinition-ext-Dosage-AsNeededFor.xlsx), [Schematron](StructureDefinition-ext-Dosage-AsNeededFor.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-Dosage-AsNeededFor",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-Dosage-AsNeededFor",
  "version" : "0.1.0",
  "name" : "ExtDosageAsNeededFor",
  "title" : "ext Dosage AsNeededFor",
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
  "description" : "Pre-adopt of the `Dosage.asNeededFor` concept from the FHIR R5 Dosage data type. In R4, `Dosage.asNeededCodeableConcept` has a maximum cardinality of 1. Additional 'asNeeded' data can be represented by adding this extension to Dosage.",
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
      "expression" : "Dosage"
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
        "definition" : "Pre-adopt from FHIR R5 of the `Dosage.asNeededFor` element."
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-Dosage-AsNeededFor"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "definition" : "Indicates whether the Medication is only taken based on a precondition for taking the Medication (CodeableConcept).",
        "comment" : "If only one 'asNeeded' concept is exchanged within a Dosage, use `Dosage.asNeeded[x]`. This extension is only used when multiple 'asNeeded' concepts are to be exchanged.",
        "type" : [
          {
            "code" : "CodeableConcept"
          }
        ]
      }
    ]
  }
}

```
