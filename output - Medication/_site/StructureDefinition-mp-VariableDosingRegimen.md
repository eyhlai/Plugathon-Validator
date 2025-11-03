# mp VariableDosingRegimen - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp VariableDosingRegimen**

## Resource Profile: mp VariableDosingRegimen 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-VariableDosingRegimen | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpVariableDosingRegimen |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
The variable-dosing regimen contains the dosing schedule as prescribed by the (external) prescriber to the patient (or his representative or administrator), specifying the instructions for use in addition to the medication agreement. The dosing schedule can be adjusted, while the medication agreement remains unchanged. 

 
This MedicationRequest resource represents the VariableDosingRegimen building block for implementations following the information standard[MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). The VariableDosingRegimen has a strong relationship with[mp-MedicationAgreement](http://nictiz.nl/fhir/StructureDefinition/mp-MedicationAgreement). This VariableDosingRegimen profile describes (additional) instructions for MedicationAgreements and is used when it is expected that the MedicationAgreement instructions will need to be adjusted frequently. By separating this into two resources, the original MedicationAgreement does not have to be adjusted as often. 
Unfortunately, a derived profile can not be made because of a fixed and mandatory`.category`code. Also, some concepts are not used. This profile reuses extensions made for the MedicationAgreement. 

**Usages:**

* Refer to this Profile: [mp MedicationAdministration2](StructureDefinition-mp-MedicationAdministration2.md) and [mp VariableDosingRegimen](StructureDefinition-mp-VariableDosingRegimen.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-VariableDosingRegimen)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-VariableDosingRegimen.csv), [Excel](StructureDefinition-mp-VariableDosingRegimen.xlsx), [Schematron](StructureDefinition-mp-VariableDosingRegimen.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-VariableDosingRegimen",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-VariableDosingRegimen",
  "version" : "0.1.0",
  "name" : "MpVariableDosingRegimen",
  "title" : "mp VariableDosingRegimen",
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
  "description" : "The variable-dosing regimen contains the dosing schedule as prescribed by the (external) prescriber to the patient (or his representative or administrator), specifying the instructions for use in addition to the medication agreement. The dosing schedule can be adjusted, while the medication agreement remains unchanged.",
  "purpose" : "This MedicationRequest resource represents the VariableDosingRegimen building block for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). The VariableDosingRegimen has a strong relationship with [mp-MedicationAgreement](http://nictiz.nl/fhir/StructureDefinition/mp-MedicationAgreement). This VariableDosingRegimen profile describes (additional) instructions for MedicationAgreements and is used when it is expected that the MedicationAgreement instructions will need to be adjusted frequently. By separating this into two resources, the original MedicationAgreement does not have to be adjusted as often.  \n\nUnfortunately, a derived profile can not be made because of a fixed and mandatory `.category` code. Also, some concepts are not used. This profile reuses extensions made for the MedicationAgreement.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
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
        "short" : "VariableDosingRegimen",
        "alias" : ["WisselendDoseerschema"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-632",
            "comment" : "VariableDosingRegimen"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-632",
            "comment" : "VariableDosingRegimen"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-646",
            "comment" : "InstructionsForUse"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-646",
            "comment" : "InstructionsForUse"
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
            "map" : "mp-dataelement9x-1343",
            "comment" : "RelationEpisodeOfCare"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1343",
            "comment" : "RelationEpisodeOfCare"
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
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-647",
            "comment" : "Description"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-647",
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
        "definition" : "**Start date**: This is the time at which the agreement was to take effect (or took effect or will take effect). This is the time at which the instructions for use in this agreement start. In the case of an agreement to discontinue use, this is the start date of the original medication agreement. The end date indicates from when the medication is to be discontinued.\r\n\r\n**End date**: The time at which the period of use ends (or ended or will end). In the case of an agreement to discontinue use, this is the time at which the medication is to be discontinued. To avoid confusion between 'to' and 'up to', the submission of time is always mandatory for the end date.\r\n\r\nWith medication for an indefinite period only a start date is indicated.",
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
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-635",
            "comment" : "PeriodOfUse"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-635",
            "comment" : "PeriodOfUse"
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
        "definition" : "The date and time when the VariableDosingRegimen was recorded. RegistrationDateTime is used to accurately determine the chronological order of agreements. Therefore, the date and time are mandatory. These values are immutable. When consulting or receiving this VariableDosingRegimen, the original RegistrationDateTime remains unchanged.\n\nNote: This data element differs from the data element RegistrationDateTime in zib RegistratieGegevens-v1.1.1 (2024NL). In zib RegistratieGegevens-v1.1.1 (2024NL), RegistrationDateTime refers to the date and time when the data was recorded. This may be the initial registration or the date and time when data was transferred. The zib concept RegistrationDateTime is not applied in MP9.",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1483",
            "comment" : "RegistrationDateTime"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1483",
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
        "short" : "VariableDosingRegimenStopType",
        "alias" : ["WisselendDoseerschemaStopType"],
        "binding" : {
          "strength" : "required",
          "description" : "WisselendDoseerschemaStopTypeCodelijst restricts StopType values, based on the ValueSet StopTypeCodelijst, which are applicable for StopType in MedicationAgreement and AdministrationAgreement.",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.48--20230112155455"
        },
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1171",
            "comment" : "VariableDosingRegimenStopType"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1171",
            "comment" : "VariableDosingRegimenStopType"
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
        "definition" : "Identification of the variable-dosing regimen. This is generated by the system of the prescriber and is globally unique and eternally persistent.",
        "alias" : ["Identificatie"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-633",
            "comment" : "Identification"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-633",
            "comment" : "Identification"
          }
        ]
      },
      {
        "id" : "MedicationRequest.status",
        "path" : "MedicationRequest.status",
        "comment" : "This element is implictly mapped to the concepts mp-dataelement9x-635 (PeriodOfUse) and mp-dataelement9x-1171 (VariableDosingRegimenStopType).\r\nUnless the status is explicitly recorded, the following guidance applies:\r\n\r\n* When the value of PeriodOfUse.startDateTime is in the past and PeriodOfUse.endDateTime exists and its value is in the future, `.status` will usually be set to _active_.\r\n* When the value of PeriodOfUse.startDateTime is in the future, `.status` will usually be set to _active_.\r\n* When PeriodOfUse.endDateTime exists and its value is in the past and VariableDosingRegimenStopType has no value, `.status` will usually be set to _completed_.\r\n* When PeriodOfUse.endDateTime exists and its value is in the past and the value of VariableDosingRegimenStopType is _410546004_, `.status` will usually be set to _stopped_.\r\n* When PeriodOfUse.Duration and PeriodOfUse.startDateTime are known, PeriodOfUse.endDateTime can be deduced and the previous rules apply. \r\n* When a system is unable to infer the status, `.status` will be set to _unknown_. The _unknown_ code is not to be used to convey other statuses. The _unknown_ code should be used when one of the statuses applies, but the authoring system doesn't know the current state of the VariableDosingRegimen.",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-635",
            "comment" : "PeriodOfUse (implicit, main mapping is on the extensions ext-TimeInterval.Period and ext-TimeInterval.Duration)"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-635",
            "comment" : "PeriodOfUse (implicit, main mapping is on the extensions ext-TimeInterval.Period and ext-TimeInterval.Duration)"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1171",
            "comment" : "VariableDosingRegimenStopType (implicit, main mapping is on the modifier extension ext-StopType)"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1171",
            "comment" : "VariableDosingRegimenStopType (implicit, main mapping is on the modifier extension ext-StopType)"
          }
        ]
      },
      {
        "id" : "MedicationRequest.intent",
        "path" : "MedicationRequest.intent",
        "definition" : "Unless `.intent` is explicitly recorded and a more appropriate code is known, the value can be set to _order_ because a VariableDosingRegimen should authorize an action for a patient, pharmacist, professional administrator et cetera."
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
        "id" : "MedicationRequest.category:variableDosingRegimenCode",
        "path" : "MedicationRequest.category",
        "sliceName" : "variableDosingRegimenCode",
        "min" : 1,
        "max" : "1",
        "patternCodeableConcept" : {
          "coding" : [
            {
              "system" : "http://snomed.info/sct",
              "code" : "395067002"
            }
          ]
        }
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
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1362",
            "comment" : "AgreedMedicine"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1362",
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
            "map" : "mp-dataelement9x-1341",
            "comment" : "RelationEncounter"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1341",
            "comment" : "RelationEncounter"
          }
        ]
      },
      {
        "id" : "MedicationRequest.authoredOn",
        "path" : "MedicationRequest.authoredOn",
        "short" : "VariableDosingRegimenDateTime",
        "definition" : "Date and time the variable-dosing regimen was created. Appointment date + time are required (order of the appointments must be clear in cases with multiple appointments on one day).",
        "alias" : ["WisselendDoseerschemaDatumTijd"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-634",
            "comment" : "VariableDosingRegimenDateTime"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-634",
            "comment" : "VariableDosingRegimenDateTime"
          }
        ]
      },
      {
        "id" : "MedicationRequest.requester",
        "path" : "MedicationRequest.requester",
        "short" : "Author",
        "definition" : "Author who entered the variable-dosing regimen.",
        "alias" : ["Auteur"],
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
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-642",
            "comment" : "Author"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-642",
            "comment" : "Author"
          }
        ]
      },
      {
        "id" : "MedicationRequest.reasonCode",
        "path" : "MedicationRequest.reasonCode",
        "short" : "ReasonModificationOrDiscontinuation",
        "definition" : "Reason for this agreement. This can be the reason to start, change or stop the medication treatment.",
        "alias" : ["RedenWijzigenOfStaken"],
        "max" : "1",
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.54--20221114181621"
        },
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-639",
            "comment" : "ReasonModificationOrDiscontinuation"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-639",
            "comment" : "ReasonModificationOrDiscontinuation"
          }
        ]
      },
      {
        "id" : "MedicationRequest.basedOn",
        "path" : "MedicationRequest.basedOn",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "profile",
              "path" : "resolve()"
            }
          ],
          "rules" : "open"
        }
      },
      {
        "id" : "MedicationRequest.basedOn:relationMedicationAgreement",
        "path" : "MedicationRequest.basedOn",
        "sliceName" : "relationMedicationAgreement",
        "short" : "RelationMedicationAgreement",
        "definition" : "Relation to the medication agreement which is specified in this dosing schedule.",
        "alias" : ["RelatieMedicatieafspraak"],
        "max" : "1",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationAgreement"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-640",
            "comment" : "RelationMedicationAgreement"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-640",
            "comment" : "RelationMedicationAgreement"
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
        "definition" : "Comments on the variable-dosing regimen.",
        "alias" : ["Toelichting"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-694",
            "comment" : "Comment"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-694",
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
        "short" : "RelationVariableDosingRegimen",
        "definition" : "Relation to the previous version of the dosing schedule.",
        "alias" : ["RelatieWisselendDoseerschema"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/MedicationRequest",
              "http://nictiz.nl/fhir/StructureDefinition/mp-VariableDosingRegimen"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1319",
            "comment" : "RelationVariableDosingRegimen"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1319",
            "comment" : "RelationVariableDosingRegimen"
          }
        ]
      }
    ]
  }
}

```
