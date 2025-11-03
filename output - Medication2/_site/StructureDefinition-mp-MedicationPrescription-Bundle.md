# mp MedicationPrescription Bundle - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp MedicationPrescription Bundle**

## Resource Profile: mp MedicationPrescription Bundle 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-MedicationPrescription-Bundle | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpMedicationPrescriptionBundle |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
Profile on the Bundle resource which represents the structure of the Send MedicationPrescription transaction conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). 

 
To define the body of the Send MedicationPrescription transaction. 

**Usages:**

* This Profile is not used by any profiles in this Implementation Guide

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-MedicationPrescription-Bundle)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-MedicationPrescription-Bundle.csv), [Excel](StructureDefinition-mp-MedicationPrescription-Bundle.xlsx), [Schematron](StructureDefinition-mp-MedicationPrescription-Bundle.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-MedicationPrescription-Bundle",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationPrescription-Bundle",
  "version" : "0.1.0",
  "name" : "MpMedicationPrescriptionBundle",
  "title" : "mp MedicationPrescription Bundle",
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
  "description" : "Profile on the Bundle resource which represents the structure of the Send MedicationPrescription transaction conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
  "purpose" : "To define the body of the Send MedicationPrescription transaction.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
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
        "id" : "Bundle.entry:medicationAgreement",
        "path" : "Bundle.entry",
        "sliceName" : "medicationAgreement",
        "min" : 1
      },
      {
        "id" : "Bundle.entry:medicationAgreement.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationAgreement"
            ]
          }
        ]
      },
      {
        "id" : "Bundle.entry:medicationAgreement.resource.meta",
        "path" : "Bundle.entry.resource.meta"
      },
      {
        "id" : "Bundle.entry:medicationAgreement.resource.meta.tag",
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
        "id" : "Bundle.entry:medicationAgreement.resource.meta.tag:actionable",
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
        "id" : "Bundle.entry:medicationAgreement.resource.intent",
        "path" : "Bundle.entry.resource.intent",
        "comment" : "Set to _order_ because this MedicationAgreement authorizes an action for a patient, pharmacist, professional administrator et cetera.",
        "fixedCode" : "order"
      },
      {
        "id" : "Bundle.entry:dispenseRequest",
        "path" : "Bundle.entry",
        "sliceName" : "dispenseRequest"
      },
      {
        "id" : "Bundle.entry:dispenseRequest.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-DispenseRequest"
            ]
          }
        ]
      },
      {
        "id" : "Bundle.entry:dispenseRequest.resource.meta",
        "path" : "Bundle.entry.resource.meta"
      },
      {
        "id" : "Bundle.entry:dispenseRequest.resource.meta.tag",
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
        "id" : "Bundle.entry:dispenseRequest.resource.meta.tag:actionable",
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
        "id" : "Bundle.entry:dispenseRequest.resource.intent",
        "path" : "Bundle.entry.resource.intent",
        "comment" : "Set to _order_ because this DispenseRequest should authorize an action for a patient, pharmacist, professional administrator et cetera.",
        "fixedCode" : "order"
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
      },
      {
        "id" : "Bundle.entry:bodyHeight",
        "path" : "Bundle.entry",
        "sliceName" : "bodyHeight",
        "max" : "1"
      },
      {
        "id" : "Bundle.entry:bodyHeight.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-BodyHeight"
            ]
          }
        ]
      },
      {
        "id" : "Bundle.entry:bodyWeight",
        "path" : "Bundle.entry",
        "sliceName" : "bodyWeight",
        "max" : "1"
      },
      {
        "id" : "Bundle.entry:bodyWeight.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-BodyWeight"
            ]
          }
        ]
      }
    ]
  }
}

```
