# 2 (3)  Any offense that requires registration as a sex offender


# (2)  Any offense that requires registration as a sex offender

## Law

610.140.2(3) Any offense that requires registration as a sex offender;

## Plan Speak

## Training

*What we need to tell pro bono attornies* 


## Information Needed

We neet to know:

1. Does the offince require registration as a sex offender.

Assumptions:

* This applies to the charge and does not disqualify the case.
  

## UX

When displaying a statute that is not elagible 

## Database

* The Offince requires_registration as a sex offended.
   * ADD `statute.requires_registration`


### Add `statues.dangerous_felony` flag

Flag has the following options:

* Offince requires registration
* Offince does not requires registration
* Not determined

How to initalize?

come baack to later

How to maintain?

1. Have someone watch the changes in law
2. Have lawyers look for errors (sanity check)
3. Will need to be maintained more frequently then some other elements.

## Logic

```
if charges.requires_registration == True
Then
   Charge cannot be expunged
```

