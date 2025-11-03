# ext DispenseRequest.FinancialIndicationCode - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **ext DispenseRequest.FinancialIndicationCode**

## Extension: ext DispenseRequest.FinancialIndicationCode 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.FinancialIndicationCode | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:ExtDispenseRequestFinancialIndicationCode |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

An extension that captures a financial indication code for reimbursement of a pharmaceutical product.

This extension represents the FinancialIndicationCode concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [mp DispenseRequest](StructureDefinition-mp-DispenseRequest.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/ext-DispenseRequest.FinancialIndicationCode)

### Formal Views of Extension Content

 [Description of Profiles, Differentials, Snapshots, and how the XML and JSON presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-ext-DispenseRequest.FinancialIndicationCode.csv), [Excel](StructureDefinition-ext-DispenseRequest.FinancialIndicationCode.xlsx), [Schematron](StructureDefinition-ext-DispenseRequest.FinancialIndicationCode.sch) 

#### Terminologiebindings

#### Constrains



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "ext-DispenseRequest.FinancialIndicationCode",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.FinancialIndicationCode",
  "version" : "0.1.0",
  "name" : "ExtDispenseRequestFinancialIndicationCode",
  "title" : "ext DispenseRequest.FinancialIndicationCode",
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
  "description" : "An extension that captures a financial indication code for reimbursement of a pharmaceutical product.",
  "purpose" : "This extension represents the FinancialIndicationCode concept for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces).",
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
        "path" : "Extension",
        "max" : "1"
      },
      {
        "id" : "Extension.url",
        "path" : "Extension.url",
        "fixedUri" : "http://nictiz.nl/fhir/StructureDefinition/ext-DispenseRequest.FinancialIndicationCode"
      },
      {
        "id" : "Extension.value[x]",
        "path" : "Extension.value[x]",
        "short" : "FinancialIndicationCode",
        "definition" : "A financial indication code used for reimbursement of the pharmaceutical product.",
        "comment" : "Applies to medication which is reimbursed based on the financial indication code.\r\n \r\nIn this element, several code systems can be used:\r\n \r\n* List indication codes (https://www.ordz.nl/huisartsen/documents/magazines/2022/05/lijst_indicatiecodes_huisartsen_2020/lijst-indicatiecodes-huisarts). Relevant for, among others, general practitioner care and mental health care. These values are exchanged using NullFlavor 'OTH' with the actual code (description) added as free text.\r\n \r\n* Declaration of add-on medicines. Relevant within specialist medical care. Codes from G-standard file 132 (Indication ID). INID: This field provides the indication ID, which connects the Z-Index number from the ZINR field with the corresponding indication(s). The indication ID is provided by the CIBG. (code 8 positions long).",
        "alias" : ["FinancieleIndicatiecode"],
        "type" : [
          {
            "code" : "CodeableConcept"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.57--20241101000000"
        }
      }
    ]
  }
}

```
