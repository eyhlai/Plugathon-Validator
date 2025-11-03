# mp MedicationPrescriptionProcessing Bundle - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp MedicationPrescriptionProcessing Bundle**

## Resource Profile: mp MedicationPrescriptionProcessing Bundle 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-MedicationPrescriptionProcessing-Bundle | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpMedicationPrescriptionProcessingBundle |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
Profile on the Bundle resource which represents the structure of the Send MedicationPrescriptionProcessing transaction conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). 

 
To define the body of the Send MedicationPrescriptionProcessing transaction. 

**Usages:**

* This Profile is not used by any profiles in this Implementation Guide

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-MedicationPrescriptionProcessing-Bundle)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-MedicationPrescriptionProcessing-Bundle.csv), [Excel](StructureDefinition-mp-MedicationPrescriptionProcessing-Bundle.xlsx), [Schematron](StructureDefinition-mp-MedicationPrescriptionProcessing-Bundle.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-MedicationPrescriptionProcessing-Bundle",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationPrescriptionProcessing-Bundle",
  "version" : "0.1.0",
  "name" : "MpMedicationPrescriptionProcessingBundle",
  "title" : "mp MedicationPrescriptionProcessing Bundle",
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
  "description" : "Profile on the Bundle resource which represents the structure of the Send MedicationPrescriptionProcessing transaction conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
  "purpose" : "To define the body of the Send MedicationPrescriptionProcessing transaction.",
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
        "id" : "Bundle.entry:administrationAgreement",
        "path" : "Bundle.entry",
        "sliceName" : "administrationAgreement",
        "min" : 1
      },
      {
        "id" : "Bundle.entry:administrationAgreement.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-AdministrationAgreement"
            ]
          }
        ]
      },
      {
        "id" : "Bundle.entry:administrationAgreement.resource.meta",
        "path" : "Bundle.entry.resource.meta"
      },
      {
        "id" : "Bundle.entry:administrationAgreement.resource.meta.tag",
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
        "id" : "Bundle.entry:administrationAgreement.resource.meta.tag:actionable",
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
        "id" : "Bundle.entry:medicationDispense",
        "path" : "Bundle.entry",
        "sliceName" : "medicationDispense"
      },
      {
        "id" : "Bundle.entry:medicationDispense.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationDispense"
            ]
          }
        ]
      },
      {
        "id" : "Bundle.entry:medicationDispense.resource.meta",
        "path" : "Bundle.entry.resource.meta"
      },
      {
        "id" : "Bundle.entry:medicationDispense.resource.meta.tag",
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
        "id" : "Bundle.entry:medicationDispense.resource.meta.tag:actionable",
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
