# ext MedicationDispense.MedicationDispenseAdditionalInformation - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext MedicationDispense.MedicationDispenseAdditionalInformation**

## Extension: ext MedicationDispense.MedicationDispenseAdditionalInformation 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-MedicationDispense.MedicationDispenseAdditionalInformation | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtMedicationDispenseMedicationDispenseAdditionalInformation |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide additional information that includes details on the structure of the medical dispense. This can be e.g. a reason for deviating from the dispense request.

This extension represents the MedicationDispenseAdditionalInformation concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp MedicationDispense](StructureDefinition-mp-MedicationDispense.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-MedicationDispense.MedicationDispenseAdditionalInformation)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-MedicationDispense.MedicationDispenseAdditionalInformation.csv), [Excel](StructureDefinition-ext-MedicationDispense.MedicationDispenseAdditionalInformation.xlsx), [Schematron](StructureDefinition-ext-MedicationDispense.MedicationDispenseAdditionalInformation.sch) 

#### Terminologiebindings

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-MedicationDispense.MedicationDispenseAdditionalInformation",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationDispense.MedicationDispenseAdditionalInformation",
  "version" : "0.1.0",
  "name" : "ExtMedicationDispenseMedicationDispenseAdditionalInformation",
  "title" : "ext MedicationDispense.MedicationDispenseAdditionalInformation",
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
  "description" : "An extension to provide additional information that includes details on the structure of the medical dispense. This can be e.g. a reason for deviating from the dispense request.",
  "purpose" : "This extension represents the MedicationDispenseAdditionalInformation concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
      "expression" : "MedicationDispense"
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
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-MedicationDispense.MedicationDispenseAdditionalInformation"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "MedicationDispenseAdditionalInformation",
        "definition" : "Additional information includes details on the structure of the medical dispense. This can be e.g. a reason for deviating from the dispense request. For now, this list is used. This list will be replaced by a thesaurus in the G standard at a later stage.",
        "alias" : ["MedicatieverstrekkingAanvullendeInformatie"],
        "type" : [
          {
            "code" : "CodeableConcept"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.33--20170505131418"
        }
      }
    ]
  }
}

```
