# ext DispenseRequest.AdditionalWishes - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext DispenseRequest.AdditionalWishes**

## Extension: ext DispenseRequest.AdditionalWishes 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.AdditionalWishes | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtDispenseRequestAdditionalWishes |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide additional wishes that includes logistics and other instructions such as: do not enter in GDS, urgent, purposeful deviation, etc.

This extension represents the AdditionalWishes concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp DispenseRequest](StructureDefinition-mp-DispenseRequest.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-DispenseRequest.AdditionalWishes)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-DispenseRequest.AdditionalWishes.csv), [Excel](StructureDefinition-ext-DispenseRequest.AdditionalWishes.xlsx), [Schematron](StructureDefinition-ext-DispenseRequest.AdditionalWishes.sch) 

#### Terminologiebindings

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-DispenseRequest.AdditionalWishes",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.AdditionalWishes",
  "version" : "0.1.0",
  "name" : "ExtDispenseRequestAdditionalWishes",
  "title" : "ext DispenseRequest.AdditionalWishes",
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
  "description" : "An extension to provide additional wishes that includes logistics and other instructions such as: do not enter in GDS, urgent, purposeful deviation, etc.",
  "purpose" : "This extension represents the AdditionalWishes concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.AdditionalWishes"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "AdditionalWishes",
        "definition" : "Logistics and other instructions such as: do not enter in GDS, urgent, purposeful deviation, etc.",
        "alias" : ["AanvullendeWensen"],
        "type" : [
          {
            "code" : "CodeableConcept"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.32--20230109105413"
        }
      }
    ]
  }
}

```
