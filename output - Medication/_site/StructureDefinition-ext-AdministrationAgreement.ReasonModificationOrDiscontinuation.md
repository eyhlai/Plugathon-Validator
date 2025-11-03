# ext AdministrationAgreement.ReasonModificationOrDiscontinuation - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext AdministrationAgreement.ReasonModificationOrDiscontinuation**

## Extension: ext AdministrationAgreement.ReasonModificationOrDiscontinuation 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-AdministrationAgreement.ReasonModificationOrDiscontinuation | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtAdministrationAgreementReasonModificationOrDiscontinuation |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension to provide a reason for modification or discontinuation of this agreement. This will often be the same reason as the one for modification or discontinuation of the medication agreement.

This extension represents the AdministrationAgreementReasonModificationOrDiscontinuation concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-AdministrationAgreement.ReasonModificationOrDiscontinuation)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-AdministrationAgreement.ReasonModificationOrDiscontinuation.csv), [Excel](StructureDefinition-ext-AdministrationAgreement.ReasonModificationOrDiscontinuation.xlsx), [Schematron](StructureDefinition-ext-AdministrationAgreement.ReasonModificationOrDiscontinuation.sch) 

#### Terminologiebindings

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-AdministrationAgreement.ReasonModificationOrDiscontinuation",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-AdministrationAgreement.ReasonModificationOrDiscontinuation",
  "version" : "0.1.0",
  "name" : "ExtAdministrationAgreementReasonModificationOrDiscontinuation",
  "title" : "ext AdministrationAgreement.ReasonModificationOrDiscontinuation",
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
  "description" : "An extension to provide a reason for modification or discontinuation of this agreement. This will often be the same reason as the one for modification or discontinuation of the medication agreement.",
  "purpose" : "This extension represents the AdministrationAgreementReasonModificationOrDiscontinuation concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
        "path" : "Extension",
        "max" : "1"
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-AdministrationAgreement.ReasonModificationOrDiscontinuation"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "AdministrationAgreementReasonModificationOrDiscontinuation",
        "definition" : "Reason for modification or discontinuation of this agreement. This will often be the same reason as the one for modification or discontinuation of the medication agreement.\r\n\r\nThis field has the option to - if applicable - enter a specific reason for modification or discontinuation of the administration agreement.",
        "alias" : ["ToedieningsafspraakRedenWijzigenOfStaken"],
        "type" : [
          {
            "code" : "CodeableConcept"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.49--20221115120643"
        }
      }
    ]
  }
}

```
