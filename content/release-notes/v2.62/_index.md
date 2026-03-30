+++
title = 'V2.62 (Apr 2026)'
+++

{{< release-notes-header version="V2.62.9575" date="04/06/26" >}}

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### New "User Login" Report has Been Created

**CACTWO-5478** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new report titled "[User Login](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#user-login-report)" has been created. This will show the login/logout activity of the user. If an inactivity reason was recorded by the user, then the prior logout will be listed as ‘inactivity’ instead of logout and the inactivity reason will be recorded in its own column.  Date range available is 31 days, the report will never show the current day’s activity.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow a Secondary Sort in Workflow Management

**CACTWO-5569** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

A new enhancement has been added to [Workflow Management](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/workflow-management/) that allows for a secondary sort order within workflows. When configuring a workflow’s list on the user’s [Account List](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/accessing-accounts/#account-list) page, items will first be organized by the primary sort, and then further refined using the secondary sort within those results.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Deleted Pending Reasons and Notes to be Viewable

**CACTWO-6727** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new checkbox has been added to the [Code Summary viewer](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/code-summary/) to allow the user to view [pending reasons](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/code-summary/#pending-reasons) (and any applicable notes) to be seen.  A marker  number next to the checkbox will show the number of currently deleted pending reasons.   When checked, the deleted pending reasons will show beneath the list of active pending reasons, and the red delete button will be grayed out to indicate this is an already deleted pending reason.

> [!note] The number and checkbox will only display if there were previously deleted pending reasons.

![Deleted Pending Reasons](DeletedPendingReasons.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add the Ability to Collapse Criteria in Workflow Management

**CACTWO-6896** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

In a [workflow management](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/workflow-management/), a new checkbox has been added under the Criteria Groups heading; Collapse all criteria groups.

![Collapse All Criteria Groups](CollapseAllCriteriaGroups.png)

When the box is checked, all criteria under that workflow will close, only showing the name of the criteria:

![Uncheck Expand all Criteria](UncheckExpandAllCriteria.png)

Unchecking the box will reopen all the criteria. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Managers to set Grid Columns to Only be Seen by Manager/Admin

**CACTWO-7164** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Managers can now restrict certain grid columns so they are visible only to users with Manager or Administrator roles.

A new “Managers Only” option has been added in [Grid Column Maintenance](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/grid-column-configuration/). When this option is selected for a column, it will be hidden from all users except those assigned a Manager or Administrator role in their User Profile.

For example, if enabled, only users with one of these roles will be able to view the Workgroup column in their grids.

![Managers Only Grid Columns](ManagersOnlyGridCols.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Identify Transferred Codes in the Show History

**CACTWO-7240** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Codes that have been added to an account via the [Transfer Account Codes](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/transfer-account-codes/) viewer will now have a ‘download’ icon next to them in the [Show History](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/code-summary/#show-history) viewer.   When hovering over the icon, the use will see a statement that indicates which account the codes were transferred from.

![Transferred Codes in Show History](TransferedCodes.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Display HAC Designation in Banner Bar 

**CACTWO-7344** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

To make an assigned diagnosis code with an HAC designation more noticeable, an HAC text will now appear in the [banner bar](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/#banner-bar), similar to a PSI or QI designation.  The HAC designation will still appear next to the assigned code in the [Assigned tree](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/#assigned-codes). 

![HAC in Banner Bar](HACinBannerBar.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Queries Sent Column to CDI Personal Dashboard

**CACTWO-7345** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new column has been added to the [CDI Personal Dashboard](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#cdi-personal-dashboard)’s Personal Stats pane.  The column is Queries Sent and will count any physician query created by a CDI Specialist or a CDI Auditor that is not cancelled.  All numbers except zero will show drill-down when the number is clicked.  This change is retroactive. 

![Queries Sent CDI Personal Dashboard](QueriesSentDash.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Force Autoload is Receiving Incorrect "No Accounts" Message

**CACTWO-7579** **{{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

An issue was identified where using browser navigation controls (such as the Back or Refresh buttons) during F[orced Autoload](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/user-management/#force-autoload) could cause the session to fall out of sync. This sometimes resulted in an incorrect “There are no accounts…” message, even when accounts were still available.

This has been resolved. The system now detects when the Forced Autoload session becomes out of sync due to unexpected actions or network interruptions and will automatically reset and reload accounts in the background. If accounts still cannot be retrieved after retrying, the message will display as expected. This enhancement helps ensure a more consistent workflow and reduces interruptions during Forced Autoload processing.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Sorting to "Work Available Queue" Admin Dashboard Panels

**CACTWO-7582** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The three administrative dashboards ([Administrative](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#administrative-dashboard), [CDI Management](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#cdi-management-dashboard), [Audit Management](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#audit-management-dashboard)) will now have a sort button at the top of each column under the [Work Available Queue](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#work-available-queue) heading. 

![Sorting Work Available on Dashboard](WorkAvailableSorting.png)

The unsorted buttons will show in blue, and when a sort is put on one of the columns, it will turn green and show which sort it is, ascending or descending.  In this case, the Workgroup Name column is sorted in Ascending order. The sort will flow through to all three administrative dashboards, and will remain in place during the session. Once logout occurs, the sort will clear. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Default Create Time (descending) Sorting Within Notes and Bookmarks

**CACTWO-7585** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

If a user changes the sort to a different column or order withing [Notes and Bookmarks](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/notes-and-bookmarks/), that preference will persist while navigating between accounts. Upon logging out or restarting Fusion CAC, the sort will reset to the default Create Time (descending) setting.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### A new "Change Auditor" Option has Been Added to Editable Audits

**CACTWO-7625** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When accessed, a selection dialog will display available auditors based on the audit type. This change was made for both [Coding Audits](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/audit-worksheet/) and [CDI Audits](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/cdi-audit/). The ability of an auditor (or cdi auditor) to change the auditor of record has been added to the Audit (and CDI Audit) worksheet.  When the button is clicked the dropdown list of users that have the audit role will be displayed. In either audit type a new button will appear, similar to the one for changing the coder (or CDI) of record:

![Change Auditor Button](ChangeAuditor.png)
![Change CDI Auditor Button](ChangeCDIAuditor.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### AG-Grid had Been Updated to the Latest Version

**CACTWO-7636** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Enable Time Zone Entry for Specific Reports

**CACTWO-7637** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new mapping called ‘Timezone’, will allow for timezone entry on 4 [reports](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/): [User Audit Trail](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#user-audit-trail-report), [User Detail](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#user-detail-report), [User Login Report](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#user-login-report) and [User Session Log](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#user-session-log-report).  This will be helpful for clients who have coders that work across time zones.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Modifier Column to Outpatient Coder Scorecard Report

**CACTWO-7641** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new column has been added to the [Outpatient Coder Scorecard report](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#outpatient-coder-scorecard); CPT Modifier Count.  This is the total number of modifiers involved in the audit of an outpatient account. This is a retroactive change. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add HCC to Outpatient Shift Reasons

**CACTWO-7647** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

‘HCC’ has been added to the [shift reason](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/account-screen/navigation-tree/physicians-and-queries/#documenting-query-shift-reasons) dialog for outpatient physician queries.  

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Retain Minimized Encoder when Editing an Assigned Code

**CACTWO-7651** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

If the [Code Editor](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/accessing-accounts/editing-codes/) is minimized when editing an assigned code, it will not close if the user moves to other areas of an account’s detail.  But if the code is edited from the document or document code list, the editor will be closed if the user moves to another document. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Custom Roles to Populate the Change Dropdown in Audits

**CACTWO-7708** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Custom Roles can be [created](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/role-management/#create-a-new-role) that will be seen in the ‘Change Coder of Record’ dropdown in an [Audit](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/audit-worksheet/), and the ‘Change CDI of Record’ dropdown in a [CDI Audit](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/cdi-audit/).  

For "Coder of Record" in [Audit Management](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/audit-worksheet/), in addition to users with the role of "Coder" or "Auditors", users with roles enabled with the following privileges are now included:

- Audit accounts as an Auditor
- Edit accounts as a Coder
- Edit accounts as a Single Path Coder

For "CDI Specialist of Record" in [CDI Audit Management](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/cdi-audit/), in addition to users with the role of "CDI Specialist" or "CDI Auditor," users with roles enabled with the following privileges are now included:

- Audit accounts as a CDI Auditor
- Edit accounts as a CDI Specialist

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Pending Reasons to the User Audit Trail Report

**CACTWO-7710** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The [User Audit Trail](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/user-reports/#user-audit-trail-report) will now show two additional message lines; a line for if a pending reason was added, and a line for is a pending reason has been deleted.  

![Pending Reason Added/Deleted User Audit Trail](PendingAddedDeleted.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add CDI Query Count to CDI Management Dashboard

**CACTWO-7716** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Two new lines of data have been added to the [CDI Management dashboard](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#cdi-management-dashboard) under the CDI Summary pane; CDI Queries Sent Today, and CDI Queries Sent in Last 7 Days.  These will also have a drill-down leading to detailed pages for those statistics. 

![Lines of data Added to CDI Summary on CDI Management Dashboard](AddedToCDISummary.png)

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Plus Buttons in DRG Reconciliation Viewer to add Codes

**CACTWO-7756** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A plus sign has been added to the left of the codes in the [DRG Reconciliation Viewer](https://dolbeysystems.github.io/fusion-cac-web-docs/account-navigation/navigation-tree/drg-reconciliation/) to allow for easy additions to the Working DRG and Final DRG.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add new Field of "Pending Reason Date Added (First)"

**CACTWO-7758** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new field has been added to [Grid Maintenance](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/grid-column-configuration/), ‘Pending Reason Date Added (First)'.  This will also show as a choice in the [Account Search](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/account-search/) and [Workflow](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/workflow-management/) Criteria dropdowns. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Change Dashboard to not Show '5,000+' as Total

**CACTWO-7771** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The [Work Available Queue](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/dashboard/#work-available-queue) on the Dashboard shows any total over 5000 as 5000+.  This has been changed to show the exact number of accounts.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### The Validation Management Display and CSV Export have been Updated

**CACTWO-7800 and 7801** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

For consistency within Fusion, the [Validation Management](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/validation-management/) page has been updated to look and act like the [Workflow Management](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/workflow-management/) and [Scheduled Reports](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/reporting/scheduled-reports/) pages.  The functionality of adding, deleting, editing and copying all remain the same.  The csv report has also been updated for better usability.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Submitted Accounts to Remain in Submitted Status to Audit

**CACTWO-7813** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When using Save and Route to send a submitted account directly to an Auditor or an [Audit workgroup](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/workflow-management/#audit), the account will now remain in Submitted (Stage A).

Previously, routing a submitted account to a user or workgroup would automatically change its stage to QA Review (Stage Q), as the system assumed the account was being sent for updates and resubmission. With this update, routing through Save and Route to an audit destination is recognized as an audit-only action, so the account status will no longer change unnecessarily.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Fields to Validation Management for Denials

**CACTWO-7819** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

In [Validation Management](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/validation-management/), when using the ‘[for each](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/validation-management/#for-each-check-box)’ option and selecting Denials from the list, a list of Denial options will be opened to complete the validation rule. 


