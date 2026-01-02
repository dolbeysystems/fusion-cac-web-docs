+++
title = 'V2.61 (Jan 2026)'
+++

{{< release-notes-header version="V2.61.9477" date="01/09/26" >}}

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add ability to schedule a report per day of the week.

**CACTWO-5976 and CACTWO-7233** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When creating a scheduled report, the user will now have the ability to schedule a report for a certain day of the week such as ‘first Tuesday of the month’ or ‘last Friday of the month’.  This has also been added to the scheduling window of the Account Search, along with the ability to report hourly. 

### Replace PSI 04 with a new failure to rescue measure.

**CACTWO-6787** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}** 

A new failure to rescue code of ISCMR will now show concurrently with PSI 04 when it applies, but it will be completely replacing PSI 04 in the future. 

### Allow scheduled reports to be restricted to particular domains

**CACTWO-7138** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new setting will now stop scheduled reports from going out to emails that are not in the configured domain.  As an example, if my setting is marked for ‘dolbey.com’, then if I put an aol.com address in the email for a scheduled report, I will be alerted that the address is not valid for the domain.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

### Make Mapping titles more noticeable

**CACTWO-7274** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Mapping titles are now in blue to make them stand out better when a user is browsing a long list. Previously they were grey and did not stand out.

![Mapping Configuration Title](MappingConfigurationTitle.png)

### Enable Columns in Account Search to be filterable

**CACTWO-7319** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The Columns button in Account Search now has a filter field at the top of the list.  Clicking on Columns brings up the column list as it is currently, and clicking the arrow lets you either select the list as "Select All" or "Unselect All". No matter how columns are pulled up, a filter box is presented at the top and will filter down the list as characters are typed. 

![Filter Columns in Account Search](AccountSearchColumnsFilter.png)

### In Audit Worksheet, add APC calculation display

**CACTWO-7515** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

For accounts with charges, the Audit Worksheet will now show APC calculations to the left of each code in the Audited Charges section if these two site_configuration settings are set to true:

1. ShowAuditAPC : true

2. ShowAuditCharges : true

### Remove trailing blank spaces in pending reson note

**CACTWO-7525** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Currently when adding a note to a pending reason, any trailing blank spaces are being saved to the record.  This has now been changed to discard trailing blank spaces upon saving the note.  

### Add Total Column to the CDI Metric Score Card report

**CACTWO-7551** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new Total column has been added to the CDI Metric Score Card which calculates the combined statistics for all months within the report.  By comparison, the Average column calculates the average statistics per month within the report. 

### Add user name to CDI Metric Score Card when sent as XLSX

**CACTWO-7575** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

If a CDI Metric Score Card report is run as XLSX and has multiple users on it, it will now split the names out on separate tabs in the XLSX report. 

### Added "Audit - Modifiers" columns to the Audits drilldown in Account Search

**CACTWO-7581** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Two new total columns have been added to the Audits Drilldown:

1. Audit- Modifiers Post Audit; AND

2. Audit-Modifiers Pre Audit.  

These will record the total based on the number of modifiers on the CPT codes or Charges.

### PC-06 designation needs to be updated for January 2026

**CACTWO-7584** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The PC-06 algorithm has been updated for January 2026 changes. This allows for a PC-06 designation for accounts that have a Discharge Disposition of ‘Transfer’ as well as ‘Expired’. 

### Remove the "No" option fromthe Final DRG Reconciliation box

**CACTWO-7588** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

An option has been added to hide the ‘No’ answer from the Final DRG Reconciliation box. The user will then only have the options to agree or cancel during reconciliation.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

### Add Total Time line to Forced Autoload Dashboard

**CACTWO-7597** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

For the sake of continuity, the line for Total Time Logged in has been added to the Forced Autoload dashboard to match the other user dashboards. 

### When moving between viewers they were marked as read-only

**CACTWO-7604** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

Under specific circumstances, when moving back and forth between viewers, they were being marked as read-only and user was unable to reopen and edit.  This has been corrected. 

### TruCode link to crosswalks was not opening

**CACTWO-7604** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

While the link for accessing crosswalks in TruCode was present, it had yet to be implemented.   That has now been added so that users can use the crosswalks. 

### Updates made to description of several reports

**CACTWO-7616** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The descriptions of the CDI Query Score Card and CDI Query Score Card by Admission Month have been updates. 

### Sync between workgroup criteria changes was not working

**CACTWO-7619** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When multiple users were in the same workgroup criteria, the ‘sync change’ ability was not working.  This has been corrected. 

### Mass Edit is not working for 'All' when adding Dx codes to CPT codes

**CACTWO-7630** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a user checkmarked the ALL button at the top of the CPT column in Mass Editing and added a DX code to the first CPT code, it was not being carried down to all of the CPT codes like it should.  This has been corrected. 

### Add new Working DRG fields foruse in Account Search

**CACTWO-7631** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

4 New fields have been added to use as search items:
* Baseline Working CC Total
* Baseline Working HAC Total
* Baseline Working HCC Total
* Baseline Working MCC Total

### Mappings were not showing all columns when using the CSV option

**CACTWO-7632** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When exporting a CSV in Mappings, some of the newly added columns were missing from the report.  This has been corrected. 

### Add checkmark next to codes in inpatient accounts

**CACTWO-7634** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A checkmark will now appear on the right of the diagnosis and procedure codes that affect the DRG according to Solventum™ or TruCode™ in these places in Fusion CAC:
* the Code Summary viewer; 
* the Final Code Summary viewer; 
* the Working CDI History viewer; 
* the Suggested DRG History viewer; AND
* the TruCode Standalone page. 

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

### Session Expiration is locking user in account

**CACTWO-7635** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a user is in an account and goes away from their session for long enough for the session to expire, the user is receiving a red error message and is not being taken out to the Login Screen.  This has been corrected. 

### Receiving an error when using invalid characters in Document Search

**CACTWO-7644** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If an invalid character is used in Document Search, ie .^$*+-?{}[]()\/|, then an invalid pattern error was showing in the Fuscion CAC log.  This has been updated so that no error occurs, and the Document Search works normally. 

### Accounts assigned to Audit workgroups were not leaving the workgroup

**CACTWO-7648** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If an auditor finished an audit and then did a Save/and route on the account to route to a custom workgroup, the account was not leaving the Audit workgroup.  This has been corrected

### Update the way diagnosis codes can be added to CPT code charges

**CACTWO-7653** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The ‘add’ table has been changed to allow better usablilty and readablity of diagnosis codes that are added to a CPT charge on an outpatient account. 

![Add Diagnoses to a CPT Code](AddDiagnosistoCPTcode.png)

![Add Diagnoses to a CPT code](AddDiagnosistoCPTcode2.png)

### E/M charges should not show in some circumstances and remarks should

**CACTWO-7658** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

ADD TEXT

### TruCode™ encoder is deleting PCS codes after clicking the 'Submit Codes' link

**CACTWO-7659** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a user has the TruCode™ encoder open and adds multiple codes via the code book, a code was being dropped when the 'Submit Codes' link was pressed to bring those codes to the Assigned codes tree.  This has been corrected. 

![Submit Codes link in TruCode™ encoder](SubmitCodesLink.png)

### Scroll Bars in TruCode™ encoder are not working properly

**CACTWO-7660** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a user changes the zoom on the encoder from 100%, the scroll bar sometimes does not go all the way to the bottom of the viewer.  This has been corrected. 

### TruCode™ encoder has drag and drop issues

**CACTWO-7661** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

In the codes section of TruCode™ encoder, when using drag and drop, the codes were getting stuck.  This has been corrected. 

### TruCode™ encoder links are not working

**CACTWO-7662** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When working in the TruCode™ encoder, if an edits icon appeared on a code indicating that additional codes should be added, clicking the “other codes” link did not open the Code Book in the Edits panel.  This has been corrected. 

### TruCode™ encoders needs a units field for CPT codes

**CACTWO-7663** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new field has been added to the TruCode™ encoder. A units field will now show at the end of each CPT code line in Outpatient runs. It will default to a count of 1.

