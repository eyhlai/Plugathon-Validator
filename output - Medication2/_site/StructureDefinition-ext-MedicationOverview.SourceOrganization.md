# Ext MedicatonOverview.SourceOrganization - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **Ext MedicatonOverview.SourceOrganization**

## Extension: Ext MedicatonOverview.SourceOrganization 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-MedicationOverview.SourceOrganization | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtMedicationOverviewSourceOrganization |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

| | | |
| :--- | :--- | :--- |
| Extension to capture the organization that was the author/source of a List. This extends the current possible reference types (Practitioner | Patient | Device) so that it includes an Organization. |

In some cases an organization can be the author/source of a List. For example, in the information standard Medication Process, an organization is responsible for and the author of a Medication Overview. This extension allows to refer to an Organization resource to provide information on the author/source of a List.

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp MedicationOverview](StructureDefinition-mp-MedicationOverview.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-MedicationOverview.SourceOrganization)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-MedicationOverview.SourceOrganization.csv), [Excel](StructureDefinition-ext-MedicationOverview.SourceOrganization.xlsx), [Schematron](StructureDefinition-ext-MedicationOverview.SourceOrganization.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-MedicationOverview.SourceOrganization",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationOverview.SourceOrganization",
  "version" : "0.1.0",
  "name" : "ExtMedicationOverviewSourceOrganization",
  "title" : "Ext MedicatonOverview.SourceOrganization",
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
  "description" : "Extension to capture the organization that was the author/source of a List. This extends the current possible reference types (Practitioner | Patient | Device) so that it includes an Organization.",
  "purpose" : "In some cases an organization can be the author/source of a List. For example, in the information standard Medication Process, an organization is responsible for and the author of a Medication Overview. This extension allows to refer to an Organization resource to provide information on the author/source of a List.",
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
      "expression" : "List.source"
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationOverview.SourceOrganization"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "AuthorIsHealthcareProvider",
        "alias" : ["AuteurIsZorgaanbieder"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthcareProvider-Organization"
            ]
          }
        ]
      }
    ]
  }
}

```
