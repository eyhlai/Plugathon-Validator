# mp DispenseRequest - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp DispenseRequest**

## Resource Profile: mp DispenseRequest 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-DispenseRequest | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpDispenseRequest |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
The dispense request is the request of a prescriber to the pharmacist to dispense medication(s) to the patient to support current medication agreements. The prescriber asks them to dispense a certain amount of medicine or to dispense medicine(s) for a period of use. 

 
This MedicationRequest resource represents the DispenseRequest building block for implementations following the information standard[MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) DispenseRequest, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set. 

**Usages:**

* Use this Profile: [mp MedicationPrescription Bundle](StructureDefinition-mp-MedicationPrescription-Bundle.md) and [mp ProposalDispenseRequest Bundle](StructureDefinition-mp-ProposalDispenseRequest-Bundle.md)
* Refer to this Profile: [mp MedicationDispense](StructureDefinition-mp-MedicationDispense.md) and [mp ReplyProposalDispenseRequest](StructureDefinition-mp-ReplyProposalDispenseRequest.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-DispenseRequest)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-DispenseRequest.csv), [Excel](StructureDefinition-mp-DispenseRequest.xlsx), [Schematron](StructureDefinition-mp-DispenseRequest.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-DispenseRequest",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-DispenseRequest",
  "version" : "0.1.0",
  "name" : "MpDispenseRequest",
  "title" : "mp DispenseRequest",
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
  "description" : "The dispense request is the request of a prescriber to the pharmacist to dispense medication(s) to the patient to support current medication agreements. The prescriber asks them to dispense a certain amount of medicine or to dispense medicine(s) for a period of use.",
  "purpose" : "This MedicationRequest resource represents the DispenseRequest building block for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) DispenseRequest, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "zib-dispenserequest-v1.0.3-2020EN",
      "uri" : "https://zibs.nl/wiki/DispenseRequest-v1.0.3(2020EN)",
      "name" : "zib DispenseRequest-v1.0.3(2020EN)"
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
        "short" : "DispenseRequest",
        "alias" : ["Verstrekkingsverzoek"],
        "mapping" : [
          {
            "identity" : "zib-dispenserequest-v1.0.3-2020EN",
            "map" : "NL-CM:9.10.19963",
            "comment" : "DispenseRequest"
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:additionalWishes",
        "path" : "MedicationRequest.extension",
        "sliceName" : "additionalWishes",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.AdditionalWishes"
            ]
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:additionalWishes.value[x]",
        "path" : "MedicationRequest.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-287",
            "comment" : "AdditionalWishes"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-287",
            "comment" : "AdditionalWishes"
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
        "id" : "MedicationRequest.extension:financialIndicationCode",
        "path" : "MedicationRequest.extension",
        "sliceName" : "financialIndicationCode",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.FinancialIndicationCode"
            ]
          }
        ]
      },
      {
        "id" : "MedicationRequest.extension:financialIndicationCode.value[x]",
        "path" : "MedicationRequest.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-592",
            "comment" : "FinancialIndicationCode"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-592",
            "comment" : "FinancialIndicationCode"
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
            "map" : "mp-dataelement9x-1347",
            "comment" : "RelationEpisodeOfCare"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1347",
            "comment" : "RelationEpisodeOfCare"
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
            "map" : "mp-dataelement9x-289",
            "comment" : "Identification"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-289",
            "comment" : "Identification"
          }
        ]
      },
      {
        "id" : "MedicationRequest.status",
        "path" : "MedicationRequest.status",
        "short" : "CanceledIndicator",
        "comment" : "This element is implicitly mapped to the zib concept NL-CM:9.10.20062 (PeriodOfUse). Unless a more appropriate status is recorded, the following guidance applies:\r\n\r\n* When the value of CanceledIndicator is _true_, `.status` will be set to _entered-in-error_.\r\n* When PeriodOfUse.startDateTime is absent and the value of PeriodOfUse.endDateTime is in the future, `.status` will usually be set to _active_.\r\n* When the value of PeriodOfUse.startDateTime is in the past or the future and PeriodOfUse.endDateTime is absent or its value is in the future, `.status` will usually be set to _active_.\r\n* When PeriodOfUse.endDateTime exists and its value is in the past, `.status` will usually be set to _completed_.\r\n* When PeriodOfUse.Duration and PeriodOfUse.startDateTime are known, PeriodOfUse.endDateTime can be deduced and the previous rules apply. \r\n* When a system is unable to infer the status, `.status` will be set to _unknown_. The _unknown_ code is not to be used to convey other statuses. The _unknown_ code should be used when one of the statuses applies, but the authoring system doesn't know the current state of the DispenseRequest.",
        "alias" : ["GeannuleerdIndicator"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-1167",
            "comment" : "CanceledIndicator"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1167",
            "comment" : "CanceledIndicator"
          },
          {
            "identity" : "zib-dispenserequest-v1.0.3-2020EN",
            "map" : "NL-CM:9.10.20062",
            "comment" : "PeriodOfUse (implicit, main mapping is on `.dispenseRequest.validityPeriod` and extension ext-TimeInterval.Duration)"
          }
        ]
      },
      {
        "id" : "MedicationRequest.intent",
        "path" : "MedicationRequest.intent",
        "comment" : "Unless `.intent` is explicitly recorded and a more appropriate code is known, the value can be set to _order_ because a DispenseRequest should authorize an action for a patient, pharmacist, professional administrator et cetera."
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
        "id" : "MedicationRequest.category:dispenseRequestCode",
        "path" : "MedicationRequest.category",
        "sliceName" : "dispenseRequestCode",
        "min" : 1,
        "max" : "1",
        "patternCodeableConcept" : {
          "coding" : [
            {
              "system" : "http://snomed.info/sct",
              "code" : "52711000146108"
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
        "short" : "MedicineToBeDispensed",
        "definition" : "The medicine to be dispensed.",
        "alias" : ["TeVerstrekkenGeneesmiddel"],
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
            "identity" : "zib-dispenserequest-v1.0.3-2020EN",
            "map" : "NL-CM:9.10.22249",
            "comment" : "MedicineToBeDispensed"
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
            "map" : "mp-dataelement9x-1345",
            "comment" : "RelationEncounter"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-1345",
            "comment" : "RelationEncounter"
          }
        ]
      },
      {
        "id" : "MedicationRequest.authoredOn",
        "path" : "MedicationRequest.authoredOn",
        "short" : "DispenseRequestDate",
        "definition" : "Time at which the dispense request is entered.",
        "alias" : ["VerstrekkingsverzoekDatum"],
        "mapping" : [
          {
            "identity" : "zib-dispenserequest-v1.0.3-2020EN",
            "map" : "NL-CM:9.10.20060",
            "comment" : "DispenseRequestDate"
          }
        ]
      },
      {
        "id" : "MedicationRequest.requester",
        "path" : "MedicationRequest.requester",
        "short" : "Author",
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
            "map" : "mp-dataelement9x-290",
            "comment" : "Author"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-290",
            "comment" : "Author"
          }
        ]
      },
      {
        "id" : "MedicationRequest.performer",
        "path" : "MedicationRequest.performer",
        "short" : "IntendedSupplier",
        "definition" : "The intended supplier is a pharmacist.",
        "comment" : "Although the nl-core-HealthcareProvider profile (with resource type Location) is the focal profile of the zib HealthcareProvider, this reference is to the nl-core-HealthcareProvider-Organization profile, because the concept is concerned with the organizational information of the intended supplier.",
        "alias" : ["BeoogdVerstrekker"],
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
              "http://hl7.org/fhir/StructureDefinition/CareTeam",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthcareProvider-Organization"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-dispenserequest-v1.0.3-2020EN",
            "map" : "NL-CM:9.10.19966",
            "comment" : "IntendedSupplier"
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
        "definition" : "A reference to the MedicationAgreement(s) that were/are the basis of this DispenseRequest.",
        "alias" : ["RelatieMedicatieafspraak"],
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
            "map" : "mp-dataelement9x-292",
            "comment" : "RelationMedicationAgreement"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-292",
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
        "definition" : "Explanation for the dispense request. This explanation can contain e.g. information on why a prescriber submits a dispense request that deviates from the norm, e.g. an extra dispense request needed because the patient has lost the medication.",
        "alias" : ["Toelichting"],
        "mapping" : [
          {
            "identity" : "zib-dispenserequest-v1.0.3-2020EN",
            "map" : "NL-CM:9.10.22274",
            "comment" : "Comment"
          }
        ]
      },
      {
        "id" : "MedicationRequest.dispenseRequest.extension:dispenseLocation",
        "path" : "MedicationRequest.dispenseRequest.extension",
        "sliceName" : "dispenseLocation",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.DispenseLocation"
            ]
          }
        ]
      },
      {
        "id" : "MedicationRequest.dispenseRequest.extension:dispenseLocation.value[x]",
        "path" : "MedicationRequest.dispenseRequest.extension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-dispenserequest-v1.0.3-2020EN",
            "map" : "NL-CM:9.10.20068",
            "comment" : "DispenseLocation"
          }
        ]
      },
      {
        "id" : "MedicationRequest.dispenseRequest.validityPeriod",
        "path" : "MedicationRequest.dispenseRequest.validityPeriod",
        "short" : "PeriodOfUse",
        "definition" : "During the approved period of use, the pharmacist has permission to dispense medicine so that the patient has a sufficient amount of medication. In many cases, the approved period of use can be described by only an end date: the approved end date of use.",
        "alias" : ["Verbruiksperiode"],
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
            "identity" : "zib-dispenserequest-v1.0.3-2020EN",
            "map" : "NL-CM:9.10.20062",
            "comment" : "PeriodOfUse"
          }
        ]
      },
      {
        "id" : "MedicationRequest.dispenseRequest.numberOfRepeatsAllowed",
        "path" : "MedicationRequest.dispenseRequest.numberOfRepeatsAllowed",
        "short" : "NumberOfRefills",
        "definition" : "The number of additional times the medication may be dispensed after the first time. In the case of Amount: The total amount that may be dispensed is: (Number of refills + 1) x amount to be dispensed.In the case of Period of Use:The total period of use is: (Number of refills + 1) x period of use",
        "alias" : ["AantalHerhalingen"],
        "mapping" : [
          {
            "identity" : "zib-dispenserequest-v1.0.3-2020EN",
            "map" : "NL-CM:9.10.22120",
            "comment" : "NumberOfRefills"
          }
        ]
      },
      {
        "id" : "MedicationRequest.dispenseRequest.quantity",
        "path" : "MedicationRequest.dispenseRequest.quantity",
        "short" : "Amount",
        "definition" : "This is the number of units of the ordered product per dispense. The number of refills indicates how often this amount is allowed to be dispensed. Optionally a translation to NHG table Gebruiksvoorschriften (Table 25) is also allowed which can be captured in the iso21090-PQ-translation extension.",
        "alias" : ["TeVerstrekkenHoeveelheid"],
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
            "identity" : "zib-dispenserequest-v1.0.3-2020EN",
            "map" : "NL-CM:9.10.19964",
            "comment" : "Amount"
          }
        ]
      }
    ]
  }
}

```
