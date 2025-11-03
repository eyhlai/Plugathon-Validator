# mp MedicationDispense - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp MedicationDispense**

## Resource Profile: mp MedicationDispense 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-MedicationDispense | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpMedicationDispense |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
A dispense is the delivery of an amount of medicine to the patient, their administrator or their representative. 

 
This MedicationDispense resource represents the MedicationDispense building block for implementations following the information standard[MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) MedicationDispense, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set. 

**Usages:**

* Use this Profile: [mp MedicationPrescriptionProcessing Bundle](StructureDefinition-mp-MedicationPrescriptionProcessing-Bundle.md)
* Refer to this Profile: [mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-MedicationDispense)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-MedicationDispense.csv), [Excel](StructureDefinition-mp-MedicationDispense.xlsx), [Schematron](StructureDefinition-mp-MedicationDispense.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-MedicationDispense",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationDispense",
  "version" : "0.1.0",
  "name" : "MpMedicationDispense",
  "title" : "mp MedicationDispense",
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
  "description" : "A dispense is the delivery of an amount of medicine to the patient, their administrator or their representative.",
  "purpose" : "This MedicationDispense resource represents the MedicationDispense building block for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) MedicationDispense, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "zib-medicationdispense-v2.0.2-2020EN",
      "uri" : "https://zibs.nl/wiki/MedicationDispense-v2.0.2(2020EN)",
      "name" : "zib MedicationDispense-v2.0.2(2020EN)"
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
        "short" : "MedicationDispense",
        "alias" : ["Medicatieverstrekking"],
        "mapping" : [
          {
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.20270",
            "comment" : "MedicationDispense"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:medicationDispenseAdditionalInformation",
        "path" : "MedicationDispense.extension",
        "sliceName" : "medicationDispenseAdditionalInformation",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationDispense.MedicationDispenseAdditionalInformation"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:medicationDispenseAdditionalInformation.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-357",
            "comment" : "MedicationDispenseAdditionalInformation"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-357",
            "comment" : "MedicationDispenseAdditionalInformation"
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:requestDate",
        "path" : "MedicationDispense.extension",
        "sliceName" : "requestDate",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationDispense.RequestDate"
            ]
          }
        ]
      },
      {
        "id" : "MedicationDispense.extension:requestDate.value[x]",
        "path" : "MedicationDispense.extension.value[x]",
        "mapping" : [
          {
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.22500",
            "comment" : "RequestDate"
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
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.20927",
            "comment" : "DistributionForm"
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
        "id" : "MedicationDispense.identifier",
        "path" : "MedicationDispense.identifier",
        "short" : "Identification",
        "alias" : ["Identificatie"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-361",
            "comment" : "Identification"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-361",
            "comment" : "Identification"
          }
        ]
      },
      {
        "id" : "MedicationDispense.status",
        "path" : "MedicationDispense.status",
        "comment" : "Sending systems that don't record an explicit status can use the following guidance to infer a value from the zib:\r\n\r\n* When MedicationDispenseDateTime exists and its value is in the past, `.status` will usually be set to _completed_.\r\n\r\nMoreover, it is expected that in most use cases only actual, executed, medication dispenses are exchanged which result in a _completed_ value.",
        "mapping" : [
          {
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.20272",
            "comment" : "MedicationDispenseDateTime (implicit, main mapping is on `.whenHandedOver`)"
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
              "code" : "373784005"
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
        "short" : "DispensedMedicine",
        "definition" : "The dispensed medicine.",
        "alias" : ["VerstrektGeneesmiddel"],
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
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.22259",
            "comment" : "DispensedMedicine"
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
        "definition" : "In almost all cases, the supplier will be a pharmacist. It could also be supplied by a webshop (in case of an online order), a drug store or a foreign pharmacist.",
        "comment" : "The 'Supplier' concept of zib MedicationDispense is mapped to both `.performer.actor` and `.location`. This is a Reference to an instance of nl-core-HealthcareProvider-Organization instead of to an instance of nl-core-HealthcareProfessional, because individuals who enter the medication dispense are not recorded.",
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
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.20858",
            "comment" : "Supplier"
          }
        ]
      },
      {
        "id" : "MedicationDispense.location",
        "path" : "MedicationDispense.location",
        "short" : "Supplier",
        "definition" : "In almost all cases, the supplier will be a pharmacist. It could also be supplied by a webshop (in case of an online order), a drug store or a foreign pharmacist.",
        "comment" : "The 'Supplier' concept of zib MedicationDispense is mapped to both `.performer.actor` and `.location`. Details of the physical location of the supplier of the medication dispense can be referenced here.",
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
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.20858",
            "comment" : "Supplier"
          }
        ]
      },
      {
        "id" : "MedicationDispense.authorizingPrescription",
        "path" : "MedicationDispense.authorizingPrescription",
        "short" : "DispenseRequest",
        "definition" : "Relationship to the dispense request.",
        "alias" : ["Verstrekkingsverzoek"],
        "max" : "1",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/MedicationRequest",
              "http://nictiz.nl/fhir/StructureDefinition/mp-DispenseRequest"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.22396",
            "comment" : "DispenseRequest"
          }
        ]
      },
      {
        "id" : "MedicationDispense.quantity",
        "path" : "MedicationDispense.quantity",
        "short" : "DispensedAmount",
        "definition" : "Number of units of the product (measured based on the relevant product code) supplied. Optionally a translation to NHG table Gebruiksvoorschriften(Table 25) is also allowed which is captured using the iso21090-PQ-translation extension.",
        "alias" : ["VerstrekteHoeveelheid"],
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
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.20923",
            "comment" : "DispensedAmount"
          }
        ]
      },
      {
        "id" : "MedicationDispense.daysSupply",
        "path" : "MedicationDispense.daysSupply",
        "short" : "DurationOfUse",
        "definition" : "The period in which the medication is expected to be used. The value depends on the dose and the dispensed amount.",
        "alias" : ["Verbruiksduur"],
        "mapping" : [
          {
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.20924",
            "comment" : "DurationOfUse"
          }
        ]
      },
      {
        "id" : "MedicationDispense.whenHandedOver",
        "path" : "MedicationDispense.whenHandedOver",
        "short" : "MedicationDispenseDateTime",
        "definition" : "The time at which the medicine was supplied. The date and time at which the medicine is delivered. Note: this is the time at which the medicine was delivered to the patient (or their administrator/representative) and not the request date.",
        "alias" : ["MedicatieverstrekkingsDatumTijd"],
        "mapping" : [
          {
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.20272",
            "comment" : "MedicationDispenseDateTime"
          }
        ]
      },
      {
        "id" : "MedicationDispense.destination",
        "path" : "MedicationDispense.destination",
        "short" : "DispenseLocation",
        "definition" : "Dispense location",
        "comment" : "The `Location.name` elements holds the DispenseLocation information.",
        "alias" : ["Afleverlocatie"],
        "mapping" : [
          {
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.20925",
            "comment" : "DispenseLocation. Use `Location.name`."
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
        "definition" : "Comments on the dispense.",
        "alias" : ["Toelichting"],
        "mapping" : [
          {
            "identity" : "zib-medicationdispense-v2.0.2-2020EN",
            "map" : "NL-CM:9.9.22276",
            "comment" : "Comment"
          }
        ]
      }
    ]
  }
}

```
