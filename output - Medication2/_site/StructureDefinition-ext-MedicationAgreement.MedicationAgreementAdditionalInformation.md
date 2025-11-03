# ext MedicationAgreement.MedicationAgreementAdditionalInformation - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext MedicationAgreement.MedicationAgreementAdditionalInformation**

## Extension: ext MedicationAgreement.MedicationAgreementAdditionalInformation 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAgreement.MedicationAgreementAdditionalInformation | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtMedicationAgreementMedicationAgreementAdditionalInformation |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide additional information that includes details on the structure of the agreement made that are relevant for pharmacovigilance and fulfillment by the pharmacist. This can be used e.g. to indicate that there was a conscious decision to deviate from the norm or that the agreement is to be structured in a certain way.

This extension represents the MedicationAgreementAdditionalInformation concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-MedicationAgreement.MedicationAgreementAdditionalInformation)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-MedicationAgreement.MedicationAgreementAdditionalInformation.csv), [Excel](StructureDefinition-ext-MedicationAgreement.MedicationAgreementAdditionalInformation.xlsx), [Schematron](StructureDefinition-ext-MedicationAgreement.MedicationAgreementAdditionalInformation.sch) 

#### Terminologiebindings

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-MedicationAgreement.MedicationAgreementAdditionalInformation",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAgreement.MedicationAgreementAdditionalInformation",
  "version" : "0.1.0",
  "name" : "ExtMedicationAgreementMedicationAgreementAdditionalInformation",
  "title" : "ext MedicationAgreement.MedicationAgreementAdditionalInformation",
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
  "description" : "An extension to provide additional information that includes details on the structure of the agreement made that are relevant for pharmacovigilance and fulfillment by the pharmacist. This can be used e.g. to indicate that there was a conscious decision to deviate from the norm or that the agreement is to be structured in a certain way.",
  "purpose" : "This extension represents the MedicationAgreementAdditionalInformation concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
      "expression" : "MedicationRequest"
    }
  ],
  "type" : "Extension",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Extension",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Extension",
        "path" : "Extension"
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAgreement.MedicationAgreementAdditionalInformation"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "MedicationAgreementAdditionalInformation",
        "definition" : "Additional information includes details on the structure of the agreement made that are relevant for pharmacovigilance and fulfillment by the pharmacist. This can be used e.g. to indicate that there was a conscious decision to deviate from the norm or that the agreement is to be structured in a certain way.",
        "alias" : ["MedicatieafspraakAanvullendeInformatie"],
        "type" : [
          {
            "code" : "CodeableConcept"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.45--20220310164013"
        }
      }
    ]
  }
}

```
