# Creating Initial Laws

Primary data sources are Change Code Manuel and Missouri Revisor.

# Load Static Data

This is data that is not updated.

## Create Exceptions

Source: manually created data taken from the statute.

Table: exceptions

## Import Missouri Laws**

Source: Missouri Revisor 

Table: ImportedMoRevisorActiveSection

## Create Missouri Chapters##

Source: ImportedMoRevisorActiveSection

Table: LawChapter

## Import 2020 and 2021 Charge Codes

There are two different programs to import since the format is different.

Source: Charge Code Manule (top)

Table: ImportedMshpChargeCodeManual

## Import 2020 and 2021 Charge Codes Ordances

Source: Charge Code Manule (bottom)

Table: ImportedMshpChargeCodeManual

## Import Transferred Charge Codes

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

## Create Laws from Charge Codes

Source: ImportedMshpChargeCodeManual, ImportedMoRevisorActiveSection, LawChapter
Table: Law

## Apply Transferred Charge Codes

Source: ImportedTransferedChargeCode

Table: Law

## Import Retired Charge Codes

Source: ImportedRetiredChargeCode

Table: Law

## Report Law and Charge Code Discrepancy Errors only for Statutes

Source: MoChargeCodes, Law

Report:  Laws without Charge Codes, and Charge Codes without Laws

## Fix Law and Charge Code Discrepancy Errors only for Statutes

Source: MoChargeCodes, Law

Table: Law - will add placeholder law for any charge code that did not have a law.




# Create Law and LawExceptioin Tables

These are tables that contain data that will change due to sources and expungement rules.

## Create Law Exceptions

Will include Ordanices

Source: MoChargeCodes, Law

Table: Law, LawExceptions

## Report Law and Charge Code Discrepancy Errors only for Statutes

Source: MoChargeCodes, Law

Report:  Laws without Charge Codes, and Charge Codes without Laws

## Fix Law and Charge Code Discrepancy Errors only for Statutes

Source: MoChargeCodes, Law

Table: Law - will add placeholder law for any charge code that did not have a law.

# Load Clinic App Data

If Clinic App has a law that we do not have, we will add it.

Source:  Export Yamal file from Clinic App

Table: Law
