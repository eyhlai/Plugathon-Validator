# ext StopType - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext StopType**

## Extension: ext StopType 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-StopType | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtStopType |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide the manner in which medication is discontinued (temporary or definitive).

This extension represents the MedicationAgreementStopType and AdministrationAgreementStopType concepts, and the MedicationUseStopType and VariableDosingRegimenStopType concepts which have a binding on a more restricted ValueSet, of the MedicationProcess9 information standard.

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md), [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md), [mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md) and [mp VariableDosingRegimen](StructureDefinition-mp-VariableDosingRegimen.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-StopType)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-StopType.csv), [Excel](StructureDefinition-ext-StopType.xlsx), [Schematron](StructureDefinition-ext-StopType.sch) 

#### Terminologiebindings

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-StopType",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-StopType",
  "version" : "0.1.0",
  "name" : "ExtStopType",
  "title" : "ext StopType",
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
  "description" : "An extension to provide the manner in which medication is discontinued (temporary or definitive).",
  "purpose" : "This extension represents the MedicationAgreementStopType and AdministrationAgreementStopType concepts, and the MedicationUseStopType and VariableDosingRegimenStopType concepts which have a binding on a more restricted ValueSet, of the MedicationProcess9 information standard.",
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
    },
    {
      "type" : "element",
      "expression" : "MedicationDispense"
    },
    {
      "type" : "element",
      "expression" : "MedicationStatement"
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
        "definition" : "This StopType modifier extension works differently than the `.status` element of resources because it has a different meaning. The `.status` element usually represents the status of the resource at the moment of exchanging the resource. This means that over the lifetime of a resource, the status may change (and is very much related to use period). That – in itself – makes solely mapping StopType (which may never change in an instance) to `.status` not suitable.\r\n\r\nFor example: suppose you want the patient to stop taking medication definitively three days from today. This is a stop medication agreement with a StopType of _definitive_. However today, tomorrow and the day after tomorrow the `.status` of this medication agreement is _active_ and only after the end date of the usage period the `.status` should be _stopped_. Status and StopType are simply not the same thing.",
        "max" : "1",
        "isModifier" : true,
        "isModifierReason" : "This element is labeled as a modifier because StopType contains codes that mark the resource as no longer active."
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-StopType"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "StopType",
        "definition" : "Stop type, the manner in which this medication is discontinued or canceled (temporary, definitive or canceled).",
        "type" : [
          {
            "code" : "CodeableConcept"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.50--20221216102010"
        }
      }
    ]
  }
}

```
