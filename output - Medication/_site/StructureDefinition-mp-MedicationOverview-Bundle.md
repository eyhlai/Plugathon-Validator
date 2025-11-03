# mp MedicationOverview Bundle - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp MedicationOverview Bundle**

## Resource Profile: mp MedicationOverview Bundle 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-MedicationOverview-Bundle | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpMedicationOverviewBundle |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
Profile on the Bundle resource which represents the structure of the Retrieve and Send MedicationOverview transactions conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). The output of the['$medication-overview'](https://simplifier.net/medicationprocess/medication-overview)operation (used in the former transaction) SHALL conform to this profile. 

 
To define the body of the Retrieve and Send MedicationOverview transactions. Moreover, this profile should provide guidance for servers in constructing the medication-overview operation outcome and enabling validation against it. For clients this profile should be helpful in expecting the response format of the medication-overview operation outcome. 

**Usages:**

* This Profile is not used by any profiles in this Implementation Guide

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-MedicationOverview-Bundle)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-MedicationOverview-Bundle.csv), [Excel](StructureDefinition-mp-MedicationOverview-Bundle.xlsx), [Schematron](StructureDefinition-mp-MedicationOverview-Bundle.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-MedicationOverview-Bundle",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationOverview-Bundle",
  "version" : "0.1.0",
  "name" : "MpMedicationOverviewBundle",
  "title" : "mp MedicationOverview Bundle",
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
  "description" : "Profile on the Bundle resource which represents the structure of the Retrieve and Send MedicationOverview transactions conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). The output of the ['$medication-overview'](https://simplifier.net/medicationprocess/medication-overview) operation (used in the former transaction) SHALL conform to this profile.",
  "purpose" : "To define the body of the Retrieve and Send MedicationOverview transactions. Moreover, this profile should provide guidance for servers in constructing the medication-overview operation outcome and enabling validation against it. For clients this profile should be helpful in expecting the response format of the medication-overview operation outcome.",
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
        "comment" : "In the Retrieve and Send MedicationOverview transactions this element should have the value 'searchset' and 'transaction', respectively."
      },
      {
        "id" : "Bundle.total",
        "path" : "Bundle.total",
        "comment" : "The total value contains the number of matching HCIMs: MedicationAgreement, AdministrationAgreement and MedicationUse2. Other included resources, such as Medication resources, are not included in the total. Note that this element is only used in the Retrieve MedicationOverview transaction."
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
        "id" : "Bundle.entry:list",
        "path" : "Bundle.entry",
        "sliceName" : "list",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "Bundle.entry:list.resource",
        "path" : "Bundle.entry.resource",
        "min" : 1,
        "type" : [
          {
            "code" : "Resource",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/mp-MedicationOverview"
            ]
          }
        ]
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
      }
    ]
  }
}

```
