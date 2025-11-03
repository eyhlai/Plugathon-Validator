# mp PharmaceuticalProduct - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp PharmaceuticalProduct**

## Resource Profile: mp PharmaceuticalProduct 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-PharmaceuticalProduct | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpPharmaceuticalProduct |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
The prescribed substance is usually medication. However, medical aids and bandages can also be prescribed and supplied via the pharmacy. Food and blood products do not strictly belong in the medication category, but can be prescribed and supplied by a pharmacy as well. 
A type of medication can be indicated with**a single code**. That code can be chosen from several possible coding systems (concretely: GPK, PRK, HPK or article numbers). Correct use of these codes in the software systems will sufficiently record the composition of the product used, making a complete product specification unnecessary. 
In addition to a primary code,**alternative codes**from other coding systems can also be entered (so that the GPK can be sent along in the event that the patient was registered based on PRK, for example). 
Entering multiple ingredients will enable you to display a compound product. If one of the composite parts is liquid, the dosage will be given in milliliters; otherwise it will be given in ‘units’. 
In that case, the**composition of the medication**can be specified implicitly (with the use of a medication code) or explicitly, for example by listing the (active) ingredient(s) of the medication. 
**Magistral prescriptions**can be entered as well. This can be done by means of the option listed above to enter coded ingredients and/or by entering the composition and preparation method as free text. This is a partial information model. 

 
This Medication resource represents the PharmaceuticalProduct building block for implementations following the information standard[MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) PharmaceuticalProduct, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set. 

**Usages:**

* Use this Profile: [mp MedicationPrescription Bundle](StructureDefinition-mp-MedicationPrescription-Bundle.md), [mp MedicationPrescriptionProcessing Bundle](StructureDefinition-mp-MedicationPrescriptionProcessing-Bundle.md), [mp ProposalDispenseRequest Bundle](StructureDefinition-mp-ProposalDispenseRequest-Bundle.md) and [mp ProposalMedicationAgreement Bundle](StructureDefinition-mp-ProposalMedicationAgreement-Bundle.md)
* Refer to this Profile: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md), [mp DispenseRequest](StructureDefinition-mp-DispenseRequest.md), [mp MedicationAdministration2](StructureDefinition-mp-MedicationAdministration2.md), [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md)...Show 4 more,[mp MedicationDispense](StructureDefinition-mp-MedicationDispense.md),[mp MedicationOverview](StructureDefinition-mp-MedicationOverview.md),[mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md)and[mp VariableDosingRegimen](StructureDefinition-mp-VariableDosingRegimen.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-PharmaceuticalProduct)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-PharmaceuticalProduct.csv), [Excel](StructureDefinition-mp-PharmaceuticalProduct.xlsx), [Schematron](StructureDefinition-mp-PharmaceuticalProduct.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-PharmaceuticalProduct",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-PharmaceuticalProduct",
  "version" : "0.1.0",
  "name" : "MpPharmaceuticalProduct",
  "title" : "mp PharmaceuticalProduct",
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
  "description" : "The prescribed substance is usually medication. However, medical aids and bandages can also be prescribed and supplied via the pharmacy. Food and blood products do not strictly belong in the medication category, but can be prescribed and supplied by a pharmacy as well.\r\n\r\nA type of medication can be indicated with **a single code**. That code can be chosen from several possible coding systems (concretely: GPK, PRK, HPK or article numbers). Correct use of these codes in the software systems will sufficiently record the composition of the product used, making a complete product specification unnecessary.\r\n\r\nIn addition to a primary code, **alternative codes** from other coding systems can also be entered (so that the GPK can be sent along in the event that the patient was registered based on PRK, for example).\r\n\r\nEntering multiple ingredients will enable you to display a compound product. If one of the composite parts is liquid, the dosage will be given in milliliters; otherwise it will be given in ‘units’.\r\n\r\nIn that case, the **composition of the medication** can be specified implicitly (with the use of a medication code) or explicitly, for example by listing the (active) ingredient(s) of the medication.\r\n\r\n**Magistral prescriptions** can be entered as well. This can be done by means of the option listed above to enter coded ingredients and/or by entering the composition and preparation method as free text.\r\nThis is a partial information model.",
  "purpose" : "This Medication resource represents the PharmaceuticalProduct building block for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) PharmaceuticalProduct, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "zib-pharmaceuticalproduct-v2.1.2-2020EN",
      "uri" : "https://zibs.nl/wiki/PharmaceuticalProduct-v2.1.2(2020EN)",
      "name" : "zib PharmaceuticalProduct-v2.1.2(2020EN)"
    },
    {
      "identity" : "mp-dataset-mp9-300-beta4-20241118",
      "uri" : "https://decor.nictiz.nl/pub/medicatieproces/mp-html-20241118T151205/ds-2.16.840.1.113883.2.4.3.11.60.20.77.1.4-2022-06-30T000000.html",
      "name" : "ART-DECOR Dataset MP9 3.0.0-beta.4 20241118"
    },
    {
      "identity" : "mp-dataset-mp9-300-rc1-20250522",
      "uri" : "https://decor.nictiz.nl/pub/medicatieproces/mp-html-20250522T132618/ds-2.16.840.1.113883.2.4.3.11.60.20.77.1.4-2022-06-30T000000.html",
      "name" : "ART-DECOR Dataset MP9 3.0.0-rc.1 20250522"
    },
    {
      "identity" : "script10.6",
      "uri" : "http://ncpdp.org/SCRIPT10_6",
      "name" : "Mapping to NCPDP SCRIPT 10.6"
    },
    {
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    },
    {
      "identity" : "w5",
      "uri" : "http://hl7.org/fhir/fivews",
      "name" : "FiveWs Pattern Mapping"
    },
    {
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
    }
  ],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Medication",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Medication",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Medication",
        "path" : "Medication",
        "short" : "PharmaceuticalProduct",
        "alias" : ["FarmaceutischProduct"],
        "mapping" : [
          {
            "identity" : "zib-pharmaceuticalproduct-v2.1.2-2020EN",
            "map" : "NL-CM:9.7.19926",
            "comment" : "PharmaceuticalProduct"
          }
        ]
      },
      {
        "id" : "Medication.extension:description",
        "path" : "Medication.extension",
        "sliceName" : "description",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-PharmaceuticalProduct.Description"
            ]
          }
        ],
        "constraint" : [
          {
            "key" : "ext-1",
            "severity" : "error",
            "human" : "Must have either extensions or value[x], not both",
            "source" : "http://hl7.org/fhir/StructureDefinition/DomainResource"
          }
        ]
      },
      {
        "id" : "Medication.code",
        "path" : "Medication.code",
        "short" : "MedicationCode",
        "definition" : "Coding medication in the Netherlands is done on the basis of the G-standaard (issued by Z-index), which is filled under the direction of Royal Dutch Pharmacists Association (KNMP).\r\n\r\nThe coded medication can be expressed as:\r\n\r\n* ZI number\r\n* Trade product code (HPK)\r\n* Prescription code (PRK)\r\n* Generic product code (GPK)\r\n\r\nThe ZI number represents the trade product and the package size.\r\nThe HPK is the trade product as registered and marketed by the manufacturer.\r\nThe PRK contains all GPK information supplemented with information needed to prescribe the right product. This level is intended to facilitate generic prescription of drugs.\r\nThe GPK defines the pharmaceutical characteristics of a product: ingredients, strengths, units, pharmaceutical form and route of administration.\r\n\r\nFurther information about the G-Standaard levels see <https://www.z-index.nl>.\r\n\r\nSo-called 90.000.000 numbers are used in local IT systems. The 90.000.000 number is used in accordance with national agreements.",
        "comment" : "Depending on the context of use, the code that was actually selected by the user (prescriber, dispenser, etc.) will have the `.coding.userSelected` set to _true_.  As described in the coding datatype: \"A coding may be marked as a \"userSelected\" if a user selected the particular coded value in a user interface (e.g. the user selects an item in a pick-list). If a user selected coding exists, it is the preferred choice for performing translations etc. Other codes can only be literal translations to alternative code systems, or codes at a lower level of granularity (e.g. a generic code for a vendor-specific primary one).\r\nIf there is no coding available, it is preferred to omit this `.coding` element. Receiving systems should anticipate on the possibility of receiving a NullFlavor from sending systems.",
        "alias" : ["ProductCode"],
        "binding" : {
          "strength" : "extensible",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.56--20230213120250"
        },
        "mapping" : [
          {
            "identity" : "zib-pharmaceuticalproduct-v2.1.2-2020EN",
            "map" : "NL-CM:9.7.19927",
            "comment" : "MedicationCode [DEPRECATED]"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-261",
            "comment" : "MedicationCode"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-261",
            "comment" : "MedicationCode"
          }
        ]
      },
      {
        "id" : "Medication.code.text",
        "path" : "Medication.code.text",
        "short" : "Medication",
        "definition" : "For medication which has no code, enter the complete name of the pharmaceutical product here.",
        "alias" : ["ProductNaam"],
        "mapping" : [
          {
            "identity" : "zib-pharmaceuticalproduct-v2.1.2-2020EN",
            "map" : "NL-CM:9.7.19929",
            "comment" : "Medication"
          }
        ]
      },
      {
        "id" : "Medication.manufacturer",
        "path" : "Medication.manufacturer",
        "constraint" : [
          {
            "key" : "ref-1",
            "severity" : "error",
            "human" : "SHALL have a contained resource if a local reference is provided",
            "source" : "http://hl7.org/fhir/StructureDefinition/Medication"
          }
        ]
      },
      {
        "id" : "Medication.form",
        "path" : "Medication.form",
        "short" : "PharmaceuticalForm",
        "definition" : "The pharmaceutical form indicates the form of the medication. Examples include: tablet, suppository, infusion liquid, ointment. If the product has a GPK code in the G standard, the form will be known in the G standard. For products without a code (free text, preparation by the pharmacy), the means of administration can be entered.",
        "alias" : ["FarmaceutischeVorm"],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.9.7.8--20200901000000"
        },
        "mapping" : [
          {
            "identity" : "zib-pharmaceuticalproduct-v2.1.2-2020EN",
            "map" : "NL-CM:9.7.19931",
            "comment" : "PharmaceuticalForm"
          }
        ]
      },
      {
        "id" : "Medication.amount",
        "path" : "Medication.amount",
        "constraint" : [
          {
            "key" : "rat-1",
            "severity" : "error",
            "human" : "Numerator and denominator SHALL both be present, or both are absent. If both are absent, there SHALL be some extension present",
            "source" : "http://hl7.org/fhir/StructureDefinition/Medication"
          }
        ]
      },
      {
        "id" : "Medication.ingredient",
        "path" : "Medication.ingredient",
        "short" : "Ingredient",
        "definition" : "A product contains one or more active substances and excipients. These are usually determined by the product code. For medication prepared or compounded by the local pharmacy, each ingredient must be entered separately.\r\n\r\nThe active substances play an important role, as they: a) determine the pharmacotherapeutic effect of the medication and b) serve as the basis for the indication of the strength of the medication (e.g. 200mg).",
        "alias" : ["Ingredient"],
        "mapping" : [
          {
            "identity" : "zib-pharmaceuticalproduct-v2.1.2-2020EN",
            "map" : "NL-CM:9.7.19932",
            "comment" : "Ingredient"
          }
        ]
      },
      {
        "id" : "Medication.ingredient.item[x]",
        "path" : "Medication.ingredient.item[x]",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "type",
              "path" : "$this"
            }
          ],
          "rules" : "open"
        }
      },
      {
        "id" : "Medication.ingredient.item[x]:itemCodeableConcept",
        "path" : "Medication.ingredient.item[x]",
        "sliceName" : "itemCodeableConcept",
        "short" : "SubstanceCode",
        "definition" : "Active substance or excipient. Here, the same codes can be used as for the MedicationCode (for dilutions and compounds in particular), but now, the ATC, SSK and SNK codes can also be used to indicate a substance (to list ingredients of local products prepared by the pharmacy).\r\n\r\n* ZI number\r\n* Trade product code (HPK)\r\n* Prescription code (PRK)\r\n* Generic product code (GPK)\r\n* Anatomical Therapeutic Chemical Classification (ATC)\r\n* Substance Name Code (SNK)\r\n* Substance Name Code, in combination with Route of Administration (SSK)\r\n\r\nFor further explanation about ATC see <https://www.whocc.no/atc/structure_and_principles/>.",
        "alias" : ["IngredientCode"],
        "type" : [
          {
            "code" : "CodeableConcept"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.121.11.13--20200901000000"
        },
        "mapping" : [
          {
            "identity" : "zib-pharmaceuticalproduct-v2.1.2-2020EN",
            "map" : "NL-CM:9.7.19934",
            "comment" : "SubstanceCode [DEPRECATED]"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-267",
            "comment" : "SubstanceCode"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-267",
            "comment" : "SubstanceCode"
          }
        ]
      },
      {
        "id" : "Medication.ingredient.strength",
        "path" : "Medication.ingredient.strength",
        "short" : "Concentration",
        "definition" : "The relative amount of this ingredient in this product.\r\nCalculation of Concentration = Ingredient Amount ÷ Product Amount.\r\n\r\nThis could be a concentration if the medication is dissolved in liquid, for example.",
        "alias" : ["Sterkte"],
        "constraint" : [
          {
            "key" : "rat-1",
            "severity" : "error",
            "human" : "Numerator and denominator SHALL both be present, or both are absent. If both are absent, there SHALL be some extension present",
            "source" : "http://hl7.org/fhir/StructureDefinition/Medication"
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-pharmaceuticalproduct-v2.1.2-2020EN",
            "map" : "NL-CM:9.7.19933",
            "comment" : "Concentration"
          }
        ]
      },
      {
        "id" : "Medication.ingredient.strength.numerator",
        "path" : "Medication.ingredient.strength.numerator",
        "short" : "IngredientAmount",
        "definition" : "The amount and unit of this ingredient. This is the numerator for the calculation of the concentration. The unit should be selected from the G-Standard (Table 902).",
        "alias" : ["IngredientHoeveelheid"],
        "type" : [
          {
            "code" : "Quantity",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-GstdSimpleQuantity"
            ]
          }
        ],
        "constraint" : [
          {
            "key" : "qty-3",
            "severity" : "error",
            "human" : "If a code for the unit is present, the system SHALL also be present",
            "source" : "http://hl7.org/fhir/StructureDefinition/Ratio"
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-pharmaceuticalproduct-v2.1.2-2020EN",
            "map" : "NL-CM:9.7.22277",
            "comment" : "IngredientAmount"
          }
        ]
      },
      {
        "id" : "Medication.ingredient.strength.denominator",
        "path" : "Medication.ingredient.strength.denominator",
        "short" : "ProductAmount",
        "definition" : "Amount of the product. This is the denominator for the calculation of the concentration. Optionally a translation to NHG table Gebruiksvoorschriften(Table 25) is also allowed.",
        "alias" : ["ProductHoeveelheid"],
        "type" : [
          {
            "code" : "Quantity",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-GstdSimpleQuantity"
            ]
          }
        ],
        "constraint" : [
          {
            "key" : "qty-3",
            "severity" : "error",
            "human" : "If a code for the unit is present, the system SHALL also be present",
            "source" : "http://hl7.org/fhir/StructureDefinition/Ratio"
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-pharmaceuticalproduct-v2.1.2-2020EN",
            "map" : "NL-CM:9.7.22278",
            "comment" : "ProductAmount"
          }
        ]
      }
    ]
  }
}

```
