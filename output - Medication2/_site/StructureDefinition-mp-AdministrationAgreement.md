# mp AdministrationAgreement - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp AdministrationAgreement**

## Resource Profile: mp AdministrationAgreement 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-AdministrationAgreement | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpAdministrationAgreement |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
An administration agreement is the use (or administering) instructions from the pharmacist to the patient (or their representative or administrator), whereby a medication agreement is structured at a concrete level. 

 
This MedicationDispense resource represents the AdministrationAgreement building block for implementations following the information standard[MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) AdministrationAgreement, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set. 

**Usages:**

* Use this Profile: [mp MedicationPrescriptionProcessing Bundle](StructureDefinition-mp-MedicationPrescriptionProcessing-Bundle.md)
* Refer to this Profile: [ext RelationAdministrationAgreement](StructureDefinition-ext-RelationAdministrationAgreement.md), [mp MedicationAdministration2](StructureDefinition-mp-MedicationAdministration2.md), [mp MedicationOverview](StructureDefinition-mp-MedicationOverview.md) and [mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-AdministrationAgreement)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-AdministrationAgreement.csv), [Excel](StructureDefinition-mp-AdministrationAgreement.xlsx), [Schematron](StructureDefinition-mp-AdministrationAgreement.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-AdministrationAgreement",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-AdministrationAgreement",
  "version" : "0.1.0",
  "name" : "MpAdministrationAgreement",
  "title" : "mp AdministrationAgreement",
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
  "description" : "An administration agreement is the use (or administering) instructions from the pharmacist to the patient (or their representative or administrator), whereby a medication agreement is structured at a concrete level.",
  "purpose" : "This MedicationDispense resource represents the AdministrationAgreement building block for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) AdministrationAgreement, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "zib-administrationagreement-v1.0.3-2020EN",
      "uri" : "https://zibs.nl/wiki/AdministrationAgreement-v1.0.3(2020EN)",
      "name" : "zib AdministrationAgreement-v1.0.3(2020EN)"
    },
    {
      "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
      "uri" : "https://zibs.nl/wiki/InstructionsForUse-v1.2.1(2020EN)",
      "name" : "zib InstructionsForUse-v1.2.1(2020EN)"
    },
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
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    },
    {
      "identity" : "w5",
      "uri" : "http://hl7.org/fhir/fivews",
      "name" : "FiveWs Pattern Mapping"
    },
    {
      "identity" : "rx-dispense-rmim",
      "uri" : "http://www.hl7.org/v3/PORX_RM020070UV",
      "name" : "V3 Pharmacy Dispense RMIM"
    },
    {
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "MedicationDispense",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/MedicationDispense",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "MedicationDispense",
        "path" : "MedicationDispense",
        "short" : "AdministrationAgreement",
        "alias" : ["Toedieningsafspraak"],
        "mapping" : [
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.20132",
            "comment" : "AdministrationAgreement"
          },
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.22098",
            "comment" : "InstructionsForUse"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:additionalInformation",
        "path" : "MedicationDispense.extension",
        "sliceName" : "additionalInformation",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-AdministrationAgreement.AdditionalInformation"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:additionalInformation.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-342",
            "comment" : "AdministrationAgreementAdditionalInformation"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-342",
            "comment" : "AdministrationAgreementAdditionalInformation"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:reasonModificationOrDiscontinuation",
        "path" : "MedicationDispense.extension",
        "sliceName" : "reasonModificationOrDiscontinuation",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-AdministrationAgreement.ReasonModificationOrDiscontinuation"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:reasonModificationOrDiscontinuation.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-333",
            "comment" : "AdministrationAgreementReasonModificationOrDiscontinuation"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-333",
            "comment" : "AdministrationAgreementReasonModificationOrDiscontinuation"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:administrationAgreementDateTime",
        "path" : "MedicationDispense.extension",
        "sliceName" : "administrationAgreementDateTime",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-AdministrationAgreement.AdministrationAgreementDateTime"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:administrationAgreementDateTime.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.20133",
            "comment" : "AdministrationAgreementDateTime"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:renderedDosageInstruction",
        "path" : "MedicationDispense.extension",
        "sliceName" : "renderedDosageInstruction",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-RenderedDosageInstruction"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:renderedDosageInstruction.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.9581",
            "comment" : "Description"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:periodOfUse",
        "path" : "MedicationDispense.extension",
        "sliceName" : "periodOfUse",
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-TimeInterval.Period"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:periodOfUse.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "short" : "PeriodOfUse",
        "definition" : "**Start date**: This is the time at which the agreement was to take effect (or took effect or will take effect). This is the time at which the instructions for use in this agreement start. In the case of an agreement to discontinue use, this is the start date of the original administration agreement. The end date indicates from when the medication is to be discontinued.\r\n\r\n**Duration**: The intended duration of use. E.g. 5 days or 8 weeks. It is not allowed to indicate the duration in months, because different months have a variable duration in days.\r\n\r\n**End date**: The time at which the period of use ends (or ended or will end). In the case of an agreement to discontinue use, this is the time at which the medication is to be discontinued. To avoid confusion between 'to' and 'up to', the submission of time is always mandatory for the end date.\r\n\r\nWith medication for an indefinite period only a start date is indicated.",
        "alias" : ["Gebruiksperiode"],
        "type" : [
          {
            "code" : "Period",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-TimeInterval"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.22660",
            "comment" : "PeriodOfUse"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:periodOfUse.value[x].extension:condition",
        "path" : "MedicationDispense.extension.value[x].extension",
        "sliceName" : "condition",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-PeriodOfUse.Condition"
            ]
          }
        ],
        "isModifier" : false
      },
      {
        "id" : "MedicationDispense.extension:periodOfUse.value[x].extension:condition.value[x]",
        "path" : "MedicationDispense.extension.value[x].extension.value[x]",
        "definition" : "Element to indicate that the start or end date is uncertain.\r\n\r\nIn certain situations the start or end date can depend on another piece of information. This is, for example, the case when a patient has to start or stop medication a few days before hospital admission. In that case this element is used to indicate (in free text): ‘start X days before hospital admission’ or ‘stop X days before hospital admission’. By doing this, it is clear that the entered start or end date is uncertain when the AdministrationAgreement is being exchanged.",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1484"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:copyIndicator",
        "path" : "MedicationDispense.extension",
        "sliceName" : "copyIndicator",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-CopyIndicator"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:copyIndicator.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-345",
            "comment" : "CopyIndicator"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-345",
            "comment" : "CopyIndicator"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:pharmaceuticalTreatmentIdentifier",
        "path" : "MedicationDispense.extension",
        "sliceName" : "pharmaceuticalTreatmentIdentifier",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-PharmaceuticalTreatment.Identifier"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:pharmaceuticalTreatmentIdentifier.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-42",
            "comment" : "Identification"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-42",
            "comment" : "Identification"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:distributionForm",
        "path" : "MedicationDispense.extension",
        "sliceName" : "distributionForm",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationDispense.DistributionForm"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:distributionForm.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1371",
            "comment" : "DistributionForm"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1371",
            "comment" : "DistributionForm"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:relationAdministrationAgreement",
        "path" : "MedicationDispense.extension",
        "sliceName" : "relationAdministrationAgreement",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-RelationAdministrationAgreement"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:relationAdministrationAgreement.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1380",
            "comment" : "RelationAdministrationAgreement"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1380",
            "comment" : "RelationAdministrationAgreement"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:registrationDateTime",
        "path" : "MedicationDispense.extension",
        "sliceName" : "registrationDateTime",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-RegistrationDateTime"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:registrationDateTime.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "definition" : "The date and time when the AdministrationAgreement was recorded. RegistrationDateTime is used to accurately determine the chronological order of agreements. Therefore, the date and time are mandatory. These values are immutable. When consulting or receiving this AdministrationAgreement, the original RegistrationDateTime remains unchanged.\r\n\r\nNote: This data element differs from the data element RegistrationDateTime in zib RegistratieGegevens-v1.1.1 (2024NL). In zib RegistratieGegevens-v1.1.1 (2024NL), RegistrationDateTime refers to the date and time when the data was recorded. This may be the initial registration or the date and time when data was transferred. The zib concept RegistrationDateTime is not applied in MP9.",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1481",
            "comment" : "RegistrationDateTime"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1481",
            "comment" : "RegistrationDateTime"
          }
        ]
      },
      {
        "id" : "MedicationDispense.modifierExtension:stopType",
        "path" : "MedicationDispense.modifierExtension",
        "sliceName" : "stopType",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://nictiz.nl/fhir/StructureDefinition/ext-StopType"]
          }
        ]
      },
      {
        "id" : "MedicationDispense.modifierExtension:stopType.value[x]",
        "path" : "MedicationDispense.modifierExtension.value[x]",
        "short" : "AdministrationAgreementStopType",
        "alias" : ["ToedieningsafspraakStopType"],
        "mapping" : [
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.22498",
            "comment" : "AdministrationAgreementStopType [DEPRECATED]"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-340",
            "comment" : "AdministrationAgreementStopType"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-340",
            "comment" : "AdministrationAgreementStopType"
          }
        ]
      },
      {
        "id" : "MedicationDispense.modifierExtension:repeatPeriodCyclicalSchedule",
        "path" : "MedicationDispense.modifierExtension",
        "sliceName" : "repeatPeriodCyclicalSchedule",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-InstructionsForUse.RepeatPeriodCyclicalSchedule"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.modifierExtension:repeatPeriodCyclicalSchedule.value[x]",
        "path" : "MedicationDispense.modifierExtension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.22505",
            "comment" : "RepeatPeriodCyclicalSchedule"
          }
        ]
      },
      {
        "id" : "MedicationDispense.identifier",
        "path" : "MedicationDispense.identifier",
        "short" : "Identification",
        "alias" : ["Identificatie"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-344",
            "comment" : "Identification"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-344",
            "comment" : "Identification"
          }
        ]
      },
      {
        "id" : "MedicationDispense.status",
        "path" : "MedicationDispense.status",
        "definition" : "A code specifying the state of the set of dispense events. In the event of an error correction, the value is set to _entered-in-error_.",
        "comment" : "The AdministrationAgreement building block does not provide much information on the logistical status as is intended by the ValueSet binding on this element. Therefore, if a system is unable to infer the status, `.status` will usually be set to _unknown_.",
        "mapping" : [
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.23034",
            "comment" : "CanceledIndicator [DEPRECATED]"
          },
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.22660",
            "comment" : "PeriodOfUse (implicit, main mapping is on the extensions ext-TimeInterval.Period and ext-TimeInterval.Duration) [DEPRECATED]"
          },
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.22498",
            "comment" : "AdministrationAgreementStopType (implicit, main mapping is on the modifier extension ext-StopType) [DEPRECATED]"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-340",
            "comment" : "AdministrationAgreementStopType (implicit, main mapping is on the modifier extension ext-StopType)"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-340",
            "comment" : "AdministrationAgreementStopType (implicit, main mapping is on the modifier extension ext-StopType)"
          }
        ]
      },
      {
        "id" : "MedicationDispense.category",
        "path" : "MedicationDispense.category",
        "min" : 1,
        "patternCodeableConcept" : {
          "coding" : [
            {
              "system" : "http://snomed.info/sct",
              "code" : "422037009"
            }
          ]
        }
      },
      {
        "id" : "MedicationDispense.category.extension:additionalCategory",
        "path" : "MedicationDispense.category.extension",
        "sliceName" : "additionalCategory",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-AdditionalCategory"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.category.extension:additionalCategory.value[x]",
        "path" : "MedicationDispense.category.extension.value[x]",
        "short" : "Type of medication dispense",
        "definition" : "Indicates the type of medication dispense (for example, where the medication is expected to be consumed or administered (i.e. inpatient or outpatient))",
        "binding" : {
          "strength" : "preferred",
          "valueSet" : "http://hl7.org/fhir/ValueSet/medicationdispense-category"
        }
      },
      {
        "id" : "MedicationDispense.medication[x]",
        "path" : "MedicationDispense.medication[x]",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "type",
              "path" : "$this"
            }
          ],
          "rules" : "open"
        }
      },
      {
        "id" : "MedicationDispense.medication[x]:medicationReference",
        "path" : "MedicationDispense.medication[x]",
        "sliceName" : "medicationReference",
        "short" : "MedicineForAdministrationAgreement",
        "definition" : "Medicine in the AdministrationAgreement.",
        "alias" : ["GeneesmiddelBijToedieningsafspraak"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Medication",
              "http://nictiz.nl/fhir/StructureDefinition/mp-PharmaceuticalProduct"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.20237",
            "comment" : "MedicineForAdministrationAgreement"
          }
        ]
      },
      {
        "id" : "MedicationDispense.subject",
        "path" : "MedicationDispense.subject",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Patient",
              "http://hl7.org/fhir/StructureDefinition/Group",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-Patient"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.performer",
        "path" : "MedicationDispense.performer",
        "max" : "1"
      },
      {
        "id" : "MedicationDispense.performer.actor",
        "path" : "MedicationDispense.performer.actor",
        "short" : "Supplier",
        "definition" : "The supplier (pharmacist) that entered the administration agreement.",
        "comment" : "The 'Supplier' concept of zib AdministrationAgreement is mapped to both `.performer.actor` and `.location`. This is a Reference to an instance of nl-core-HealthcareProvider-Organization instead of to an instance of nl-core-HealthcareProfessional, because individuals who enter the administration agreement are not recorded.",
        "alias" : ["Verstrekker"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Practitioner",
              "http://hl7.org/fhir/StructureDefinition/PractitionerRole",
              "http://hl7.org/fhir/StructureDefinition/Organization",
              "http://hl7.org/fhir/StructureDefinition/Patient",
              "http://hl7.org/fhir/StructureDefinition/Device",
              "http://hl7.org/fhir/StructureDefinition/RelatedPerson",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthcareProvider-Organization"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.22097",
            "comment" : "Supplier"
          }
        ]
      },
      {
        "id" : "MedicationDispense.location",
        "path" : "MedicationDispense.location",
        "short" : "Supplier",
        "definition" : "The supplier (pharmacist) that entered the administration agreement.",
        "comment" : "The 'Supplier' concept of zib AdministrationAgreement is mapped to both `.performer.actor` and `.location`. Details of the physical location of the supplier of the administration agreement can be referenced here.",
        "alias" : ["Verstrekker"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Location",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthcareProvider"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.22097",
            "comment" : "Supplier"
          }
        ]
      },
      {
        "id" : "MedicationDispense.authorizingPrescription",
        "path" : "MedicationDispense.authorizingPrescription",
        "short" : "MedicationAgreement",
        "definition" : "Relationship to the medication agreement on which the administration agreement is based.",
        "alias" : ["Medicatieafspraak"],
        "max" : "1",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/MedicationRequest",
              "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationAgreement"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.22394",
            "comment" : "MedicationAgreement"
          }
        ]
      },
      {
        "id" : "MedicationDispense.note",
        "path" : "MedicationDispense.note",
        "max" : "1"
      },
      {
        "id" : "MedicationDispense.note.text",
        "path" : "MedicationDispense.note.text",
        "short" : "Comment",
        "definition" : "Comments on the administration agreement.",
        "alias" : ["Toelichting"],
        "mapping" : [
          {
            "identity" : "zib-administrationagreement-v1.0.3-2020EN",
            "map" : "NL-CM:9.8.22275",
            "comment" : "Comment"
          }
        ]
      },
      {
        "id" : "MedicationDispense.dosageInstruction",
        "path" : "MedicationDispense.dosageInstruction",
        "short" : "DosingInstructions / InstructionsForUse",
        "definition" : "Instructions for administering the medication, e.g. dose and route of administration.",
        "alias" : ["Gebruiksinstructie"],
        "type" : [
          {
            "code" : "Dosage",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-InstructionsForUse.DosageInstructions"
            ]
          }
        ]
      }
    ]
  }
}

```
