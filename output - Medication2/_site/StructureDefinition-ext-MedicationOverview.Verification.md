# Ext MedicatonOverview.Verification - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Ext MedicatonOverview.Verification**

## Extension: Ext MedicatonOverview.Verification 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-MedicationOverview.Verification | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtMedicationOverviewVerification |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

Extension to capture if a patient and/or health professional verified the medication overview and the corresponding date the verification took place.

To indicate if and when a medication overview is verified with a patient or health professional.

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp MedicationOverview](StructureDefinition-mp-MedicationOverview.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-MedicationOverview.Verification)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-MedicationOverview.Verification.csv), [Excel](StructureDefinition-ext-MedicationOverview.Verification.xlsx), [Schematron](StructureDefinition-ext-MedicationOverview.Verification.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-MedicationOverview.Verification",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationOverview.Verification",
  "version" : "0.1.0",
  "name" : "ExtMedicationOverviewVerification",
  "title" : "Ext MedicatonOverview.Verification",
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
  "description" : "Extension to capture if a patient and/or health professional verified the medication overview and the corresponding date the verification took place.",
  "purpose" : "To indicate if and when a medication overview is verified with a patient or health professional.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    }
  ],
  "kind" : "complex-type",
  "abstract" : false,
  "context" : [
    {
      "type" : "element",
      "expression" : "List"
    }
  ],
  "type" : "Extension",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Extension",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Extension",
        "path" : "Extension",
        "short" : "VerificationPatient / VerificationHealthProfessional",
        "definition" : "Verification with patient and health professional.",
        "alias" : ["VerificatiePatiënt", "VerificatieZorgverlener"],
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "Extension.extension",
        "path" : "Extension.extension",
        "min" : 2
      },
      {
        "id" : "Extension.extension:verificationPatient",
        "path" : "Extension.extension",
        "sliceName" : "verificationPatient",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "Extension.extension:verificationPatient.url",
        "path" : "Extension.extension.url",
        "fixedUri" : "verificationPatient"
      },
      {
        "id" : "Extension.extension:verificationPatient.value[x]",
        "path" : "Extension.extension.value[x]",
        "short" : "VerifiedWithPatient?",
        "definition" : "Verified with patient?",
        "alias" : ["GeverifieerdMetPatiënt?"],
        "type" : [
          {
            "code" : "boolean"
          }
        ]
      },
      {
        "id" : "Extension.extension:verificationPatientDate",
        "path" : "Extension.extension",
        "sliceName" : "verificationPatientDate",
        "max" : "1"
      },
      {
        "id" : "Extension.extension:verificationPatientDate.url",
        "path" : "Extension.extension.url",
        "fixedUri" : "verificationPatientDate"
      },
      {
        "id" : "Extension.extension:verificationPatientDate.value[x]",
        "path" : "Extension.extension.value[x]",
        "short" : "VerificationDate",
        "definition" : "Date of verification.",
        "alias" : ["VerificatieDatum"],
        "type" : [
          {
            "code" : "dateTime"
          }
        ]
      },
      {
        "id" : "Extension.extension:verificationHealthProfessional",
        "path" : "Extension.extension",
        "sliceName" : "verificationHealthProfessional",
        "min" : 1,
        "max" : "1"
      },
      {
        "id" : "Extension.extension:verificationHealthProfessional.url",
        "path" : "Extension.extension.url",
        "fixedUri" : "verificationHealthProfessional"
      },
      {
        "id" : "Extension.extension:verificationHealthProfessional.value[x]",
        "path" : "Extension.extension.value[x]",
        "short" : "VerifiedWithHealthProfessional?",
        "definition" : "Verified with health professional?",
        "alias" : ["GeverifieerdMetZorgverlener?"],
        "type" : [
          {
            "code" : "boolean"
          }
        ]
      },
      {
        "id" : "Extension.extension:verificationHealthProfessionalDate",
        "path" : "Extension.extension",
        "sliceName" : "verificationHealthProfessionalDate",
        "max" : "1"
      },
      {
        "id" : "Extension.extension:verificationHealthProfessionalDate.url",
        "path" : "Extension.extension.url",
        "fixedUri" : "verificationHealthProfessionalDate"
      },
      {
        "id" : "Extension.extension:verificationHealthProfessionalDate.value[x]",
        "path" : "Extension.extension.value[x]",
        "short" : "VerificationDate",
        "definition" : "Date of verification.",
        "alias" : ["VerificatieDatum"],
        "type" : [
          {
            "code" : "dateTime"
          }
        ]
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationOverview.Verification"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "max" : "0"
      }
    ]
  }
}

```
