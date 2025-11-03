# Artifacts Summary - v0.1.0

* [**Table of Contents**](toc.md)
* **Artifacts Summary**

## Artifacts Summary

This page provides a list of the FHIR artifacts defined as part of this implementation guide.

### Structures: Resource Profiles 

These define constraints on FHIR resources for systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [mp AdministrationAgreement](StructureDefinition-mp-AdministrationAgreement.md) | An administration agreement is the use (or administering) instructions from the pharmacist to the patient (or their representative or administrator), whereby a medication agreement is structured at a concrete level. |
| [mp DispenseRequest](StructureDefinition-mp-DispenseRequest.md) | The dispense request is the request of a prescriber to the pharmacist to dispense medication(s) to the patient to support current medication agreements. The prescriber asks them to dispense a certain amount of medicine or to dispense medicine(s) for a period of use. |
| [mp MedicationAdministration2](StructureDefinition-mp-MedicationAdministration2.md) | Medication administration is the registration of the individual administrations of the medicine on the patient by the administrator (e.g. a nurse or patient themselves), in relation to the entered agreements. |
| [mp MedicationAgreement](StructureDefinition-mp-MedicationAgreement.md) | A medication agreement is a prescriber’s proposal for a patient to use medication. An agreement to discontinue the use of medication is also a medication agreement. |
| [mp MedicationDispense](StructureDefinition-mp-MedicationDispense.md) | A dispense is the delivery of an amount of medicine to the patient, their administrator or their representative. |
| [mp MedicationOverview](StructureDefinition-mp-MedicationOverview.md) | Profile on the List resource which represents the medication overview conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). |
| [mp MedicationOverview Bundle](StructureDefinition-mp-MedicationOverview-Bundle.md) | Profile on the Bundle resource which represents the structure of the Retrieve and Send MedicationOverview transactions conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). The output of the['$medication-overview'](https://simplifier.net/medicationprocess/medication-overview)operation (used in the former transaction) SHALL conform to this profile. |
| [mp MedicationPrescription Bundle](StructureDefinition-mp-MedicationPrescription-Bundle.md) | Profile on the Bundle resource which represents the structure of the Send MedicationPrescription transaction conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). |
| [mp MedicationPrescriptionProcessing Bundle](StructureDefinition-mp-MedicationPrescriptionProcessing-Bundle.md) | Profile on the Bundle resource which represents the structure of the Send MedicationPrescriptionProcessing transaction conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). |
| [mp MedicationUse2](StructureDefinition-mp-MedicationUse2.md) | MedicationUse2 is a statement on the historic, current or intended use of a certain medicine. |
| [mp PharmaceuticalProduct](StructureDefinition-mp-PharmaceuticalProduct.md) | The prescribed substance is usually medication. However, medical aids and bandages can also be prescribed and supplied via the pharmacy. Food and blood products do not strictly belong in the medication category, but can be prescribed and supplied by a pharmacy as well. A type of medication can be indicated with**a single code**. That code can be chosen from several possible coding systems (concretely: GPK, PRK, HPK or article numbers). Correct use of these codes in the software systems will sufficiently record the composition of the product used, making a complete product specification unnecessary. In addition to a primary code,**alternative codes**from other coding systems can also be entered (so that the GPK can be sent along in the event that the patient was registered based on PRK, for example). Entering multiple ingredients will enable you to display a compound product. If one of the composite parts is liquid, the dosage will be given in milliliters; otherwise it will be given in ‘units’. In that case, the**composition of the medication**can be specified implicitly (with the use of a medication code) or explicitly, for example by listing the (active) ingredient(s) of the medication.**Magistral prescriptions**can be entered as well. This can be done by means of the option listed above to enter coded ingredients and/or by entering the composition and preparation method as free text. This is a partial information model. |
| [mp ProposalDispenseRequest Bundle](StructureDefinition-mp-ProposalDispenseRequest-Bundle.md) | Profile on the Bundle resource which represents the structure of the Send ProposalDispenseRequest transaction conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). |
| [mp ProposalMedicationAgreement Bundle](StructureDefinition-mp-ProposalMedicationAgreement-Bundle.md) | Profile on the Bundle resource which represents the structure of the Send ProposalMedicationAgreement transaction conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). |
| [mp ReplyProposalDispenseRequest](StructureDefinition-mp-ReplyProposalDispenseRequest.md) | Profile on the Communication resource which represents the reply proposal dispense request conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). |
| [mp ReplyProposalDispenseRequest Bundle](StructureDefinition-mp-ReplyProposalDispenseRequest-Bundle.md) | Profile on the Bundle resource which represents the structure of the Send ReplyProposalDispenseRequest transaction conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). |
| [mp ReplyProposalMedicationAgreement](StructureDefinition-mp-ReplyProposalMedicationAgreement.md) | Profile on the Communication resource which represents the reply proposal medication agreement conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). |
| [mp ReplyProposalMedicationAgreement Bundle](StructureDefinition-mp-ReplyProposalMedicationAgreement-Bundle.md) | Profile on the Bundle resource which represents the structure of the Send ReplyProposalMedicationAgreement transaction conform information standard['Medication Process'](https://informatiestandaarden.nictiz.nl/wiki/Landingspagina_Medicatieproces). |
| [mp VariableDosingRegimen](StructureDefinition-mp-VariableDosingRegimen.md) | The variable-dosing regimen contains the dosing schedule as prescribed by the (external) prescriber to the patient (or his representative or administrator), specifying the instructions for use in addition to the medication agreement. The dosing schedule can be adjusted, while the medication agreement remains unchanged. |

### Structures: Data Type Profiles 

These define constraints on FHIR data types for systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [mp InstructionsForUse.DosageInstructions](StructureDefinition-mp-InstructionsForUse.DosageInstructions.md) | Instructions for the use or administration of the medication, e.g. dose and route of administration. In the medication building block MedicationUse, this is the pattern of use established by the patient or which the patient followed. |

### Structures: Extension Definitions 

These define constraints on FHIR data types for systems conforming to this implementation guide.

| | |
| :--- | :--- |
| [Ext MedicatonOverview.SourceOrganization](StructureDefinition-ext-MedicationOverview.SourceOrganization.md) | 
| | | |
| :--- | :--- | :--- |
| Extension to capture the organization that was the author/source of a List. This extends the current possible reference types (Practitioner | Patient | Device) so that it includes an Organization. |
 |
| [Ext MedicatonOverview.Verification](StructureDefinition-ext-MedicationOverview.Verification.md) | Extension to capture if a patient and/or health professional verified the medication overview and the corresponding date the verification took place. |
| [ext AdministrationAgreement.AdditionalInformation](StructureDefinition-ext-AdministrationAgreement.AdditionalInformation.md) | An extension to provide additional information that includes details on the structure of the agreement made. |
| [ext AdministrationAgreement.AdministrationAgreementDateTime](StructureDefinition-ext-AdministrationAgreement.AdministrationAgreementDateTime.md) | An extension to provide the time at which the agreement was made. |
| [ext AdministrationAgreement.ReasonModificationOrDiscontinuation](StructureDefinition-ext-AdministrationAgreement.ReasonModificationOrDiscontinuation.md) | An extension to provide a reason for modification or discontinuation of this agreement. This will often be the same reason as the one for modification or discontinuation of the medication agreement. |
| [ext AsAgreedIndicator](StructureDefinition-ext-AsAgreedIndicator.md) | An extension to indicate if the medicine is used or administered as outlined in the medication respectively medication/administration agreement. |
| [ext Communication.Payload.ContentCodeableConcept](StructureDefinition-ext-Communication.Payload.ContentCodeableConcept.md) | An extension to extend`Communication.payload.content`with a CodeableConcept data type. This is a pre-adopt of R5 in which the string data type of this element is changed to a CodeableConcept. |
| [ext DispenseRequest.AdditionalWishes](StructureDefinition-ext-DispenseRequest.AdditionalWishes.md) | An extension to provide additional wishes that includes logistics and other instructions such as: do not enter in GDS, urgent, purposeful deviation, etc. |
| [ext DispenseRequest.DispenseLocation](StructureDefinition-ext-DispenseRequest.DispenseLocation.md) | An extension to provide a reference to the Location resource to indicate where the medication is (to be) dispensed. |
| [ext DispenseRequest.FinancialIndicationCode](StructureDefinition-ext-DispenseRequest.FinancialIndicationCode.md) | An extension that captures a financial indication code for reimbursement of a pharmaceutical product. |
| [ext Dosage AsNeededFor](StructureDefinition-ext-Dosage-AsNeededFor.md) | Pre-adopt of the`Dosage.asNeededFor`concept from the FHIR R5 Dosage data type. In R4,`Dosage.asNeededCodeableConcept`has a maximum cardinality of 1. Additional 'asNeeded' data can be represented by adding this extension to Dosage. |
| [ext InstructionsForUse.RepeatPeriodCyclicalSchedule](StructureDefinition-ext-InstructionsForUse.RepeatPeriodCyclicalSchedule.md) | The repeated period in a cyclical schedule (of one or more dosing instructions). A cyclical schedule is noted in days, the corresponding dosing duration is also in days. The dosage instructions are interpreted differently if RepeatPeriodCyclicalSchedule is present. Therefore this extension is labeled as a modifier extension. |
| [ext MedicationAdministration2.AgreedDateTime](StructureDefinition-ext-MedicationAdministration2.AgreedDateTime.md) | An extension to provide the date and time in the medication or administration agreement to which this administration pertains. |
| [ext MedicationAdministration2.InjectionPatchSite](StructureDefinition-ext-MedicationAdministration2.InjectionPatchSite.md) | An extension to provide the site of the patient's body where an injection has been administered or where adhesive medical dressing has been applied. |
| [ext MedicationAdministration2.ReasonForDeviation](StructureDefinition-ext-MedicationAdministration2.ReasonForDeviation.md) | An extension to provide the reason why the medication was not taken or administered or was taken or administered differently. |
| [ext MedicationAgreement.MedicationAgreementAdditionalInformation](StructureDefinition-ext-MedicationAgreement.MedicationAgreementAdditionalInformation.md) | An extension to provide additional information that includes details on the structure of the agreement made that are relevant for pharmacovigilance and fulfillment by the pharmacist. This can be used e.g. to indicate that there was a conscious decision to deviate from the norm or that the agreement is to be structured in a certain way. |
| [ext MedicationAgreement.NextPractitioner](StructureDefinition-ext-MedicationAgreement.NextPractitioner.md) | An extension to provide the practitioner that is supposed to take over the pharmaceutical treatment of this MedicationAgreement. |
| [ext MedicationAgreement.RelationMedicationUse](StructureDefinition-ext-MedicationAgreement.RelationMedicationUse.md) | An extension to provide a relation to a MedicationUse2 on which the MedicationAgreement is based. |
| [ext MedicationDispense.DistributionForm](StructureDefinition-ext-MedicationDispense.DistributionForm.md) | An extension to provide the distribution form. |
| [ext MedicationDispense.MedicationDispenseAdditionalInformation](StructureDefinition-ext-MedicationDispense.MedicationDispenseAdditionalInformation.md) | An extension to provide additional information that includes details on the structure of the medical dispense. This can be e.g. a reason for deviating from the dispense request. |
| [ext MedicationDispense.RequestDate](StructureDefinition-ext-MedicationDispense.RequestDate.md) | An extension to provide the time at which a pharmacist records an intended dispense. |
| [ext MedicationUse2.Author](StructureDefinition-ext-MedicationUse2.Author.md) | An extension to provide information on who is the author of the MedicationUse2. |
| [ext MedicationUse2.Prescriber](StructureDefinition-ext-MedicationUse2.Prescriber.md) | An extension to reference the health professional that entered the medication agreement with the patient. |
| [ext PharmaceuticalTreatment.Identifier](StructureDefinition-ext-PharmaceuticalTreatment.Identifier.md) | This extension provides an identifier to unambiguously identify the set of interdependent medication building blocks that belong to one pharmaceutical treatment. |
| [ext RegistrationDateTime](StructureDefinition-ext-RegistrationDateTime.md) | An extension to provide the date and time a certain medication agreement, variable-dosing regimen, administration agreement or medication administration was recorded. For the medication administration this extension can be seen as a pre-adopt of the`MedicationAdministration.recorded`element that has been added in FHIR R5. |
| [ext RelationAdministrationAgreement](StructureDefinition-ext-RelationAdministrationAgreement.md) | An extension to provide a relation to an AdministrationAgreement on which the MedicationAgreement or AdministrationAgreement is based. |
| [ext RenderedDosageInstruction](StructureDefinition-ext-RenderedDosageInstruction.md) | Pre-adopt of the`.renderedDosageInstructions`concept from the FHIR R5 medication resources. It provides a full representation of the dose of the medication included in all dosage instructions. To be used when multiple dosage instructions are included to represent complex dosing such as increasing or tapering doses. |
| [ext ResourceCategory](StructureDefinition-ext-ResourceCategory.md) | This extension is used to augment a reference with the target resource category, in cases when`Reference.type`is not precise enough to determine the functional counterpart of the reference and`Reference.identifier`is used. The value of this extension is often a semantic code (e.g. the zib's root definition code) which identifies the target resource category. |
| [ext StopType](StructureDefinition-ext-StopType.md) | An extension to provide the manner in which medication is discontinued (temporary or definitive). |
| [ext-PeriodOfUse.Condition](StructureDefinition-ext-PeriodOfUse.Condition.md) | An extension to provide a Condition to a PeriodOfUse. |

