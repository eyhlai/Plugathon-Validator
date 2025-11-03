# ext ResourceCategory - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext ResourceCategory**

## Extension: ext ResourceCategory 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-ResourceCategory | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtResourceCategory |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

This extension is used to augment a reference with the target resource category, in cases when `Reference.type` is not precise enough to determine the functional counterpart of the reference and `Reference.identifier` is used. The value of this extension is often a semantic code (e.g. the zib's root definition code) which identifies the target resource category.

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-ResourceCategory)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-ResourceCategory.csv), [Excel](StructureDefinition-ext-ResourceCategory.xlsx), [Schematron](StructureDefinition-ext-ResourceCategory.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-ResourceCategory",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-ResourceCategory",
  "version" : "0.1.0",
  "name" : "ExtResourceCategory",
  "title" : "ext ResourceCategory",
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
  "description" : "This extension is used to augment a reference with the target resource category, in cases when `Reference.type` is not precise enough to determine the functional counterpart of the reference and `Reference.identifier` is used. The value of this extension is often a semantic code (e.g. the zib's root definition code) which identifies the target resource category.",
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
      "expression" : "Reference"
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-ResourceCategory"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "definition" : "The expected resource category of the target of the reference. \r\n\r\nThe ResourceCategory is a semantic code that represents the category of the resource this reference refers to.",
        "comment" : "This element is used to indicate the resource's category of the target of the reference in cases when the `Reference.type` is not precise enough to determine the functional counterpart of the reference element.",
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
