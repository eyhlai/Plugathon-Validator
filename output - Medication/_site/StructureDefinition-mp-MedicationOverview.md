# mp MedicationOverview - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp MedicationOverview**

## Resource Profile: mp MedicationOverview 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-MedicationOverview | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpMedicationOverview |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
Profile on the List resource which represents the medication overview conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). 

 
To define the medication overview as stated in the information standard Medication Process. 

**Usages:**

* Use this Profile: [mp MedicationOverview Bundle](StructureDefinition-mp-MedicationOverview-Bundle.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-MedicationOverview)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-MedicationOverview.csv), [Excel](StructureDefinition-mp-MedicationOverview.xlsx), [Schematron](StructureDefinition-mp-MedicationOverview.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-MedicationOverview",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationOverview",
  "version" : "0.1.0",
  "name" : "MpMedicationOverview",
  "title" : "mp MedicationOverview",
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
  "description" : "Profile on the List resource which represents the medication overview conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
  "purpose" : "To define the medication overview as stated in the information standard Medication Process.",
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
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    },
    {
      "identity" : "w5",
      "uri" : "http://hl7.org/fhir/fivews",
      "name" : "FiveWs Pattern Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "List",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/List",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "List",
        "path" : "List",
        "short" : "DocumentData",
        "definition" : "Document data.",
        "alias" : ["Documentgegevens"],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-500",
            "comment" : "DocumentData"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-500",
            "comment" : "DocumentData"
          }
        ]
      },
      {
        "id" : "List.extension",
        "path" : "List.extension",
        "min" : 1
      },
      {
        "id" : "List.extension:verification",
        "path" : "List.extension",
        "sliceName" : "verification",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationOverview.Verification"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-506",
            "comment" : "VerificationPatient"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-506",
            "comment" : "VerificationPatient"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-509",
            "comment" : "VerificationHealthProfessional"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-509",
            "comment" : "VerificationHealthProfessional"
          }
        ]
      },
      {
        "id" : "List.extension:verification.extension:verificationPatient",
        "path" : "List.extension.extension",
        "sliceName" : "verificationPatient"
      },
      {
        "id" : "List.extension:verification.extension:verificationPatient.value[x]",
        "path" : "List.extension.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-507",
            "comment" : "VerifiedWithPatient?"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-507",
            "comment" : "VerifiedWithPatient?"
          }
        ]
      },
      {
        "id" : "List.extension:verification.extension:verificationPatientDate",
        "path" : "List.extension.extension",
        "sliceName" : "verificationPatientDate"
      },
      {
        "id" : "List.extension:verification.extension:verificationPatientDate.value[x]",
        "path" : "List.extension.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-508",
            "comment" : "VerificationDate"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-508",
            "comment" : "VerificationDate"
          }
        ]
      },
      {
        "id" : "List.extension:verification.extension:verificationHealthProfessional",
        "path" : "List.extension.extension",
        "sliceName" : "verificationHealthProfessional"
      },
      {
        "id" : "List.extension:verification.extension:verificationHealthProfessional.value[x]",
        "path" : "List.extension.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-510",
            "comment" : "VerifiedWithHealthProfessional?"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-510",
            "comment" : "VerifiedWithHealthProfessional?"
          }
        ]
      },
      {
        "id" : "List.extension:verification.extension:verificationHealthProfessionalDate",
        "path" : "List.extension.extension",
        "sliceName" : "verificationHealthProfessionalDate"
      },
      {
        "id" : "List.extension:verification.extension:verificationHealthProfessionalDate.value[x]",
        "path" : "List.extension.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-511",
            "comment" : "VerificationDate"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-511",
            "comment" : "VerificationDate"
          }
        ]
      },
      {
        "id" : "List.code",
        "path" : "List.code",
        "min" : 1,
        "patternCodeableConcept" : {
          "coding" : [
            {
              "system" : "http://snomed.info/sct",
              "code" : "11181000146103"
            }
          ]
        }
      },
      {
        "id" : "List.subject",
        "path" : "List.subject",
        "short" : "Patient",
        "alias" : ["Patient"],
        "min" : 1,
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : ["http://nictiz.nl/fhir/StructureDefinition/nl-core-Patient"]
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
        "id" : "List.date",
        "path" : "List.date",
        "short" : "DocumentDate",
        "definition" : "The time at which the medication overview was prepared.",
        "alias" : ["DocumentDatum"],
        "min" : 1,
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-501",
            "comment" : "DocumentDate"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-501",
            "comment" : "DocumentDate"
          }
        ]
      },
      {
        "id" : "List.source",
        "path" : "List.source",
        "short" : "Author",
        "alias" : ["Auteur"],
        "min" : 1,
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://hl7.org/fhir/StructureDefinition/Practitioner",
              "http://hl7.org/fhir/StructureDefinition/PractitionerRole",
              "http://hl7.org/fhir/StructureDefinition/Patient",
              "http://hl7.org/fhir/StructureDefinition/Device",
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-Patient"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-502",
            "comment" : "Author"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-502",
            "comment" : "Author"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-503",
            "comment" : "AuthorIsPatient (implicit; AuthorIsPatient = true when this element refers to the same Patient as subject)"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-503",
            "comment" : "AuthorIsPatient (implicit; AuthorIsPatient = true when this element refers to the same Patient as subject)"
          }
        ]
      },
      {
        "id" : "List.source.extension:organization",
        "path" : "List.source.extension",
        "sliceName" : "organization",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationOverview.SourceOrganization"
            ]
          }
        ]
      },
      {
        "id" : "List.source.extension:organization.value[x]",
        "path" : "List.source.extension.value[x]",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-504",
            "comment" : "AuthorIsHealthcareProvider"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-504",
            "comment" : "AuthorIsHealthcareProvider"
          }
        ]
      },
      {
        "id" : "List.entry",
        "path" : "List.entry",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "profile",
              "path" : "item.reference.resolve()"
            }
          ],
          "rules" : "open"
        }
      },
      {
        "id" : "List.entry:medicationAgreement",
        "path" : "List.entry",
        "sliceName" : "medicationAgreement"
      },
      {
        "id" : "List.entry:medicationAgreement.item",
        "path" : "List.entry.item",
        "short" : "MedicationAgreement",
        "alias" : ["Medicatieafspraak"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationAgreement"
            ],
            "aggregation" : ["bundled"]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-43",
            "comment" : "MedicationAgreement"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-43",
            "comment" : "MedicationAgreement"
          }
        ]
      },
      {
        "id" : "List.entry:administrationAgreement",
        "path" : "List.entry",
        "sliceName" : "administrationAgreement"
      },
      {
        "id" : "List.entry:administrationAgreement.item",
        "path" : "List.entry.item",
        "short" : "AdministrationAgreement",
        "alias" : ["Toedieningsafspraak"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-AdministrationAgreement"
            ],
            "aggregation" : ["bundled"]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-294",
            "comment" : "AdministrationAgreement"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-294",
            "comment" : "AdministrationAgreement"
          }
        ]
      },
      {
        "id" : "List.entry:medicationUse",
        "path" : "List.entry",
        "sliceName" : "medicationUse"
      },
      {
        "id" : "List.entry:medicationUse.item",
        "path" : "List.entry.item",
        "short" : "MedicationUse",
        "alias" : ["Medicatiegebruik"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationUse2"
            ],
            "aggregation" : ["bundled"]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-362",
            "comment" : "MedicationUse"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-362",
            "comment" : "MedicationUse"
          }
        ]
      },
      {
        "id" : "List.entry:pharmaceuticalProduct",
        "path" : "List.entry",
        "sliceName" : "pharmaceuticalProduct"
      },
      {
        "id" : "List.entry:pharmaceuticalProduct.item",
        "path" : "List.entry.item",
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-PharmaceuticalProduct"
            ]
          }
        ]
      },
      {
        "id" : "List.entry:bodyHeight",
        "path" : "List.entry",
        "sliceName" : "bodyHeight",
        "max" : "1"
      },
      {
        "id" : "List.entry:bodyHeight.item",
        "path" : "List.entry.item",
        "short" : "BodyHeight",
        "alias" : ["Lichaamslengte"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-BodyHeight"
            ],
            "aggregation" : ["bundled"]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-448",
            "comment" : "BodyHeight"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-448",
            "comment" : "BodyHeight"
          }
        ]
      },
      {
        "id" : "List.entry:bodyWeight",
        "path" : "List.entry",
        "sliceName" : "bodyWeight",
        "max" : "1"
      },
      {
        "id" : "List.entry:bodyWeight.item",
        "path" : "List.entry.item",
        "short" : "BodyWeight",
        "alias" : ["Lichaamsgewicht"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-BodyWeight"
            ],
            "aggregation" : ["bundled"]
          }
        ],
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-453",
            "comment" : "BodyWeight"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-453",
            "comment" : "BodyWeight"
          }
        ]
      }
    ]
  }
}

```
