+++
title = 'Custom Fields'
weight = 20
+++

The following table lists common fields that are implemented on an as-needed basis depending on
requirements and licensing.

| Display Name                           | Field Description                                                                                                                                                                                      |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Charge CPT Codes                       | Computed as a list of CPT codes assigned to Charges. Does not apply to Transactions.                                                                                                                   |
| Charge Revenue Codes                   | Computed as a list of Revenue Codes assigned to Charges. Does not apply to Transactions.                                                                                                               |
| Is Prior HCC Present                   | Computed as True if any prior account of the patient contains an HCC code. Field is defined in the site's ADT script and performs a database lookup upon receipt of ADT for prior accounts.            |
| Last Suggested Calculation Date/Time   | This is the last suggested DRG calculation date and time. The site must be licensed to use Suggested DRG Module.                                                                                       |
| Last Suggested DRG                     | This is the last suggested DRG. Site must be licensed to use Suggested DRG Module.                                                                                                                     |
| Last Suggested DRG Description         | This is the last suggested DRG Description. Site must be licensed to use Suggested DRG Module.                                                                                                         |
| Last Suggested DRG Weight              | This is the last suggested DRG Weight. Site must be licensed to use Suggested DRG Module.                                                                                                              |
| Last Suggested Estimated Reimbursement | This is the last suggested DRG Estimated Reimbursement. Site must be licensed to use Suggested DRG Module.                                                                                             |
| PSI Indicator                          | This is the PSI’s that were identified by a coder user. The PSI indicator is identified by using the patient safety indicator technical specifications. This field requires the quality module.        |
| Quality Measure                        | This is a field used to identified if a coder user identified PC-06. The PC-06 indicator is identified by using the quality measures technical specifications. This field requires the quality module. |
| CDI PSI Indicator                      | This is the PSI’s that were identified by a CDI user. The PSI indicator is identified by using the patient safety indicator technical specifications. This field requires the quality module.          |
| CDI Quality Measure                    | This is a field used to identified if a CDI user identified PC-06. The PC- 06 indicator is identified by using the quality measures technical specifications. This field requires the quality module   |

