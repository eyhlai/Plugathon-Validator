# ext DispenseRequest.DispenseLocation - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext DispenseRequest.DispenseLocation**

## Extension: ext DispenseRequest.DispenseLocation 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.DispenseLocation | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtDispenseRequestDispenseLocation |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide a reference to the Location resource to indicate where the medication is (to be) dispensed.

This extension represents the DispenseLocation concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp DispenseRequest](StructureDefinition-mp-DispenseRequest.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-DispenseRequest.DispenseLocation)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-DispenseRequest.DispenseLocation.csv), [Excel](StructureDefinition-ext-DispenseRequest.DispenseLocation.xlsx), [Schematron](StructureDefinition-ext-DispenseRequest.DispenseLocation.sch) 

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-DispenseRequest.DispenseLocation",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.DispenseLocation",
  "version" : "0.1.0",
  "name" : "ExtDispenseRequestDispenseLocation",
  "title" : "ext DispenseRequest.DispenseLocation",
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
  "description" : "An extension to provide a reference to the Location resource to indicate where the medication is (to be) dispensed.",
  "purpose" : "This extension represents the DispenseLocation concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
      "expression" : "MedicationRequest.dispenseRequest"
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.DispenseLocation"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "DispenseLocation",
        "definition" : "Dispense location. Use `Location.name`.",
        "comment" : "Although the mapping is placed on this Reference element and not a string thereby deviating from the zib, the actual information will be a string in `Location.name`. A reference to a Location resource has been chosen over an extension with a string to allow for more detailed information to be captured in use cases not accounted for by the zib.",
        "alias" : ["Afleverlocatie"],
        "type" : [
          {
            "code" : "Reference",
            "targetProfile" : [
              "http://nictiz.nl/fhir/StructureDefinition/nl-core-HealthcareProvider"
            ]
          }
        ]
      }
    ]
  }
}

```
