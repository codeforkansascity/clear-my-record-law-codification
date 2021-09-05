# MSHP Charge Codes

Useful for classifying State Statutes as well  as Local Ordinance
The website has [The 2020-2021 Missouri Charge Code Manual](https://www.mshp.dps.missouri.gov/CJ08Client/Home/ChargeCode).  It contains PDF's of the charge codes and related information as well as documentation to interpret the codes.  You can download the Current Datasets in .csv format.

## Contents of the site


The primary document is the "Missouri Charge Code Manual"  August 28, 2020 - August 27, 2021 SHP-179 N 6/2020.  It contains

*  Charge Code Manual Instructions: SOR indicated if registration as a sex offender is required upon conviction
*  Data in PDF Table "MISSOURI STATE HIGHWAY PATROL CHARGE CODE MANUAL"
*  Section II: NCIC Categories and Modifiers
*  Ordinance Charge Code Structure

### DownLoads (See upper right-hand side of the website)

The following three downloads are all documented in [Charge Code File Layout](https://www.mshp.dps.missouri.gov/MSHPWeb/PatrolDivisions/CRID/documents/ChargeCodeFileLayout0882019.pdf)

*  Charge Code CSV 2021-05-03


*  NCIC CSV 2021-05-03   -- Caution 1 Values include 0=No Caution, 1=Violent, 2=Armed, 3=Assaulted Officer


*  NCIC Modifiers CSV 2021-05-03

# NICI Codes

[NCIC Code Manual as of
March 31, 2021](https://wilenet.widoj.gov/sites/default/files/public_files-2021-04/ncic_code_manual_mar_31_2021.pdf)
See chapter: Uniform Offense Data Codes starting on page 402.

# Review of Charge Codes

* Effective Date
    * Does not correspond with MO Revisor Versions (Legislative Updates)
    * Is a part of the Charge Code allowing the charge code to go back into history

* Charge code 
    * has effective date’s year embedded in it.  571.030-007N202052


* Do we have to go back into history, and if so in what situations?
* MSHP has a Charge Code.  We need to see if they plead to a reduced sentence if the Charge Code changes between arrest and court action.
* Add Charge code to Law Tracker

* Description
There is some "data" in the description of the Charge Code Manual that may help us determine eligibility on some of the other exceptions.  If L/E is Law Enforcement, See p90 of [2021 Charge Code Manual](https://www.mshp.dps.missouri.gov/MSHPWeb/PatrolDivisions/CRID/documents/August2021ChargeCodeManual.pdf) 
* 565.027-002Y202009__._.    INVOLUNTARY MANSLAUGHTER - 2ND DEGREE - L/E OR RELATIVE
* 565.052-004Y202013__._.    ASSAULT - 2ND DEGREE - SPECIAL VICTIM


**_The following has not been verified_**

From Charge Code Manual 2021

| Name                                                 | Value      |
| ---------------------------------------------------- | ---------: |
| First Effective Date                                 | 07/09/1925 |
| Last Effective Date                                  | 01/01/2021 |
| Number of Laws                                       | 1227       |
| Number of Laws with multiple Effective Dates         | 446        |
| Number of Laws that are F / A for any Effective Date | 37         |
| Number of Laws any Felony for any Effective Date     | 609        |

## Chapters in the three files that have the Charge Code field

| Chapter | Manual | Charge Code | NCIC Modifier | MO Revisor
| ----------- |------- | ----------- | ------------- | ------
| 28          | NULL   | 28          | 28            | Secretary of State
| 42          | NULL   | 42          | 42            | Veterans' Affairs
| 118         | NULL   | 118         | 118           | Missing
| 202         | NULL   | NULL        | 202           | Missing
| 300         | NULL   | 300         | 300           | Model Traffic Ordinance
| 312         | NULL   | 312         | 312           | Nonintoxicating Beer
| 400         | NULL   | 400         | 400           | Uniform Commercial Code
| 546         | NULL   | 546         | 546           | Trials, Judgments and Executions in Criminal Cases
| 549         | NULL   | 549         | 549           | Probation, Pardons and Paroles
| 556         | NULL   | 556         | 556           | Preliminary Provisions (Criminal Code)
| 563         | NULL   | 563         | 563           | Defense of Justification
| 564         | NULL   | 564         | 564           | Inchoate Offenses

* 564 Is Attempt “Rules”
* 563 Rules for Self Defense
* 556 Definition and how it works
* 549 Definition
* **312 and 42 - We will want to have someone look into**


## Compared to MO Revisor
### Effective Date

Does not correspond with MO Revisor Versions (Legislative Updates)

### Desicription
There is a charge code for each **_part of_** the statute.


```
  577.013.   Boating while intoxicated — sentencing restrictions. — 1.  A person commits the offense of boating while intoxicated if he or she operates a vessel while in an intoxicated condition.
  2.  The offense of boating while intoxicated is:
  (1)  A class B misdemeanor;
  (2)  A class A misdemeanor if:
  (a)  The defendant is a prior boating offender; or
  (b)  A person less than seventeen years of age is present in the vessel;
  (3)  A class E felony if:
  (a)  The defendant is a persistent boating offender; or
  (b)  While boating while intoxicated, the defendant acts with criminal negligence to cause physical injury to another person;
```

![image](https://user-images.githubusercontent.com/447024/129508750-270676b0-41b6-48c0-bb7c-5692b6b7cd78.png)


| charge_code                  | ncic           | state | description                                                             | class | dna | sor | roc | type |
|----------------------------- |--------------- |------ |------------------------------------------------------------------------ | ----- | --- | --- | --- | ---- |
| 577.013-001Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - HABITUAL - 2ND OR SUBSEQUE ... | F / A | C   | N   | N   | F    |  
| 577.013-004Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - HABITUAL                                      | F / B | C   | N   | N   | F    |  
| 577.013-005Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - DEATH OF LAW ENFORCEMENT  ...                    | F / B | C   | N   | N   | F    |  
| 577.013-007Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - CHRONIC                                       | F / C | C   | N   | N   | F    |  
| 577.013-008Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - SERIOUS PHYSICAL INJURY TO EMERGENCY ... | F / C | C   | N   | N   | F    |
| 577.013-009Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - DEATH OF ANOTHER                              | F / C | C   | N   | N   | F    |  
| 577.013-010Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - AGGRAVATED                                    | F / D | C   | N   | N   | F    |  
| 577.013-011Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - PHYSICAL INJURY TO LAW PERSONNEL  ... | F / D | C   | N   | N   | F    |
| 577.013-012Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - SERIOUS PHYSICAL INJURY                       | F / D | C   | N   | N   | F    |  
| 577.013-013Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - PERSISTENT                                    | F / E | C   | N   | N   | F    |  
| 577.013-014Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - PHYSICAL INJURY                               | F / E | C   | N   | N   | F    |  
| 577.013-015Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - PRIOR                                         | M / A | N   | N   | N   | M    |  
| 577.013-016Y202054  | 03, 04, 05, 99 | 0 1 2 | BWI - PERSON LESS THAN 17 YEARS ...                    | M / A | N   | N   | N   | M    |  
| 577.013-017Y202054  | 03, 04, 05, 99 | 0 1 2 | BOATING WHILE INTOXICATED                           | M / B | N   | N   | N   | M    |


## Multiple Effective Dates

From Revisor:

(L. 1994 S.B. 590, A.L. 1999 H.B. 603, et al. merged with S.B. 19)
Enacted 1994,  Amended in 1999

![image](https://user-images.githubusercontent.com/447024/129509023-df258d74-b0d5-4a6f-a44d-9c57e38ddfb8.png)


### Had one charge code in 1994, they decided to break out by levels of penalties ???

![image](https://user-images.githubusercontent.com/447024/129509048-d90d1bcd-8d9c-4ad8-b5f4-201bec587d73.png)


## Other


| effective_date | charge_code                  | description                                                                                                                                                                                     | class | dna | sor | roc |
| -------------- | ---------------------------- | --- | ----- | --- | --- | --- |
| 1994-08-28 | 643.355-001N199454| MISREPRESENT INSPECTION STATION/MANUF... | M / B | N   | N   | N   |   
| 1994-08-28 | 643.355-002N199454| MISREPRESENT INSPECTION STATION/MANUF... | M / C | N   | N   | N   |   
| 1994-08-28 | 643.355-003N199454| DISPLAY OR PERMIT THE DISPLAY OF ILLE... | I     | N   | N   | N   |   
| 1994-08-28 | 643.355-004N199454| VIOLATE REQUIREMENTS OF SECTIONS 643.... | I     | N   | N   | N   |   
|  |  |  |  |  |  |  |
| 2019-01-01 | 643.355-005N201954| OPERATE MOTOR VEHICLE W/O DISPLAYING | M / B | N   | N   | N   |   
| 2019-01-01 | 643.355-006N201954| OPERATE MOTOR VEHICLE W/O DISPLAYING | M / C | N   | N   | N   |   
| 2019-01-01 | 643.355-007N201954| OPERATE MOTOR VEHICLE W/O DISPLAYING | I     | N   | N   | N   |   


| law     | charge_code                  | substr(description,1,50)                           | class |
| ------- | ---------------------------- | -------------------------------------------------- | ----- |
| 571.030 | 571.030-001Y202052    ._     | DISCHARGE/SHOOT FIREARM AT OR FROM MOTOR VEHICLE/S | F / B |
| 571.030 | 571.030-002Y202052    ._     | DISCHARGE/SHOOT FIREARM AT OR FROM MOTOR VEHICLE/S | F / B |
| 571.030 | 571.030-003Y20205299._       | AIDING/ABETTING A PERSON DISCHARGING/SHOOTING A FI | F / A |
| 571.030 | 571.030-004Y20205299._       | AIDING/ABETTING A PERSON DISCHARGING/SHOOTING A FI | F / B |
| 571.030 | 571.030-005Y20205299._       | AIDING/ABETTING A PERSON DISCHARGING/SHOOTING A FI | F / B |
| 571.030 | 571.030-006Y20205299._       | AIDING/ABETTING A PERSON DISCHARGING/SHOOTING A FI | F / B |
| 571.030 | 571.030-007N202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 1 - CARRIES CO | M / B |
| 571.030 | 571.030-008Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 2-SPRING GUN   | F / E |
| 571.030 | 571.030-009Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 3 - DISCHARGE  | F / E |
| 571.030 | 571.030-010Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 4 - EXHIBITING | F / E |
| 571.030 | 571.030-011Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 5 - WHILE INTO | F / E |
| 571.030 | 571.030-012Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 6 - DISCHARGE  | M / B |
| 571.030 | 571.030-013Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 7 - DISCHARGE  | M / B |
| 571.030 | 571.030-014Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 8 - CARRY INTO | M / B |
| 571.030 | 571.030-015Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 9 - SHOOT AT/F | F / A |
| 571.030 | 571.030-016Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 5 - WHILE INTO | M / A |
| 571.030 | 571.030-017Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 10 - CARRIES L | F / E |
| 571.030 | 571.030-018Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 10 - CARRIES U | M / A |
| 571.030 | 571.030-019Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 11 - POSSESS W | F / E |
| 571.030 | 571.030-020Y202052    ._     | UNLAWFUL USE OF WEAPON - SUBSECTION 9 - SHOOT AT/F | F / B |



  
