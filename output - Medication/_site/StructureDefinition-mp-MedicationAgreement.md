# mp MedicationAgreement - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp MedicationAgreement**

## Resource Profile: mp MedicationAgreement 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-MedicationAgreement | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpMedicationAgreement |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
A medication agreement is a prescriber’s proposal for a patient to use medication. An agreement to discontinue the use of medication is also a medication agreement. 

 
This MedicationRequest resource represents the MedicationAgreement building block for implementations following the information standard[MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) MedicationAgreement, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set. 

**Usages:**

* Use this Profile: [mp MedicationPrescription Bundle](StructureDefinition-mp-MedicationPrescription-Bundle.md) and [mp ProposalMedicationAgreement Bundle](StructureDefinition-mp-ProposalMedicationAgreement-Bundle.md)
* Refer to this Profile: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md), [mp DispenseRequest](StructureDefinition-mp-DispenseRequest.md), [mp MedicationAdministration2](StructureDefinition-mp-MedicationAdministration2.md), [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md)...Show 4 more,[mp MedicationOverview](StructureDefinition-mp-MedicationOverview.md),[mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md),[mp ReplyProposalMedicationAgreement](StructureDefinition-mp-ReplyProposalMedicationAgreement.md)and[mp VariableDosingRegimen](StructureDefinition-mp-VariableDosingRegimen.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-MedicationAgreement)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-MedicationAgreement.csv), [Excel](StructureDefinition-mp-MedicationAgreement.xlsx), [Schematron](StructureDefinition-mp-MedicationAgreement.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-MedicationAgreement",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationAgreement",
  "version" : "0.1.0",
  "name" : "MpMedicationAgreement",
  "title" : "mp MedicationAgreement",
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
  "description" : "A medication agreement is a prescriber’s proposal for a patient to use medication. An agreement to discontinue the use of medication is also a medication agreement.",
  "purpose" : "This MedicationRequest resource represents the MedicationAgreement building block for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) MedicationAgreement, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "zib-medicationagreement-v1.2-2020EN",
      "uri" : "https://zibs.nl/wiki/MedicationAgreement-v1.2(2020EN)",
      "name" : "zib MedicationAgreement-v1.2(2020EN)"
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
      "identity" : "script10.6",
      "uri" : "http://ncpdp.org/SCRIPT10_6",
      "name" : "Mapping to NCPDP SCRIPT 10.6"
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
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "MedicationRequest",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/MedicationRequest",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "MedicationRequest",
        "path" : "MedicationRequest",
        "short" : "MedicationAgreement",
        "alias" : ["Medicatieafspraak"],
        "mapping" : [
          {
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.9580",
            "comment" : "MedicationAgreement"
          },
          {
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.23240",
            "comment" : "InstructionsForUse"
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:medicationAgreementAdditionalInformation",
        "path" : "MedicationRequest.extension",
        "sliceName" : "medicationAgreementAdditionalInformation",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAgreement.MedicationAgreementAdditionalInformation"
            ]
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:medicationAgreementAdditionalInformation.value[x]",
        "path" : "MedicationRequest.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-90",
            "comment" : "MedicationAgreementAdditionalInformation"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-90",
            "comment" : "MedicationAgreementAdditionalInformation"
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:renderedDosageInstruction",
        "path" : "MedicationRequest.extension",
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
        "id" : "MedicationRequest.extension:renderedDosageInstruction.value[x]",
        "path" : "MedicationRequest.extension.value[x]",
        "short" : "Description",
        "definition" : "Textual description of the complete instructions for use.",
        "alias" : ["Omschrijving"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.9581",
            "comment" : "Description"
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:periodOfUse",
        "path" : "MedicationRequest.extension",
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
        "id" : "MedicationRequest.extension:periodOfUse.value[x]",
        "path" : "MedicationRequest.extension.value[x]",
        "short" : "PeriodOfUse",
        "definition" : "**Start date**: This is the time at which the agreement was to take effect (or took effect or will take effect). This is the time at which the instructions for use in this agreement start. In the case of an agreement to discontinue use, this is the start date of the original medication agreement. The end date indicates from when the medication is to be discontinued.\r\n\r\n**Duration**: The intended duration of use. E.g. 5 days or 8 weeks. It is not allowed to indicate the duration in months, because different months have a variable duration in days.\r\n\r\n**End date**: The time at which the period of use ends (or ended or will end). In the case of an agreement to discontinue use, this is the time at which the medication is to be discontinued. To avoid confusion between 'to' and 'up to', the submission of time is always mandatory for the end date.\r\n\r\nWith medication for an indefinite period only a start date is indicated.",
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
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.19936",
            "comment" : "PeriodOfUse"
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:periodOfUse.value[x].extension:condition",
        "path" : "MedicationRequest.extension.value[x].extension",
        "sliceName" : "condition",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-PeriodOfUse.Condition"
            ]
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:periodOfUse.value[x].extension:condition.value[x]",
        "path" : "MedicationRequest.extension.value[x].extension.value[x]",
        "definition" : "Element to indicate that the start or end date is uncertain.\r\n\r\nIn certain situations the start or end date can depend on another piece of information. This is, for example, the case when a patient has to start or stop medication a few days before hospital admission. In that case this element is used to indicate (in free text): ‘start X days before hospital admission’ or ‘stop X days before hospital admission’. By doing this, it is clear that the entered start or end date is uncertain when the MedicationAgreement is being exchanged.",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1365"
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:pharmaceuticalTreatmentIdentifier",
        "path" : "MedicationRequest.extension",
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
        "id" : "MedicationRequest.extension:pharmaceuticalTreatmentIdentifier.value[x]",
        "path" : "MedicationRequest.extension.value[x]",
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
        "id" : "MedicationRequest.extension:relationEpisodeOfCare",
        "path" : "MedicationRequest.extension",
        "sliceName" : "relationEpisodeOfCare",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-Context-EpisodeOfCare"
            ]
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:relationEpisodeOfCare.value[x]",
        "path" : "MedicationRequest.extension.value[x]",
        "short" : "RelationEpisodeOfCare",
        "alias" : ["RelatieZorgepisode"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-843",
            "comment" : "RelationEpisodeOfCare"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-843",
            "comment" : "RelationEpisodeOfCare"
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:nextPractitioner",
        "path" : "MedicationRequest.extension",
        "sliceName" : "nextPractitioner",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAgreement.NextPractitioner"
            ]
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:nextPractitioner.value[x]",
        "path" : "MedicationRequest.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1382",
            "comment" : "NextPractitioner"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1382",
            "comment" : "NextPractitioner"
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:registrationDateTime",
        "path" : "MedicationRequest.extension",
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
        "id" : "MedicationRequest.extension:registrationDateTime.value[x]",
        "path" : "MedicationRequest.extension.value[x]",
        "definition" : "The date and time when the MedicationAgreement was recorded. RegistrationDateTime is used to accurately determine the chronological order of agreements. Therefore, the date and time are mandatory. These values are immutable. When consulting or receiving this MedicationAgreement, the original RegistrationDateTime remains unchanged.\n\nNote: This data element differs from the data element RegistrationDateTime in zib RegistratieGegevens-v1.1.1 (2024NL). In zib RegistratieGegevens-v1.1.1 (2024NL), RegistrationDateTime refers to the date and time when the data was recorded. This may be the initial registration or the date and time when data was transferred. The zib concept RegistrationDateTime is not applied in MP9.",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1480",
            "comment" : "RegistrationDateTime"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1480",
            "comment" : "RegistrationDateTime"
          }
        ]
      },
      {
        "id" : "MedicationRequest.modifierExtension:stopType",
        "path" : "MedicationRequest.modifierExtension",
        "sliceName" : "stopType",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://nictiz.nl/fhir/StructureDefinition/ext-StopType"]
          }
        ]
      },
      {
        "id" : "MedicationRequest.modifierExtension:stopType.value[x]",
        "path" : "MedicationRequest.modifierExtension.value[x]",
        "short" : "MedicationAgreementStopType",
        "alias" : ["MedicatieafspraakStopType"],
        "mapping" : [
          {
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.19954",
            "comment" : "MedicationAgreementStopType [DEPRECATED]"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-88",
            "comment" : "MedicationAgreementStopType"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-88",
            "comment" : "MedicationAgreementStopType"
          }
        ]
      },
      {
        "id" : "MedicationRequest.modifierExtension:repeatPeriodCyclicalSchedule",
        "path" : "MedicationRequest.modifierExtension",
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
        "id" : "MedicationRequest.modifierExtension:repeatPeriodCyclicalSchedule.value[x]",
        "path" : "MedicationRequest.modifierExtension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.22505",
            "comment" : "RepeatPeriodCyclicalSchedule"
          }
        ]
      },
      {
        "id" : "MedicationRequest.identifier",
        "path" : "MedicationRequest.identifier",
        "short" : "Identification",
        "alias" : ["Identificatie"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-194",
            "comment" : "Identification"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-194",
            "comment" : "Identification"
          }
        ]
      },
      {
        "id" : "MedicationRequest.status",
        "path" : "MedicationRequest.status",
        "comment" : "This element is implictly mapped to the zib concept NL-CM:9.6.19936 (PeriodOfUse) and the concept mp-dataelement9x-88 (MedicationAgreementStopType).\r\nUnless the status is explicitly recorded, the following guidance applies:\r\n\r\n* When the value of PeriodOfUse.startDateTime is in the future, `.status` will usually be set to _active_.\r\n* When the value of PeriodOfUse.startDateTime is in the past and PeriodOfUse.endDateTime exists and its value is in the future, `.status` will usually be set to _active_.\r\n* When PeriodOfUse.endDateTime exists and its value is in the past and MedicationAgreementStopType has no value, `.status` will usually be set to _completed_.\r\n* When PeriodOfUse.endDateTime exists and its value is in the past and MedicationAgreementStopType is _385655000_, `.status` will usually be set to _on-hold_.\r\n* When PeriodOfUse.endDateTime exists and its value is in the past, and the value of MedicationAgreementStopType is _410546004_, `.status` will usually be set to _stopped_.\r\n* When the value of PeriodOfUse.startDateTime is in the future, the value of PeriodOfUse.endDateTime equals the value of PeriodOfUse.startDateTime and the value of MedicationAgreementStopType is _89925002_, `.status` will usually be set to _cancelled_.\r\n* When PeriodOfUse.Duration and PeriodOfUse.startDateTime are known, PeriodOfUse.endDateTime can be deduced and the previous rules apply. \r\n* When a system is unable to infer the status, `.status` will be set to _unknown_. The _unknown_ code is not to be used to convey other statuses. The _unknown_ code should be used when one of the statuses applies, but the authoring system doesn't know the current state of the MedicationAgreement.",
        "mapping" : [
          {
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.19936",
            "comment" : "PeriodOfUse (implicit, main mapping is on the extensions ext-TimeInterval.Period and ext-TimeInterval.Duration)"
          },
          {
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.19954",
            "comment" : "MedicationAgreementStopType (implicit, main mapping is on the modifier extension ext-StopType) [DEPRECATED]"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-88",
            "comment" : "MedicationAgreementStopType (implicit, main mapping is on the modifier extension ext-StopType)"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-88",
            "comment" : "MedicationAgreementStopType (implicit, main mapping is on the modifier extension ext-StopType)"
          }
        ]
      },
      {
        "id" : "MedicationRequest.intent",
        "path" : "MedicationRequest.intent",
        "definition" : "Unless `.intent` is explicitly recorded and a more appropriate code is known, the value can be set to _order_ because a MedicationAgreement should authorize an action for a patient, pharmacist, professional administrator et cetera."
      },
      {
        "id" : "MedicationRequest.category",
        "path" : "MedicationRequest.category",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "value",
              "path" : "$this"
            }
          ],
          "rules" : "open"
        },
        "min" : 1
      },
      {
        "id" : "MedicationRequest.category:medicationAgreementCode",
        "path" : "MedicationRequest.category",
        "sliceName" : "medicationAgreementCode",
        "min" : 1,
        "max" : "1",
        "patternCodeableConcept" : {
          "coding" : [
            {
              "system" : "http://snomed.info/sct",
              "code" : "33633005"
            }
          ]
        }
      },
      {
        "id" : "MedicationRequest.reported[x]",
        "path" : "MedicationRequest.reported[x]",
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
        "id" : "MedicationRequest.reported[x]:reportedBoolean",
        "path" : "MedicationRequest.reported[x]",
        "sliceName" : "reportedBoolean",
        "short" : "CopyIndicator",
        "definition" : "An indication whether the resource is original (false) or a copy from a different source (true).",
        "alias" : ["KopieIndicator"],
        "type" : [
          {
            "code" : "boolean"
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-273",
            "comment" : "CopyIndicator"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-273",
            "comment" : "CopyIndicator"
          }
        ]
      },
      {
        "id" : "MedicationRequest.medication[x]",
        "path" : "MedicationRequest.medication[x]",
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
        "id" : "MedicationRequest.medication[x]:medicationReference",
        "path" : "MedicationRequest.medication[x]",
        "sliceName" : "medicationReference",
        "short" : "AgreedMedicine",
        "definition" : "The medicine agreed upon to be used.",
        "alias" : ["AfgesprokenGeneesmiddel"],
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
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.19925",
            "comment" : "AgreedMedicine"
          }
        ]
      },
      {
        "id" : "MedicationRequest.subject",
        "path" : "MedicationRequest.subject",
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
        "id" : "MedicationRequest.encounter",
        "path" : "MedicationRequest.encounter",
        "short" : "RelationEncounter",
        "alias" : ["RelatieContact"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Encounter",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-Encounter"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-199",
            "comment" : "RelationEncounter"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-199",
            "comment" : "RelationEncounter"
          }
        ]
      },
      {
        "id" : "MedicationRequest.authoredOn",
        "path" : "MedicationRequest.authoredOn",
        "short" : "MedicationAgreementDateTime",
        "definition" : "The time at which the agreement was made. Appointment date + time are required (order of the appointments must be clear in cases with multiple appointments on one day)",
        "alias" : ["MedicatieafspraakDatumTijd"],
        "mapping" : [
          {
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.19757",
            "comment" : "MedicationAgreementDateTime"
          }
        ]
      },
      {
        "id" : "MedicationRequest.requester",
        "path" : "MedicationRequest.requester",
        "short" : "Prescriber",
        "definition" : "The health professional that entered the medication agreement with the patient.",
        "alias" : ["Voorschrijver"],
        "type" : [
          {
            "code" : "Reference",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-NlCoreHealthProfessionalReference"
            ],
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Practitioner",
              "http://hl7.org/fhir/StructureDefinition/PractitionerRole",
              "http://hl7.org/fhir/StructureDefinition/Organization",
              "http://hl7.org/fhir/StructureDefinition/Patient",
              "http://hl7.org/fhir/StructureDefinition/RelatedPerson",
              "http://hl7.org/fhir/StructureDefinition/Device",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthProfessional-PractitionerRole"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.1030",
            "comment" : "Prescriber"
          }
        ]
      },
      {
        "id" : "MedicationRequest.reasonCode",
        "path" : "MedicationRequest.reasonCode",
        "short" : "ReasonModificationOrDiscontinuation",
        "definition" : "Reason for modification or discontinuation of the medication agreement.",
        "alias" : ["RedenWijzigenOfStaken"],
        "max" : "1",
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.42--20221114132525"
        },
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-89",
            "comment" : "ReasonModificationOrDiscontinuation"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-89",
            "comment" : "ReasonModificationOrDiscontinuation"
          }
        ]
      },
      {
        "id" : "MedicationRequest.reasonReference",
        "path" : "MedicationRequest.reasonReference",
        "short" : "PrescriptionReason",
        "definition" : "The medical reason for the prescription or for use of the medication. This can be used to enter a medical indication which was the direct cause for prescription or for use of the medication in question. \r\nIt can concern every type of problem (or condition) of the patient, almost all diagnoses, complaints or symptoms. Please note: The BST401T file of the G standard contains a “special reference” to indicate that “exchange of the reason for prescription is essential”.",
        "alias" : ["RedenVanVoorschrijven"],
        "max" : "1",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Condition",
              "http://hl7.org/fhir/StructureDefinition/Observation",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-Problem"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.23133",
            "comment" : "PrescriptionReason"
          }
        ]
      },
      {
        "id" : "MedicationRequest.basedOn.extension:relationAdministrationAgreement",
        "path" : "MedicationRequest.basedOn.extension",
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
        "id" : "MedicationRequest.basedOn.extension:relationAdministrationAgreement.value[x]",
        "path" : "MedicationRequest.basedOn.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1328",
            "comment" : "RelationAdministrationAgreement"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1328",
            "comment" : "RelationAdministrationAgreement"
          }
        ]
      },
      {
        "id" : "MedicationRequest.basedOn.extension:relationMedicationUse",
        "path" : "MedicationRequest.basedOn.extension",
        "sliceName" : "relationMedicationUse",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAgreement.RelationMedicationUse"
            ]
          }
        ]
      },
      {
        "id" : "MedicationRequest.basedOn.extension:relationMedicationUse.value[x]",
        "path" : "MedicationRequest.basedOn.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1327",
            "comment" : "RelationMedicationUse"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1327",
            "comment" : "RelationMedicationUse"
          }
        ]
      },
      {
        "id" : "MedicationRequest.note",
        "path" : "MedicationRequest.note",
        "max" : "1"
      },
      {
        "id" : "MedicationRequest.note.text",
        "path" : "MedicationRequest.note.text",
        "short" : "Comment",
        "definition" : "Comments regarding to the medication agreement. For example: in consultation with the medical specialist.",
        "alias" : ["Toelichting"],
        "mapping" : [
          {
            "identity" : "zib-medicationagreement-v1.2-2020EN",
            "map" : "NL-CM:9.6.22273",
            "comment" : "Comment"
          }
        ]
      },
      {
        "id" : "MedicationRequest.dosageInstruction",
        "path" : "MedicationRequest.dosageInstruction",
        "short" : "DosingInstructions / InstructionsForUse",
        "definition" : "Instructions for the use of the medication, e.g. dose and route of administration.",
        "alias" : ["Gebruiksinstructie"],
        "type" : [
          {
            "code" : "Dosage",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-InstructionsForUse.DosageInstructions"
            ]
          }
        ]
      },
      {
        "id" : "MedicationRequest.priorPrescription",
        "path" : "MedicationRequest.priorPrescription",
        "short" : "RelationMedicationAgreement",
        "definition" : "A link to a medication agreement that is altered or canceled.",
        "alias" : ["RelatieMedicatieafspraak"],
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
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-195",
            "comment" : "RelationMedicationAgreement"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-195",
            "comment" : "RelationMedicationAgreement"
          }
        ]
      }
    ]
  }
}

```
