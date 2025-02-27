+++
title = 'V2.56 (Sep 2024)'
+++

{{< release-notes-header version="V2.56.9036.0" date="09/27/2024" >}}

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Multiple Audits on a Single Account

**CACTWO-5379 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Allow Multiple Audits on a single account
Users of Audit Management can now be updated to allow for multiple audits 
on a single account. At the top of the Audit viewer, a new button has been 
added called ‘Add Audit’. Clicking that will open an empty audit form. The 
accounts can have many audits added to it with this change. 

**For Audit Module users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Display Physician Coder Diagnosis Changes to Charges in Show History

**CACTWO-5527 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Display Physician Coder diagnosis changes to Charges in Show History
If a Physician Coder or Single Path coder makes a change to diagnosis codes 
in a charge, that will now show in the Visual Difference Column of the Show 
History tab.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Display Changes to Physicians in Show History

**CACTWO-5591 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Any changes made to account level physicians will now show in the Visual 
Difference column of the Show History tab.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Show More Audit Data in the Show History and User Audit Trail Report

**CACTWO-5680 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Show more audit data in the Show History and User Audit Trail report
The Show History tab of an account will now show Auditor work in the Visual 
Differences column. 
 
The Audit Trail user report will also show several Audit actions in the report: 
Audit open, Audit Closed, Audit Reopened, Audit Rebutted, Audit Closed and 
Audit Printed.

**For Audit Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Ability to Copy Validation Management Rules

**CACTWO-6065 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Ability to copy Validation Management rules
Validation Management Rules now have a copy button to the right of the 
directional buttons.
When clicked, a duplicate of the rule and its criteria will appear at the bottom 
of the rule list, ready for editing.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Root Cause Field for Denial Management

**CACTWO-6182 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Add root cause field for Denial Management
Denial Management viewer wll now have the ability to select multiple entries
for each denial, as needed. The field is located above the Code(s) in Question 
entry. 
Clicking into the Root Cause field will display a dropdown with default 
choices.To note if you would like to change these values you can add a 
mapping the ID is DenialRootCauses.

**For Denials Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Validation Rule to Report on Audit Status

**CACTWO-6323 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Allow Validation Rule to report on Audit status
In Validation Rules a new ‘for each’ option of Audits has been added so that a 
validation rules can be created for audit options.

**For Audit Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Display in Show History Phsycian and Modifier Changes to Charges for Physician Coder

**CACTWO-6403 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Display in Show History physician and modifier changes to charges for 
Physician Coder
If a Physician Coder makes any changes to a physician or code modifier, those 
will now show in the Visual Difference column of the Show History tab.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Physician Coders to Select Multiple Codes

**CACTWO-6427 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Allow Physician Coders to select multiple codes
Within the charge viewer allow physician coders to select multiple diganosis 
codes to associate to a charge by clicking control and selecting codes. This 
way multiple codes can be added as needed. 

**For Physician Coding or Outpatient CDI users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add and Move Some Identifiers in Show History Chart

**CACTWO-6444 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

In the Show History tab, the Location and Patient Type sections have been 
removed and those identifiers have been added to the Event section. New 
identifiers have been added to the Events section: Payor, Financial Class, 
Admit Source, Admit Type and Discharge Disposition. By clicking on the 
ledgend to the top right it color cods the events for easy viewing.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add a Rebill Checkbox to Denial Management Viewer

**CACTWO-6452 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new checkbox to indicate a rebill is needed has been added to the Denial 
Management viewer. It appears after the Denial Complete checkbox. 

**For Denials Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Auto Populate Coder With First Submitted, but Allow Users to Edit

**CACTWO-6453 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Auto populate Coder with First Submitted but, allow users to change it if its 
incorrect.The ‘Coder’ field in the Denial Management worksheet will now be 
defaulted to the first Submitter.

**For Denials Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Linking of Related Queries to a Denial 

**CACTWO-6454 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

t Allow linking of related queries to a Denial
A new field has been added to the Denial Management viewer for related 
queries. It is located after ‘Code(s) in Question, and if there are any closed, 
non-canceled physician queries, they will appear in a dropdown when the 
field is clicked. 
**For Denial Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Show Roles in the Summary of User Actions

**CACTWO-6455 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

On the Code Summary viewer, each user listed in the Summary of User Actions 
will now also display that users current role. 

To Note: **This feature is not retroactive.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow the Created by User on a Physician Query to be Editable

**CACTWO-6481 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Once a physician query is saved, the Created By field will show. This is now 
changeable, whether or not the query is closed or still open. A Save button at 
the bottom of the query will save the change.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Quantity to be Modified Under Charges Viewer by Physcian Coder

**CACTWO-6524 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A physician Coder will now see the edit symbol on the Quantity line in the 
Charges Viewer. The Quantity can be changed and saved. 
**For Physician Coding or Outpatient CDI users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### 3M™ not Closing Properly When User Changes Roles

**CACTWO-6558 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When using 3M™, if a user changed his role to a role that had a disabled 
encoder, 3M™ would not close or reopen properly when the user changed 
back to his role that had the encoder enabled. This has been fixed. 

> [!note] 3M™ Users Only
This change only applies to 3M Users.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add 'Primary' to Add Diagnosis Codes Window in Charges Viewer

**CACTWO-6565 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

If a user goes into the codes in a Charges Viewer and moves the codes around, 
the top code will always become the primary code. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Display Multiple DRGs in the Shift Reason Dialog Window

**CACTWO-6570 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

If there are multiple DRGs on an account, when a query is closed and presents 
the Shift Reason window, all DRGs will show, with the first one expanded and 
the other collapsed. Both DRGs are expandable/collapsible.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Field Onto Denials Viewer for Letter Received by Facility 

**CACTWO-6574 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new field has been added to the Denial Management Viewer in addition this
field has been added into the drilldown in Account Search.
**For Denial Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Columns to the CDI Activity Report

**CACTWO-6608 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

In the CDI Activity user report, reviews and queries are now counted under 
new columns of either Concurrent or Retrospective. Queries created during 
DRG reconciliation are counted under Retrospective. With the additional 
columns, the report will now show in landscape when PDF is chosen.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Columns to the CDI Financial Benefit Report

**CACTWO-6611 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Add columns to the CDI Financial Benefit report
Columns for First CDI Saver and First Submitter columns have been added to 
the CDI Financial Benefit user report. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add new Section to the DRG Comparison Report

**CACTWO-6612 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

This user report has two DRG sections: one for Baseline and one for Final. A 
new section for Working DRG has been added. This DRG is the last Working 
DRG figured before the account was submitted.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add More Fields to Workflow Management 

**CACTWO-6623 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Several new fields have been added to Workflow Management to allow 
criteria to detect a user’s assigned roles:

- First CDI Owner Roles Last CDI Owner Roles
- First CDI Saver Roles Last CDI Saver Roles
- First Coder Roles Last Saver Roles
- First Submitter Roles Last Submitter Roles
- Owner Roles Last Viewer Roles

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Audit Rebuttal to Always Show on the Audit Viewer

**CACTWO-6634 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Currently, a rebuttal on an audit viewer will be hidden once the coder clicks 
the Agree button. Going forward, the rebuttal will continue to show, even 
after the coder agrees. 

**For Audit Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Coder to Save a Review of a Finished Audit

**CACTWO-6672 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When an auditor marks an audit as finished and the account is manually 
routed to a coder, the coder will now see a "Save Account as Reviewed" 
button at the bottom of the audit if it’s their first time reviewing it. This button 
marks the audit as "Saved Review" and records this action in both the 
account's Show History and the User Audit Trail report. The "Save Account as 
Reviewed" button will appear under these conditions:
- The audit has been closed.
- The account is routed to the coder’s personal queue.
- The coder is viewing the closed audit.
- The coder has not previously reviewed the audit.
When the coder clicks "Save Account as Reviewed," an "Are you sure?" dialog 
will appear. A new audit event will be logged to show that the coder reviewed 
the completed audit, and this will be visible in both the Show History and the 
User Audit Trail. 
 
**For Audit Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add MRN Lookup to Transfer Account Code Viewer

**CACTWO-6676 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The account number and MRN now appear with radio buttons on the Transfer 
Account Codes viewer. When the user selects the MRN radio button, the MRN 
of the currently opened account will automatically be populated.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add the Ability to Add a Summary Field to Saved Account Searches

**CACTWO-6681 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When saving a search in Account Search, a new field labeled "Filter Summary" 
will appear in the save box. If this field is completed, the summary will be 
displayed in the search banner.
 
It will show next to the Drill-Down Level.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Conditional Triggers for PSI/PDI Based on Exclusion Code Position 

**CACTWO-6682 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

PSI and PDI indicators originally did not trigger if a code that caused an exclusion for 
that indicator was within the the top 25 codes (or limit that customer has set). 
This has been changed so that if that happens, the PSI/PDI will still show in 
the banner bar, with an asterisk next to it, to indicate the PSI was conditionally 
applied. The algorithm at the bottom of the Code Summary viewer will show 
the reason why.

**For Quality Module users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Filters to Grid Colum Configuration

**CACTWO-6684 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Filters now appear at the top of the location columns in the Grid Column 
Configuration. Clicking on a filter will reorder the column, displaying all 
assigned columns either at the top or bottom.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Weight Breakdown for Elixhauser

**CACTWO-6695 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When Elixhauser coding is applicable, a new table under the Elixhauser 
section of the Code Summary sheet will appear, showing weight totals for 
each item that triggers.

**For Elixhauser users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add ROM/SOI Information Field on Diagnosis Section 

**CACTWO-6699 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The SOI/ROM will now show in the Audit Worksheet, next to each code and 
then in the Codes section of the sheet, it will show numbers matching whether 
there was a change in those numbers, 1 increase or decrease for each change. 

**For Audit Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Print Button is Missing in User Report

**CACTWO-6703 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

Print button is missing in User Reports
The updated PDF viewer in a previous release within user reports removed 
the Print button, but it has now been modified to restore any missing buttons. 
Users can print or download PDF reports from the User Reports page. 

> [!info] Additional Configuration Required
If you wish to restrict this setting, please contact CAC Support.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Account Search Drilldown Erroring When Searching Large List

**CACTWO-6705 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The Account Search drilldown was creating an error when a right click ‘View 
Account Detail’ was done on an account from a large list of accounts.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Change all Verification Window Buttons to Yes or No

**CACTWO-6707 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

For any pop-up window that begins with the question “Are you sure...” has 
been updated. The buttons that previously displayed as "Cancel" and "OK" will 
now appear as "Yes" and "No."

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Vertical Scroll bar to Account Search Criteria if Criteria is Very Long

**CACTWO-6711 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

In Account Search, criteria that has a lot of data causing a lot of vertical space 
to be used extending beyond the viewing screen, making the grid unreadable. 
A new vertical scroll bar has been added to ensure users can access and view 
all data without losing information beyond the filter's edges.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add red tag Next to Applied PSI/PDI for Improved Visibility

**CACTWO-6712 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When a PSI/PDI is applied to an account, it was previously difficult to identify 
in the algorithm section of the Code Summary viewer. A new red tag has been 
added to enhance visibility, making it easier for users to quickly locate the 
PSI/PDI algorithm that was applied.

**For Quality Module users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Unable to Remove a Matched Criteria Template in Workflow

**CACTWO-6726 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

A ‘Matched Criteria Query Template’ dropdown only appears in Workflow if a 
criterion with the field ‘Evaluation Script’ which is used by CDI/Clinical Alerts is 
present. When copying and pasting that criterion, the user has no way to 
remove that template to choose another. A small gray ‘x’ has been added to 
the box to allow removal of the template after pasting. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow 'Frequency Edits' for TruCode ™

**CACTWO-6730 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

TruCode™ has an option to include frequency edits among the medical 
necessity edits returned by TruCode. This has now been enabled.

> [!note] TruCode&#8482; Users Only
This fix only applies to TruCode&#8482; users.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Increase Filter Length and Labels for Improved Usability

**CACTWO-6732 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The filter dropdown 
length has been extended in account search to display more of the filter name, 
reducing the need to click the down arrow, especially for filters with similar 
names. The field for the account search name is now longer, and the "Delete 
Filter" option has been replaced with a garbage can icon to save space
allowing for room for the increased length. Additionally, the "Tools" button 
has been renamed "Columns" for better clarity.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### 'Unexpected Error' Messaging Occuring in Account Search

**CACTWO-6734 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When using the Queries drilldown in a filter in Account Search that resulted 
in a large amount of accounts returned, a red toast error message to contact 
Dolbey Support was happening. This has been corrected.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Update PSI/PDI Algorithms

**CACTWO-6737 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

PSI/PDI algorithms have been updated to AHRQ v 2024.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Code Dropdown Does not Reflect Date of Service in Denial Management Viewer

**CACTWO-6740 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The codes that were reflected in the codes dropdown of the Denial 
Management viewer was displaying current day codes vs date of service 
relavant codes. This was corrected to use the accounts Admit date for 
outpatient or Discharge Date for inpatient to determine which codes to 
display. 

**For Denials Management users only.**

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Error Occuring When Closing Physician Query/Shift Reason Window

**CACTWO-6742 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When closing a Physician Query or Shift Reason dialog box when the 
Physicians & Queries viewer was not visible, a console error was occurring. 
This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Hide 'Route to' Buttons in Audit Worksheet

**CACTWO-6745 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The ‘Route to Auditor’ and ‘Route to Coder’ buttons in the Audit Worksheet
can now be hidden with a new site-configuration setting.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow Readmission Viewer to Show Multiple Accounts

**CACTWO-6746 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

If an account has multiple re-admissions, they will now all show if they are in 
the default time of 30 days. A new setting has been added to allow the 
number of days to be changed. If the setting is updated to an amount other 
than 30, that new amount will show in the Re-admission Viewer AND in the 
red tag in the banner.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Clicking on Code From Unassigned Code Tree Doesn't Scroll to the Position in the Document Viewer

**CACTWO-6749 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a user has a zoom on their document viewer, and they click on an 
unassigned code in the unassigned tree, the document in the viewer will scroll 
towards it, but leave the highlighted code offscreen. This has been corrected 
so that even with a zoom in place, the viewer will scroll to make the 
highlighted code viewable. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Improve Copy to Clipboard Functionality Adding Intential Line Breaks

**CACTWO-6746 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

There are some issues around intentional line breaks. The functionality has 
been improved to alleviate those issues.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Copy Single Line and Copy to Table was Added to the Flowsheet Viewer

**CACTWO-6746 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When using the Flowsheet viewer, two changes have been made to the right 
click menu:
- Copy Row as a Single Line has been renamed Copy Row as Text, and now 
copies each result value to its own line.
Copy Row to Clipboard has been renamed Copy Row as Table for clarity.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### DRG Reconciliation Tooltip is Displaying Incorrect Data

**CACTWO-6754 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The tooltip in the DRG Reconciliation viewer was not giving correct 
information. These changes have been instituted: The tooltip on the left 
side for deleted codes will now say ‘Deleted in Final DRG’. The tooltip on the 
right for a resequened code will say ‘Higher in sequence than in Working DRG’. 
The tooltip of the corresponding code on the left side will say ‘Lower in 
Sequence in Final DRG’.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Changes to Procedure Details Were Applying Even if Canceled

**CACTWO-6756 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If changes to procedure codes were made using Edit Procedure Details, the 
changes were saving even if the user clicked Cancel. This has been corrected.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Change Display of SOI and ROM in all Viewers

**CACTWO-6760 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Currently this is displayed as ROM then SOI. The order has been corrected to 
show as SOI, then ROM in all viewers.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Charts With Answered Queries had HTML Code in Their View Diff Viewers

**CACTWO-6763 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If an account had an answered query and the View Diff viewer was deployed, 
HTML code showed throughout the viewer. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Resizing Physican Query Causes the Footer to Overlap the Content 

**CACTWO-6769 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a user opens a Physician Query and then makes the box smaller by pulling 
up from the corner of the dialog box, the footer was overlapping the Buttons 
at the bottom of the query. A scroll bar has been added, and now the bottom 
buttons remain outside of the data inside the query.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Query Reports Erroring When Displaying Large Amount of Data

**CACTWO-6771 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The Query Impact and Query Impact by Discharge reports have been 
corrected for an error that was occurring if these reports were run over a long 
time period.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Summary to System Search Filter

**CACTWO-6773 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When saving a filter in System Search, the Save box will now have the added 
field ‘Filter Summary’ for addition of a note or comment. 
This will then show above the filter criteria:

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### SOI and ROM Calculations are not Matching in Physician Query Pre/Post DRG and Shift Reason 

**CACTWO-6776 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

The SOI and ROM values in a Physician Query were sometimes not matching 
the ROM and SOI values of the Shift Reason screen. If the site is using 3M and 
an account has both an APR for a primary grouper and an additional APR as a 
secondary or tertiary, the values will always match the SOI and ROM 
calculations of the primary APR instead of the latter APR.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Physician Coder Submitting an Account is Closing an Audit

**CACTWO-6784 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

A physician coders submit now prevents a closing an open audit. Only a 
facility coder can close an audit.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Update CAC Technical Support Page

**CACTWO-6790 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The CAC Technical Support page found under the above the banner bar 
has been updated.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Copy to CDI/Clinical Alerts Function is not Appearing for Caution Code Documents

**CACTWO-6798 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

When a user highlights text and right clicks from a caution code document, 
the funtion Copy to CDI/Clinical Alert does not appear. This has been corrected. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### View Differences Viewer Showing HTML Tags

**CACTWO-6805 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a user attempts to ‘View Diff’ on documents that contain ‘html’ and ‘body’ 
tags, HTML code was showing in the viewer. This has been corrected.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Personal Stats Dashboard is not Loading for Some Users

**CACTWO-6806 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If a large amount of accounts were assigned by a user in Account Search, if 
the user then tried to look at their personal Dashboard, it would not load. This 
has been corrected.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Patient's Current Age to the Banner Bar

**CACTWO-6812 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A patients current age or discharge age will now be shown in the banner bar
if it is different than their admit age. If the account is not discharged, the age 
will be the current day’s age. If it has been discharged, it will show the 
discharge age. If the Admit and current/discharge date age are the same, 
only the admit age will show, as usual.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### 3M™ is not Alerting User That the Encoder is Already Open 

**CACTWO-6815 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

In the case of a 3M™ encoder being open, with the user then opening a 
physician query and attempting to compute a DRG, the user was not being 
warned that the encoder was already open. The user closed the query and 
was then stuck in the acount. This has been corrected. A blue warning box 
will now occur if the Compute button in a physician query is clicked while the 
encoder is already open.

> [!note] 3M™ Users Only
This change only applies to 3M Users.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### CDI Activity Report is not Displaying 'Friendly Name' in Facility Column

**CACTWO-6816 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

All reports show the ‘friendly’ name, but this one was showing the key of the 
mapping instead. This has been corrected to now show the ‘friendly’ name if 
the mapping is set up for that Facility.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Rename the Encoder tab on the Main Menu List

**CACTWO-6820 {{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Since Encoder can be taken to mean that clicking on it will open the regular 
Encoder, a request came in to make that say Standalone Encoder. A new 
setting has been created to change that name.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Prevent POA From Changing When Editing Codes Using Code Lookup 

**CACTWO-6822 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If the user launches and returns the 3M or TruCode codebook from the Code 
Editor dialog when editing a diagnosis code, the POA will reset to its default 
value. This has been corrected.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Last Auditor to Save an Account is now Recorded as the Last Saver

**CACTWO-6827 {{< rawhtml >}}<span style="color:#2a7d1f">(Important)</span>{{< /rawhtml >}}**

If an auditor saves or submits an account, the Last Saver on the account was 
not updated. This has been corrected. Additionally, a new set of “Last 
Auditor” fields have been added to account grids, account search, and 
workflow to determine the last auditor to save an account.s