# Database Overview

## How to mark laws that are not eligible?

Currently, 29-Mar-2021, we mark them as 
* Eleigable, 
* Not Eleigable,
* Possibly Eleigable,
* Undetermiend Elegiability

There is no reason given is given for if the law is not eligible.

We would like the application to report back why something is not eligible.
* A reason field
* A field indicating the law creating the ineligibility

## How to mark charges that are not eligible?

We have cases where it is not just the law, but the combination of the law and some other attribute.

An example is *2(4) Any felony offense where death is an element of the offense* 

```
if charges.conviction_charge_type == Felony
and statute.death_is_a_element is true
Then
   Charge cannot be expunged
```
