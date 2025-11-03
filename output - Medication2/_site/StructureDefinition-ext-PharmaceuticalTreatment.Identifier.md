# ext PharmaceuticalTreatment.Identifier - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext PharmaceuticalTreatment.Identifier**

## Extension: ext PharmaceuticalTreatment.Identifier 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-PharmaceuticalTreatment.Identifier | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtPharmaceuticalTreatmentIdentifier |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

This extension provides an identifier to unambiguously identify the set of interdependent medication building blocks that belong to one pharmaceutical treatment.

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md), [mp DispenseRequest](StructureDefinition-mp-DispenseRequest.md), [mp MedicationAdministration2](StructureDefinition-mp-MedicationAdministration2.md), [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md)...Show 3 more,[mp MedicationDispense](StructureDefinition-mp-MedicationDispense.md),[mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md)and[mp VariableDosingRegimen](StructureDefinition-mp-VariableDosingRegimen.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-PharmaceuticalTreatment.Identifier)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-PharmaceuticalTreatment.Identifier.csv), [Excel](StructureDefinition-ext-PharmaceuticalTreatment.Identifier.xlsx), [Schematron](StructureDefinition-ext-PharmaceuticalTreatment.Identifier.sch) 

#### Terminologiebindings

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-PharmaceuticalTreatment.Identifier",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-PharmaceuticalTreatment.Identifier",
  "version" : "0.1.0",
  "name" : "ExtPharmaceuticalTreatmentIdentifier",
  "title" : "ext PharmaceuticalTreatment.Identifier",
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
  "description" : "This extension provides an identifier to unambiguously identify the set of interdependent medication building blocks that belong to one pharmaceutical treatment.",
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
      "expression" : "MedicationStatement"
    },
    {
      "type" : "element",
      "expression" : "MedicationAdministration"
    },
    {
      "type" : "element",
      "expression" : "MedicationDispense"
    },
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
        "path" : "Extension",
        "max" : "1"
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-PharmaceuticalTreatment.Identifier"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "Pharmaceutical Treatment Identifier",
        "definition" : "The identifier of the pharmaceutical treatment that this resource belongs to. This identifier is used to group the disparate resources that belong to a single pharmaceutical treatment.",
        "alias" : ["Medicamenteuze behandeling identificatie"],
        "type" : [
          {
            "code" : "Identifier"
          }
        ]
      },
      {
        "id" : "Extension.value[x].system",
        "path" : "Extension.value[x].system",
        "min" : 1
      },
      {
        "id" : "Extension.value[x].value",
        "path" : "Extension.value[x].value",
        "min" : 1
      }
    ]
  }
}

```
