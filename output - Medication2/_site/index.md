# Plugathon validation IG - v0.1.0

* [**Table of Contents**](toc.md)
* **Plugathon validation IG**

## Plugathon validation IG

| | |
| :--- | :--- |
| *Official URL*:http://example.org/fhir/PlugathonValidationIG/ImplementationGuide/example.org.fhir.plugathon.validation | *Version*:0.1.0 |
| Draft as of 2025-10-30 | *Computable Name*:PlugathonValidationIG |

See the [QA results](qa.md).



## Resource Content

```json
{
  "resourceType" : "ImplementationGuide",
  "id" : "example.org.fhir.plugathon.validation",
  "language" : "en-US",
  "url" : "http://example.org/fhir/PlugathonValidationIG/ImplementationGuide/example.org.fhir.plugathon.validation",
  "version" : "0.1.0",
  "name" : "PlugathonValidationIG",
  "status" : "draft",
  "experimental" : true,
  "date" : "2025-10-30T15:05:26+00:00",
  "packageId" : "example.org.fhir.plugathon.validation",
  "license" : "CC0-1.0",
  "fhirVersion" : ["4.0.1"],
  "dependsOn" : [
    {
      "id" : "hl7tx",
      "extension" : [
        {
          "url" : "http://hl7.org/fhir/tools/StructureDefinition/implementationguide-dependency-comment",
          "valueMarkdown" : "Automatically added as a dependency - all IGs depend on HL7 Terminology"
        }
      ],
      "uri" : "http://terminology.hl7.org/ImplementationGuide/hl7.terminology",
      "packageId" : "hl7.terminology.r4",
      "version" : "6.5.0"
    },
    {
      "id" : "hl7ext",
      "extension" : [
        {
          "url" : "http://hl7.org/fhir/tools/StructureDefinition/implementationguide-dependency-comment",
          "valueMarkdown" : "Automatically added as a dependency - all IGs depend on the HL7 Extension Pack"
        }
      ],
      "uri" : "http://hl7.org/fhir/extensions/ImplementationGuide/hl7.fhir.uv.extensions",
      "packageId" : "hl7.fhir.uv.extensions.r4",
      "version" : "5.2.0"
    },
    {
      "uri" : "http://hl7.eu/fhir/mpd/ImplementationGuide/hl7.fhir.eu.mpd",
      "packageId" : "hl7.fhir.eu.mpd",
      "version" : "0.1.0-ballot"
    }
  ],
  "definition" : {
    "extension" : [
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "i18n-default-lang"
          },
          {
            "url" : "value",
            "valueString" : "nl-NL"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "autoload-resources"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "path-liquid"
          },
          {
            "url" : "value",
            "valueString" : "template/liquid"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "path-liquid"
          },
          {
            "url" : "value",
            "valueString" : "input/liquid"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "path-qa"
          },
          {
            "url" : "value",
            "valueString" : "temp/qa"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "path-temp"
          },
          {
            "url" : "value",
            "valueString" : "temp/pages"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "path-output"
          },
          {
            "url" : "value",
            "valueString" : "output"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "path-suppressed-warnings"
          },
          {
            "url" : "value",
            "valueString" : "input/ignoreWarnings.txt"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "path-history"
          },
          {
            "url" : "value",
            "valueString" : "http://example.org/fhir/PlugathonValidationIG/history.html"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "template-html"
          },
          {
            "url" : "value",
            "valueString" : "template-page.html"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "template-md"
          },
          {
            "url" : "value",
            "valueString" : "template-page-md.html"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "apply-contact"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "apply-context"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "apply-copyright"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "apply-jurisdiction"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "apply-license"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "apply-publisher"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "apply-version"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "apply-wg"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "active-tables"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "fmm-definition"
          },
          {
            "url" : "value",
            "valueString" : "http://hl7.org/fhir/versions.html#maturity"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "propagate-status"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "excludelogbinaryformat"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueString" : "tabbed-snapshots"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-internal-dependency",
        "valueCode" : "hl7.fhir.uv.tools.r4#0.8.0"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "i18n-default-lang"
          },
          {
            "url" : "value",
            "valueString" : "nl-NL"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "autoload-resources"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "path-liquid"
          },
          {
            "url" : "value",
            "valueString" : "template/liquid"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "path-liquid"
          },
          {
            "url" : "value",
            "valueString" : "input/liquid"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "path-qa"
          },
          {
            "url" : "value",
            "valueString" : "temp/qa"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "path-temp"
          },
          {
            "url" : "value",
            "valueString" : "temp/pages"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "path-output"
          },
          {
            "url" : "value",
            "valueString" : "output"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "path-suppressed-warnings"
          },
          {
            "url" : "value",
            "valueString" : "input/ignoreWarnings.txt"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "path-history"
          },
          {
            "url" : "value",
            "valueString" : "http://example.org/fhir/PlugathonValidationIG/history.html"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "template-html"
          },
          {
            "url" : "value",
            "valueString" : "template-page.html"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "template-md"
          },
          {
            "url" : "value",
            "valueString" : "template-page-md.html"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "apply-contact"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "apply-context"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "apply-copyright"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "apply-jurisdiction"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "apply-license"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "apply-publisher"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "apply-version"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "apply-wg"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "active-tables"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "fmm-definition"
          },
          {
            "url" : "value",
            "valueString" : "http://hl7.org/fhir/versions.html#maturity"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "propagate-status"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "excludelogbinaryformat"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      },
      {
        "extension" : [
          {
            "url" : "code",
            "valueCode" : "tabbed-snapshots"
          },
          {
            "url" : "value",
            "valueString" : "true"
          }
        ],
        "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-parameter"
      }
    ],
    "resource" : [
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-AdministrationAgreement.AdditionalInformation"
        },
        "name" : "ext AdministrationAgreement.AdditionalInformation",
        "description" : "An extension to provide additional information that includes details on the structure of the agreement made."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-AdministrationAgreement.AdministrationAgreementDateTime"
        },
        "name" : "ext AdministrationAgreement.AdministrationAgreementDateTime",
        "description" : "An extension to provide the time at which the agreement was made."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-AdministrationAgreement.ReasonModificationOrDiscontinuation"
        },
        "name" : "ext AdministrationAgreement.ReasonModificationOrDiscontinuation",
        "description" : "An extension to provide a reason for modification or discontinuation of this agreement. This will often be the same reason as the one for modification or discontinuation of the medication agreement."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-AsAgreedIndicator"
        },
        "name" : "ext AsAgreedIndicator",
        "description" : "An extension to indicate if the medicine is used or administered as outlined in the medication respectively medication/administration agreement."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-Communication.Payload.ContentCodeableConcept"
        },
        "name" : "ext Communication.Payload.ContentCodeableConcept",
        "description" : "An extension to extend `Communication.payload.content` with a CodeableConcept data type. This is a pre-adopt of R5 in which the string data type of this element is changed to a CodeableConcept."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-DispenseRequest.AdditionalWishes"
        },
        "name" : "ext DispenseRequest.AdditionalWishes",
        "description" : "An extension to provide additional wishes that includes logistics and other instructions such as: do not enter in GDS, urgent, purposeful deviation, etc."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-DispenseRequest.DispenseLocation"
        },
        "name" : "ext DispenseRequest.DispenseLocation",
        "description" : "An extension to provide a reference to the Location resource to indicate where the medication is (to be) dispensed."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-DispenseRequest.FinancialIndicationCode"
        },
        "name" : "ext DispenseRequest.FinancialIndicationCode",
        "description" : "An extension that captures a financial indication code for reimbursement of a pharmaceutical product."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-Dosage-AsNeededFor"
        },
        "name" : "ext Dosage AsNeededFor",
        "description" : "Pre-adopt of the `Dosage.asNeededFor` concept from the FHIR R5 Dosage data type. In R4, `Dosage.asNeededCodeableConcept` has a maximum cardinality of 1. Additional 'asNeeded' data can be represented by adding this extension to Dosage."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-InstructionsForUse.RepeatPeriodCyclicalSchedule"
        },
        "name" : "ext InstructionsForUse.RepeatPeriodCyclicalSchedule",
        "description" : "The repeated period in a cyclical schedule (of one or more dosing instructions). A cyclical schedule is noted in days, the corresponding dosing duration is also in days.\r\n\r\nThe dosage instructions are interpreted differently if RepeatPeriodCyclicalSchedule is present. Therefore this extension is labeled as a modifier extension."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationAdministration2.AgreedDateTime"
        },
        "name" : "ext MedicationAdministration2.AgreedDateTime",
        "description" : "An extension to provide the date and time in the medication or administration agreement to which this administration pertains."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationAdministration2.InjectionPatchSite"
        },
        "name" : "ext MedicationAdministration2.InjectionPatchSite",
        "description" : "An extension to provide the site of the patient's body where an injection has been administered or where adhesive medical dressing has been applied."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationAdministration2.ReasonForDeviation"
        },
        "name" : "ext MedicationAdministration2.ReasonForDeviation",
        "description" : "An extension to provide the reason why the medication was not taken or administered or was taken or administered differently."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationAgreement.MedicationAgreementAdditionalInformation"
        },
        "name" : "ext MedicationAgreement.MedicationAgreementAdditionalInformation",
        "description" : "An extension to provide additional information that includes details on the structure of the agreement made that are relevant for pharmacovigilance and fulfillment by the pharmacist. This can be used e.g. to indicate that there was a conscious decision to deviate from the norm or that the agreement is to be structured in a certain way."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationAgreement.NextPractitioner"
        },
        "name" : "ext MedicationAgreement.NextPractitioner",
        "description" : "An extension to provide the practitioner that is supposed to take over the pharmaceutical treatment of this MedicationAgreement."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationAgreement.RelationMedicationUse"
        },
        "name" : "ext MedicationAgreement.RelationMedicationUse",
        "description" : "An extension to provide a relation to a MedicationUse2 on which the MedicationAgreement is based."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationDispense.DistributionForm"
        },
        "name" : "ext MedicationDispense.DistributionForm",
        "description" : "An extension to provide the distribution form."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationDispense.MedicationDispenseAdditionalInformation"
        },
        "name" : "ext MedicationDispense.MedicationDispenseAdditionalInformation",
        "description" : "An extension to provide additional information that includes details on the structure of the medical dispense. This can be e.g. a reason for deviating from the dispense request."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationDispense.RequestDate"
        },
        "name" : "ext MedicationDispense.RequestDate",
        "description" : "An extension to provide the time at which a pharmacist records an intended dispense."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationOverview.SourceOrganization"
        },
        "name" : "Ext MedicatonOverview.SourceOrganization",
        "description" : "Extension to capture the organization that was the author/source of a List. This extends the current possible reference types (Practitioner | Patient | Device) so that it includes an Organization."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationOverview.Verification"
        },
        "name" : "Ext MedicatonOverview.Verification",
        "description" : "Extension to capture if a patient and/or health professional verified the medication overview and the corresponding date the verification took place."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationUse2.Author"
        },
        "name" : "ext MedicationUse2.Author",
        "description" : "An extension to provide information on who is the author of the MedicationUse2."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-MedicationUse2.Prescriber"
        },
        "name" : "ext MedicationUse2.Prescriber",
        "description" : "An extension to reference the health professional that entered the medication agreement with the patient."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-PeriodOfUse.Condition"
        },
        "name" : "ext-PeriodOfUse.Condition",
        "description" : "An extension to provide a Condition to a PeriodOfUse."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-PharmaceuticalTreatment.Identifier"
        },
        "name" : "ext PharmaceuticalTreatment.Identifier",
        "description" : "This extension provides an identifier to unambiguously identify the set of interdependent medication building blocks that belong to one pharmaceutical treatment."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-RegistrationDateTime"
        },
        "name" : "ext RegistrationDateTime",
        "description" : "An extension to provide the date and time a certain medication agreement, variable-dosing regimen, administration agreement or medication administration was recorded.\r\n\r\nFor the medication administration this extension can be seen as a pre-adopt of the `MedicationAdministration.recorded` element that has been added in FHIR R5."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-RelationAdministrationAgreement"
        },
        "name" : "ext RelationAdministrationAgreement",
        "description" : "An extension to provide a relation to an AdministrationAgreement on which the MedicationAgreement or AdministrationAgreement is based."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-RenderedDosageInstruction"
        },
        "name" : "ext RenderedDosageInstruction",
        "description" : "Pre-adopt of the `.renderedDosageInstructions` concept from the FHIR R5 medication resources. It provides a full representation of the dose of the medication included in all dosage instructions. To be used when multiple dosage instructions are included to represent complex dosing such as increasing or tapering doses."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-ResourceCategory"
        },
        "name" : "ext ResourceCategory",
        "description" : "This extension is used to augment a reference with the target resource category, in cases when `Reference.type` is not precise enough to determine the functional counterpart of the reference and `Reference.identifier` is used. The value of this extension is often a semantic code (e.g. the zib's root definition code) which identifies the target resource category."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:extension"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/ext-StopType"
        },
        "name" : "ext StopType",
        "description" : "An extension to provide the manner in which medication is discontinued (temporary or definitive)."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-AdministrationAgreement"
        },
        "name" : "mp AdministrationAgreement",
        "description" : "An administration agreement is the use (or administering) instructions from the pharmacist to the patient (or their representative or administrator), whereby a medication agreement is structured at a concrete level."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-DispenseRequest"
        },
        "name" : "mp DispenseRequest",
        "description" : "The dispense request is the request of a prescriber to the pharmacist to dispense medication(s) to the patient to support current medication agreements. The prescriber asks them to dispense a certain amount of medicine or to dispense medicine(s) for a period of use."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:complex-type"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-InstructionsForUse.DosageInstructions"
        },
        "name" : "mp InstructionsForUse.DosageInstructions",
        "description" : "Instructions for the use or administration of the medication, e.g. dose and route of administration. In the medication building block MedicationUse, this is the pattern of use established by the patient or which the patient followed."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-MedicationAdministration2"
        },
        "name" : "mp MedicationAdministration2",
        "description" : "Medication administration is the registration of the individual administrations of the medicine on the patient by the administrator (e.g. a nurse or patient themselves), in relation to the entered agreements."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-MedicationAgreement"
        },
        "name" : "mp MedicationAgreement",
        "description" : "A medication agreement is a prescriber’s proposal for a patient to use medication. An agreement to discontinue the use of medication is also a medication agreement."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-MedicationDispense"
        },
        "name" : "mp MedicationDispense",
        "description" : "A dispense is the delivery of an amount of medicine to the patient, their administrator or their representative."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-MedicationOverview-Bundle"
        },
        "name" : "mp MedicationOverview Bundle",
        "description" : "Profile on the Bundle resource which represents the structure of the Retrieve and Send MedicationOverview transactions conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). The output of the ['$medication-overview'](https://simplifier.net/medicationprocess/medication-overview) operation (used in the former transaction) SHALL conform to this profile."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-MedicationOverview"
        },
        "name" : "mp MedicationOverview",
        "description" : "Profile on the List resource which represents the medication overview conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces)."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-MedicationPrescription-Bundle"
        },
        "name" : "mp MedicationPrescription Bundle",
        "description" : "Profile on the Bundle resource which represents the structure of the Send MedicationPrescription transaction conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces)."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-MedicationPrescriptionProcessing-Bundle"
        },
        "name" : "mp MedicationPrescriptionProcessing Bundle",
        "description" : "Profile on the Bundle resource which represents the structure of the Send MedicationPrescriptionProcessing transaction conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces)."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-MedicationUse2"
        },
        "name" : "mp MedicationUse2",
        "description" : "MedicationUse2 is a statement on the historic, current or intended use of a certain medicine."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-PharmaceuticalProduct"
        },
        "name" : "mp PharmaceuticalProduct",
        "description" : "The prescribed substance is usually medication. However, medical aids and bandages can also be prescribed and supplied via the pharmacy. Food and blood products do not strictly belong in the medication category, but can be prescribed and supplied by a pharmacy as well.\r\n\r\nA type of medication can be indicated with **a single code**. That code can be chosen from several possible coding systems (concretely: GPK, PRK, HPK or article numbers). Correct use of these codes in the software systems will sufficiently record the composition of the product used, making a complete product specification unnecessary.\r\n\r\nIn addition to a primary code, **alternative codes** from other coding systems can also be entered (so that the GPK can be sent along in the event that the patient was registered based on PRK, for example).\r\n\r\nEntering multiple ingredients will enable you to display a compound product. If one of the composite parts is liquid, the dosage will be given in milliliters; otherwise it will be given in ‘units’.\r\n\r\nIn that case, the **composition of the medication** can be specified implicitly (with the use of a medication code) or explicitly, for example by listing the (active) ingredient(s) of the medication.\r\n\r\n**Magistral prescriptions** can be entered as well. This can be done by means of the option listed above to enter coded ingredients and/or by entering the composition and preparation method as free text.\r\nThis is a partial information model."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-ProposalDispenseRequest-Bundle"
        },
        "name" : "mp ProposalDispenseRequest Bundle",
        "description" : "Profile on the Bundle resource which represents the structure of the Send ProposalDispenseRequest transaction conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces)."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-ProposalMedicationAgreement-Bundle"
        },
        "name" : "mp ProposalMedicationAgreement Bundle",
        "description" : "Profile on the Bundle resource which represents the structure of the Send ProposalMedicationAgreement transaction conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces)."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-ReplyProposalDispenseRequest-Bundle"
        },
        "name" : "mp ReplyProposalDispenseRequest Bundle",
        "description" : "Profile on the Bundle resource which represents the structure of the Send ReplyProposalDispenseRequest transaction conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces)."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-ReplyProposalDispenseRequest"
        },
        "name" : "mp ReplyProposalDispenseRequest",
        "description" : "Profile on the Communication resource which represents the reply proposal dispense request conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces)."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-ReplyProposalMedicationAgreement-Bundle"
        },
        "name" : "mp ReplyProposalMedicationAgreement Bundle",
        "description" : "Profile on the Bundle resource which represents the structure of the Send ReplyProposalMedicationAgreement transaction conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces)."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-ReplyProposalMedicationAgreement"
        },
        "name" : "mp ReplyProposalMedicationAgreement",
        "description" : "Profile on the Communication resource which represents the reply proposal medication agreement conform information standard ['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces)."
      },
      {
        "extension" : [
          {
            "url" : "http://hl7.org/fhir/tools/StructureDefinition/resource-information",
            "valueString" : "StructureDefinition:resource"
          }
        ],
        "reference" : {
          "reference" : "StructureDefinition/mp-VariableDosingRegimen"
        },
        "name" : "mp VariableDosingRegimen",
        "description" : "The variable-dosing regimen contains the dosing schedule as prescribed by the (external) prescriber to the patient (or his representative or administrator), specifying the instructions for use in addition to the medication agreement. The dosing schedule can be adjusted, while the medication agreement remains unchanged."
      }
    ],
    "page" : {
      "extension" : [
        {
          "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-page-name",
          "valueUrl" : "toc.html"
        }
      ],
      "nameUrl" : "toc.html",
      "title" : "Table of Contents",
      "generation" : "html",
      "page" : [
        {
          "extension" : [
            {
              "url" : "http://hl7.org/fhir/tools/StructureDefinition/ig-page-name",
              "valueUrl" : "index.html"
            }
          ],
          "nameUrl" : "index.html",
          "title" : "Plugathon validation IG",
          "generation" : "markdown"
        }
      ]
    },
    "parameter" : [
      {
        "code" : "path-pages",
        "value" : "input/pages"
      },
      {
        "code" : "path-resource",
        "value" : "input/capabilities"
      },
      {
        "code" : "path-resource",
        "value" : "input/examples"
      },
      {
        "code" : "path-resource",
        "value" : "input/extensions"
      },
      {
        "code" : "path-resource",
        "value" : "input/models"
      },
      {
        "code" : "path-resource",
        "value" : "input/operations"
      },
      {
        "code" : "path-resource",
        "value" : "input/profiles"
      },
      {
        "code" : "path-resource",
        "value" : "input/resources"
      },
      {
        "code" : "path-resource",
        "value" : "input/vocabulary"
      },
      {
        "code" : "path-resource",
        "value" : "input/maps"
      },
      {
        "code" : "path-resource",
        "value" : "input/testing"
      },
      {
        "code" : "path-resource",
        "value" : "input/history"
      },
      {
        "code" : "path-resource",
        "value" : "fsh-generated/resources"
      },
      {
        "code" : "path-pages",
        "value" : "template/config"
      },
      {
        "code" : "path-pages",
        "value" : "input/images"
      },
      {
        "code" : "path-tx-cache",
        "value" : "input-cache/txcache"
      }
    ]
  }
}

```
