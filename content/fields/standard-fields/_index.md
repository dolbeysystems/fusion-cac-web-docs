+++
title = 'Standard Fields'
weight = 10
+++

The following table contains a list of all standard fields available. 

| Display Name                   | Field Description |
| ------------------------------ | ----------------- |
| Abstract Patient Class         | This is the abstraction Patient Class for the patient chart. |
| Account Number                 | This is the account number for the patient chart. |
| Account Status                 | This is the account status for the patient chart. |
| Active Matched Criteria Groups | This is the total number of active criteria groups on a patient chart. |
| Added to Images                | This is how many total codes were added to an image document. |
| Admit Date                     | This is the admit date of the patient. Even though the field is named admit date time it only displays the date. |
| Admit Date w/ Time             | Computed to display the patient's admit date with the admit time |
| Admit Diagnosis Codes          | This is the admit diagnosis code of the patient chart. |
| Admit Reason                   | This is the admit reason which comes from ADT. |
| Admit Source                   | This is the admit source of the patient chart. |
| Admit Type                     | This is the admit type on the patient chart. |
| Admitting Physician            | Computed to display the first physician name with a role of Admitting. |
| Admitting Physician ID         | Computed to display the first physician ID with a role of Admitting. |
| Age in Years                   | Computed to display the patient's age in years. |
| Assigned CPT Code              | This is used to search for a chart with an assigned CPT code. |
| Assigned Diagnosis Code        | This is used to search for a chart with an assigned diagnosis code. |
| Assigned POA                   | |
| Assigned Procedure Codes       | This is used to search for a chart with an assigned procedure (PCS) code. |
| Assigned Visit Reason Codes    | This is used to search for a chart with an assigned visit reason code. |
| Attending Physician            | Computed to display the first physician name with a role of Attending |
| Attending Physician ID         | Computed to display the first physician ID with a role of Attending |
| AutoClose Date/Time            | This is the date and time the patient chart was autoclosed. |
| AutoClose Rejection Reason     | This is the reason why the patient chart was rejected from autoclose. |
| Baseline Working APRDRG        | This is the Baseline APR-DRG. |
| Baseline Working DRG           | This is the Baseline DRG. |
| Baseline Working DRG Weight    | This is the Baseline DRG Weight. |
| Baseline Working Estimated Reimbursement | This is the Baseline DRG Estimated Reimbursement. |
| Billing Countdown              | The billing countdown will tell you how many days left to bill the payor. In Mapping Configuration, if you add or edit a mapping for "Payor", you see a new "Default Bill Days" field in the header and a new "Bill Days" column for each Payor. These fields contain numbers zero or higher or blank to indicate the number of days to add to the discharge date (current date is there is no discharge date) to calculate what is basically a billing due date. The billing date is compared to the current date (or the last submitted date if the account is already submitted) to compute the "Billing Countdown" – the number of days left to submit an account. If an account has no payor, no matching payor mapping, or payor mapping with no "bill days" defined, the "default bill days" is used (zero if "default bill days" is blank as well.) |
| Bed                            | This is the last known patients bed. |
| Birth Weight (g)               | This is the patients birth weight in grams. This can be provided either through the ADT interface or manually entered by a coder. |
| Building                       | This is the last known patients building which is usually equal to the nursing unit or location. |
| Campus                         | This is the last known patient’s campus. |
| Category                       | This is a Dolbey created patient type to assist with reporting because often a patient type field needed to be joined with a location, hospital service or other fields to alter reporting for productivity categories join those fields to create custom patient types for easy productivity and DNFC reporting. |
| Calculated Date/Time           | This field shows you the last time the encoder was last run, if it's blank, the encoder needs to be run. This is so that in Account Search and workflow. This can help find an accounts that the user should have an APC, DRG or if you are reviewing to see if a coder clicked on the encode to run edits |
| CDI Physician Queries Agreed   | This is the outcome of the query reporting by the CDI user closing the query. Agree commonly means that the physician provided the CDI with a valid diagnosis. |
| CDI Physician Queries Cancelled | Not accessible in Form Designer. You can customize these by adding a mapping table using this key PhysicianQueryCancelReasons this will overwrite the default cancel options. |
| CDI Physician Queries Closed   | This is the total number of physician queries closed issued by a CDI user. |
| CDI Physician Queries Disagreed | This is the outcome of the query reporting by the CDI user closing the query. Disagree commonly means that the physician provided the CDI with a different result than expected. |
| CDI Physician Queries No Opinion | This is the outcome of the query reporting by the CDI user closing the query. No Opinion commonly means that the physician provided the CDI with a clinically insignificant diagnosis. |
| CDI Physician Queries No Response | This is the total number of physician queries closed by a CDI user due to no response from the physician. |
| CDI Physician Queries Open     | This is the total number of physician queries still open issued by a CDI user. |
| CDI Physician Queries Responded | This is the total number of physician queries responded to by Physician for issued by a CDI user. |
| CDI Physician Query Total      | This is the total number of physician queries issued by a CDI user regardless of if the query is open or closed. If a user was in an account that had an open physician query, and an external interface closed that query, the query total on the account is updated upon closing the account. |
| Coding Ready End Date/Time     | This is a field used to identify the end date used for when a chart is completed by coding. |
| Coding Ready Start Date/Time   | This is a field used to identify the start date used for when a chart is ready for coding. |
| Days to First Submit           | This column will show the difference between the Discharge Date and the date the account was first submitted. This will also include the time along with the date, so the number will be shown as a decimal. |
| Denial Billed DRG              | This is a field from the denial management viewer to display the billed DRG. |
| Denial Code Change Needed      | This is a field from the denial management viewer to display if a code change is needed. |
| Denial Coder Id                | This is a field from the denial management viewer to display the Coder Id that is to work the denial which could also be the coder of record. |
| Denial Codes in Question       | This is a field from the denial management viewer to display the Code(s) in Question. |
| Denial Complete                | This is a field from the denial management viewer to display if the denial is completed. |
| Denial DRG Change Needed       | This is a field from the denial management viewer to display the if a DRG change is needed. |
| Denial Final Appeal Date       | This is a field from the denial management viewer to display the Final Appeal Date. |
| Denial First Appeal Date       | This is a field from the denial management viewer to display the First Appeal Date. |
| Denial First Appeal Sent Date  | This is a field from the denial management viewer to display the First Appeal Sent Date. |
| Denial HIMS Received Date      | This is a field from the denial management viewer to display the HIMS Received Date. |
| Denial Manager Assigned Date   | This is a field from the denial management viewer to display the Manager Assigned Date. |
| Denial Notification Letter Date | This is a field from the denial management viewer to display the Notification Letter Date. |
| Denial Outcome                 | This is a field from the denial management viewer to display the Outcome of the Denial. |
| Denial Payer DRG               | This is a field from the denial management viewer to display the Payer DRG. |
| Denial Reason                  | This is a field from the denial management viewer to display the reason of the Denial. |
| Denial Response Due Date       | This is a field from the denial management viewer to display the Response Due Date. |
| Denial Reviewer ID             | This is a field from the denial management viewer to display the Reviewer ID. |
| Denial Second Appeal Route     | This is a field from the denial management viewer to display the Second Appeal Route. |
| Denial Second Appeal Sent Date | This is a field from the denial management viewer to display the Second Appeal Sent Date. |
| Denial Status                  | This is a field from the denial management viewer to display the status of the Denial. |
| Denial Third Appeal Route      | This is a field from the denial management viewer to display the Third Appeal Route. |
| Denial Third Appeal Sent Date  | This is a field from the denial management viewer to display the Third Appeal Sent Date. |
| Denial Type                    | This is a field from the denial management viewer to display the type of the Denial. |
| Discharge Date                 | This is the discharge date of the patient. |
| Discharge Date w/ Time         | This is the discharge date with the time of the patient. |
| Discharge Disposition          | This is the discharge disposition of the patient. |
| Discharge Date w/ Time         | Computed to display the patient's discharge date with discharge time |
| Discharged To                  | This is where the patient was discharged to. |
| Document Code                  | This is used to find any code suggested by the engine or added by a user assigned or unassigned. |
| Document Type                  | This is a field to identify a unique document name that is on a patient chart. |
| DRG Weight Difference          | Computed to display the Final DRG Weight minus the Baseline Working DRG Weight |
| Effective Date                 | This is a field used to drive reoccurring patient charts. If the coder is coding multiple encounters within a single encounter in order to generate a bill for each they would code, set an effective date and save to generate an outbound message. If they need to code for another encounter date within the same they would change the date and re-save the account. |
| Exclude from Matched Criteria  | This is a field to identify when we do not want a criteria group to display on the match criteria viewer. |
| Facility                       | This is the facility of the patient. |
| Final ALOS                     | This is the final ALOS on the patient chart. |
| Final APR-DRG                  | This is the final APR-DRG on the patient chart. |
| Final APR-DRG Description      | This is the final APR-DRG Description on the patient chart. |
| Final APR-DRG GLOS             | This is the final APR-DRG GMLOS on the patient chart. |
| Final APR-DRG Weight           | This is the final APR-DRG weight on the patient chart. |
| Final CC Total                 | This is the final CC total on the patient chart. |
| Final DRG                      | This is the final DRG on the patient chart. |
| Final DRG Description          | This is the final DRG Description on the patient chart. |
| Final DRG Weight               | This is the final DRG weight on the patient chart. |
| Final Estimated Reimbursement  | This is the final DRG Estimated Reimbursement on the patient chart. |
| Final GLOS                     | This is the final DRG GMLOS on the patient chart. |
| Final HAC Total                | This is the final HAC total on the patient chart. |
| Final HCC Total                | This is the final HCC total on the patient chart. |
| Final MCC Total                | This is the final MCC total on the patient chart. |
| Final PPC Total                | This is the final PPC total on the patient chart. |
| Final Risk of Mortality        | This is the final APR-DRG ROM on the patient chart. |
| Final Severity of Illness      | This is the final APR-DRG SOI on the patient chart. |
| Financial Class                | This is the financial class of the patient. |
| First CDI Owner First Name     | This is the first CDI owner first name on the patient chart. |
| First CDI Owner Last Name      | This is the first CDI owner last name on the patient chart. |
| First CDI Owner Date           | This is the first CDI owner date on the patient chart. |
| First CDI Owner                | This is the first CDI owner user Id on the patient chart. |
| First CDI Saver First Name     | This is the first CDI saver first name on the patient chart. |
| First CDI Saver Last Name      | This is the first CDI saver last name on the patient chart. |
| First CDI Saver Date           | This is the first CDI saver date on the patient chart. |
| First CDI Saver                | This is the first CDI saver user Id on the patient chart. |
| First Coded Date               | This is the first time the chart was submitted. |
| First Coder First Name         | This is the first users first name that submitted the chart. |
| First Coder Last Name          | This is the first users last name that submitted the chart. |
| First Coder User ID            | This is the first users user Id that submitted the chart. |
| First CPT Code                 | This is the first sequenced CPT code coded by a coder. |
| First Diagnosis Code           | This is the first sequenced Diagnosis code coded by a coder. |
| First Procedure Code           | This is the first sequenced Procedure PCS code coded by a coder. |
| First Submitter First Name     | This is the first users first name to submit the patient chart. |
| First Submitter Last Name      | This is the first users last name to submit the patient chart. |
| First Submitted Date           | This is the first date the patient chart was submitted. |
| First Submitter User ID        | This is the first user id to submit the patient chart. |
| Floor                          | This is the last known patients floor location. |
| Has Late-Arriving Documents    | This field identifies if there are late arriving documents. The field "Has Late-Arriving Documents" is a true/false field that exists only in Workflow Management. It is not a "grid column". For Account Search, the field "Late Document Count" is a numeric field that displays the number of late-arriving documents. The criteria "Late Document Count > 0" in Account Search is equivalent to "Has Late-Arriving Documents equals True" in Workflow Management. |
| Hospital Service               | This field is used to identify the patients hospital service. |
| Is AutoClosed                  | This is a field that will tell if you if the chart was autoclose by the system. True means that it was. |
| Is Emergency Room Visit        | This field identifies if the chart is an ER visit. |
| Is Inpatient                   | This field identifies if the chart is an inpatient chart. |
| Is DRG Reconciled              | This is a field to tell if a patient chart was reconciled on submit. True means that either the Last known Working or alternative DRG matched the Final DRG. False means that either the patient charts Last known Working or alternative DRG listed did not match the Final DRG. This field is only applicable on inpatient charts. |
| Is Released by CDI             | This field shows if the CDI user released the chart while in the reconciliation process on behalf of the coder from the submit state the coder originally submitted. |
| Is Resubmitted                 | Is Resubmitted is a term used to mean the chart was completed by coding and the chart had already had a submit action performed. If Is Resubmitted is True that means a coder has submitted this chart to billing a subsequent time. If Is Resubmit is equal to false then the chart has not been resubmitted and it was only submitted a single time. |
| Last Interface Update          | This is the last date and time the interface received an update to the account. |
| Last CDI Owner First Name      | This is the last CDI Owners first name. An ownership can be claimed by selecting the owner button on the code summary viewer. |
| Last CDI Owner Last Name       | This is the last CDI Owners last name. An ownership can be claimed by selecting the owner button on the code summary viewer. |
| Last CDI Owner Date            | This is the last CDI Owner date they saved the account. An ownership can be claimed by selecting the owner button on the code summary viewer |
| Last CDI Owner User ID         | This is the last CDI Owners user id. An ownership can be claimed by selecting the owner button on the code summary viewer. |
| Last CDI Saver First Name      | This is the last CDI user that saved the accounts first name. |
| Last CDI Saver Last Name       | This is the last CDI user that saved the accounts last name. |
| Last CDI Saver Date            | This is the last CDI user that saved the accounts date. |
| Last CDI Saver User ID         | This is the last CDI user that saved the accounts user id. |
| Last Saver First Name          | This is the last coder user that saved the accounts first name. |
| Last Saver Last Name           | This is the last coder user that saved the accounts last name. |
| Last Saved Date                | This is the last coder user that saved the accounts date. |
| Last Saver User ID             | This is the last coder user that saved the accounts user id. |
| Last Submitter First Name      | This is the last coder user that submitted the accounts first name. |
| Last Submitter Last Name       | This is the last coder user that submitted the accounts last name. |
| Last Submitted                 | Date This is the last coder user that submitted the accounts date. |
| Last Submitter User ID         | This is the last coder user that submitted the accounts user id. |
| Last Viewer First Name         | This is the last viewer’s first name to view the account without saving or submitting. |
| Last Viewer Last Name          | This is the last viewer’s last name to view the account without saving or submitting. |
| Last Viewer                    | This is the last viewer’s user id to view the account without saving or submitting. |
| Last Viewed Date/Time          | This is the last viewer’s date they viewed the account without saving or submitting. |
| Late Document Count            | This is the total documents that were late. Late is defined as post submit. |
| Late Document Type             | This is the document types that are late arriving. |
| Length of Stay                 | Calculated; This is the current Length of Stay on the patient’s chart. This is Admit Date to Discharge Date and if Discharge Date is not present then it’s calculated to today's date. This is different than the ALOS and the GMLOS that is calculated by the encoder. Often referred to as the LOS. |
| Location                       | This field can store the location but, commonly the location is stored within the building field not the location field. |
| Locked By                      | This is the current user that has the account locked which is defined by actively in use. |
| Locked Date/Time               | This is the date and time the account became locked in use by the current user. |
| Next Review Date               | This field can be changed to a different date other than the default which is every day. This field is used by the CDI team to indicate the date that they want the chart routed back to the follow-up review worklist. This field can be found on the code summary page changing the calendar date field from the date displayed to a future date. This will tell the chart to not route back to the “Follow-up Review” until the current calendar date matches the date you changed the next review date to. |
| New Document Flag              | Computed to true if any documents were imported onto account after the last time the account was saved. The user would see in the accounts grid a check mark to indicate True; Not accessible in Form Designer |
| Owner First Name               | This is the current Owners first name. An ownership can be claimed by selecting the owner button on the code summary viewer. |
| Owner Last Name                | This is the current Owners last name. An ownership can be claimed by selecting the owner button on the code summary viewer. |
| Owner Name                     | This is the current Owner date they saved the account. An ownership can be claimed by selecting the owner button on the code summary viewer. |
| Owner User ID                  | This is the current Owners user id. An ownership can be claimed by selecting the owner button on the code summary viewer. |
| Patient Birth Date             | This is the patients birth date. |
| Patient First Name             | This is the patient’s first name. |
| Patient Gender                 | This is the patient’s gender. |
| Patient Last Name              | This is the patient’s last name. |
| Patient MRN                    | This is the patients’ medical record number. |
| Patient Middle Name            | This is the patient’s middle name. |
| Patient Class                  | This is the patient class of the account. |
| Patient Type                   | This is the patient type of the account. |
| Payor                          | This is the primary payor of the account. |
| Payor (Secondary)              | This is the secondary payor of the account. |
| Pending Reason                 | An account can have zero or more pending reasons. Each pending reason can have additional properties Mappings Configuration and provides the client to control what pending reason are displayed for the role the end user has in addition to what other information should be recorded with a pending reason such as provider and date. Commonly, pending reasons can also trigger workflow and validation rules to ask the end user to take other actions such as adding a form to collect additional data such as CDI Questions or Quality Initiatives detail. |
| Pending Reason Physician Name  | This is the physicians name that is attached to the pending reason. |
| Pending Reason Physician ID    | This is the physicians Id that is attached to the pending reason. |
| Physician Coding Stage         | This is the stage of the account for physician coding which is independent from the stage field which is known as the facility stage. |
| Physician Queries Agreed       | This is the outcome of the query reporting by the physician coding user closing the query. Agree commonly means that the physician provided the CDI with a valid diagnosis. |
| Physician Queries Cancelled    | This is the outcome of the query reporting by the physician coding user closing the query as cancelled. You can customize these by adding a mapping table using this key PhysicianQueryCancelReasons this will overwrite the default cancel options. |
| Physician Queries Closed       | This is the total number of physician queries closed issued by a physician coding user |
| Physician Queries Disagreed    | This is the outcome of the query reporting by the physician coding user closing the query. Disagree commonly means that the physician provided the physician coding with a different result than expected. |
| Physician Queries No Opinion   | This is the outcome of the query reporting by the physician coding user closing the query. No Opinion commonly means that the physician provided the physician coding with a clinically insignificant diagnosis. |
| Physician Queries No Response  | This is the total number of physician queries closed by a physician coding user due to no response from the physician. |
| Physician Queries Open         | This is the total number of physician queries still open issued by a physician coding user. |
| Physician Query Responded      | This is the total number of physician queries responded to by Physician for issued by a physician coding user. |
| Physician Query Total          | This is the total number of physician queries issued by a physician coding user regardless of if the query is open or closed. If a user was in an account that had an open physician query, and an external interface closed that query, the query total on the account is updated upon closing the account. |
| Pre-Bill Working DRG           | This is the working DRG pre-bill. |
| Pre-Bill Working DRG Description | This is the working DRG Description pre-bill. |
| Pre-Bill Working DRG Weight    | This is the working DRG Weight pre-bill. |
| Pre-Bill Final DRG             | This is the final DRG pre-bill. |
| Pre-Bill Final DRG Description | This is the final DRG Description pre-bill. |
| Pre-Bill Final DRG Weight      | This is the final DRG Weight pre-bill. |
| Pre-Bill DRG Match             | This field is shows true or false. True meaning that there was a pre- bill DRG match of the last know working and the final DRG. |
| Pre-Visit Account Number       | Not accessible in Form Designer |
| Primary Grouper                | This is the primary grouper of the account. |
| Principal CPT Code             | This is the principal CPT code on the account. |
| Principal CPT Physician        | This is the principal CPT code abstracted physician. |
| Principal CPT Modifier         | This is the principal CPT code modifier(s). The user can add up to 4 modifiers unless they are using the 3M CRS encoder, then they will be able to add up to 5 modifiers. |
| Principal Diagnosis Code       | This is the principal diagnosis code on the account. |
| Principal Procedure Code       | This is the principal procedure (PCS) code on the account. |
| Principal Procedure Physician  | This is the principal procedure (PCS) code abstracted physician. |
| PSI Indicator                  | This is the PSI’s that were identified by a coder user. The PSI indicator is identified by using the patient safety indicator technical specifications. This field requires the quality module. |
| Public Note User ID            | This is the users id that created the public note. |
| Public Note Date/Time          | This is the date and time that the public note was created. |
| Public Note                    | This is the public note. |
| Random Inclusion Factor        | Computed to display a random number between 1 and 100; Not accessible in Form Designer |
| Room                           | This is the last known room of the patient. |
| Secondary Grouper              | This is the secondary grouper of the account. |
| Service Type                   | This is the service type of the account. |
| Stage                          | The stage of the patient tells you if the patient chart is unbilled, billed (submitted), In Review (QA). |
| Submit Account for Post- QA    | This is used in workflow to define when a chart qualifies for a QA Review worklist if it should be prebill or post bill review. True indicates it will be a post bill account and False is Prebill. |
| Time Spent By CDI              | This is the total time spent in an account for a user with a CDI role. |
| Time Spent By First Coder      | This is the total time spent in an account for the first timefor a user with a Coder role. |
| Time Spent By Coding           | This is the total time spent in an account and any subsequent time after the first time it was saved or submitted for a user with a Coder role |
| Total Charges                  | This is the total charges on the patient chart. Commonly, this information is sent on the ADT interface. |
| Total Documents                | Computed to display the total number of documents on the account. |
| Transfer From                  | This is where the patient was transferred from. |
| Transfer To                    | This is where the patient was transferred to. |
| Validation Rule Count at Submit | This tells you if there were any active validation rules at Submit. |
| Workflow Trigger Date          | Not accessible in Form Designer |
| Workgroup                      | This field identifies what current default workgroup the patient chart is currently within. |
| Workgroup Assigned By          | This is used to indicate that user manually assigned the chart to another user’s “You” worklist. |
| Workgroup Category             | This field identifies what current workgroup(s) category the patient chart is currently within. |
| Workgroup Assigned Date        | This field identifies the date that the patient chart qualified for the current workgroup. |
| Workgroup Submitted            | This is used in QA workflow to identify that a chart should not requalify for a QA workgroup if it was previously submitted from it to prevent chart looping. |
| Workgroup Type                 | In Workflow Management, each workgroup now has a new "WorkGroup Type" field. This field is optional, but sites can designate a type for each workgroup. The purpose of doing so is for current and future reporting. For this feature, setting a workgroup to a type besides "Coding" will exclude the account's time assigned to it in the "Coding Chart Status Report". |
| Working Admit Diagnosis Code   | This is the working admit diagnosis code. |
| Working ALOS                   | This is the working ALOS. |
| Working APRDRG                 | This is the working APR-DRG. |
| Working APRDRG Description     | This is the working APR-DRG Description. |
| Working APRDRG GLOS            | This is the working APR-DRG GMLOS. |
| Working CC Total               | This is the working CC total count. |
| Working CPT Codes              | This is used to identify working CPT Codes. |
| Working Diagnosis Codes        | This is used to identify working diagnosis Codes. |
| Working DRG                    | This is the working DRG. |
| Working DRG Description        | This is the working DRG Description. |
| Working DRG Weight             | This is the working DRG Weight. |
| Working Estimated Reimbursement | This is the working DRG Estimated Reimbursement. |
| Working GLOS                   | This is the working DRG GMLOS. |
| Working HAC Total              | This is the working HAC total count. |
| Working HCC Total              | This is the working HCC total count. |
| Working MCC Total              | This is the working MCC total count. |
| Working PPC Total              | This is the working PPC total count. |
| Working Principal CPT Code     | This is used to identify working principal CPT Codes. |
| Working Principal Diagnosis Code | This is used to identify working principal diagnosis Codes. |
| Working Principal Procedure Code | This is used to identify working principal procedure (PCS) Codes. |
| Working Procedure Codes        | This is used to identify working procedure (PCS) Codes. |
| Working Risk of Mortality      | This is the working APR-DRG ROM. |
| Working Severity of Illness    | This is the working APR-DRG SOI. |
| Working Visit Reason Codes     | This is used to identify working Visit Reason Codes. |

