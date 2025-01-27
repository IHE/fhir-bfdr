After the child is born, an Encounter record will be created for the child (Encounter-Birth) and will reference this encounter using the partOf property.

### Form Mapping
This profile is mapped to:
 * Item **28. Mother Transferred for Maternal Medical or Fetal Indications for Delivery?** in the [2003 Revision of the U.S. Standard Certificate of Live Birth](https://www.cdc.gov/nchs/data/dvs/birth11-03final-ACC.pdf)
 * Item **23. Was the mother transferred to this facility for maternal medical or fetal indications for delivery?** in the [2016 US Standard Facility Worksheet for the Live Birth Certificate](https://www.cdc.gov/nchs/data/dvs/facility-worksheet-2016-508.pdf)
 * Item **7. Place Where Delivery Occurred** in the [2003 Revision of the U.S. Standard Report of Fetal Death](https://www.cdc.gov/nchs/data/dvs/FDEATH11-03finalACC.pdf)
 * Item **8. Facility Name / address** in the [2003 Revision of the U.S. Standard Report of Fetal Death](https://www.cdc.gov/nchs/data/dvs/FDEATH11-03finalACC.pdf)
 * Item **9. Facility Id** in the [2003 Revision of the U.S. Standard Report of Fetal Death](https://www.cdc.gov/nchs/data/dvs/FDEATH11-03finalACC.pdf)
 * Item **1. Facility name** in the [2019 US Standard Facility Worksheet for the Report of Fetal Death](https://www.cdc.gov/nchs/data/dvs/fetal-death-facility-worksheet-2019-508.pdf)
 * Item **1. Facility address** in the [2019 US Standard Facility Worksheet for the Report of Fetal Death](https://www.cdc.gov/nchs/data/dvs/fetal-death-facility-worksheet-2019-508.pdf)
 * Item **2. Facility I.D. (National Provider Identifier)** in the [2019 US Standard Facility Worksheet for the Report of Fetal Death](https://www.cdc.gov/nchs/data/dvs/fetal-death-facility-worksheet-2019-508.pdf)
 * Item **5. Place of delivery** in the [2019 US Standard Facility Worksheet for the Report of Fetal Death](https://www.cdc.gov/nchs/data/dvs/fetal-death-facility-worksheet-2019-508.pdf)

### IJE Mapping

| **Use Case** | **IJE Field#** | **Description** | **IJE Name** | **Field** |
| ------------ | -------------- | --------------- | ------------ | --------- |
| Natality | 302 | Facility Mother Moved From (if transferred) | HOSPFROM | hospitalization.origin |
| Natality | 125 | Mother Transferred? | TRAN | Encounter-maternity.hospitalization.admitSource |
| Fetal Death | 231 | Place of Delivery Street Address | ADDRESS_D | address |
| Fetal Death | 230 | Place of Delivery Unit or Apartment Number | APTNUMB_D | location.location.address |
| Fetal Death | 349 | Date Signed by Certifier--Day | CERTIFIED_DY | participant:certifier.period.start |
| Fetal Death | 348 | Date Signed by Certifier--Month | CERTIFIED_MO | participant:certifier.period.start |
| Fetal Death | 347 | Date Signed by Certifier--Year | CERTIFIED_YR | participant:certifier.period.start |
| Fetal Death | 234 | Place of Delivery City/Town/Place (literal)  | CITY_D | location.location.address |
| Fetal Death | 233 | Place of Delivery County (literal) | CNTY_D | location.location.address |
| Fetal Death | 236 | Place of Delivery Country (literal) | COUNTRY_D | location.location.address |
| Fetal Death | 11 | Place Where Delivery Occurred | DPLACE | location.physicalType |
| Fetal Death | 12 | Facility ID (NPI) - If available | FNPI | location.identifier |
| Fetal Death | 224 | Name of Delivery Facility | HOSP_D | name |
| Fetal Death | 339 | Facility Mother Moved From (if transferred) | HOSPFROM | hospitalization.origin |
| Fetal Death | 229 | Place of Delivery Post Directional | POSTDIR_D | location.location.address |
| Fetal Death | 226 | Place of Delivery Pre Directional | PREDIR_D | location.location.address |
| Fetal Death | 13 | Facility ID (State-Assigned) | SFN | identifer |
| Fetal Death | 235 | State, U.S. Territory or Canadian Province of Place of Delivery - literal | STATE_D | location.location.address |
| Fetal Death | 228 | Place of Delivery Street designator | STDESIG_D | location.location.address |
| Fetal Death | 227 | Place of Delivery Street name | STNAME_D | location.location.address |
| Fetal Death | 225 | Place of Delivery Street number | STNUM_D | location.location.address |
| Fetal Death | 232 | Place of Delivery Zip code and Zip+4 | ZIPCODE_D | location.location.address |
{: .grid }
