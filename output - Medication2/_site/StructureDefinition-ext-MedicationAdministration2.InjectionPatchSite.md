# ext MedicationAdministration2.InjectionPatchSite - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext MedicationAdministration2.InjectionPatchSite**

## Extension: ext MedicationAdministration2.InjectionPatchSite 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAdministration2.InjectionPatchSite | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtMedicationAdministration2InjectionPatchSite |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide the site of the patient's body where an injection has been administered or where adhesive medical dressing has been applied.

This extension represents the InjectionPatchSite concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp MedicationAdministration2](StructureDefinition-mp-MedicationAdministration2.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-MedicationAdministration2.InjectionPatchSite)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-MedicationAdministration2.InjectionPatchSite.csv), [Excel](StructureDefinition-ext-MedicationAdministration2.InjectionPatchSite.xlsx), [Schematron](StructureDefinition-ext-MedicationAdministration2.InjectionPatchSite.sch) 

#### Terminologiebindings

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-MedicationAdministration2.InjectionPatchSite",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAdministration2.InjectionPatchSite",
  "version" : "0.1.0",
  "name" : "ExtMedicationAdministration2InjectionPatchSite",
  "title" : "ext MedicationAdministration2.InjectionPatchSite",
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
  "description" : "An extension to provide the site of the patient's body where an injection has been administered or where adhesive medical dressing has been applied.",
  "purpose" : "This extension represents the InjectionPatchSite concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
      "expression" : "MedicationAdministration"
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationAdministration2.InjectionPatchSite"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "InjectionPatchSite",
        "definition" : "Site of the patient's body where an injection has been administered or where adhesive medical dressing has been applied.",
        "alias" : ["PrikPlakLocatie"],
        "type" : [
          {
            "code" : "CodeableConcept"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.53--20220323181942"
        }
      },
      {
        "id" : "Extension.value[x].extension:laterality",
        "path" : "Extension.value[x].extension",
        "sliceName" : "laterality",
        "max" : "1",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-AnatomicalLocation.Laterality"
            ]
          }
        ]
      }
    ]
  }
}

```
