+++
title = 'V2.55'
+++

{{< release-notes-header version="V2.55.8945" date="06/28/2024" >}}

### CACTWO-4974 (Enhancement)

**Security – create two factor authentication**

Fusion CAC now allows organizations to use two factor authentication. When
enabled, the first time a user logs in after activation, a new panel will appear
on the login screen with a QR code or setup key to scan/enter into an
authenticator app. In the user’s authentication app, they will see 

```Fusion CAC [the environmentName appSetting] : [User's Login ID]```

When logging in, the user will add the code after their password.

> [!note] Additional Configuration Required
Please contact Support to enable this feature.

### CACTWO-5677 (Enhancement)

**Add metrics to CDI Query Scorecard reports**

A new section called CDI Team Metrics has been added to the CDI Query
Scorecard/Scorecard by Admission date reports. This lists the accounts and
reviews per month. The review counts are determined by the discharge date
for CDI Query Scorecard.

### CACTWO-5682 (Enhancement)

**Add additional abstracting questions to the Audit Worksheet**

Several new bullet point style questions can be added to the top of the
Abstracting section of an Audit worksheet. By default, there is no change to
the Audit Management viewer. However, a site can request additional
prompts to be added to the Abstraction section of the Audit Management
viewer.

![](image-827.jpg)

> [!note] Additional Configuration Required
Please contact Support to enable this feature.

### CACTWO-6051 (Enhancement)

**Allow Workflow to retain collapse state in memory**

The Workflow Magement page will now save how each users collapse/expand
criteria settings. After collapsing or expanding criteria throughout the page,
the user will see that remain when there is movement between pages, or a
signoff/signon action. This is automatically retained; the user does not have
to click the Save Workflow button.

### CACTWO-6190 (Enhancement)

**Allow to copy a row as a single line**

A new right click menu option has been added to the Flowsheet Viewer. This
will allow the user to highlight a row and choose ‘Copy Row as a Single Line’
to paste it into a text style editor.

### CACTWO-6214 (Enhancement)

**Allow user to Copy sections of an HTML document to clipboard so they don’t**

lose format
When copying an HTML document into an a text field, forms or Physician
Query, the format was being lost. This has been corrected so that the HTML
will hold its format, while removing code suggestions and extra blank lines.

### CACTWO-6271 (Enhancement)

**Create Coder Detailed Activity Report**

The new report Coder Detailed Activity Report is similar to the Coder Activity
Report, but has 2 new columns. Chart Touches will count the number of
unique times an account was touched, and the times for submitting and for
saving have been split.

### CACTWO-6321 (Enhancement)

**Add new column to the Query Impact reports**

Both the Query Impact and the Query Impact by Discharge Date report will
now have a new column; Query Reason.

### CACTWO-6345 (Enhancement)

**Add more columns to the Pending Reason report**

The Pending Reason report will now have two additional columns; Attending
Provider (first if there are multiple), and Discharge date.

### CACTWO-6377 (Enhancement)

**Add last/prior login date to User Profile**

There are now two dates that can be seen in User Profile. It wil show the Last
Login (which is the last, or in some cases current time the user was logged in)
and Prior Login, which is the date previous to the current or last login.

![](image-828.jpg)

Note that the first time a user logs in after the upgrade that enables this
tracking, there will be no Prior Date. Administrators can open the profiles of
other users from User Management and see their last and prior login
date/times.

### CACTWO-6393 (Enhancement)

**Add Auditor options to the Validation Manager**

Validation Manager now has two new user options; Is Auditor, and Is Not
Auditor. Please note that for profiles that have multiple roles, using these will
only trigger on an account if the current role is Auditor.

![](image-829.jpg)

### CACTWO-6398 (Enhancement)

**Create a way to collapse all Categories in Workflow Management**

A button has been added to the top of the left side Workflow list in Workflow
Management. Clicking this button will perform either a Collapse all or Expand
all Categories as needed.

![](image-830.jpg)

### CACTWO-6451 (Enhancement)

**Changes have been made to Denial Management**

The “Comments” box in the Denial Management viewer will now wrap text
and auto-expand as needed. Alsoif you highligh overtop of the text it will now
bring up the text edit styling box.

### CACTWO-6460 (Enhancement)

**Allow TruCode to compute a DRG without sequencing codes**

A new option has been added for TruCode encoder users to the Compute
button’s right side dropdown called ‘Compute w/o Resequence’. This will
compute the DRG without ordering DX codes according to quality indicators.

![](image-831.jpg)

> [!note] TruCode&#8482; Users Only
This fix only applies to TruCode&#8482; users.

### CACTWO-6479 (Enhancement)

**Add ability to reconcile all DRGs, not just the primary**

With a new setting that support can enable you can now add the ability for
sites to trigger DRG Reconciliation if any DRGs or DRG Weights.

> [!note] Additional Configuration Required
Please contact Support to enable this feature.

### CACTWO-6480 (Enhancement)

**Create a DRG Reconciliation viewer**

A new DRG Reconciliation viewer has been created. This will be available for
Inpatient accounts that have been reconciled and submitted by a coder. It is
for view only, and will display the Working DRG on the left, Final DRG on the
right. Symbols will be next to all codes indicating if they have been added,
removed, or moved to a different position.

![](image-832.jpg)

> [!note] Additional Configuration Required
Please contact Support to enable this feature.

### CACTWO-6482 (Enhancement)

**Add ‘exclude’ to report filters on most CDI reports**

These five filters that can be found on CDI user reports will now give the user
the option to filter as ‘ include’ or ‘exclude’. The filters are: Category, Facility,
Financial Class, Hospital Service and Pending Reason.

![](image-833.jpg)

If the filters are left blank, then Include stands for ‘All’ and Exclude stands for
‘None’. These are the reports it was added to:

- CDI Activity Report
- CDI Executive Summary
- CDI Financial Benefit
- CDI Metric Score Card
- CDI Productivity - Admission Month
- CDI Productivity by Review Type
- CDI Query Detail Report
- CDI Query Score Card
- CDI Query Score Card - Admission Month
- Inpatient Audit Score Card (Audit Management only)
- Inpatient Auditor Productivity (Audit Management only)
- Inpatient Coder Score Card (Audit Management only)
- Outpatient Audit Score Card (Audit Management only)
- Outpatient Auditor Productivity (Audit Management only)
- Outpatient Coder Score Card (Audit Management only)

### CACTWO-6494 (Important)

**CPT error rate is not refreshing properly in Audit Management**

In Audit Management, when there is a change to ‘Total Modifiers Added’ or
‘Total Modifiers Removed’, the CPT error rate is not refreshing. This has been
corrected to update the CPT error rate immediately.

### CACTWO-6499 (Important)

**Some patient birth dates are showing as 1 day earlier in account grids**

Due to how certain dates are evaluated in Daylight Savings Time, some birth
dates of patients were appearing off by one day between various grids. This
has been corrected.

### CACTWO-6522 (Enhancement)

**Allow Admin users to have access to create/edit documentation review without the need for privilages to be added**

Administrators will now be able to create or edit documentation reviews
without having the explicit privilege ‘Create/Edit Documentation Reviews”. It
is uncommon to use documenation reviews for CDI users.

### CACTWO-6525 (Important)

**Incorrect document is staying in focus**

If a code from the Show All Codes tree is assigned to more than one
document, and the user clicks on one of those documents, it opens in the
document viewer. But if the user then clicks on a different document and
adds a code to it, the former document shows in the viewer instead of the
currrently opened one. This has been corrected.

### CACTWO-6528 (Enhancement)

**Allow collapses and expands to auto save in new Workflow Management**

Upon opening up the Workflow Mangement page after updating, all
workgroups will be in a collapsed state. From that point on, Workflow will
save any collapse or expand that the user does without having to click the
save button.

### CACTWO-6535 (Enhancement)

**Add Duplicate code icon for 3M™ users**

When a code is added via 3M™, but is already in the unassigned code tree,
the unassigned code will no longer be visible, but clicking on the Show All
Codes tree will show the code with a duplicate icon.

![](image-834.jpg)

> [!note] 3M™ Users Only
This fix only applies to 3M Users.

### CACTWO-6547 (Important)

**Valid Value error occurring in some Account Search filters**

An error message asking for a valid value was occuring during some Account
Search filters that used the ‘=’ sign. This was occuring when fields had a
mapping that did not include a blank key. This has been corrected. An
example was if you had Stage = Unbilled then switched the equal to not equal
it would give you the error. Previously you would have to click on unbilled
switch off of it then back on it in the drop down for it to take effect. This has
been corrected.

### CACTWO-6548 (Enhancement)

**Allow Audit reports to filter by Audit Type**

Audit Type is now an Include/Exclude filter on all Audit reports

![](image-835.jpg)

### CACTWO-6560 (Enhancement)

**Add ability to remove quick complete button from physician query**

A new setting has been created that will allow you to remove the quick
complete button on the Physician queries dialog box. If the setting is set as
false, the user will see a Quick Complete button and the Send button will say
Send to Physician. If the setting is set as true, the Send button will only say
Send.

![](image-836.jpg)

> [!note] Additional Configuration Required
Please contact Support to enable this feature.

### CACTWO-6562 (Enhancement)

**Create Physician Coder Activity Report**

A new report called Physician Coding Activity has been created to report on
data for Physician Coder and Single Path coder activity.

> [!note] Additional Configuration Required
Please contact Support to add this report with a Physician Coding interface.

### CACTWO-6566 (Important)

**Forced Autoload limits are being ignored**

When a forced autoload user has limits on their workgroups, and they are on
the last account of a limit, if an account is manually assigned to them, the limit
restarts. This has been corrected so that the limit amount is never changed
during a manual assignment.

### CACTWO-6568 (Enhancement)

**Add HCC designation in Charges viewer**

When a code with an HCC icon is added to the charges viewer by an Physician
Coder, it will now show the designation just like the Assigned Codes tree

![](image-837.jpg)

### CACTWO-6573 (Enhancement)

**Comment field added for Denials in Account Search**

The Denials drilldown in Account Search will now show a Comments field.

### CACTWO-6576 (Enhancement)

**Requested changes to Code Suggestion Use by Coder report**

Multiple changes have been made to this report:
- Name changed to Engine Outcome Summary by Coder
- New column Total Codes Assigned added
- The column Added has been split into Added Text and Added Non- Text (which includes worksheet)
- The column Direct will contain codes added via 3M™, but also suggested by FAE
- The column Image has been split into Image (duplicate) and Image (non-duplicate)
- The column Worksheet has been removed
- The calulation of the column Score(now called Usage Score)
  - Score is (Accepted +Edited + Added Text + Image non-duplicate) / Total Codes Assigned.

### CACTWO-6577 (Enhancement)

**Requested changes to Engine Outcome reports**

The Engine Outcome per Coder (or per CDI) have been changed to Engine
Outcome Detail per Coder (or per CDI). The other changes made are:

- Duplicate codes added to the top of text documents are now counted in the Added Non-Text rather than Added Text
- Added Non-Text will now include codes added via 3M™ but also suggested by FAE
- The column Duplicate is now Added Duplicate
  - It additionally counts codes duplicated on images and worksheets
- The column Duplicate Codes now includes codes duplicated on images and worksheets
- The calculation of User Score is now 1.0 – ((Added Duplicate + Added Nontext) / Total assigned).
- The calculation of Engine Accuracy is now 1.0 – (Added Text / Total Assigned).

These changes are retroactive except the ‘Added Non-text” column
calculatoin. This column will retroactively include codes assigned directly
within 3M™ that were not suggested by FAE

### CACTWO-6584 (Important)

**Elixhauser mapping has been updated for prefix of ELIX_**

The Elixhauser mapping comes with a bunch of default prefixes. The prefix of
ELIX_ has been added.

### CACTWO-6585 (Enhancement)

**Add GMLOS columns to Query Impact reports**

The Query Impact and Query Impact by Discharge Date reports now have
GMLOS columns under the Before Query, After Query and Difference portions
of the report.

![](image-838.jpg)

### CACTWO-6586 (Enhancement)

**Allow CDI to change baseline DRG after submission**

Previously, once an account has been submitted, CDI Specialists could no
longer change the baseline DRG. This has been changed so that the baseline
can also be changed after submission of the account.

### CACTWO-6605 (Enhancement)

**Allow Forced Autoload coder to receive same account in the same day**

Previously, once a Forced Autoload coder submitted an account that had
directly assigned, if it was manually assigned back it would not appear in that
coder’s list until the next day. This has been changed so that if a manually
assigned account was submitted and then assigned back to the same coder,
they will receive it as their next forced autoload account instead of waiting
one day.

### CACTWO-6627 (Important)

**Date range information missing from CDI Metric Score Card**

When running the CDI Metric Score Card report, the report description does
not identify what date range is acceptable. This has been added to the
description.

### CACTWO-6638 (Important)

**Abstraction pre-audit calculation is incorrect**

In the Audit Management viewer, the "Abstraction Pre-Audit" calculation is
incorrect, although user reports correctly displayed the accurate calculation
in releases v2.53 and v2.54. In these releases, the calculation omitted the
procedure codes for which users had recorded a procedure date or physician.
This issue affected only the display in the audit viewer, not the Audit user
reports.

### CACTWO-6463 (Enhancement)

**New way of viewing linked discrete values from CDI Alerts**

If a discrete value's name appears in more than one category within the
discrete data viewer within a major category when it is linked from the CDI
Alerts viewer, the entire major category will be highlighted in the Flowsheet
viewer. Otherwise, the original functionality of just highlighting its single
category applies.

### CACTWO-6532 (Enhancement)

**Collapse all CDI Alerts when opening CDI Alerts Viewer**

Previously, all CDI Alerts were expanded making it hard to view all alerts. This
requests was to initially be collapsed when the account is loaded.

### CACTWO-6578 (Enhancement)

**Add Other choice with drop down on the Close CDI Alert Dialog Box**

Add new option of Other with the ability to add drop down box on the Close
CDI Alert Dialog Box. This allows the user to Close an Alert because it did not
require a query to be sent and not because the Alert was wrong. They state
occasionally even though an Alert triggered appropriately; after reviewing a
query is not needed, they do not want to count it negatively as the alert did
what it was supposed to.

It will only appear if a mapping with the ID
"DrillDownMatchedCriteriaGroups_OtherOutcome" is created in Mappings
Configuration with additional alternate outcomes. The alternate outcomes
will be displayed in the Closed CDI Alert.

![](image-839.jpg)

### CACTWO-6580 (Enhancement)

**Add line spacing to evidence**

Previously, the spacing was condensed; this adjustment provides more
vertical spacing, making the alert evidence easier to read.

![](image-840.jpg)
