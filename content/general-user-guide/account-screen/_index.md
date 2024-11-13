+++
title = 'Account Screen'
weight = 50
+++

## Account Action Bar

![Account Action Bar](AccountActionBar.png)

The blue bar accross the top of the screen is the Account Action Bar. This bar displays specific account information such as the account status,the account number/HAR, and the dates of service. Additonally, the Account Action Bar houses buttons allowing the user to compute, cancel, save, or submit the account as needed.

## Banner Bar

![Banner Bar](AccountBannerBar.png)

Below the Accounts Action Bar is the Banner Bar, which contains 

### Patient Information 

Information in the banner bar may include:

- Admit details
- Discharge details
- Patient Name – Last Name, First Name & Middle Initial
- Gender
- Patinet Age and date of birth
- Medical Record Number (MRN)

> [!info] Banner Bar Collapse/Expand
> Clicking the patient's name will collapse the banner bar to provide more vertical screen space.
> Clicking the patient's name again will expand the banner bar and the information displayed. 


### DRG/APC

From the Banner Bar, you can toggle between demographic information and Primary DRG
information by clicking on the Primary DRG hyperlink. 

![Primary Grouper](PrimaryGrouperLink.png)

The DRG view displays information available from the encoder for the computed DRG. The DRG or APC information will appear on the Banner Bar after codes have been assigned and DRG or APC computed and returned from the encoder.

![Banner Bar - DRG/APC](DRGs.png)


## Navigation Pane

The Navigation Pane sits above the Documents Pane on the left-hand side of the Account Screen. 
The Navigation Pane includes hyperlinks to pages within the chart providing summary views of
coding information, demographic information, as well as clinical documentation, workflow, and 
worksheets.

Any Navigation link highlighted in **{{< rawhtml >}}<span style="color:#a00">RED</span>{{< /rawhtml >}}**
indicates action items  required to finalize the chart or  additional information available for review and reference. 

### +Add

Click on the Add Document button to add a document configured based on your user role.

### Code Summary

**When the Code Summary link displays RED, there are validation errors on the chart that must be 
resolved prior to submission.**

### Account Information

### Notes & Bookmars

### Physicians & Queries

### Addtional Viewers

> [!note] Optional Viewers
> The following viewers are part of optional
> [add-on modules](https://dolbeysystems.github.io/fusion-cac-web-docs/general-user-guide/add-on-modules/)
> and may not be used at all organizations. If you are unsure if a module is relevant to your
> organization, please contact your  supervisor. Organizations looking for more information on
> these modules should reach out to the Dolbey SME team via email (smeteam@dolbey.com).

##### Audit Viewer

![Audit Viewer](AuditViewer.png)

The audit viewer displays when the account is opened by a user in the rold of Auditor. The audit viewer can be popped out onto a separate screen, allowing the auditor to have a screen for reviewing the chart. By selecting “Show All” codes in the unassigned code tree, the auditor is taken to the documents/documentation supporting that code.  This will help streamline the audit process. 

An account can have one or more audits added to it. By clicking "+ Add Audit," a new, blank audit worksheet will be created. These worksheets are numbered and displayed at the top of the audit viewer, along with a date stamp indicating when each worksheet was opened. The worksheet currently being viewed will be highlighted with a green background.

Data in the audit viewer is only intended for coder education and administrative staff to score how the coder is doing in a report card. The auditor will need to add the coder of record so that the coder of record, any auditor, or other user role that has been given access can view the audit worksheets. 

##### Denials Management

![Denials Viewer](DenialManagementViewer.png)

The denial management viewer displays on submitted accounts. Clicking on this viewer presents a form with several fields to be filled in when an account has been denied payment. 

Denial management tracking involves monitoring cases where a patient's submitted billing chart is rejected by the payer. Various reasons, such as medical necessity, code, or DRG assignment, could lead to these denials. This tool is designed to comprehensively record the specifics related to denial management and tracking. It is capable of documenting multiple denials for each chart, with the ability to log and categorize them for the purpose of tracking, managing workflows, and generating reports.

![Denial Worksheet](DenialWorksheet.png)

Mutiple denial sheets can be created within the viewer, if applicable. 

![Multiple Denails](MultipleDenials.png)

Sheets can be removed from the account by clicking on the red X to the right of each denial heading. For reporting within Account Search, a Denials drilldown is available. **This drilldown only reports on the first denial on the account**. 

The viewer has a multiselect entry for each denial.  The field is located above the Code(s) in Question entry. Clicking into the Root Causes field will cause a list to dropdown. Default options include: 

- Incorrect DX
- Incorrect PCS
- Incorrect PDX
- Incorrect POA
- Added DX
- Added PCS
- Removed DX
- Removed PCS

Options in the dropdown lists can be customized per organization by editing the appropriate mapping table in [mapping configuration](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/mapping-configuration/).

- DenialType
- DenialStatus
- DenialOutcome
- DenialAppealRoute
- DenialReason
- DenialCodeChangeNeeded
- DenialDRGChangeNeeded

Each field (except Comments) can be added to [Grid Column Configuration](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/grid-column-configuration/) for display in Account Search, these fields can also be used in workflow if necessary. 


##### ER E/M Viewer
