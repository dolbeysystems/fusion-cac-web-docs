+++
title = 'V2.59 (Jun 2025)'
+++

{{< release-notes-header version="V2.59.9302" date="06/20/25" >}}

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Validation Rules for Query Details

**CACTWO-6102** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A [Validation Rule](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/code-summary/review-validation-rules/) can now be created to trigger based on physician query details. The option of ‘Queries’ has been added in the For Each selection to allow this to be possible. 

![Create Query Rule](QueryRuleForEach.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Column to Tuning Dashboard Code drill down

**CACTWO-6508 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

In the [Tuning](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tuning/) Dashboard, clicking on a code to open it will now display a new column ‘Submitted By’, with the submitter’s full name. 

![Submitted By Tuning Drill Down](SubmittedByColumn.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Document Date to hover over

**CACTWO-6777 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

In the [Document tree](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/#documents-tree), the hover over on the document name provides a physician’s name if it exists. The date of the document will now also show in the hover over if it exists. 

![Document Hover Over](DocumentHoverOver.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Change Mapping Values to Descriptions in Show History

**CACTWO-6987 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

[Show History](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/code-summary/#show-history) shows the mapping value (key) in the Visual Difference column. This has been changed to use the description of the mapping (friendly name) so that the change is more easily understood. 

![Mapping Value in Show History](MappingValueShowHistory.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Active CDI/Clinical Alerts as Selectable Criteria

**CACTWO-7024 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Active Alerts has been added as a [Grid Column](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/grid-column-configuration/), and has been added to [Workflow](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/workflow-management/) Criteria so that workflow can be created using Active Alerts as a property. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add an Option to Factor in Estimated Reimbursement Differences During the DRG Reconciliation Process.

**CACTWO-7055** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new configuration setting is now available that can require DRG Reconciliation when there is a discrepancy in the estimated reimbursement between the Working DRG and the Final DRG.
When a CDI performs reconciliation, a prompt appears allowing them to select which DRG to accept. A new "Reimb." column has been added to display the estimated reimbursement amounts, assisting in the decision-making process.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add new Columns for Denial Drill Down in Account Search

**CACTWO-7058** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Two new columns have been added to the Denial [drill down](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/account-search/#drill-down-level) in the [Account Search](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/account-search/) menu:
- Denial – Created Date
- Denial – Closed Date
  - will only populate if the “Denial Complete?” box is checked in the denial

![Denial Closed and Created Date Columns](DenialClosedCreatedDates.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Workgroups with a ‘0’ Count to Show in Account List

**CACTWO-7118** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new setting has been created for those users that want to see their assigned workgroups that have a ‘0’ count in their Assigned To dropdown list. 

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Remove CPT Codes on Inpatient Accounts With LOS >= 5 days

**CACTWO-7127** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

If an inpatient account has a length of stay equal to or greater than 5 days, suggested CPT codes will be automatically removed. The only CPT codes that will show in documents will be those manually added by a user. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Shift Reason column to Account Search Criteria

**CACTWO-7134** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new option has been added to the dropdown list when adding criteria for an [Account Search](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/account-search/): Query Shift Reasons.  This will show all shift reasons per query, including ‘other’ reasons that are based on a Mapping Configuration setting. 

![Query - Shift Reasons Column](QueryShiftReasons.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Field for Appeal Received Date to the Denial Worksheet

**CACTWO-7154** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

In [Denial Management](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/denial-management/) in the [Navigation tree](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/#navigation-tree) of an account, a new field has been added called “Decision Letter Received Date” to each denial appeal indicated. The name of this field will change depending on if it is the First, Second, or Third appeal.

![First Appeal Letter Date Field](FirstAppealLetterDate.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### General TruCode™ Edits are now Accessible in Custom Rules Scripts

**CACTWO-7158** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

General edits from [TruCode™](https://dolbeysystems.github.io/fusion-cac-web-docs/trucode-user-guide/) can now be provided to validation rule scripts. 

>[!Note] This is only relevant to the TruCode Encoder.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Detail to the Hover Over of a Grayed out Submit Button

**CACTWO-7160** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When the [submit](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/accessing-accounts/exiting-a-chart/#submit) button on an account is grayed out, hovering over gives data on that disabling; Errors exist on account. Added to that is that statement: Check Code Summary for Validation Results. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Columns to the Transfer Codes viewer

**CACTWO-7191** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Additional columns can been added to the [Transfer Codes viewer](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/transfer-account-codes/) when searching by MRN. If a user searches for an MRN and more than two accounts share that MRN, the MRN selection box will appear, now displaying the newly added columns.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

![MRN Columns Transfer Codes Viewer](TransferCodesMRN.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Audit and Denial Workflow Criteria Does not Work for Multiple Instances

**CACTWO-7193** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

 [Audits](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/audit-worksheet/) and [Denials](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/denial-management/) workflow criteria previously did not support multiple worksheet instances. While multiple Audit and Denial worksheets could exist, the workflow criteria only evaluated the first worksheet, ignoring subsequent ones. As a result, if the first worksheet was closed and a newer one was open, the workflow would incorrectly interpret the status as closed. This has been corrected—workflow criteria will now evaluate the most recent worksheet when multiple instances are present.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### TruCode™ Real-Time Edits Were not Using ASC Groupers When Applicable

**CACTWO-7238** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

Outpatient accounts using a primary grouper of ASC were not computing real-time edits. This has been corrected. 

>[!Note] This is only relevant to the TruCode Encoder.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Audit Management Dashboard is not Allowing Facility Filter

**CACTWO-7230** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The [Audit Management Dashboard](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#audit-management-dashboard) was showing as blank or as spinning circles when using the Facility Filter at the top of the page. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Audits Were Missing from the Audit Dashboards

**CACTWO-7231** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The [Audit Management](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#audit-management-dashboard) and [Aduit Personal](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#audit-personal-dashboard) dashboards were not taking multiple audits into consideration in some instances. Secondary audits were only considered if the secondary audit occurred within 30 days of the first audit. This has been changed to a default of 6 months. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Incorrect Values Showing in Timeline of Show History

**CACTWO-7234** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If certain fields were changed by the user, the timeline hover-overs in [Show History](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/code-summary/#show-history) was not showing the update value, instead showing the previous value. This has been corrected for the following fields: Admit Source, Admit Type, Discharge Disposition, Financial Class, Patient Type, and Payor.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Force Autoload is not Providing new Accounts After a Workgroup Change

**CACTWO-7244** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a workgroup assignment was changed for a [Forced Autoload](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/user-management/#force-autoload) user while they were working their list, when they clicked ‘Get Next Account’, there was a chance that autoload was not finding anything. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Coder ID to the Recurring Account Productivity Report

**CACTWO-7251** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A column to display the Coder ID has been added to the [Recurring Account Productivity Report](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#recurring-account-productivity-report) when it is exported as an XLSX.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Error Assigning Account to a Workgroup

**CACTWO-7257** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When in [Account Search](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/account-search/) and assigning an account to a workgroup, if the account did not have any prior workflow assignment, an error could occur. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Visual Difference Column is Showing Coding Data

**CACTWO-7261** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

In [Show History](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/code-summary/#show-history), if a workgroup name had a change after the 50th character, it would show in the Visual Difference column with coding data in it. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Display Issues with Mappings Configuration and Scheduled reports

**CACTWO-7268** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

In smaller monitor resolutions, the delete buttons of [mappings](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/mapping-configuration/) and [scheduled user reports](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/scheduled-reports/) could overlap text. This has been corrected. 


<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Edit All Codes not Displaying Admit Diagnosis Change

**CACTWO-7277** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When in the [Edit All](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/accessing-accounts/editing-codes/#mass-editing-codes) Codes window, if the user edited the Admit Diagnosis by clicking the pencil to open the encoder’s code book, the change was not displaying correctly within the window. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Prevent Coder From Closing Account With TruCode™ Codebook Open

**CACTWO-7281** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

To stop the possibility of a lockup, if a user tries to close out of an account when the [TruCode™](https://dolbeysystems.github.io/fusion-cac-web-docs/trucode-user-guide/) code book is open, they will see the same red bar alert over the Cancel, Save, Release buttons that they would see if the encoder was open. 

![Close Encoder Error](CloseEncoderToContinue.png)

>[!Note] This is only relevant to the TruCode Encoder.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Audit Worksheet Leaving Escalation box Open When Audit is Closed

**CACTWO-7282** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

Once an [audit](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/audit-worksheet/) is closed, all fields should be read-only. The escalation response box was not following that rule, remaining open to the addition of text. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Days not Showing for Schedules That are Hourly

**CACTWO-7287** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When creating a [scheduled report](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/scheduled-reports/), if it was set as hourly and days were chosen, the days were not showing in the report data on the left. This has been corrected. Because there are 2 days that start with T and S, Thursday shows as R and Sunday shows as U. 

![Scheduled Hourly Report](HourlyScheduledReport.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Scheduled Report Timing Changes Were not Displaying Properly

**CACTWO-7288, CACTWO-7299** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

After making a change to the timing of a [scheduled report](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/scheduled-reports/), the change was not showing on the report itself. This was happening whether the change was made via [Account Search](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/account-search/), or in the Scheduled Report page. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Validation Rules are Showing Multiple Times When They Shouldn’t

**CACTWO-7300** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

A [validation rule](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/code-summary/review-validation-rules/) can show multiple times if it has a ‘For Each’ criteria in the rule. But when that For Each criteria was removed and the Validation Rule saved, it was still showing up multiple times in the Account. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Correct Retrospective Followup Reviews Calculation

**CACTWO-7301** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

CDI reviews performed after a first submit when the DRGs match after reconciliation as retrospective follow up reviews on the [CDI Activity](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#cdi-activity-report) and [Detailed Activity](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#coder-detailed-activity-report) reports were not being counted. This has been corrected so that they are now included in those calculations. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Show a Tertiary DRG if Applicable

**CACTWO-7302** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

If there are 3 DRG’s on an account, all three will now show when printing the [Code Summary](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/code-summary/) page. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add encoder computations from Baseline Working DRG to Account Search

**CACTWO-7303** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

In [Account Search](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/account-search/), additional columns can be added to Account Search to provide information on Baseline Working DRG computations.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Improved Performance Processing Responses From Solventum™ CRS on Large Accounts

**CACTWO-7307** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

To improve application performance, the calculation of validation rules will no longer happen during the processing of a response from Solventum™. Validation rule computations will resume after the response is fully processed.

>[!note] 
> This fix only applies to sites using the Solventum encoder.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Medication evidence from CDI Alerts may not linking correctly.

**CACTWO-7308** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

Medication evidence, when clicked on from the [Clinical Alerts viewer](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/cdi-clinical-alerts/#viewing-cdiclinical-alerts), may not show the medication in the [Medications viewer](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/medications-viewer/). This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add new Column to the CDI Financial Benefit Report

**CACTWO-7312** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new column for ‘CDI Queries’ has been added just before the Baseline DRG Data block in the [CDI Financial Benefit](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#cdi-financial-benefit-report) report. 

![CDI Queries Column CDI Financial Benefit Report](CDIQueriesColumn.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Audit is Able to be Saved Without a Coder of Record

**CACTWO-7320** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

In the case of a CDI being the last user in and the owner of an account before it is audited, the Coder of Record was blank. The audit should not be saveable if a coder is not selected. This has been corrected so that if an Auditor attempts to save or route an audit without a coder of record, a red error message will occur stating the coder of record needs to be set. 

![Coder of Record Needed Error](CoderOfRecordError.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Description change for the  Coder DRG Summary report

**CACTWO-7322** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The description for the [Coder DRG Summary report](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#coder-drg-summary) has been changed to read:

![Coder DRG Summary](CoderDRGSummaryDes.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Display codes only present in physician queries in the Unassigned codes tree

**CACTWO-7327** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Codes that are added via the Pre and Post DRG computation within a [Physician Query](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/physicians-and-queries/) will now show in the [Unassigned Codes Tree](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/#unassigned-codes) if the codes are not present elsewhere on the account.  The codes will be identified with a question mark in front of them, and cannot be edited unless assigned to the account or added to a document.

>[!note] 
> This fix only applies to sites using the Solventum encoder.s

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### User is unable to unassign account without the Router role

**CACTWO-7330** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

A user could not unassign an account if the user was not granted the privilege to route accounts from [Roles Management](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/role-management/). This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Dashboard experiencing slowness due to retrieval query

**CACTWO-7332** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When the [Admin Dashboard](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#administrative-dashboard) loaded, its performance was being slowed down due to how the discharged pended accounts data was retrieved. This has been updated for faster performance. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Number of discharged accounts is incorrect on CDI Query Scorecard reports

**CACTWO-7334** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If multiple queries on an account fell in the same month, the number of the discharged accounts was being counted more than once.  This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Update the description of the Physician Coding Activity report

**CACTWO-7337** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The phrase “then the total number of Queries created” has been removed, since this report does not include the number of queries created by physician coders. 

![Physician Coding Activity Description](PhysCodingActReportDesc.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Default Search Field in Transfer Codes Viewer Updated to MRN#

**CACTWO-7342** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

 The default search field in the [Transfer Codes viewer](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/transfer-account-codes/) when accessed from the Navigation Pane within an account—has been updated to use the MRN# instead of the Account Number. If you prefer to revert the default back to Account Number, please contact Support to request a custom ticket.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Query Shift Reasons Now Display Mapping Friendly Descriptions 

**CACTWO-7343** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

[Account Search](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/account-search/), previously, when [Query Shift Reasons](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/physicians-and-queries/#documenting-query-shift-reasons) were based on a mapping, the system displayed the mapping key instead of the user-friendly description. This has been updated so that the description from the mapping is now shown, improving clarity for users.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Audit Executive Summary Report is not Calculating Correctly

**CACTWO-7348** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The number of Total Eligible Cases in the [Audit Executive Summary report](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#audit-executive-summary) was being under counted.  This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Physician Coder Manager Needs Access to the User Session Log report

**CACTWO-7358** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The User Session Log has been updated to allow access to the physician coder manager as long as the privilege is checked in [Role Management](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/role-management/). 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Denial Management is not Correctly Assigning the Coder Field

**CACTWO-7365** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

On a [Denial](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/denial-management/), the coder field was not defaulting to the first submitting coder, or leaving as blank if not submitted.  This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### CDI Today’s Productivity Time in Chart Calculation

**CACTWO-7371** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The time in the chart should be showing all the time spent, even if a working DRG is not calculated. It was not calculating time in chart that was worked and saved without a DRG. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Change of Admit Source Should Clear DRGs

**CACTWO-7386** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a DRG is calculated and afterwards the Admit Source is changed, the DRGs should clear. This was not happening and has been fixed. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Physician Query Recipient is Being Overwritten by Responding Physician

**CACTWO-7390** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When a different physician is set as the responder on a [query](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/physicians-and-queries/), it was temporarily overwriting the recipient physician on the query. When saved, it was showing correctly in the physician query viewer, so the correct Physicians were being recorded. The appearance of the overwrite within the query has been corrected.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Changing Audit Type was not Clearing the Audit Subtype

**CACTWO-7396** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

With subtypes being attached to [Audit](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/audit-worksheet/) Types through [mappings](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/mapping-configuration/), the subtype should be clearing in the audit if the type is changed. This was not happening and has now been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Pending Reason Historical Report is not Showing Correct Submitter

**CACTWO-7392** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The [Pending Reason Historical Report](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/) was showing the user that created the pending reason as the last submitter. This has been corrected.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Grid Column not Forcing a Save if a Title was Changed

**CACTWO-7402** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a user clicked in the Title field and made a change to the names, trying to move to another menu like [Account List](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/accessing-accounts/#account-list) was not causing the 'Do You Want to Save' message to pop. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### The 'Query For' Checkbox is not Being Saved on the Template

**CACTWO-7404** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When the '[Query For](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/query-designer/#blank-query-template)' box is checked on a query template worksheet, saving gave a green message, but if you went back into the template the checkbox was unchecked. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Copy Row function for Flowsheet have ability to Copy to CDI/Clinical Alert

**CACTWO-6767** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Fusion CAC now supports copying an entire row of a discrete value from flowsheet viewer into CDI/Clinical Alerts, as outlined in the comment above. Any hidden columns will be excluded from the [CDI/Clinical Alert](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/cdi-clinical-alerts/) evidence, enabling more precise control over which data is transferred.  

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Strike through Evidence if Document Code is no Longer Present

**CACTWO-7132** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Fusion CAC now enhances the [CDI/Clinical Alerts](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/cdi-clinical-alerts/) experience by displaying evidence with a strike through in the viewer if the originally abstracted evidence is no longer present in the document. This typically occurs when a document has been amended and the evidence previously identified has been removed.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Use Friendly Document Name in Copy to CDI/Clinical Alerts Function

**CACTWO-7241** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When evidence is copied to a [CDI/Clinical Alert](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/cdi-clinical-alerts/) from a document, the document type's friendly name will be displayed instead of its interface name. Previously it was using interface name.

<hr style="height:1px;border-width:0;color:gray;background-color:black">








