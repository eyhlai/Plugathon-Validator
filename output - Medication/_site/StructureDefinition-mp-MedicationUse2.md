# mp MedicationUse2 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp MedicationUse2**

## Resource Profile: mp MedicationUse2 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-MedicationUse2 | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpMedicationUse2 |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
MedicationUse2 is a statement on the historic, current or intended use of a certain medicine. 

 
This MedicationStatement resource represents the MedicationUse2 building block for implementations following the information standard[MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) PharmaceuticalProduct, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set. 

**Usages:**

* Refer to this Profile: [ext MedicationAgreement.RelationMedicationUse](StructureDefinition-ext-MedicationAgreement.RelationMedicationUse.md) and [mp MedicationOverview](StructureDefinition-mp-MedicationOverview.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-MedicationUse2)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-MedicationUse2.csv), [Excel](StructureDefinition-mp-MedicationUse2.xlsx), [Schematron](StructureDefinition-mp-MedicationUse2.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-MedicationUse2",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationUse2",
  "version" : "0.1.0",
  "name" : "MpMedicationUse2",
  "title" : "mp MedicationUse2",
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
  "description" : "MedicationUse2 is a statement on the historic, current or intended use of a certain medicine.",
  "purpose" : "This MedicationStatement resource represents the MedicationUse2 building block for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) PharmaceuticalProduct, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "zib-medicationuse2-v1.1.1-2020EN",
      "uri" : "https://zibs.nl/wiki/MedicationUse2-v1.1.1(2020EN)",
      "name" : "zib MedicationUse2-v1.1.1(2020EN)"
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
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "MedicationStatement",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/MedicationStatement",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "MedicationStatement",
        "path" : "MedicationStatement",
        "short" : "MedicationUse",
        "comment" : "The original comment on MedicationStatement present in FHIR R4 is incorrect and should not be taken into account while interpreting this profile (that comment has been removed in later FHIR releases).",
        "alias" : ["Medicatiegebruik"],
        "mapping" : [
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.21338",
            "comment" : "MedicationUse"
          },
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.22504",
            "comment" : "InstructionsForUse"
          }
        ]
      },
      {
        "id" : "MedicationStatement.extension:renderedDosageInstruction",
        "path" : "MedicationStatement.extension",
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
        "id" : "MedicationStatement.extension:renderedDosageInstruction.value[x]",
        "path" : "MedicationStatement.extension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.9581",
            "comment" : "Description"
          }
        ]
      },
      {
        "id" : "MedicationStatement.extension:prescriber",
        "path" : "MedicationStatement.extension",
        "sliceName" : "prescriber",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationUse2.Prescriber"
            ]
          }
        ]
      },
      {
        "id" : "MedicationStatement.extension:prescriber.value[x]",
        "path" : "MedicationStatement.extension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.23290",
            "comment" : "Prescriber"
          }
        ]
      },
      {
        "id" : "MedicationStatement.extension:asAgreedIndicator",
        "path" : "MedicationStatement.extension",
        "sliceName" : "asAgreedIndicator",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-AsAgreedIndicator"
            ]
          }
        ]
      },
      {
        "id" : "MedicationStatement.extension:asAgreedIndicator.value[x]",
        "path" : "MedicationStatement.extension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.22492",
            "comment" : "AsAgreedIndicator"
          }
        ]
      },
      {
        "id" : "MedicationStatement.extension:pharmaceuticalTreatmentIdentifier",
        "path" : "MedicationStatement.extension",
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
        "id" : "MedicationStatement.extension:pharmaceuticalTreatmentIdentifier.value[x]",
        "path" : "MedicationStatement.extension.value[x]",
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
        "id" : "MedicationStatement.extension:copyIndicator",
        "path" : "MedicationStatement.extension",
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
        "id" : "MedicationStatement.extension:copyIndicator.value[x]",
        "path" : "MedicationStatement.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-418",
            "comment" : "CopyIndicator"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-418",
            "comment" : "CopyIndicator"
          }
        ]
      },
      {
        "id" : "MedicationStatement.extension:author",
        "path" : "MedicationStatement.extension",
        "sliceName" : "author",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationUse2.Author"
            ]
          }
        ]
      },
      {
        "id" : "MedicationStatement.extension:author.value[x]",
        "path" : "MedicationStatement.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-623",
            "comment" : "Author"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-623",
            "comment" : "Author"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-624",
            "comment" : "AuthorIsHealthcareProvider"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-624",
            "comment" : "AuthorIsHealthcareProvider"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-626",
            "comment" : "AuthorIsPatient (implicit; AuthorIsPatient = true when this element refers to the same Patient as subject)"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-626",
            "comment" : "AuthorIsPatient (implicit; AuthorIsPatient = true when this element refers to the same Patient as subject)"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-627",
            "comment" : "AuthorIsHealthProfessional"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-627",
            "comment" : "AuthorIsHealthProfessional"
          }
        ]
      },
      {
        "id" : "MedicationStatement.modifierExtension:stopType",
        "path" : "MedicationStatement.modifierExtension",
        "sliceName" : "stopType",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://nictiz.nl/fhir/StructureDefinition/ext-StopType"]
          }
        ]
      },
      {
        "id" : "MedicationStatement.modifierExtension:stopType.value[x]",
        "path" : "MedicationStatement.modifierExtension.value[x]",
        "short" : "MedicationUseStopType",
        "alias" : ["MedicatiegebruikStopType"],
        "binding" : {
          "strength" : "required",
          "description" : "MedicatiegebruikStopTypeCodelijst restricts StopType values, based on the ValueSet StopTypeCodelijst, which are applicable for StopType in MedicationAgreement and AdministrationAgreement.",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.55--20230119145802"
        },
        "mapping" : [
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.23132",
            "comment" : "MedicationUseStopType [DEPRECATED]"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-408",
            "comment" : "MedicationUseStopType"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-408",
            "comment" : "MedicationUseStopType"
          }
        ]
      },
      {
        "id" : "MedicationStatement.modifierExtension:repeatPeriodCyclicalSchedule",
        "path" : "MedicationStatement.modifierExtension",
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
        "id" : "MedicationStatement.modifierExtension:repeatPeriodCyclicalSchedule.value[x]",
        "path" : "MedicationStatement.modifierExtension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.22505",
            "comment" : "RepeatPeriodCyclicalSchedule"
          }
        ]
      },
      {
        "id" : "MedicationStatement.identifier",
        "path" : "MedicationStatement.identifier",
        "short" : "Identification",
        "alias" : ["Identificatie"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-411",
            "comment" : "Identification"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-411",
            "comment" : "Identification"
          }
        ]
      },
      {
        "id" : "MedicationStatement.status",
        "path" : "MedicationStatement.status",
        "short" : "UseIndicator",
        "definition" : "Status may contain information on the stop type, the manner in which this medication is discontinued (temporary or definitive) and if the medicine is used or not.",
        "comment" : "This element is mapped to the zib concept NL-CM:9.11.22399 (UseIndicator), and is moreover implicitly mapped to NL-CM:9.11.22663 (PeriodOfUse) and mp-dataelement9x-408 (MedicationUseStopType).\r\nUnless the status is explicitly recorded, the following guidance applies:\r\n\r\n* When the value of MedicationUseStopType is _385655000_, `.status` will usually be set to _on-hold_.\r\n* When the value of MedicationUseStopType is _410546004_, `.status` will usually be set to _stopped_.\r\n* When the value of UseIndicator is _false_ and MedicationUseStopType is empty, `.status` will be set to _not-taken_.\r\n* When PeriodOfUse is empty, `.status` will usually be set to _unknown_.\r\n* In all other cases, `.status` will usually be set to _active_. Note that this simplifed representation of `.status` (not taking into account the actual values of PeriodOfUse or the value of MedicationUseDateTime) pre-adopts the use of `.status` in the current R5 build of the MedicationStatement resource type.",
        "alias" : ["GebruikIndicator"],
        "mapping" : [
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.22399",
            "comment" : "UseIndicator"
          },
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.22663",
            "comment" : "PeriodOfUse (implicit, main mapping is on `.effective[x]:effectivePeriod` and extension ext-TimeInterval.Duration)"
          },
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.23132",
            "comment" : "MedicationUseStopType (implicit, main mapping is on the modifier extension ext-StopType) [DEPRECATED]"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-408",
            "comment" : "MedicationUseStopType (implicit, main mapping is on the modifier extension ext-StopType)"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-408",
            "comment" : "MedicationUseStopType (implicit, main mapping is on the modifier extension ext-StopType)"
          }
        ]
      },
      {
        "id" : "MedicationStatement.statusReason",
        "path" : "MedicationStatement.statusReason",
        "short" : "ReasonModificationOrDiscontinuationOfUse",
        "definition" : "Reason for changing or discontinuing use of medication.",
        "alias" : ["RedenWijzigenOfStoppenGebruik"],
        "max" : "1",
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.43--20221115122002"
        },
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-409",
            "comment" : "ReasonModificationOrDiscontinuationOfUse [DEPRECATED]"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-TODO",
            "map" : "mp-dataelement9x-409",
            "comment" : "ReasonModificationOrDiscontinuationOfUse"
          }
        ]
      },
      {
        "id" : "MedicationStatement.category",
        "path" : "MedicationStatement.category",
        "min" : 1,
        "patternCodeableConcept" : {
          "coding" : [
            {
              "system" : "http://snomed.info/sct",
              "code" : "422979000"
            }
          ]
        }
      },
      {
        "id" : "MedicationStatement.category.extension:additionalCategory",
        "path" : "MedicationStatement.category.extension",
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
        "id" : "MedicationStatement.category.extension:additionalCategory.value[x]",
        "path" : "MedicationStatement.category.extension.value[x]",
        "short" : "Type of medication usage",
        "definition" : "Indicates where the medication is expected to be consumed or administered.",
        "binding" : {
          "strength" : "preferred",
          "valueSet" : "http://hl7.org/fhir/ValueSet/medication-statement-category"
        }
      },
      {
        "id" : "MedicationStatement.medication[x]",
        "path" : "MedicationStatement.medication[x]",
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
        "id" : "MedicationStatement.medication[x]:medicationReference",
        "path" : "MedicationStatement.medication[x]",
        "sliceName" : "medicationReference",
        "short" : "ProductUsed",
        "definition" : "The product used. This is usually medication. Food, blood products, aids and bandages do not strictly fall under the category of medication, but can be recorded as well.\r\nIn principle, this will be the prescribed product, but the product used may differ from the prescribed product.",
        "alias" : ["Gebruiksproduct"],
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
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.21339",
            "comment" : "ProductUsed"
          }
        ]
      },
      {
        "id" : "MedicationStatement.subject",
        "path" : "MedicationStatement.subject",
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
        "id" : "MedicationStatement.context",
        "path" : "MedicationStatement.context",
        "short" : "RelationEncounter / RelationEpisodeOfCare",
        "comment" : "The ext-Context-EpisodeOfCare extension is used to capture a reference to a related EpisodeOfCare if both a reference to an Encounter and an EpisodeOfCare need to be exchanged, or to capture additional EpisodeOfCare resources if multiple related EpisodeOfCare resources need to be exchanged. This `.context` element will then contain the reference to the Encounter resource or the 'first' EpisodeOfCare, respectively.",
        "alias" : ["RelatieContact", "RelatieZorgepisode"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Encounter",
              "http://hl7.org/fhir/StructureDefinition/EpisodeOfCare",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-Encounter",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-EpisodeOfCare"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1349",
            "comment" : "RelationEncounter"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1349",
            "comment" : "RelationEncounter"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1351",
            "comment" : "RelationEpisodeOfCare"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1351",
            "comment" : "RelationEpisodeOfCare"
          }
        ]
      },
      {
        "id" : "MedicationStatement.context.extension:relationEpisodeOfCare",
        "path" : "MedicationStatement.context.extension",
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
        "id" : "MedicationStatement.context.extension:relationEpisodeOfCare.value[x]",
        "path" : "MedicationStatement.context.extension.value[x]",
        "short" : "RelationEpisodeOfCare",
        "alias" : ["RelatieZorgepisode"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1351",
            "comment" : "RelationEpisodeOfCare"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1351",
            "comment" : "RelationEpisodeOfCare"
          }
        ]
      },
      {
        "id" : "MedicationStatement.effective[x]",
        "path" : "MedicationStatement.effective[x]",
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
        "id" : "MedicationStatement.effective[x]:effectivePeriod",
        "path" : "MedicationStatement.effective[x]",
        "sliceName" : "effectivePeriod",
        "short" : "PeriodOfUse",
        "definition" : "Medication use can be recorded for a certain moment or over a certain period. Thus, medication use can be recorded multiple times during the use of medication. The usage period is the period or moment over which the data is recorded.\n**Start date:** This is the time at which the agreement was to take effect (or took effect or will take effect). \n**End date:** The time at which the period of use ends (or ended or will end). To avoid confusion between 'to' and 'up to', the submission of time is always mandatory for the end date.",
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
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.22663",
            "comment" : "PeriodOfUse"
          }
        ]
      },
      {
        "id" : "MedicationStatement.dateAsserted",
        "path" : "MedicationStatement.dateAsserted",
        "short" : "MedicationUseDateTime",
        "definition" : "Date on which this use is entered.",
        "alias" : ["MedicatiegebruikDatumTijd"],
        "mapping" : [
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.22398",
            "comment" : "MedicationUseDateTime"
          }
        ]
      },
      {
        "id" : "MedicationStatement.informationSource",
        "path" : "MedicationStatement.informationSource",
        "type" : [
          {
            "code" : "Reference",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-NlCoreHealthProfessionalReference"
            ],
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Patient",
              "http://hl7.org/fhir/StructureDefinition/Practitioner",
              "http://hl7.org/fhir/StructureDefinition/PractitionerRole",
              "http://hl7.org/fhir/StructureDefinition/RelatedPerson",
              "http://hl7.org/fhir/StructureDefinition/Organization",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-Patient",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthProfessional-PractitionerRole",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-ContactPerson"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-593",
            "comment" : "Informant"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-593",
            "comment" : "Informant"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-594",
            "comment" : "Person"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-594",
            "comment" : "Person"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-620",
            "comment" : "InformantIsPatient (InformantIsPatient = true when informationSource refers to the same Patient as subject)"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-620",
            "comment" : "InformantIsPatient (InformantIsPatient = true when informationSource refers to the same Patient as subject)"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-621",
            "comment" : "InformantIsHealthProfessional"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-621",
            "comment" : "InformantIsHealthProfessional"
          }
        ]
      },
      {
        "id" : "MedicationStatement.derivedFrom",
        "path" : "MedicationStatement.derivedFrom",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "pattern",
              "path" : "extension.value"
            }
          ],
          "rules" : "open"
        }
      },
      {
        "id" : "MedicationStatement.derivedFrom:relationMedicationAgreement",
        "path" : "MedicationStatement.derivedFrom",
        "sliceName" : "relationMedicationAgreement",
        "short" : "RelationMedicationAgreement",
        "definition" : "Medication agreement to which the entered medication use refers. In case medication use is recorded as 'as agreed', the agreement to which is referred, is stated here.",
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
            "map" : "mp-dataelement9x-413",
            "comment" : "RelationMedicationAgreement"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-413",
            "comment" : "RelationMedicationAgreement"
          }
        ]
      },
      {
        "id" : "MedicationStatement.derivedFrom:relationMedicationAgreement.extension:resourceCategory",
        "path" : "MedicationStatement.derivedFrom.extension",
        "sliceName" : "resourceCategory",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-ResourceCategory"
            ]
          }
        ]
      },
      {
        "id" : "MedicationStatement.derivedFrom:relationMedicationAgreement.extension:resourceCategory.value[x]",
        "path" : "MedicationStatement.derivedFrom.extension.value[x]",
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
        "id" : "MedicationStatement.derivedFrom:relationAdministrationAgreement",
        "path" : "MedicationStatement.derivedFrom",
        "sliceName" : "relationAdministrationAgreement",
        "short" : "RelationAdministrationAgreement",
        "definition" : "Administration agreement to which the entered medication use refers. In case medication use is recorded as 'as agreed', the agreement to which is referred, is stated here.",
        "alias" : ["RelatieToedieningsafspraak"],
        "max" : "1",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-AdministrationAgreement"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1329",
            "comment" : "RelationAdministrationAgreement"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1329",
            "comment" : "RelationAdministrationAgreement"
          }
        ]
      },
      {
        "id" : "MedicationStatement.derivedFrom:relationAdministrationAgreement.extension:resourceCategory",
        "path" : "MedicationStatement.derivedFrom.extension",
        "sliceName" : "resourceCategory",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-ResourceCategory"
            ]
          }
        ]
      },
      {
        "id" : "MedicationStatement.derivedFrom:relationAdministrationAgreement.extension:resourceCategory.value[x]",
        "path" : "MedicationStatement.derivedFrom.extension.value[x]",
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
        "id" : "MedicationStatement.derivedFrom:relationMedicationDispense",
        "path" : "MedicationStatement.derivedFrom",
        "sliceName" : "relationMedicationDispense",
        "short" : "RelationMedicationDispense",
        "definition" : "Medication dispense which is the basis for entering the medication use.",
        "alias" : ["RelatieMedicatieverstrekking"],
        "max" : "1",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationDispense"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-416",
            "comment" : "RelationMedicationDispense"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-416",
            "comment" : "RelationMedicationDispense"
          }
        ]
      },
      {
        "id" : "MedicationStatement.derivedFrom:relationMedicationDispense.extension:resourceCategory",
        "path" : "MedicationStatement.derivedFrom.extension",
        "sliceName" : "resourceCategory",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-ResourceCategory"
            ]
          }
        ]
      },
      {
        "id" : "MedicationStatement.derivedFrom:relationMedicationDispense.extension:resourceCategory.value[x]",
        "path" : "MedicationStatement.derivedFrom.extension.value[x]",
        "patternCodeableConcept" : {
          "coding" : [
            {
              "system" : "http://snomed.info/sct",
              "code" : "373784005"
            }
          ]
        }
      },
      {
        "id" : "MedicationStatement.reasonCode",
        "path" : "MedicationStatement.reasonCode",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "exists",
              "path" : "text"
            }
          ],
          "rules" : "open"
        }
      },
      {
        "id" : "MedicationStatement.reasonCode:reasonForUse",
        "path" : "MedicationStatement.reasonCode",
        "sliceName" : "reasonForUse",
        "max" : "1"
      },
      {
        "id" : "MedicationStatement.reasonCode:reasonForUse.text",
        "path" : "MedicationStatement.reasonCode.text",
        "short" : "ReasonForUse",
        "definition" : "The reason for using the medication, particularly in self-care medicine purchased by the patient themselves.",
        "alias" : ["RedenGebruik"],
        "min" : 1,
        "mapping" : [
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.22491",
            "comment" : "ReasonForUse"
          }
        ]
      },
      {
        "id" : "MedicationStatement.note",
        "path" : "MedicationStatement.note",
        "max" : "1"
      },
      {
        "id" : "MedicationStatement.note.text",
        "path" : "MedicationStatement.note.text",
        "short" : "Comment",
        "definition" : "Comments on the medication use.",
        "alias" : ["Toelichting"],
        "mapping" : [
          {
            "identity" : "zib-medicationuse2-v1.1.1-2020EN",
            "map" : "NL-CM:9.11.21624",
            "comment" : "Comment"
          }
        ]
      },
      {
        "id" : "MedicationStatement.dosage",
        "path" : "MedicationStatement.dosage",
        "short" : "DosingInstructions / InstructionsForUse",
        "definition" : "Instructions for the use of the medication, e.g. dose and route of administration. In the event of medication use, this is the pattern of use established by the patient or which the patient followed.",
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
