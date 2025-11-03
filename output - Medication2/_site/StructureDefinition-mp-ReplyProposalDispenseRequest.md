# mp ReplyProposalDispenseRequest - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp ReplyProposalDispenseRequest**

## Resource Profile: mp ReplyProposalDispenseRequest 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-ReplyProposalDispenseRequest | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpReplyProposalDispenseRequest |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
Profile on the Communication resource which represents the reply proposal dispense request conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). 

 
To define the reply proposal dispense request as stated in the information standard Medication Process. 

**Usages:**

* Use this Profile: [mp ReplyProposalDispenseRequest Bundle](StructureDefinition-mp-ReplyProposalDispenseRequest-Bundle.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-ReplyProposalDispenseRequest)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-ReplyProposalDispenseRequest.csv), [Excel](StructureDefinition-mp-ReplyProposalDispenseRequest.xlsx), [Schematron](StructureDefinition-mp-ReplyProposalDispenseRequest.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-ReplyProposalDispenseRequest",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-ReplyProposalDispenseRequest",
  "version" : "0.1.0",
  "name" : "MpReplyProposalDispenseRequest",
  "title" : "mp ReplyProposalDispenseRequest",
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
  "description" : "Profile on the Communication resource which represents the reply proposal dispense request conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
  "purpose" : "To define the reply proposal dispense request as stated in the information standard Medication Process.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "mp-dataset-mp9-300-beta4-20241118",
      "uri" : "https://decor.nictiz.nl/pub/medicatieproces/mp-html-20241118T151205/ds-2.16.840.1.113883.2.4.3.11.60.20.77.1.4-2022-06-30T000000.html",
      "name" : "ART-DECOR Dataset MP9 3.0.0-beta.4 20241118"
    },
    {
      "identity" : "mp-dataset-mp9-300-rc1-20250522",
      "uri" : "https://decor.nictiz.nl/pub/medicatieproces/mp-html-20250522T132618/ds-2.16.840.1.113883.2.4.3.11.60.20.77.1.4-2022-06-30T000000.html",
      "name" : "ART-DECOR Dataset MP9 3.0.0-rc.1 20250522"
    },
    {
      "identity" : "workflow",
      "uri" : "http://hl7.org/fhir/workflow",
      "name" : "Workflow Pattern"
    },
    {
      "identity" : "w5",
      "uri" : "http://hl7.org/fhir/fivews",
      "name" : "FiveWs Pattern Mapping"
    },
    {
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Communication",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Communication",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Communication",
        "path" : "Communication",
        "short" : "Response",
        "definition" : "Response to the proposal dispense request.",
        "alias" : ["Antwoord"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-539",
            "comment" : "Response"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-539",
            "comment" : "Response"
          }
        ]
      },
      {
        "id" : "Communication.meta",
        "path" : "Communication.meta"
      },
      {
        "id" : "Communication.meta.tag",
        "path" : "Communication.meta.tag",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "pattern",
              "path" : "$this"
            }
          ],
          "rules" : "open"
        },
        "min" : 1
      },
      {
        "id" : "Communication.meta.tag:actionable",
        "path" : "Communication.meta.tag",
        "sliceName" : "actionable",
        "min" : 1,
        "max" : "1",
        "patternCoding" : {
          "system" : "http://terminology.hl7.org/CodeSystem/common-tags",
          "code" : "actionable"
        }
      },
      {
        "id" : "Communication.identifier",
        "path" : "Communication.identifier",
        "short" : "Identification",
        "definition" : "The identification of the response to the proposal. This identification is generated by the system of the person who registers the response and is globally unique and eternally persistent.",
        "alias" : ["Identificatie"],
        "min" : 1,
        "max" : "1",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-540",
            "comment" : "Identification"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-540",
            "comment" : "Identification"
          }
        ]
      },
      {
        "id" : "Communication.basedOn",
        "path" : "Communication.basedOn",
        "short" : "RelationToProposalData",
        "definition" : "Relation to proposal data.",
        "alias" : ["RelatieVoorstelGegevens"],
        "min" : 1,
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Resource",
              "http://nictiz.nl/fhir/StructureDefinition/mp-DispenseRequest"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-544",
            "comment" : "RelationToProposalData"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-544",
            "comment" : "RelationToProposalData"
          }
        ]
      },
      {
        "id" : "Communication.subject",
        "path" : "Communication.subject",
        "short" : "Patient",
        "alias" : ["Patient"],
        "min" : 1,
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Patient",
              "http://hl7.org/fhir/StructureDefinition/Group",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-Patient"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1",
            "comment" : "Patient"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1",
            "comment" : "Patient"
          }
        ]
      },
      {
        "id" : "Communication.sent",
        "path" : "Communication.sent",
        "short" : "ResponseDate",
        "definition" : "Date of the response to the proposal.",
        "alias" : ["AntwoordDatum"],
        "min" : 1,
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-541",
            "comment" : "ResponseDate"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-541",
            "comment" : "ResponseDate"
          }
        ]
      },
      {
        "id" : "Communication.sender",
        "path" : "Communication.sender",
        "short" : "Author",
        "definition" : "Author of the response to the proposal.",
        "alias" : ["Auteur"],
        "min" : 1,
        "type" : [
          {
            "code" : "Reference",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-NlCoreHealthProfessionalReference"
            ],
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Device",
              "http://hl7.org/fhir/StructureDefinition/Organization",
              "http://hl7.org/fhir/StructureDefinition/Patient",
              "http://hl7.org/fhir/StructureDefinition/Practitioner",
              "http://hl7.org/fhir/StructureDefinition/PractitionerRole",
              "http://hl7.org/fhir/StructureDefinition/RelatedPerson",
              "http://hl7.org/fhir/StructureDefinition/HealthcareService",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthProfessional-PractitionerRole"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-542",
            "comment" : "Author"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-542",
            "comment" : "Author"
          }
        ]
      },
      {
        "id" : "Communication.payload",
        "path" : "Communication.payload",
        "min" : 1
      },
      {
        "id" : "Communication.payload.content[x]",
        "path" : "Communication.payload.content[x]",
        "type" : [
          {
            "code" : "string"
          }
        ]
      },
      {
        "id" : "Communication.payload.content[x].extension",
        "path" : "Communication.payload.content[x].extension",
        "min" : 1
      },
      {
        "id" : "Communication.payload.content[x].extension:contentCodeableConcept",
        "path" : "Communication.payload.content[x].extension",
        "sliceName" : "contentCodeableConcept",
        "comment" : "This is a pre-adopt of R5 in which the string data type of `.payload.content` is changed to a CodeableConcept.",
        "min" : 1,
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-Communication.Payload.ContentCodeableConcept"
            ]
          }
        ]
      },
      {
        "id" : "Communication.payload.content[x].extension:contentCodeableConcept.value[x]",
        "path" : "Communication.payload.content[x].extension.value[x]",
        "short" : "ResponseDispenseRequest",
        "definition" : "Response to the proposed dispense request.",
        "alias" : ["AntwoordVerstrekkingsverzoek"],
        "min" : 1,
        "binding" : {
          "strength" : "required",
          "description" : "Response to the proposed dispense request.",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.36--20180412153353"
        },
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-546",
            "comment" : "ResponseDispenseRequest"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-546",
            "comment" : "ResponseDispenseRequest"
          }
        ]
      }
    ]
  }
}

```
