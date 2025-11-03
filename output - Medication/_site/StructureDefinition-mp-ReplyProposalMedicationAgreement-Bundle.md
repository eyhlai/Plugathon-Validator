# mp ReplyProposalMedicationAgreement Bundle - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp ReplyProposalMedicationAgreement Bundle**

## Resource Profile: mp ReplyProposalMedicationAgreement Bundle 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-ReplyProposalMedicationAgreement-Bundle | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpReplyProposalMedicationAgreementBundle |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
Profile on the Bundle resource which represents the structure of the Send ReplyProposalMedicationAgreement transaction conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). 

 
To define the body of the Send ReplyProposalMedicationAgreement transaction. 

**Usages:**

* This Profile is not used by any profiles in this Implementation Guide

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-ReplyProposalMedicationAgreement-Bundle)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-ReplyProposalMedicationAgreement-Bundle.csv), [Excel](StructureDefinition-mp-ReplyProposalMedicationAgreement-Bundle.xlsx), [Schematron](StructureDefinition-mp-ReplyProposalMedicationAgreement-Bundle.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-ReplyProposalMedicationAgreement-Bundle",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-ReplyProposalMedicationAgreement-Bundle",
  "version" : "0.1.0",
  "name" : "MpReplyProposalMedicationAgreementBundle",
  "title" : "mp ReplyProposalMedicationAgreement Bundle",
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
  "description" : "Profile on the Bundle resource which represents the structure of the Send ReplyProposalMedicationAgreement transaction conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
  "purpose" : "To define the body of the Send ReplyProposalMedicationAgreement transaction.",
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
        "id" : "Bundle.entry:replyProposalMedicationAgreement",
        "path" : "Bundle.entry",
        "sliceName" : "replyProposalMedicationAgreement",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "Bundle.entry:replyProposalMedicationAgreement.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-ReplyProposalMedicationAgreement"
            ]
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
