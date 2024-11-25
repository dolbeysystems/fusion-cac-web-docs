+++
title = 'Fields and Definitions'
weight = 80
+++

This section contains an alphabetical list of fields and definitions in the application.

Fields are configured to be available in account search,workflow, and account list grid. These fields and their friendly names are set in the [grid columns configuration](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/tools/grid-column-configuration/) by administrative users. This list may not have the full listing of fields as some fields are custom, however those listed are the most common.

## Admit Reason 

This is the reason that registration has typed in; this is not the admit reason set
by the coder. That information is displayed in the Admit Dx Code field.

## Category

A category is a ‘Dolbey’ created field that is used to further specify a patient
type, if applicable. At some sites, category might equal patient type while
others may have a category that is comprised of multiple fields to create that
category. For example, if you would like to report on how many charts a coder
completed for inpatient and then define them by LOS, you then have a category
to define the difference between LOS patient types or service lines.

- Inpatient 1-10 LOS
- Inpatient 11-20 LOS
- Inpatient 21 +
- Outpatient Radiology

## New Review Date 

Next review date is set either automatically by the system or manually by the
CDI user if they choose to override the system automatic default date. The default
date is whatever your management team has selected as a default interval for
follow up reviews to occur. This may mean that the default is set for the next
business day or two days later. This field is can be manually overridden by a
CDS in the Code Summary viewer.
Why would a CDS manually override this field? If you have reviewed the chart
and know the patient is going to have surgery in a few days and there is no
reason for a follow up review based on your sites policy’s. You may choose to
augment the next review date for after the scheduled surgery.

## 30 Day Readmit

This field is an optional feature add-on that a site can see if the patient has
been readmitted within 30 days of the admit date. This field will populate with
the previous account number, thus you can report on data to see if accounts
exist with this data.

## Baseline

Baseline is defined as the baseline data of the chart that would have been
coded and billed without the intervention of the CDI staff. This data is used to
measure the impact that CDI has on a patient’s chart is then measured as the
difference between the Baseline DRG and the Billed DRG (either the weights or
the reimbursement).

## Working

Working is defined as the working information due to the intervention of the
CDI staff. The CDI staff will update this information concurrently until the
patient is discharged with additional data surrounding presenting problems or
provisional diagnosis.

## Final

Final is defined as the coded data added to the chart be billed out.

## Reconciliation

Reconciliation typically refers to a process that occurs when the working and
final DRG’s do not match. Charts get flagged with a field called ‘Is DRG
reconciled’. If there is a check mark then the chart has been reviewed and the
chart has been reconciled either as an agree to disagree or agree and an
adjustment is made to the working or final DRG once CDI and/or Coding does
another review.

## DRG Reconciled?

Reconciliation typically refers to a process that occurs when the working and
final DRG’s do not match. Charts get flagged with a field called ‘Is DRG
reconciled’. If there is a check mark, then the chart has been reviewed and the
chart has been reconciled either as an agree to disagree or agree and an
adjustment is made to the working or final DRG once CDI and/or Coding does
another review.

## Document Type

The document(s) that are present on the patient account. The document types
for searching and/workflow are required to have the interface name, not the
friendly name. If you do not know the document names that are available to
use, Dolbey can provide a table which provides this information. Send an email
to results@dolbey.com requesting the document table names.

## Assigned

Assigned means that the code was used for billing purposes. If you are looking
for codes that are suggested or added by CDI for working/baseline purposes
you would use the document code. Note: If designing workflow it is recommended
this field is used for CDI, but for QA purposes its recommended that ‘Assigned’ is used
to ensure you are QA on what was billed vs what was suggested.

## Document Code

Document Code is defined as any code on a chart whether manually entered,
Suggested. The code can be unassigned which means it’s not used for billing or
assigned which is used for billing.
Note: If designing workflow it is recommended this field is used for CDI, but for
QA purposes it’s recommended that ‘Assigned’ is used to ensure you are QA on
what was billed vs what was suggested.

## Physician Queries Open

Physician Queries Open is the number of physician queries on the account that
have not been closed. A physician response could have been received, but if it
hasn't been viewed by a user within CAC, the physician query is still considered
"open".

## Physician Query Total

Physician Queries Total is defined as how many queries a chart has on it
regardless of whether the queries are opened or closed. If a user was in an
account that had an open physician query, and an external interface closed that
query, the query total on the account is updated upon closing the account.

## Workgroup

A list of charts to be completed for coding, CDI or QA. Most charts flow into a
Workgroup based upon automatic criteria, however admin user can route a
chart to Workgroup (uncommon)

