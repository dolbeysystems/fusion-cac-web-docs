+++
title = 'V2.64 (Oct 2026)'
+++

{{< release-notes-header version="V2.63.9680" date="07/06/26" >}}

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Ability for the end User to add Custom Subheadings in the CDI Alerts Editor

**CACTWO-6448** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Previously, subheadings such as Clinical Evidence, Laboratory Studies, and Vital Signs only appeared in the [CDI Alerts](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/cdi-clinical-alerts/) Evidence Editor when evidence already existed under them, so users had no way to add a subheading that was missing. A new Add button has been added to the Evidence Editor that lets users select and add a subheading from a configured mapping list. Once added, the subheading can be dragged and dropped to resequence it, and evidence can be moved into it or added to it from an abstraction, discrete value, or medication. A new mapping with the ID "CdiAlertTopicSubHeaders" must be created in Mappings Configuration to populate the list of available subheadings.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow an end User to Manually add a CDI/Clinical Alert

**CACTWO-7161** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Users can now add a CDI/Clinical Alert from a predefined list of topics, even when the system has not automatically identified that topic on the account. This lets CDI specialists gather evidence in an Alert and use the Query button to carry those details into a query, reducing the need to copy and paste information manually.

A manually added Alert displays **“Manually added”** beside its name, along with a person-and-plus icon. Alert topic names can no longer be edited in the Evidence Editor.

If the system later identifies the same topic, it will create a separate automated Alert. The automated Alert may include additional evidence and subcategory information.

When closing a manually added Alert, users can select **“Created by accident”** to remove one opened in error. The **“Insufficient clinical evidence,”** **“Documentation already present,”** and **“Other”** outcomes are unavailable for manually added Alerts.

Previously, a CDI/Clinical Alert topic could only appear on an account if the system automatically triggered it, so users had no way to open an alert for a topic that hadn't yet been flagged. Users can now manually add a new CDI/Clinical Alert from a preselected list of topics, using a mapping called "CdiAlertTopicHeaders." 

Manually added alerts will show ‘Manually added’ next to the name, along with a person and plus sign icon. All Alert Topics can non longer have their name edited in the Evidence Editor, the edit icon has been removed. If the system later automatically detects the same topic, it will still create its own active alert, since the automated version pulls in additional data and subcategory information. 


> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add a Days from Discharge column to Account Search

**CACTWO-7533** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new "Days from Discharge" column has been added for use in Account Search. When added to a grid through Grid Column Maintenance, it displays the number of days between today and the account's discharge date. If an account has a blank discharge date, the value is treated as zero. This field is intended for display only.  This column is also supported in scheduled Account Search reports run through JSReport. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Charge and Abstraction Audit Columns to the Outpatient Coder Scorecard

**CACTWO-7898** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The Audit Outpatient Coder Scorecard report has been updated to add up to six new columns. When the site configuration setting "ShowAuditCharges" is enabled, Charge Audit, Charge Errors, and Charge Accuracy Rate columns appear after the CPT related columns. Abstraction Audit, Abstraction Errors, and Abstraction Accuracy Rate columns always appear before the Training Topics column. These fields match the values shown in Audit Management for an outpatient account, and no Accuracy Rate value displays when the Audit count is zero.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add a Close All Active Alerts Button to the CDI Alerts Viewer

**CACTWO-7939** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Users can now close all active CDI Alerts on a chart at once when the chart is fully optimized and no further CDI action is needed. The new Close All button appears at the top of the CDI Alerts Viewer, eliminating the need to close each Alert individually. Selecting Close All opens a confirmation dialog. If the user confirms, all active Alerts on the chart are closed with the reason Chart Optimized. If an Alert requires a different close reason, the user can cancel and close that Alert individually. Closing Alerts that no longer need action helps keep worklists and opportunity counts accurate.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Drilldown and Additional Metrics to the Coder Scorecard

**CACTWO-7975** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The Coder Scorecard on the **Coder Personal** and **Forced Autoload** dashboards now gives coders more visibility into how their accuracy scores are calculated. **Principal PCS Code** has been added as a tracked metric, and each accuracy percentage now shows **Total Opportunities** and **Total Errors** beneath it.

The **Closed Audit** metric opens a detailed view showing each account number, its errors and accuracy results, and its overall accuracy. Account numbers display as text in this view.

A new **Routed to Coder** section shows which charts have been routed to the coder, helping users identify work waiting for them, particularly at sites that do not use workflow. **View All Audits** opens the Accuracy Rate table and the charts included in its results in a new tab.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add a Sequence Property for Validation Messages Using For Each

**CACTWO-8234** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Validation messages can now identify the specific item that needs attention when a rule uses **For Each** to evaluate an array. This helps users find and correct an issue without searching through every audit, denial, or diagnosis on the chart.

In the Validation Editor, add {Sequence} to the message text to display the matching item’s number. For example, if the second denial is missing a Billed DRG, the message Denial #{Sequence} is missing a Billed DRG appears in the Code Summary as **“Denial #2 is missing a Billed DRG.”**

{Sequence} can be used with any **For Each** array.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Physician Query Drafts to be Viewed as Read Only

**CACTWO-8238** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Previously, when an account was opened as read-only, a physician query draft created by another user could not be viewed, even though the Physicians & Queries section of the Navigation Tree indicated a draft existed. 
This has been changed so that a user with the privilege to create or edit queries can now view another user's draft as read-only when the account is locked. No changes can be made to the draft while viewing it this way. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Improve Readability of Show History Timeline

**CACTWO-8239** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Checkboxes have been added to the Show History timeline, allowing each group, such as Workflow, to be individually shown or hidden. All groups are checked, and therefore visible, by default. 
This makes it easier to focus on the entries that matter by temporarily hiding categories that generate a large number of system-generated events, such as workflow activity. Hiding a group only affects the timeline display and has no effect on the Changes or Visual Difference columns.

![Show History Timeline](ShowHistory.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Replace Form Editor in Worksheet Designer and Query Designer

**CACTWO-8240** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The form editor used within the Worksheet Designer and Query Designer has been replaced in its entirety. 
All existing features have been retained, though some, such as adding sections and editing tables, may be implemented differently. Existing worksheets and queries will continue to work as before, and all editing and toolbar options, such as sizes, styles, and colors, remain available in the new editor.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add a New Field to the CDI Query SOI Impact per Month Report

**CACTWO-8243** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new field called ‘Charts Not Yet Submitted’ has been added to the [CDI Query SOI Impact per Month](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#cdi-query-soi-impact-per-month) report.  The new field shows the number of inpatient accounts that have a stage of ‘P’, indicating they are not yet submitted. 

![CDI Query SOI Impact per Month](QuerySOIImpact.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Visually Identify Pinned Columns in Grids

**CACTWO-8244** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Pinned column headers now display with a darker blue background throughout the application, making it easier to visually identify which columns are pinned. 

This applies to any column pinned by the user, as well as columns that are pinned by default, such as in Physicians & Queries and Flowsheet grids, so that pinned columns are displayed consistently across all grids.  In this example, the left two columns are pinned. 

![Pinned Columns](PinnedColumns.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Question Level Weighting for Query Compliance and Other Sections in CDI Audit

**CACTWO-8250** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Administrators can now apply a custom weight to individual questions within the Query Compliance and Other sections of the CDI Audit Worksheet. 

A new Weight column has been added to mappings with the ids "QueryCompliance" or "CdiAuditOtherQuestions" in Mappings Configuration, allowing a positive whole number or decimal value, up to two decimal points, to be set for each question. Existing mappings default to a weight of 1, and any question without a specified weight also defaults to 1. 

When a weighted question is answered "Criteria Met" or "Education Opportunity" on a CDI Audit, the error rate and accuracy rate adjust according to that question's weight. This change may not apply retroactively to existing CDI audits.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow CPT Code to be Removed in Additional Charges Section of ER E/M Configuration

**CACTWO-8259** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Since CPT Codes were made optional in the Additional Charges section, an easy way to remove one once entered was still needed, previously requiring a user to delete and re-add the entire row. 

A clear "x" button has been added next to the CPT Code dropdown in the Additional Charges configuration section of ER E/M Configuration, allowing the code to be removed without deleting the row. This option is only available in the Additional Charges section, since CPT Codes are optional there only.

![ER E/M Additional Charges Configuration](AdditionalCharges.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Hide Delete Symbol for Pending Reasons Added by Validation Rules

**CACTWO-8276** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

In the Code Summary, a Pending Reason that was added automatically by a Validation Rule still displayed a Delete symbol, making it appear that it could be manually deleted. 

The Delete symbol has been disabled for Pending Reasons added by a Validation Rule, since these should only be removed once the Validation Rule is no longer in effect.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Associate a "Query Sent" Outcome to a Query When Closing a CDI Alert

**CACTWO-8279** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Previously, when a user closed a CDI/Clinical Alert with the "Query Sent" outcome without creating the query directly from the alert, no association was made between the alert and the query. 

This created a data gap that made it difficult to determine which query resulted from an alert or what financial impact should be attributed to it, affecting ROI reporting. Now, when a user selects "Query Sent" while closing an alert, a dropdown appears listing the existing queries on the account so the user can select the appropriate one before the alert can be closed. 

If no matching query exists, the user can create a new one from this dialog, which is then associated with the alert. The dropdown displays each query's date and time, query template, physician name, and, when applicable, the Query For value.

![Query Sent Outcome](QuerySentOutcome.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Remove Association Between CDI Alert and Query if Query is Cancelled

**CACTWO-8280** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When a CDI query created from a CDI/Clinical alert was cancelled, the alert remained linked to that cancelled query. This prevented users from creating a new query from the same alert and properly associating it, so the appropriate dollar impact could not be assigned. This has been resolved so that cancelling a query removes the association between the alert and that query. Users can now click the envelope icon on a completed alert and open a new, blank query ready to send, allowing the CDI impact to be assigned correctly.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Organize Columns Dialog to Account Search

**CACTWO-8302** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new "Organize Columns" button has been added to the upper right corner of the Account Search page. 

This button opens a dialog that makes it easier to organize columns, including dragging and dropping fields to reorder them, entering a specific position for a field, using arrows to move fields up, down, or to the top or bottom, and searching to quickly locate fields. Users can also add or remove individual fields or all fields at once, and the dialog can be expanded or minimized to fit the screen.

![Organize Columns](OrganizeColumns.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Pre and Post Query DRG Fields to Account Search Drilldown

**CACTWO-8304** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The **Queries** drilldown in Account Search now includes eight fields for comparing DRG information before and after a query: **Pre-DRG, Pre-DRG Description, Pre-DRG Weight, Pre-DRG Reimbursement, Post-DRG, Post-DRG Description, Post-DRG Weight, and Post-DRG Reimbursement.**

These fields are also available in scheduled Account Searches.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Filters Lost and Busy Indicator Missing on Account List After Routing from Context Menu

**CACTWO-8314** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

On the Account List page, assigning or unassigning an account using the context menu would clear any column filters that had been applied after the grid refreshed, and the busy indicator would not display during the refresh. 

This has been resolved so that column filters are now retained, and the busy indicator appears as expected when assigning or unassigning accounts from the Account List.



















