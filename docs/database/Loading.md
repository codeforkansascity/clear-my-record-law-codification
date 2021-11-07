# Data used to load

## MO Statutes

From the [Publications](https://revisor.mo.gov/main/Info.aspx) page of the Mo Revisor are 
* a list of [active sections with headnotes](https://revisor.mo.gov/main/Info.aspx?doc=ALLSN) (tab delimited)
* a list of [repealers and transfers](https://revisor.mo.gov/main/Info.aspx?doc=REPXF) (tab delimited)

It does not look like it includes Municipal Ordances.

### active sections with headnotes

This files has two lines at the top that describe the contents and should be ignored.
The bottom part is sections to the MO Constitution and should be ignored.

Load looks for a first column that matches 999.999

### repealers and transfers

Contains 
* Repeals
* Combine
* Transfers

```
As of 11/7/2021 3:09:24 PM^M
Repealers and Transfers^M
^M
Repealers (list is incomplete)^M
1.022   (Repealed L. 1975 H.B. 945 § 1) 9/28/1975^M
1.110   (Repealed L. 1978 H.B. 1634 § A)        1/2/1979^M

198.041 (Transferred 1994; now 199.350)         8/28/1994^M
202.240	(Repealed L. 1980 H.B. 1724 § 1)	8/13/1980
202.250 (1969; Combined with 202.240)   8/28/1969^M
```


Note 
* "Transferred" and "Repealed" are not alwas at the beginning of the line.
* Repealed statutes are not in the list of active sections with headnotes.
* Statutes that have been transferd are not in the list of active sections with headnotes.
* 

We have been using the term Superceded instead of Transfer"
