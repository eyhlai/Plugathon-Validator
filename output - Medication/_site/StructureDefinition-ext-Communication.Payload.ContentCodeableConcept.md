# ext Communication.Payload.ContentCodeableConcept - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext Communication.Payload.ContentCodeableConcept**

## Extension: ext Communication.Payload.ContentCodeableConcept 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-Communication.Payload.ContentCodeableConcept | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtCommunicationPayloadContentCodeableConcept |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to extend `Communication.payload.content` with a CodeableConcept data type. This is a pre-adopt of R5 in which the string data type of this element is changed to a CodeableConcept.

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp ReplyProposalDispenseRequest](StructureDefinition-mp-ReplyProposalDispenseRequest.md) and [mp ReplyProposalMedicationAgreement](StructureDefinition-mp-ReplyProposalMedicationAgreement.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-Communication.Payload.ContentCodeableConcept)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-Communication.Payload.ContentCodeableConcept.csv), [Excel](StructureDefinition-ext-Communication.Payload.ContentCodeableConcept.xlsx), [Schematron](StructureDefinition-ext-Communication.Payload.ContentCodeableConcept.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-Communication.Payload.ContentCodeableConcept",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-Communication.Payload.ContentCodeableConcept",
  "version" : "0.1.0",
  "name" : "ExtCommunicationPayloadContentCodeableConcept",
  "title" : "ext Communication.Payload.ContentCodeableConcept",
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
  "description" : "An extension to extend `Communication.payload.content` with a CodeableConcept data type. This is a pre-adopt of R5 in which the string data type of this element is changed to a CodeableConcept.",
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
      "expression" : "Communication.payload.content"
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-Communication.Payload.ContentCodeableConcept"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
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
