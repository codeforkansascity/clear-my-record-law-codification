# [MSHP Web Service Interface](https://www.mshp.dps.missouri.gov/CJ08Client/Home/WebService)

## Tools

* [XMLSpy](https://www.altova.com/xmlspy-xml-editor)
* 

## [Missouri Charge Code Service](https://www.mshp.dps.mo.gov/cj08service/api/chargeCodes/xml) – offers the ability to retrieve the latest version of State Charge Codes to be used for incident and criminal history reporting purposes.

   * [Comparative Analysis of Common Charge Tables](https://mail.google.com/mail/u/0?ui=2&ik=2e3975107f&attid=0.1&permmsgid=msg-f:1711925958527800195&th=17c1fb96cfd1d383&view=att&disp=inline) Has definitions of variable names.  Also talks about National Information Exchange Model (NIEM).
   * [NIEM GitHub](http://niem.github.io/niem-releases/) and [Home Page](http://niem.github.io/) More NIEM

## [NCIC Modifier Service](https://www.mshp.dps.mo.gov/cj08service/api/NcicModifier/xml) – offers the ability to retrieve the latest version of NCIC Modifiers that are associated with State Charge Codes.
## [IBR Offense Code Service](https://www.mshp.dps.mo.gov/cj08service/api/ibrOffenseCode/xml) – offers the ability to retrieve the latest version of IBR Offense Codes for UCR incident-based reporting purposes.
## [SRS Offense Code Service](https://www.mshp.dps.mo.gov/cj08service/api/srsOffenseCode/xml)  – offers the ability to retrieve the latest version of SRS Offense Codes for UCR summary-based reporting purposes.

```
Array
(
    [SRSOffenseCode] => Array
        (
            [0] => Array
                (
                    [code] => 1A
                    [description] => Murder and Nonnegligent Manslaughter				
                    [modifiedWhen] => Array
                        (
                        )

                )

            [1] => Array
                (
                    [code] => 1B
                    [description] => Manslaughter by Negligence
                    [modifiedWhen] => Array
                        (
                        )

                )

```

## [web service specifications](https://www.mshp.dps.mo.gov/cj08service/swagger.json)
