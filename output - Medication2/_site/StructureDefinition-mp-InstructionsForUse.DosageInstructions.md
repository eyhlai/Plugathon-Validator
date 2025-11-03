# mp InstructionsForUse.DosageInstructions - v0.1.0

* [**Table of Contents**](toc.md)
* [**Artifacts Summary**](artifacts.md)
* **mp InstructionsForUse.DosageInstructions**

## Data Type Profile: mp InstructionsForUse.DosageInstructions 

| | |
| :--- | :--- |
| *Official URL*:http://nictiz.nl/fhir/StructureDefinition/mp-InstructionsForUse.DosageInstructions | *Version*:0.1.0 |
| Active as of 2025-10-30 | *Computable Name*:MpInstructionsForUseDosageInstructions |
| **Copyright/Legal**: Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise. | |

 
Instructions for the use or administration of the medication, e.g. dose and route of administration. In the medication building block MedicationUse, this is the pattern of use established by the patient or which the patient followed. 

 
This Dosage data type profile**mainly**represents the DosingInstructions concept of the sub building block InstructionsForUse, for implementations following the information standard[MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) InstructionsForUse, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set. 
This profile also includes the concepts AdditionalInstructions and RouteOfAdministration. These concepts are placed on the same level as DosingInstructions in the zib, but are in FHIR part of the Dosage data type. As a consequence, these concepts may be duplicated if this Dosage profile is instantiated multiple times. 
This profile should be used in medication related resources that define dosage instructions and supplemented by the extensions[ext-RenderedDosageInstruction](http://nictiz.nl/fhir/StructureDefinition/ext-RenderedDosageInstruction)and[ext-InstructionsForUse.RepeatPeriodCyclicalSchedule](http://nictiz.nl/fhir/StructureDefinition/ext-InstructionsForUse.RepeatPeriodCyclicalSchedule)to implement the remaining concepts Description and RepeatPeriodCyclicalSchedule. 

**Usages:**

* Use this DataType Profile: [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md), [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md), [mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md) and [mp VariableDosingRegimen](StructureDefinition-mp-VariableDosingRegimen.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/example.org.fhir.plugathon.validation|current/StructureDefinition/mp-InstructionsForUse.DosageInstructions)

### Formal Views of Profile Content

 [Description of Profiles, Differentials, Snapshots and how the different presentations work](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](StructureDefinition-mp-InstructionsForUse.DosageInstructions.csv), [Excel](StructureDefinition-mp-InstructionsForUse.DosageInstructions.xlsx), [Schematron](StructureDefinition-mp-InstructionsForUse.DosageInstructions.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "mp-InstructionsForUse.DosageInstructions",
  "url" : "http://nictiz.nl/fhir/StructureDefinition/mp-InstructionsForUse.DosageInstructions",
  "version" : "0.1.0",
  "name" : "MpInstructionsForUseDosageInstructions",
  "title" : "mp InstructionsForUse.DosageInstructions",
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
  "description" : "Instructions for the use or administration of the medication, e.g. dose and route of administration. In the medication building block MedicationUse, this is the pattern of use established by the patient or which the patient followed.",
  "purpose" : "This Dosage data type profile _mainly_ represents the DosingInstructions concept of the sub building block InstructionsForUse, for implementations following the information standard [MP9](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). This profile is based on the Dutch zib ('Zorginformatiebouwsteen', i.e. Health and Care Information Model) InstructionsForUse, but has no dependency on the corresponding nl-core profile because it contains non-compatible changes. Where compatible, mappings to zib concepts are defined. Additional concepts or concepts that are not compatible with their zib counterparts contain a mapping to the MP9 data set.\n\nThis profile also includes the concepts AdditionalInstructions and RouteOfAdministration. These concepts are placed on the same level as DosingInstructions in the zib, but are in FHIR part of the Dosage data type. As a consequence, these concepts may be duplicated if this Dosage profile is instantiated multiple times.\n\nThis profile should be used in medication related resources that define dosage instructions and supplemented by the extensions [ext-RenderedDosageInstruction](http://nictiz.nl/fhir/StructureDefinition/ext-RenderedDosageInstruction) and [ext-InstructionsForUse.RepeatPeriodCyclicalSchedule](http://nictiz.nl/fhir/StructureDefinition/ext-InstructionsForUse.RepeatPeriodCyclicalSchedule) to implement the remaining concepts Description and RepeatPeriodCyclicalSchedule.",
  "copyright" : "Copyright and related rights waived via CC0, https://creativecommons.org/publicdomain/zero/1.0/. This does not apply to information from third parties, for example a medical terminology system. The implementer alone is responsible for identifying and obtaining any necessary licenses or authorizations to utilize third party IP in connection with the specification or otherwise.",
  "fhirVersion" : "4.0.1",
  "mapping" : [
    {
      "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
      "uri" : "https://zibs.nl/wiki/InstructionsForUse-v1.2.1(2020EN)",
      "name" : "zib InstructionsForUse-v1.2.1(2020EN)"
    },
    {
      "identity" : "zib-range-v1.0.1-2020EN",
      "uri" : "https://zibs.nl/wiki/Range-v1.0.1(2020EN)",
      "name" : "zib Range-v1.0.1(2020EN)"
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
      "identity" : "rim",
      "uri" : "http://hl7.org/v3",
      "name" : "RIM Mapping"
    },
    {
      "identity" : "v2",
      "uri" : "http://hl7.org/v2",
      "name" : "HL7 v2 Mapping"
    }
  ],
  "kind" : "complex-type",
  "abstract" : false,
  "type" : "Dosage",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Dosage",
  "derivation" : "constraint",
  "differential" : {
    "element" : [
      {
        "id" : "Dosage",
        "path" : "Dosage",
        "short" : "DosingInstructions",
        "definition" : "Indicates how the medication is/was taken or should be taken by the patient. Instructions for the administrator to administer the medication (the patient themselves, a nurse or other aid). When taking stock of medication use, the dosage describes the pattern of use established by the patient.",
        "comment" : "This element _mostly_ represents the DosingInstructions container from zib InstructionsForUse, but also includes the AdditionalInstructions and RouteOfAdministration concepts, which are normally placed on the same level as this container. As a result, these concepts are **duplicated** in every repetition of this element, even though these concepts should be present just once according to the zib.\r\n\r\nThis element does not contain a mapping to the Dosage container from zib InstructionsForUse. However, all child concepts of the Dosage concept are mapped. If an instance of zib container DosingInstructions contains multiple Dosage containers, each of these results in a separate instance of the FHIR Dosage data type conforming to this profile, wherein `.sequence` (zib concept SequenceNumber) and `.timing.repeat.bounds[x]:boundsDuration` (zib concept DoseDuration) are equal.",
        "alias" : ["Doseerinstructie"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.22095",
            "comment" : "DosingInstructions"
          }
        ]
      },
      {
        "id" : "Dosage.extension:asNeeded",
        "path" : "Dosage.extension",
        "sliceName" : "asNeeded",
        "type" : [
          {
            "code" : "Extension",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/ext-Dosage-AsNeededFor"
            ]
          }
        ]
      },
      {
        "id" : "Dosage.extension:asNeeded.value[x]",
        "path" : "Dosage.extension.value[x]",
        "short" : "Condition",
        "definition" : "The condition for administering medication can be:\r\n\r\n* a physiological measurement value (plasma glucose concentration, body temperature, blood pressure);\r\n* a symptom or other circumstance (in the event of a headache, or itch).\r\n\r\nSupplemental information from G-standard bst362 make up the list of values for coded entering of this concept. Also always include the textual description of that code. Physiological measurement values or other conditions that do not occur in bst362 do not need to be coded. These can be expressed in free text in the Description concept.",
        "alias" : ["Criterium"],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.9.12.4--20200901000000"
        },
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19945",
            "comment" : "Condition"
          }
        ]
      },
      {
        "id" : "Dosage.sequence",
        "path" : "Dosage.sequence",
        "short" : "SequenceNumber",
        "definition" : "This indicates the sequence of the dosing instructions within the medication agreement.",
        "alias" : ["Volgnummer"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.22503",
            "comment" : "SequenceNumber"
          }
        ]
      },
      {
        "id" : "Dosage.additionalInstruction",
        "path" : "Dosage.additionalInstruction",
        "short" : "AdditionalInstructions",
        "definition" : "The additional instructions contain extra information on the use of the current prescription. The additional instructions applies to the entire instructions for use and not to an individual dosage.\r\n\r\nThis includes all instructions for use. The text can come from the original “paper\" medication prescription, but can also be generated from the coded information.\r\n\r\nThe instructions may not conflict with other components of the medication agreement/ administration agreement.\r\n\r\nThe instructions can also refer to an existing protocol. In the case of an external dosing regimen (e.g., \"according to thrombosis service regimen\"), OTH is used.\r\n\r\nThe texts in the G-standard that can support this attribute are included in table 362 where the texts from the general practitioner' standard 'NHG-Tabel 25-component b: 'aanvullende teksten’ ' are included. These texts can only be used when it is not possible to include this information in the other structured elements of the Instructions for Use.\r\n\r\nA free-text explanation of the Instructions for Use can be placed under code OTH if it is not possible to record it in a structured manner within the Instructions for Use.",
        "comment" : "Please note that in contrast to the zib, this AdditionalInstructions concept is grouped under the DosingInstructions concept. This `.additionalInstruction` element shall have the same value when there are multiple DosingInstructions.",
        "alias" : ["AanvullendeInstructie"],
        "binding" : {
          "strength" : "required",
          "description" : "WCIAv3 Tabel 25 B-codes subset voor aanvullende gebruiksinstructies",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.20.77.11.9--20160407000000"
        },
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-51",
            "comment" : "AdditionalInstructions"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-51",
            "comment" : "AdditionalInstructions"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-649",
            "comment" : "AdditionalInstructions"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-649",
            "comment" : "AdditionalInstructions"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-300",
            "comment" : "AdditionalInstructions"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-300",
            "comment" : "AdditionalInstructions"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-368",
            "comment" : "AdditionalInstructions"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-368",
            "comment" : "AdditionalInstructions"
          }
        ]
      },
      {
        "id" : "Dosage.timing",
        "path" : "Dosage.timing",
        "short" : "AdministeringSchedule",
        "definition" : "Specifications of the times at which the medication is to be administered. This is indicated as follows:\r\n* Time(s) (16:00) or indications (“before meals”) at which the medication is to be taken each day.\r\n* A specific number of times the medication is to be taken each day (\"3x a day\"), indicated with the frequency.\r\n* A time interval between consecutive doses (“Every 2 hours”, “every 3 days”), indicated with the word Interval.\r\n* Combined periods with an interval and duration (“1 daily for three out of four weeks: the pill schedule”)\r\n\r\nIf a certain medication is not to be taken daily, the aforementioned can be combined with daily indications:\r\n\r\n* One or more week days on which the medication is to be administered (e.g. “Monday, Wednesday, Friday”)\r\n* ”3x a week”, “2x a month”.\r\n\r\nThe specified administration “infinite” is automatically to be repeated until:\r\n* The end date and time has been reached\r\n* The total administration duration has been reached (14 days)\r\n* A specific amount of administrations has been reached (“20 doses”), to be entered in the Frequency concept.",
        "alias" : ["Toedieningsschema"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19948",
            "comment" : "AdministeringSchedule"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.extension:timingExact",
        "path" : "Dosage.timing.repeat.extension",
        "sliceName" : "timingExact",
        "type" : [
          {
            "code" : "Extension",
            "profile" : ["http://hl7.org/fhir/StructureDefinition/timing-exact"]
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.extension:timingExact.value[x]",
        "path" : "Dosage.timing.repeat.extension.value[x]",
        "definition" : "Indicates that the timing as specified by `.frequency`, `.period` and `.periodUnit` should be strictly interpreted. This is the case when the zib concept Interval is expressed using these elements (as opposed to the zib concept Frequency).\r\n\r\nThe times can be chosen freely, but distribution throughout the day is more precise, and the interval between times is important (e.g. in the case of antibiotics). In the case of Baxter packs and intramural care, such a prescription is used to draw up a (location-specific) outline for distribution times (logistics).",
        "comment" : "Notes on the zib concepts Frequency and Interval:\n1. An interval (in FHIR) is just a normal frequency of 1 (combined with a period based on the interval length) and is represented in FHIR as just another frequency using `.frequency` (set to 1), `.period` and `.periodUnit`. However, the zib differentiates between the two concepts in the timing precision (the Interval concept defines precise intervals while the Frequency concept defines approximate intervals). When the interval is precise, this is communicated using the extension in `.extension:timingExact`.\n2. On the other hand, the zib Frequency concept might be used to express a single-use, non-repeating series by omitting the time unit. In FHIR, this is _not_ represented as a frequency, but with the `.count` element.\n3. Lastly, the Frequency concept may be used to express either a single nominal value or a range. A range is represented by respectively setting the minimum and maximum value to `.frequency` and `.frequencyMax`, or to `.count` and `.countMax` for single-use events. A nominal value is expressed by setting its value to `.frequency` or to `.count` for single-use events, and leaving `.frequencyMax` and `.countMax` unpopulated.\n\nIn summary:\n* zib concept Frequency:\n    * With time unit:\n        * Nominal value: `.frequency`, `.period` and `.periodUnit`\n        * Range: `.frequency`, `.frequencyMax`, `.period` and `.periodUnit`\n    * Without time unit:\n        * Nominal value: `.count`\n        * Range: `.count` and `.countMax`\n* zib concept Interval: `.frequency` (set to 1), `.period`, `.periodUnit` and `.extension:timingExact` (set to _true_)",
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19950",
            "comment" : "Interval (implicit, main mapping is on `.frequency`, `.period` and `.periodMax`)"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-271",
            "comment" : "(negative of) IsFlexible"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-271",
            "comment" : "(negative of) IsFlexible"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-672",
            "comment" : "(negative of) IsFlexible"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-672",
            "comment" : "(negative of) IsFlexible"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-580",
            "comment" : "(negative of) IsFlexible"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-580",
            "comment" : "(negative of) IsFlexible"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-412",
            "comment" : "(negative of) IsFlexible"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-412",
            "comment" : "(negative of) IsFlexible"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.bounds[x]",
        "path" : "Dosage.timing.repeat.bounds[x]",
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
        "id" : "Dosage.timing.repeat.bounds[x]:boundsDuration",
        "path" : "Dosage.timing.repeat.bounds[x]",
        "sliceName" : "boundsDuration",
        "short" : "DoseDuration",
        "definition" : "The intended time duration for these dosing instructions, e.g. 5 days or 8 weeks. \r\nIn the case of medication for an indefinite period, the dosing duration is left empty in the last dosing instruction.",
        "alias" : ["Doseerduur"],
        "type" : [
          {
            "code" : "Duration"
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.22506",
            "comment" : "DoseDuration"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.count",
        "path" : "Dosage.timing.repeat.count",
        "short" : "Frequency / minimumValue / nominalValue",
        "definition" : "Usually, frequency comprises both amount and time unit (3 times a day), but it can occur without the time unit (single use). This is represented by this `.count` element and optionally `.countMax` if a range should be represented.",
        "comment" : "Notes on the zib concept Frequency can be found in the comment of the `.frequency` element.",
        "alias" : ["Frequentie", "nominaleWaarde", "minimumWaarde"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19949",
            "comment" : "Frequency (single use only)"
          },
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.2",
            "comment" : "minimumValue"
          },
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.4",
            "comment" : "nominalValue"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.countMax",
        "path" : "Dosage.timing.repeat.countMax",
        "short" : "Frequency / maximumValue",
        "definition" : "Usually, frequency comprises both amount and time unit (3 times a day), but it can occur without the time unit (single use). This is represented by the `.count` element and optionally `.countMax` if a range should be represented.",
        "comment" : "Notes on the zib concept Frequency can be found in the comment of the `.frequency` element.",
        "alias" : ["Frequentie", "maximumWaarde"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19949",
            "comment" : "Frequency"
          },
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.3",
            "comment" : "maximumValue"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.duration",
        "path" : "Dosage.timing.repeat.duration",
        "short" : "DurationOfAdministration",
        "definition" : "The duration of administration defines the length of time during which the drug is administered and is mainly used in the slow parenteral administration of fluids. The `durationUnit` defines the time unit.",
        "alias" : ["Toedieningsduur"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.23141",
            "comment" : "DurationOfAdministration"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.durationUnit",
        "path" : "Dosage.timing.repeat.durationUnit",
        "short" : "DurationOfAdministration",
        "definition" : "The units of time, in UCUM units, for the duration of administration of time during which the drug is administered.",
        "alias" : ["Toedieningsduur"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.23141",
            "comment" : "DurationOfAdministration"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.frequency",
        "path" : "Dosage.timing.repeat.frequency",
        "short" : "Frequency / minimumValue / nominalValue / Interval",
        "definition" : "The `.frequency` element indicates either the number of dose moments per time unit (zib concept Frequency) or the time between dose times (zib concept Interval).\r\n\r\nIf `.frequencyMax` is present, this `.frequency`  element indicates the lower bound of the allowed range of the frequency.",
        "comment" : "Notes on the zib concepts Frequency and Interval, The zib differentiates between the two concepts in the specific usage of the extension `.extension:timingExact` and the element `.timeOfDay` combined:\n1. The zib Interval (in FHIR) is just a normal frequency of 1 (combined with a period based on the interval length) and is represented in FHIR as just another frequency using `.frequency` (set to 1), `.period`, `.periodUnit`, the extension `.extension:timingExact` set to _true_ and the absence of the element `.timeOfDay`.\n2. The zib Frequency concept might be used to express a single-use, non-repeating series by omitting the time unit. In FHIR, this is _not_ represented as a frequency, but with the `.count` element.\n3. Lastly, the Frequency concept may be used to express either a single nominal value or a range. The extension `.extension:timingExact` can be used to specify the precision of the timing of the administration (i.e. the element `.timeOfDay`). When this element is meant to convey the zib Frequency concept this can be, unlike the zib concept Interval, either _true_or _false_. A range is represented by respectively setting the minimum and maximum value to `.frequency` and `.frequencyMax`, or to `.count` and `.countMax` for single-use events as mentioned in the second point. A nominal value is expressed by setting its value to `.frequency` or to `.count` for single-use events, and leaving `.frequencyMax` and `.countMax` unpopulated.\n\nIn summary:\n* zib concept Frequency:\n    * With time unit (precision of the timing can be further specified with the extension `.extension:timingExact`):\n        * Nominal value: `.frequency`, `.period` and `.periodUnit`\n        * Range: `.frequency`, `.frequencyMax`, `.period` and `.periodUnit`\n    * Without time unit:\n        * Nominal value: `.count`\n        * Range: `.count` and `.countMax`\n* zib concept Interval: `.frequency` (set to 1), `.period`, `.periodUnit`, `.extension:timingExact` (SHALL be set to _true_) and the absence of `.timeOfDay`.",
        "alias" : ["Frequentie", "minimumWaarde", "nominaleWaarde", "Interval"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19949",
            "comment" : "Frequency"
          },
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.2",
            "comment" : "minimumValue"
          },
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.4",
            "comment" : "nominalValue"
          },
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19950",
            "comment" : "Interval"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.frequencyMax",
        "path" : "Dosage.timing.repeat.frequencyMax",
        "short" : "Frequency / maximumValue",
        "comment" : "Notes on the zib concept Frequency can be found in the comment of the `.frequency` element.",
        "alias" : ["maximumWaarde", "Frequentie"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19949",
            "comment" : "Frequency"
          },
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.3",
            "comment" : "maximumValue"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.period",
        "path" : "Dosage.timing.repeat.period",
        "short" : "Frequency / Interval",
        "definition" : "Indicates the duration of time over which repetitions are to occur; e.g. to express \"3 times per day\", 3 would be the frequency and \"1 day\" would be the period. If `.periodMax` is present, this element indicates the lower bound of the allowed range of the period length.",
        "comment" : "Notes on the zib concepts Frequency and Interval can be found in the comment of the `.frequency` element.",
        "alias" : ["Frequentie", "Interval"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19949",
            "comment" : "Frequency"
          },
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19950",
            "comment" : "Interval"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.periodUnit",
        "path" : "Dosage.timing.repeat.periodUnit",
        "short" : "Frequency / Interval",
        "definition" : "The units of time for the period in UCUM units for Frequency and Interval.",
        "comment" : "Notes on the zib concepts Frequency and Interval can be found in the comment of the `.frequency` element.",
        "alias" : ["Frequentie", "Interval"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19949",
            "comment" : "Frequency. When frequency is used, set `.extension.timingExact` to false."
          },
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19950",
            "comment" : "Interval"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.dayOfWeek",
        "path" : "Dosage.timing.repeat.dayOfWeek",
        "short" : "WeekDay",
        "definition" : "WeekDay indicates a pattern of doses on fixed week days.",
        "comment" : "If no days are specified, the action is assumed to happen every day as otherwise specified.",
        "alias" : ["Weekdag"],
        "binding" : {
          "strength" : "required",
          "description" : "Use ConceptMap 'WeekdagCodelijst_to_DaysOfWeek' to translate zib terminology to profile terminology in ValueSet 'DaysOfWeek'",
          "valueSet" : "http://hl7.org/fhir/ValueSet/days-of-week|4.0.1",
          "_valueSet" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/11179-permitted-value-conceptmap",
                "valueCanonical" : "http://nictiz.nl/fhir/ConceptMap/WeekdagCodelijst-to-DaysOfWeek"
              }
            ]
          }
        },
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19952",
            "comment" : "WeekDay"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.timeOfDay",
        "path" : "Dosage.timing.repeat.timeOfDay",
        "short" : "AdministrationTime",
        "definition" : "The time of administration is a specific time of day (on the clock). This time usually isn’t (intended to be) exact. There can be multiple administering times in one day. \r\n\r\nThe ideal time of administration can also be entered as a time of day (morning, afternoon, evening, night-time). The administration time is then to be left empty, and the time of day can be entered in the TimeOfDay concept.",
        "comment" : "If there's a `.timeOfDay`, there cannot be a `.when`, or vice versa.",
        "alias" : ["Toedientijd"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19951",
            "comment" : "AdministrationTime"
          }
        ]
      },
      {
        "id" : "Dosage.timing.repeat.when",
        "path" : "Dosage.timing.repeat.when",
        "short" : "TimeOfDay",
        "definition" : "Time of day: morning, afternoon, evening, night.",
        "comment" : "If there's a `.timeOfDay`, there cannot be a `.when`, or vice versa.",
        "alias" : ["Dagdeel"],
        "binding" : {
          "strength" : "required",
          "description" : "Use ConceptMap 'DagdeelCodelijst_to_EventTiming' to translate zib terminology to profile terminology in ValueSet 'EventTiming'",
          "valueSet" : "http://hl7.org/fhir/ValueSet/event-timing",
          "_valueSet" : {
            "extension" : [
              {
                "url" : "http://hl7.org/fhir/StructureDefinition/11179-permitted-value-conceptmap",
                "valueCanonical" : "http://nictiz.nl/fhir/ConceptMap/DagdeelCodelijst-to-EventTiming"
              }
            ]
          }
        },
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19953",
            "comment" : "TimeOfDay"
          }
        ]
      },
      {
        "id" : "Dosage.asNeeded[x]",
        "path" : "Dosage.asNeeded[x]",
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
        "id" : "Dosage.asNeeded[x]:asNeededCodeableConcept",
        "path" : "Dosage.asNeeded[x]",
        "sliceName" : "asNeededCodeableConcept",
        "short" : "Condition",
        "definition" : "The condition for administering medication can be:\r\n\r\n* a physiological measurement value (plasma glucose concentration, body temperature, blood pressure);\r\n* a symptom or other circumstance (in the event of a headache, or itch).\r\n\r\nSupplemental information from G-standard bst362 make up the list of values for coded entering of this concept. Also always include the textual description of that code. Physiological measurement values or other conditions that do not occur in bst362 do not need to be coded. These can be expressed in free text in the Description concept.",
        "alias" : ["Criterium"],
        "type" : [
          {
            "code" : "CodeableConcept"
          }
        ],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.9.12.4--20200901000000"
        },
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19945",
            "comment" : "Condition"
          }
        ]
      },
      {
        "id" : "Dosage.asNeeded[x]:asNeededCodeableConcept.text",
        "path" : "Dosage.asNeeded[x].text",
        "mapping" : [
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-272",
            "comment" : "Description"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-272",
            "comment" : "Description"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-677",
            "comment" : "Description"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-677",
            "comment" : "Description"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-582",
            "comment" : "Description"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-582",
            "comment" : "Description"
          },
          {
            "identity" : "mp-dataset-mp9-300-beta4-20241118",
            "map" : "mp-dataelement9x-514",
            "comment" : "Description"
          },
          {
            "identity" : "mp-dataset-mp9-300-rc1-20250522",
            "map" : "mp-dataelement9x-514",
            "comment" : "Description"
          }
        ]
      },
      {
        "id" : "Dosage.route",
        "path" : "Dosage.route",
        "short" : "RouteOfAdministration",
        "definition" : "The route through which the medication is administered (oral, nasal, intravenous, etc.).",
        "comment" : "Please note that in contrast to the zib, this RouteOfAdministration concept is grouped under the DosingInstructions concept. This `.route` element shall have the same value when there are multiple DosingInstructions.",
        "alias" : ["Toedieningsweg"],
        "binding" : {
          "strength" : "required",
          "valueSet" : "http://decor.nictiz.nl/fhir/ValueSet/2.16.840.1.113883.2.4.3.11.60.40.2.9.12.1--20200901000000"
        },
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19941",
            "comment" : "RouteOfAdministration"
          }
        ]
      },
      {
        "id" : "Dosage.doseAndRate.dose[x]",
        "path" : "Dosage.doseAndRate.dose[x]",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "type",
              "path" : "$this"
            }
          ],
          "rules" : "open"
        },
        "short" : "Dose",
        "definition" : "The dose indicates the amount/unit per administration. The unit can be any unit that can occur with this particular medicine.",
        "alias" : ["Keerdosis"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19940",
            "comment" : "Dose"
          }
        ]
      },
      {
        "id" : "Dosage.doseAndRate.dose[x]:doseRange",
        "path" : "Dosage.doseAndRate.dose[x]",
        "sliceName" : "doseRange",
        "type" : [
          {
            "code" : "Range"
          }
        ]
      },
      {
        "id" : "Dosage.doseAndRate.dose[x]:doseRange.low",
        "path" : "Dosage.doseAndRate.dose[x].low",
        "short" : "minimumValue",
        "definition" : "The minimal value of the range. The boundary is inclusive.",
        "alias" : ["minimumWaarde"],
        "type" : [
          {
            "code" : "Quantity",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-GstdSimpleQuantity"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.2",
            "comment" : "minimumValue"
          }
        ]
      },
      {
        "id" : "Dosage.doseAndRate.dose[x]:doseRange.high",
        "path" : "Dosage.doseAndRate.dose[x].high",
        "short" : "maximumValue",
        "definition" : "The maximum value of the range. The boundary is inclusive.",
        "alias" : ["maximumWaarde"],
        "type" : [
          {
            "code" : "Quantity",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-GstdSimpleQuantity"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.3",
            "comment" : "maximumValue"
          }
        ]
      },
      {
        "id" : "Dosage.doseAndRate.dose[x]:doseQuantity",
        "path" : "Dosage.doseAndRate.dose[x]",
        "sliceName" : "doseQuantity",
        "short" : "nominalValue",
        "definition" : "Amount of medication per dose. The nominal value of the quantity.",
        "alias" : ["nominaleWaarde"],
        "type" : [
          {
            "code" : "Quantity",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-GstdSimpleQuantity"
            ]
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.4",
            "comment" : "nominalValue"
          }
        ]
      },
      {
        "id" : "Dosage.doseAndRate.rate[x]",
        "path" : "Dosage.doseAndRate.rate[x]",
        "slicing" : {
          "discriminator" : [
            {
              "type" : "type",
              "path" : "$this"
            }
          ],
          "rules" : "open"
        },
        "short" : "AdministeringSpeed",
        "definition" : "The administering speed is used in slow administration of liquid. In practice, the measuring unit is almost always ml/hour, but can also be parametric with i.e. body weight or body surface area (in the case of a MedicationAgreement, VariableDosingRegimen or AdministrationAgreement). Entering an interval (such as 0-10 ml/hour) is also a commonly used option.\r\n\nFor example, with an administering speed of 10ml/hour:\r\n* value = 10\r\n* unit = ml/hour",
        "alias" : ["Toedieningssnelheid"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19942",
            "comment" : "AdministeringSpeed"
          }
        ]
      },
      {
        "id" : "Dosage.doseAndRate.rate[x]:rateRange",
        "path" : "Dosage.doseAndRate.rate[x]",
        "sliceName" : "rateRange",
        "type" : [
          {
            "code" : "Range"
          }
        ]
      },
      {
        "id" : "Dosage.doseAndRate.rate[x]:rateRange.low",
        "path" : "Dosage.doseAndRate.rate[x].low",
        "short" : "minimumValue",
        "definition" : "The minimal value of the range. The boundary is inclusive.",
        "alias" : ["minimumWaarde"],
        "mapping" : [
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.2",
            "comment" : "minimumValue"
          }
        ]
      },
      {
        "id" : "Dosage.doseAndRate.rate[x]:rateRange.high",
        "path" : "Dosage.doseAndRate.rate[x].high",
        "short" : "maximumValue",
        "definition" : "The maximum value of the range. The boundary is inclusive.",
        "alias" : ["maximumWaarde"],
        "mapping" : [
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.3",
            "comment" : "maximumValue"
          }
        ]
      },
      {
        "id" : "Dosage.doseAndRate.rate[x]:rateQuantity",
        "path" : "Dosage.doseAndRate.rate[x]",
        "sliceName" : "rateQuantity",
        "short" : "nominalValue",
        "definition" : "The nominal value of the quantity.",
        "alias" : ["nominaleWaarde"],
        "type" : [
          {
            "code" : "Quantity"
          }
        ],
        "mapping" : [
          {
            "identity" : "zib-range-v1.0.1-2020EN",
            "map" : "NL-CM:20.1.4",
            "comment" : "nominalValue"
          }
        ]
      },
      {
        "id" : "Dosage.maxDosePerPeriod",
        "path" : "Dosage.maxDosePerPeriod",
        "short" : "MaximumDose",
        "definition" : "A maximum dose maximizes (in time) the usage of a drug in an 'as needed' prescription.",
        "alias" : ["MaximaleDosering"],
        "mapping" : [
          {
            "identity" : "zib-instructionsforuse-v1.2.1-2020EN",
            "map" : "NL-CM:9.12.19946",
            "comment" : "MaximumDose"
          }
        ]
      },
      {
        "id" : "Dosage.maxDosePerPeriod.numerator",
        "path" : "Dosage.maxDosePerPeriod.numerator",
        "type" : [
          {
            "code" : "Quantity",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-GstdSimpleQuantity"
            ]
          }
        ]
      },
      {
        "id" : "Dosage.maxDosePerPeriod.denominator",
        "path" : "Dosage.maxDosePerPeriod.denominator",
        "type" : [
          {
            "code" : "Quantity",
            "profile" : [
              "http://nictiz.nl/fhir/StructureDefinition/pattern-GstdSimpleQuantity"
            ]
          }
        ]
      }
    ]
  }
}

```
