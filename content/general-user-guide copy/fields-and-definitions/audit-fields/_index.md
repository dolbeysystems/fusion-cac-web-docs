+++
title = 'Audit Fields'
weight = 40
+++

Below are the section of the audit worksheet and the definition of the field as to how it was calculated. If the
auditor disagrees with any of the auto-calculated fields below the auditor can choose to override the field by
entering in the value that makes sense per the audit, the system will provide an audit trail to show what the
value was changed from and to for transparency along with the user that made the change and the date/time
the change was performed.

| Field                            | Field Description                                                                             |
| -------------------------------- | --------------------------------------------------------------------------------------------- |
| Audit Closed by First Name       | This is the auditor/coder first name who closed the audit.                                    |
| Audit Closed by Last Name        | This is the auditor/coder last name who closed the audit.                                     |
| Audit Closed by User Id          | This is the auditor/coder user Id who closed the audit.                                       |
| Audit Closed Date                | This is the date the audit was closed.                                                        |
| Audit Coder Agree                | This is if the coder agreed with the audit or if they decided to rebuttal.                    |
| Audit Coder of Record First Name | This is the coders first name that last submitted the chart prior to audit start.             |
| Audit Coder of Record Last Name  | This is the coders last name that last submitted the chart prior to audit start.              |
| Audit Coder of Record User Id    | This is the coders user Id that last submitted the chart prior to audit start.                |
| Audit Opened by First Name       | This is the auditor first name whom opened the audit.                                         |
| Audit Opened by Last Name        | This is the auditor’s last name who opened the audit.                                         |
| Audit Opened by User Id          | This is the auditor user Id who opened the audit.                                             |
| Audit Opened Date                | This is the date the audit was opened by the auditor.                                         |
| Audit Rebutted by First Name     | This is the coders first name who rebutted the audit.                                         |
| Audit Rebutted by Last Name      | This is the coders last name who rebutted the audit.                                          |
| Audit Rebutted by User Id        | This is the coders user Id who rebutted the audit.                                            |
| Audit Rebutted Date              | This is the date the audit was first rebutted.                                                |
| Audit Rebuttal Comment           | This is the rebuttal comment from the coder.                                                  |
| Audit Response to Rebuttal       | This is the response from the auditor for the rebuttal from the coder.                        |
| Audit Returned Date              | This is the date that the audit was returned to the coder.                                    |
| Audit Sub-Types                  | This is the audit sub-type.                                                                   |
| Audit Type                       | This is the audit type.                                                                       |
| Audit Training Topics            | These are the training topics if applicable that the auditor recommends for the coder.        |
| Audit Training Recommendations   | This is the training recommendations if applicable that the auditor recommends for the coder. |
| Discharge Disposition Changed?   | This is a true or false field. If the Discharge Disposition was changed from the previous Disposition assignment the field will result in true which is counted as one error and if it was not changed it will result in false which is not counted as an error. N/A is available in the event the auditor wants to list it as not applicable to the audit.|
| Abstracting Pre-Audit            | The total is the number of abstracting components there were at the time the audit is started. Abstractions Pre-Audit = (Total Procedure and CPT Codes x 2) + 1 for Discharge Disposition + 1 for Consulting Providers if Present). Procedure and CPT Codes are multiplied by two since there are to abstraction opportunities which is date of service and preforming provider. |
| Abstracting Errors               | This is the total codes that appear in the above boxes the formula is as followed: Abstracting Errors = Procedure (PCS/CPT) Date Changes + Procedure (PCS/CPT) Provider Changes + Discharge Disposition Changes + Consulting Provider Changes.|
| Abstracting Error Rate           | This is the total abstracting error rate as a percentage the formula is: Abstracting Errors = Procedure (PCS/CPT) Date Changes + Procedure (PCS/CPT) Provider Changes + Discharge Disposition Changes + Consulting Provider Changes/Abstracting Pre-Audit.|
| Abstracting Accuracy Rate        | This is the total abstracting accuracy as a percentage the formula is: Abstracting Error Rate = (Procedure (PCS/CPT) Date Changes + Procedure (PCS/CPT) Provider Changes + Discharge Disposition Changes + Consulting Provider Changes/Abstracting Pre-Audit) – 100%.   
| CPT Codes Pre-Audit              | The total is the number of CPT codes including principal and secondary at the time the audit is started.|
| CPT Codes Post-Audit    | The total is the number of CPT codes including principal and secondary at the time the auditor selects the Update Codes button|
| CPT Codes Edited        | This is the count of the total of edit actions by the auditor for principal and secondary codes once the auditor selects the update codes button. An edit is defined as a simple change to the same code category such as the last digit of a code however if the auditor replaced the full code this is still counted as an edit rather than an unassign and an add. The editing action is defined by right clicking on a code from the assigned code tree and selecting edit CPT code with a replacement procedure code.|
| CPT Codes Unassigned    | This is the count of the total of deleted or unassign actions by the auditor for principal and secondary codes once the auditor selects the update codes button. The unassign action is defined by right clicking on a code from the assigned code tree and selecting one of the unassign principal code, unassign as secondary, unassign all episodes or by selecting edit procedure code and deleting the code.|
| CPT Codes Added         | This is the count of the total of added or assign actions by the auditor for principal and secondary codes once the auditor selects the update codes button. The assign action is defined by right clicking on a code from the unassigned code tree and selecting assign as principal or secondary, right clicking on a code to validate from a document or adding a code that did not exist previously.|
| Principal CPT Changed   | This is a true or false field. If the principal CPT was changed from the previous code assignment the field will result in true which is counted as one error and if it was not changed it will result in false which is not counted as an error. N/A is available in the event the auditor wants to list it as not applicable to the audit.|
| Total Modifiers Added   | This is the count of the total of added modifiers on a CPT by the auditor where the code previously existed. If the code was already counted within the CPT Codes Added section to prevent duplication of errors. The added action is defined by right clicking on a code from the assigned code tree and selecting to edit to add a modifier.|
| Total Modifiers Removed | This is the count of the total of removed modifiers on a CPT by the auditor where the code previously existed. If the code was already counted within the CPT Codes Added section to prevent duplication of errors. The removed action is defined by right clicking on a code from the assigned code tree and selecting to edit to remove an existing modifier.|
| CPT Errors              | This is the total codes that appear in the above boxes the formula is as followed: CPT Errors = CPT Codes Added + CPT Codes Edited + CPT Codes Unassigned + Principal CPT Changed.|
| CPT Error Rate          | This is the total codes that appear in the above boxes the formula is as followed: CPT Error Rate = Procedure Codes Added + Procedure Codes Edited + Procedure Codes Unassigned + Principal CPT Changed/CPT Codes Pre-Audit|
| CPT Accuracy Rate       | This is the total codes that appear in the above boxes the formula is as followed: CPT Error Rate = (CPT Codes Added + CPT Codes Edited + CPT Codes Unassigned + Principal CPT Changed/CPT Codes Pre-Audit) – 100%                                                                                                                                                                               

