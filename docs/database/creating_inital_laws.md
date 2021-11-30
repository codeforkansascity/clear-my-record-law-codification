# Creating Inital Laws

Primary data sources are Change Code Manule and Missouri Revisor.

# Load Static Data

This is data that is not updated.

## Create Exceptions

Source: manuly created data taken from the statute.

Table: exceptions

## Import Missouri Laws**

Source: Missouri Revisor 

Table: ImportedMoRevisorActiveSection

## Create Missouri Chapters##

Source: ImportedMoRevisorActiveSection

Table: LawChapter

## Import 2020 and 2021 Charge Codes

Source: Charge Code Manule

Table: ImportedMshpChargeCodeManual

## Import Transfered Charge Codes

Source: Active by New Code - Charge Code Manual page

Table: ImportedTransferedChargeCode

## Import Retired Charge Codes

Source: Retired by New Code - Charge Code Manual page

Table: ImportedRetiredChargeCode

# Create Law Tables

Laws and LawException tables. 

## Create Charge Codes

Source: ImportedMshpChargeCodeManual, ImportedTransferedChargeCode, ImportedRetiredChargeCode

Table: MoChargeCodes

## Create Laws from Charege Codes

Source: ImportedMshpChargeCodeManual, ImportedMoRevisorActiveSection, LawChapter
Table: Law

## Report Law and Charge Code Descrepancy Errors

Source: MoChargeCodes, Law

Report:  Laws without Charge Codes, and Charge Codes without Laws

## Fix Law and Charge Code Descrepancy Errors

Source: MoChargeCodes, Law

Table: Law - will add place holder law for any charge code that did not have a law.

## Create Law Exceptions




