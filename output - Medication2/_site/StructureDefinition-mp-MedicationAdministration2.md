# mp MedicationAdministration2 - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp MedicationAdministration2**

## Resource Profile: mp MedicationAdministration2 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-MedicationAdministration2 | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpMedicationAdministration2 |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
Medication administration is the registration of the individual administrations of the medicine on the patient by the administrator (e.g. a nurse or patient themselves), in relation to the entered agreements. 

 
This MedicationAdministration resource represents the MedicationAdministration2 building block for implementations following the information standard[MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) MedicationAdministration2, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set. 

**Usages:**

* This Profile is not used by any profiles in this Implementation Guide

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-MedicationAdministration2)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-MedicationAdministration2.csv), [Excel](StructureDefinition-mp-MedicationAdministration2.xlsx), [Schematron](StructureDefinition-mp-MedicationAdministration2.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-MedicationAdministration2",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationAdministration2",
  "version" : "0.1.0",
  "name" : "MpMedicationAdministration2",
  "title" : "mp MedicationAdministration2",
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
  "description" : "Medication administration is the registration of the individual administrations of the medicine on the patient by the administrator (e.g. a nurse or patient themselves), in relation to the entered agreements.",
  "purpose" : "This MedicationAdministration resource represents the MedicationAdministration2 building block for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) MedicationAdministration2, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
      "uri" : "https://zibs.nl/wiki/MedicationAdministration2-v1.1.1(2020EN)",
      "name" : "zib MedicationAdministration2-v1.1.1(2020EN)"
    },
    {
      "identity" : "zib-range-v1.0.1-2020EN",
      "uri" : "https://zibs.nl/wiki/Range-v1.0.1(2020EN)",
      "name" : "zib Range-v1.0.1(2020EN)"
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
    },
    {
      "identity" : "w3c.prov",
      "uri" : "http://www.w3.org/ns/prov",
      "name" : "W3C PROV"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "MedicationAdministration",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/MedicationAdministration",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "MedicationAdministration",
        "path" : "MedicationAdministration",
        "short" : "MedicationAdministration",
        "alias" : ["Medicatietoediening"],
        "mapping" : [
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.20928",
            "comment" : "MedicationAdministration"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.extension:agreedDateTime",
        "path" : "MedicationAdministration.extension",
        "sliceName" : "agreedDateTime",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAdministration2.AgreedDateTime"
            ]
          }
        ]
      },
      {
        "id" : "MedicationAdministration.extension:agreedDateTime.value[x]",
        "path" : "MedicationAdministration.extension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.23171",
            "comment" : "AgreedDateTime"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.extension:medicationAdministrationReasonForDeviation",
        "path" : "MedicationAdministration.extension",
        "sliceName" : "medicationAdministrationReasonForDeviation",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAdministration2.ReasonForDeviation"
            ]
          }
        ]
      },
      {
        "id" : "MedicationAdministration.extension:medicationAdministrationReasonForDeviation.value[x]",
        "path" : "MedicationAdministration.extension.value[x]",
        "comment" : "This MedicationAdministrationReasonForDeviation extension has overlap with `.statusReason`. Both concepts allow the documentation of reasons why an administration did not take place, potentially resulting in duplicated information in both places. This extension, however, has a broader scope because it also covers the reasons why administrations are performed differently than the agreement.",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-444",
            "comment" : "MedicationAdministrationReasonForDeviation"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-444",
            "comment" : "MedicationAdministrationReasonForDeviation"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.extension:pharmaceuticalTreatmentIdentifier",
        "path" : "MedicationAdministration.extension",
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
        "id" : "MedicationAdministration.extension:pharmaceuticalTreatmentIdentifier.value[x]",
        "path" : "MedicationAdministration.extension.value[x]",
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
        "id" : "MedicationAdministration.extension:injectionPatchSite",
        "path" : "MedicationAdministration.extension",
        "sliceName" : "injectionPatchSite",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAdministration2.InjectionPatchSite"
            ]
          }
        ]
      },
      {
        "id" : "MedicationAdministration.extension:injectionPatchSite.value[x]",
        "path" : "MedicationAdministration.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-702",
            "comment" : "InjectionPatchSite"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-702",
            "comment" : "InjectionPatchSite"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.extension:registrationDateTime",
        "path" : "MedicationAdministration.extension",
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
        "id" : "MedicationAdministration.extension:registrationDateTime.value[x]",
        "path" : "MedicationAdministration.extension.value[x]",
        "definition" : "The date and time when the MedicationAdministration was recorded. RegistrationDateTime is used to accurately determine the chronological order of agreements. Therefore, the date and time are mandatory. These values are immutable. When consulting or receiving this MedicationAdministration, the original RegistrationDateTime remains unchanged.\n\nNote: This data element differs from the data element RegistrationDateTime in zib RegistratieGegevens-v1.1.1 (2024NL). In zib RegistratieGegevens-v1.1.1 (2024NL), RegistrationDateTime refers to the date and time when the data was recorded. This may be the initial registration or the date and time when data was transferred. The zib concept RegistrationDateTime is not applied in MP9.",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1482",
            "comment" : "RegistrationDateTime"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1482",
            "comment" : "RegistrationDateTime"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.identifier",
        "path" : "MedicationAdministration.identifier",
        "short" : "Identification",
        "alias" : ["Identificatie"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-447",
            "comment" : "Identification"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-447",
            "comment" : "Identification"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.status",
        "path" : "MedicationAdministration.status",
        "short" : "MedicationAdministrationStatus",
        "definition" : "The status of the administration, as a description of the stage within the administering process. Only the status codes ‘completed’ and ‘cancelled’ apply to indivisible products (such as tablets or suppositories). For divisible products (such as infusions), doses can also be ‘suspended’ or ‘aborted’.  \r\n\r\nWhen documenting this, the following interpretations are used: \r\n\r\n- Active: The product is administered.\r\n- Interrupted: Use has (temporarily) been interrupted, because of a side effect, for example. Later, the patient and/or doctor can decide whether or not to resume or discontinue use.\r\n- Discontinued: Administration has stopped.\r\n- Completed: Administration has been completed.\r\n- Not started: The product was never administered.",
        "comment" : "If no value for MedicationAdministrationStatus is present, and the system is thus unable to infer the status, `.status` will be set to _unknown_.",
        "alias" : ["MedicatietoedieningStatus"],
        "binding" : {
          "strength" : "required",
          "description" : "Use ConceptMap 'MedicatieToedieningStatusCodelijst-to-MedicationAdministrationStatusCodes' to translate zib terminology to profile terminology in ValueSet 'MedicationAdministration Status Codes'",
          "valueSet" : "http://hl7.org/fhir/ValueSet/medication-admin-status|4.0.1",
          "_valueSet" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/11179-permitted-value-conceptmap",
                "valueCanonical" : "http://nictiz.nl/fhir/ConceptMap/MedicatieToedieningStatusCodelijst-to-MedicationAdministrationStatusCodes"
              }
            ]
          }
        },
        "mapping" : [
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.21191",
            "comment" : "MedicationAdministrationStatus"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.category",
        "path" : "MedicationAdministration.category",
        "min" : 1,
        "patternCodeableConcept" : {
          "coding" : [
            {
              "system" : "http://snomed.info/sct",
              "code" : "18629005"
            }
          ]
        }
      },
      {
        "id" : "MedicationAdministration.category.extension:additionalCategory",
        "path" : "MedicationAdministration.category.extension",
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
        "id" : "MedicationAdministration.category.extension:additionalCategory.value[x]",
        "path" : "MedicationAdministration.category.extension.value[x]",
        "short" : "Type of medication usage",
        "definition" : "Indicates where the medication is expected to be consumed or administered.",
        "binding" : {
          "strength" : "preferred",
          "valueSet" : "http://hl7.org/fhir/ValueSet/medication-admin-category"
        }
      },
      {
        "id" : "MedicationAdministration.medication[x]",
        "path" : "MedicationAdministration.medication[x]",
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
        "id" : "MedicationAdministration.medication[x]:medicationReference",
        "path" : "MedicationAdministration.medication[x]",
        "sliceName" : "medicationReference",
        "short" : "AdministrationProduct",
        "definition" : "The product taken or administered. This is usually medication. Food, blood products, aids and bandages do not strictly fall under the category of medication, but can be reported as well. \r\n\r\nIn principle, this will be the prescribed product, but the administrator may substitute it by replacing the product with an equivalent product. For example: two 50mg tablets can be administered instead of one 100mg tablet.",
        "alias" : ["ToedieningsProduct"],
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
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.20929",
            "comment" : "AdministrationProduct"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.subject",
        "path" : "MedicationAdministration.subject",
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
        "id" : "MedicationAdministration.context",
        "path" : "MedicationAdministration.context",
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
            "map" : "mp-dataelement9x-1353",
            "comment" : "RelationEncounter"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1353",
            "comment" : "RelationEncounter"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1355",
            "comment" : "RelationEpisodeOfCare"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1355",
            "comment" : "RelationEpisodeOfCare"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.context.extension:relationEpisodeOfCare",
        "path" : "MedicationAdministration.context.extension",
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
        "id" : "MedicationAdministration.context.extension:relationEpisodeOfCare.value[x]",
        "path" : "MedicationAdministration.context.extension.value[x]",
        "short" : "RelatedEpisodeOfCare",
        "alias" : ["RelatieZorgepisode"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1355",
            "comment" : "RelationEpisodeOfCare"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1355",
            "comment" : "RelationEpisodeOfCare"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.supportingInformation",
        "path" : "MedicationAdministration.supportingInformation",
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
        "id" : "MedicationAdministration.supportingInformation:administrationAgreement",
        "path" : "MedicationAdministration.supportingInformation",
        "sliceName" : "administrationAgreement",
        "short" : "AdministrationAgreement",
        "definition" : "Administration agreement on which this administration is based.",
        "alias" : ["Toedieningsafspraak"],
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
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.23237",
            "comment" : "AdministrationAgreement"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.supportingInformation:variableDosingRegimen",
        "path" : "MedicationAdministration.supportingInformation",
        "sliceName" : "variableDosingRegimen",
        "short" : "VariableDosingRegimen",
        "definition" : "Variable dosing regimen on which this administration is based.",
        "alias" : ["WisselendDoseerSchema"],
        "max" : "1",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-VariableDosingRegimen"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1325",
            "comment" : "RelationVariableDosingRegimen"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1325",
            "comment" : "RelationVariableDosingRegimen"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.effective[x]",
        "path" : "MedicationAdministration.effective[x]",
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
        "id" : "MedicationAdministration.effective[x]:effectiveDateTime",
        "path" : "MedicationAdministration.effective[x]",
        "sliceName" : "effectiveDateTime",
        "short" : "AdministrationDateTime",
        "definition" : "The date and time at which the medication was administered.",
        "alias" : ["ToedieningsDatumTijd"],
        "type" : [
          {
            "code" : "dateTime"
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.21193",
            "comment" : "AdministrationDateTime"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.performer",
        "path" : "MedicationAdministration.performer",
        "short" : "Administrator",
        "definition" : "The concept describes the person who administered the product. This is a professional authorised administrator, the patient themselves or the informal carer, for example.",
        "alias" : ["Toediener"],
        "max" : "1",
        "mapping" : [
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.21196",
            "comment" : "Administrator [DEPRECATED]"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-437",
            "comment" : "Administrator"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-437",
            "comment" : "Administrator"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.performer.actor",
        "path" : "MedicationAdministration.performer.actor",
        "short" : "Patient / HealthProfessional / Caregiver",
        "alias" : ["Patiënt", "Zorgverlener", "Mantelzorger"],
        "type" : [
          {
            "code" : "Reference",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-NlCoreHealthProfessionalReference"
            ],
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Practitioner",
              "http://hl7.org/fhir/StructureDefinition/PractitionerRole",
              "http://hl7.org/fhir/StructureDefinition/Patient",
              "http://hl7.org/fhir/StructureDefinition/RelatedPerson",
              "http://hl7.org/fhir/StructureDefinition/Device",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-Patient",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthProfessional-PractitionerRole",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-ContactPerson"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.23380",
            "comment" : "Patient"
          },
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.23172",
            "comment" : "HealthProfessional"
          },
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.23355",
            "comment" : "Caregiver"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.request",
        "path" : "MedicationAdministration.request",
        "short" : "MedicationAgreement",
        "definition" : "Medication agreement on which this administration is based.",
        "alias" : ["Medicatieafspraak"],
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
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.23170",
            "comment" : "MedicationAgreement"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.note",
        "path" : "MedicationAdministration.note",
        "max" : "1"
      },
      {
        "id" : "MedicationAdministration.note.text",
        "path" : "MedicationAdministration.note.text",
        "short" : "Comment",
        "definition" : "Comments on administering the medication.",
        "alias" : ["Toelichting"],
        "mapping" : [
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.21337",
            "comment" : "Comment"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.dosage.route",
        "path" : "MedicationAdministration.dosage.route",
        "short" : "RouteOfAdministration",
        "definition" : "The route through which the medication is administered (oral, nasal, intravenous,...).",
        "alias" : ["Toedieningsweg"],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.9.13.2--20200901000000"
        },
        "mapping" : [
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.21195",
            "comment" : "RouteOfAdministration"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.dosage.dose",
        "path" : "MedicationAdministration.dosage.dose",
        "short" : "AdministeredAmount",
        "definition" : "Amount of the administered product.",
        "alias" : ["ToegediendeHoeveelheid"],
        "type" : [
          {
            "code" : "Quantity",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-GstdSimpleQuantity"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.21194",
            "comment" : "AdministeredAmount"
          }
        ]
      },
      {
        "id" : "MedicationAdministration.dosage.rate[x]",
        "path" : "MedicationAdministration.dosage.rate[x]",
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
        "id" : "MedicationAdministration.dosage.rate[x]:rateQuantity",
        "path" : "MedicationAdministration.dosage.rate[x]",
        "sliceName" : "rateQuantity",
        "short" : "AdministeringSpeed / nominalValue",
        "definition" : "The administering speed is used in slow administration of liquid. In practice, the measuring unit is almost always ml/hour.\r\n\nFor example, with an administering speed of 10ml/hour: \r\n* value = 10\r\n* unit = ml/hour",
        "alias" : ["Toedieningssnelheid", "nominaleWaarde"],
        "type" : [
          {
            "code" : "Quantity"
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-medicationadministration2-v1.1.1-2020EN",
            "map" : "NL-CM:9.13.23159",
            "comment" : "AdministeringSpeed"
          },
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.4",
            "comment" : "nominalValue"
          }
        ]
      }
    ]
  }
}

```
