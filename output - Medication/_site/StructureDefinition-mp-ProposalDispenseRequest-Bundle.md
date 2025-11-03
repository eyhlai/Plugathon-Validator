# mp ProposalDispenseRequest Bundle - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp ProposalDispenseRequest Bundle**

## Resource Profile: mp ProposalDispenseRequest Bundle 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-ProposalDispenseRequest-Bundle | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpProposalDispenseRequestBundle |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
Profile on the Bundle resource which represents the structure of the Send ProposalDispenseRequest transaction conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). 

 
To define the body of the Send ProposalDispenseRequest transaction. 

**Usages:**

* This Profile is not used by any profiles in this Implementation Guide

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-ProposalDispenseRequest-Bundle)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-ProposalDispenseRequest-Bundle.csv), [Excel](StructureDefinition-mp-ProposalDispenseRequest-Bundle.xlsx), [Schematron](StructureDefinition-mp-ProposalDispenseRequest-Bundle.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-ProposalDispenseRequest-Bundle",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-ProposalDispenseRequest-Bundle",
  "version" : "0.1.0",
  "name" : "MpProposalDispenseRequestBundle",
  "title" : "mp ProposalDispenseRequest Bundle",
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
  "description" : "Profile on the Bundle resource which represents the structure of the Send ProposalDispenseRequest transaction conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
  "purpose" : "To define the body of the Send ProposalDispenseRequest transaction.",
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
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
    },
    {
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    },
    {
      "identity" : "cda",
      "uri" : "http://hl7.org/v3/cda",
      "name" : "CDA (R2)"
    },
    {
      "identity" : "w5",
      "uri" : "http://hl7.org/fhir/fivews",
      "name" : "FiveWs Pattern Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Bundle",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Bundle",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Bundle",
        "path" : "Bundle"
      },
      {
        "id" : "Bundle.type",
        "path" : "Bundle.type",
        "fixedCode" : "transaction"
      },
      {
        "id" : "Bundle.entry",
        "path" : "Bundle.entry",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "profile",
              "path" : "resource"
            }
          ],
          "rules" : "open"
        },
        "min" : 1
      },
      {
        "id" : "Bundle.entry:proposalDispenseRequest",
        "path" : "Bundle.entry",
        "sliceName" : "proposalDispenseRequest",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "Bundle.entry:proposalDispenseRequest.resource",
        "path" : "Bundle.entry.resource",
        "short" : "Proposal",
        "definition" : "Data of the proposal dispense request.",
        "alias" : ["Voorstel"],
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-DispenseRequest"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-527",
            "comment" : "Proposal"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-527",
            "comment" : "Proposal"
          }
        ]
      },
      {
        "id" : "Bundle.entry:proposalDispenseRequest.resource.meta",
        "path" : "Bundle.entry.resource.meta"
      },
      {
        "id" : "Bundle.entry:proposalDispenseRequest.resource.meta.tag",
        "path" : "Bundle.entry.resource.meta.tag",
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
        "id" : "Bundle.entry:proposalDispenseRequest.resource.meta.tag:actionable",
        "path" : "Bundle.entry.resource.meta.tag",
        "sliceName" : "actionable",
        "min" : 1,
        "max" : "1",
        "patternCoding" : {
          "system" : "http://terminology.hl7.org/CodeSystem/common-tags",
          "code" : "actionable"
        }
      },
      {
        "id" : "Bundle.entry:proposalDispenseRequest.resource.extension:proposalComment",
        "path" : "Bundle.entry.resource.extension",
        "sliceName" : "proposalComment",
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://nictiz.nl/fhir/StructureDefinition/ext-Comment"]
          }
        ]
      },
      {
        "id" : "Bundle.entry:proposalDispenseRequest.resource.extension:proposalComment.value[x]",
        "path" : "Bundle.entry.resource.extension.value[x]",
        "label" : "Toelichting",
        "short" : "Comment",
        "definition" : "Comments regarding the proposal.",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-538",
            "comment" : "Comment"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-538",
            "comment" : "Comment"
          }
        ]
      },
      {
        "id" : "Bundle.entry:proposalDispenseRequest.resource.identifier",
        "path" : "Bundle.entry.resource.identifier",
        "definition" : "The identification of the proposal. This identification is generated by the system of the person who registers the proposal and is globally unique and eternally persistent.",
        "comment" : "The Identification (of the DispenseRequest building block, mp-dataelement9x-289) does not exist within the proposal. The fact that it is overwritten by the Identification (of the proposal) here, therefore does not cause any issues.",
        "min" : 1,
        "max" : "1",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-528",
            "comment" : "Identification"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-528",
            "comment" : "Identification"
          }
        ]
      },
      {
        "id" : "Bundle.entry:proposalDispenseRequest.resource.intent",
        "path" : "Bundle.entry.resource.intent",
        "comment" : "Set to _plan_ because this Proposal DispenseRequest is intended to be acted upon by a patient, pharmacist, professional administrator et cetera.",
        "fixedCode" : "plan"
      },
      {
        "id" : "Bundle.entry:proposalDispenseRequest.resource.authoredOn",
        "path" : "Bundle.entry.resource.authoredOn",
        "short" : "ProposalDate",
        "definition" : "Date of the proposal.",
        "comment" : "The DispenseRequestDate does not exist within the proposal. The fact that it is overwritten by the ProposalDate here, therefore does not cause any issues.",
        "alias" : ["VoorstelDatum"],
        "min" : 1,
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-529",
            "comment" : "ProposalDate"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-529",
            "comment" : "ProposalDate"
          }
        ]
      },
      {
        "id" : "Bundle.entry:proposalDispenseRequest.resource.requester",
        "path" : "Bundle.entry.resource.requester",
        "definition" : "Author of the proposal.",
        "comment" : "The Author (of the DispenseRequest building block, mp-dataelement9x-290) does not exist within the proposal. The fact that it is overwritten by the Author (of the proposal) here, therefore does not cause any issues.",
        "min" : 1,
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Practitioner",
              "http://hl7.org/fhir/StructureDefinition/PractitionerRole",
              "http://hl7.org/fhir/StructureDefinition/Organization",
              "http://hl7.org/fhir/StructureDefinition/Patient",
              "http://hl7.org/fhir/StructureDefinition/RelatedPerson",
              "http://hl7.org/fhir/StructureDefinition/Device",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthProfessional-PractitionerRole",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-Patient",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthcareProvider-Organization"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-530",
            "comment" : "Author"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-530",
            "comment" : "Author"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-531",
            "comment" : "AuthorIsPatient (implicit; AuthorIsPatient = true when this element refers to the same Patient as subject)"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-531",
            "comment" : "AuthorIsPatient (implicit; AuthorIsPatient = true when this element refers to the same Patient as subject)"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-532",
            "comment" : "AuthorIsHealthProfessional"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-532",
            "comment" : "AuthorIsHealthProfessional"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1366",
            "comment" : "AuthorIsHealthcareProvider"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1366",
            "comment" : "AuthorIsHealthcareProvider"
          }
        ]
      },
      {
        "id" : "Bundle.entry:patient",
        "path" : "Bundle.entry",
        "sliceName" : "patient",
        "max" : "1"
      },
      {
        "id" : "Bundle.entry:patient.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : ["http://nictiz.nl/fhir/StructureDefinition/nl-core-Patient"]
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
        "id" : "Bundle.entry:pharmaceuticalProduct",
        "path" : "Bundle.entry",
        "sliceName" : "pharmaceuticalProduct"
      },
      {
        "id" : "Bundle.entry:pharmaceuticalProduct.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-PharmaceuticalProduct"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-260",
            "comment" : "PharmaceuticalProduct"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-260",
            "comment" : "PharmaceuticalProduct"
          }
        ]
      },
      {
        "id" : "Bundle.entry:healthProfessional-PractitionerRole",
        "path" : "Bundle.entry",
        "sliceName" : "healthProfessional-PractitionerRole"
      },
      {
        "id" : "Bundle.entry:healthProfessional-PractitionerRole.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthProfessional-PractitionerRole"
            ]
          }
        ]
      },
      {
        "id" : "Bundle.entry:healthProfessional-Practitioner",
        "path" : "Bundle.entry",
        "sliceName" : "healthProfessional-Practitioner"
      },
      {
        "id" : "Bundle.entry:healthProfessional-Practitioner.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthProfessional-Practitioner"
            ]
          }
        ]
      },
      {
        "id" : "Bundle.entry:healthcareProvider",
        "path" : "Bundle.entry",
        "sliceName" : "healthcareProvider"
      },
      {
        "id" : "Bundle.entry:healthcareProvider.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthcareProvider"
            ]
          }
        ]
      },
      {
        "id" : "Bundle.entry:healthcareProvider-Organization",
        "path" : "Bundle.entry",
        "sliceName" : "healthcareProvider-Organization"
      },
      {
        "id" : "Bundle.entry:healthcareProvider-Organization.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthcareProvider-Organization"
            ]
          }
        ]
      }
    ]
  }
}

```
