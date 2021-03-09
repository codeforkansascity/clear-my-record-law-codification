# 2(1)  Any class A felony offense;

We will look at the Charge Type & Class to determine how the charge was clasified

## Data Source

MSHP - is the best source of what is charged.
[PLEASE VERIFY]

## Database

* charges.conviction_charge_type: Felony, Misdemeanor, ...
* charges.conviction_class_type: A through X

## Code

```
if charges.conviction_charge_type == Felony
and charges.conviction_class_type == A
Then
   Charge is NOT expungable
```
