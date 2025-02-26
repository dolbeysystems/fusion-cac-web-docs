+++
title = 'Code Summary'
weight = 20
+++


{{% children depth=999 %}}


![Code Summary](CodeSummary.png)

The Code Summary is the last pane to be reviewed prior to chart submission. This screen shows a summary of activity on the account and provides activity buttons to **Claim Ownership**, **Show History**, and **Print Summary** *(if a printer is configured)*. This viewer also provides information on Current Owner, First Coder, Last Saver, and Last Submitter. Users can expand the width of the Code Summary pane by clicking on the arrow in the top right of the pane. 

![Code Summary Viewer](CodeSummaryPane.png)

### Show History

The {{%button%}}Show History{{%/button%}} button provides a timeline view of activity on the account along with an audit trail of account activity from point of admission to the current date. It includes a visual timeline and below the timeline there will be an audit trail of account activity. 

![Show History View](ShowHistory.png)

Upon opening Show History, users will see the entire history from a birds-eye view.  The user has the option of using the Zoom In and Zoom Out buttons to expand or collapse the timeline.  The Zoom Fit will bring the visual timeline back to its original collapsed grid.  Hover over any of the event boxes and the contents will be displayed. 

The legend can be found by clicking {{%button%}}Show Legend{{%/button%}} button to let the user know what the colors represent without having to hover over them.  When clicked, it will open the Legend and the button name will change to "Hide Legend".  Click again to close. 

Click on an entry by date to view the changes that were made to the account on the date and time indicated.

![Audit Trail](AuditTrail.png)

### Review Validation Results

When the Code Summary link displays **{{< rawhtml >}}<span style="color:#a00">RED</span>{{< /rawhtml >}}**, there are [validation errors](https://dolbeysystems.github.io/fusion-cac-web-docs/administrative-user-guide/validation-management/) on the chart that must be resolved prior to submission.

![Red Code Summary](RedCodeSummary.png)

Any errors preventing submission of the chart will be highlighted in the box under Validation Results on the Code Summary screen. Validation Results within the chart that should be reviewed and validated before the chart is finalized and submitted for billing.

**ERROR** results will display in **{{< rawhtml >}}<span style="color:#a00">RED</span>{{< /rawhtml >}}**. These are hard stops that will prevent the chart from being submitted. The {{%button%}}Submit{{%/button%}} button will be grayed out until errors have been resolved, including pending reasons that have been assigned.

**Warning** results will display in **{{< rawhtml >}}<span style="color:#FFBF00">YELLOW</span>{{< /rawhtml >}}**. These are reminders/suggestions for the user. Warnings do *not need to be resolved* before submitting the chart. 

![Code Summary Validation Results](ValidationResults.png)

Once all necessary validations results are resolved, the Code Summary link in the Navigation tree will return to black and users can hit the {{%button%}}Submit{{%/button%}} button to complete the chart.

### Pending Reasons

A list of Pending Reasons assigned to the account can be found within the Code Summary pane below Validation Results.

![Pending Reasons](PendingReasons.png)

Pending reasons are used when a chart cannot be completed or routed to another Workgroup. The number of pending reasons selected is unlimited.  Pending reasons will be different for each facility based on system configuration specifications.  Please contact your {{%icon icon="user-tie"%}} manager for definition and use of available pending reasons.

Pending Reasons can be added to the account by clicking on the drop-down menu and selecting the applicable Pending Reason. If the organization has selected to allow a physician to be tied to a pending reason, the user will be prompted to assign a physician to the pending reason, and will see an additional physician field in the list of pending reasons. 

>[!Note] If physicians have been turned on for pending reasons, not all pending reasons may be tied to a physician. This option is set within the mapping configuration.

If a pending reason is added to an account, the Submit button will be grayed out and unavailable.  Click on the Save button to save all changes and exit the chart. Charts with pending reasons will stay within the existing Workgroup until the Pending Reason is removed. Pending Reasons can also be deleted/removed from accounts by clicking on the "X" next to the Pending Reason to be removed. 

##### Pending Reason Notes
On any account, an edit button will appear to the left of the pending reason. Clicking that button will drop down a note entry where the user can record a note. Pressing ENTER will record the note. Keep in mind that a note can be deleted by clicking a trash can symbol to its left. In Account Search, the "Pending Reasons" drill down will now include the "Note" field.

![Pending Reason Note](PendingReasonNote.png)

### Admit Diagnosis 

The Admit Diagnosis code and description are displayed below any Validation Results and/or Pending Reasons.

![Admit Diagnosis](AdmitDx.png)

### Visit Reasons

Listed beneath Admit Diagnosis are the Visit Reason codes in code sequence order. The list includes the Visit Reason code and description.

![Visit Reasons](VisitReasons.png)

### Assigned Diagnosis Codes

The Assigned Diagnosis Codes are listed in code sequence order below Visit Reasons.  The listing includes the diagnosis code, description, and POA assignment (Y/N).

![Assigned Diagnoses Codes](AssignedDxCodes.png)

### Assigned Procedure Codes

Listed beneath Assigned Diagnosis Codes are the Assigned Procedure Codes in code sequence order. The list includes the procedure code, description, Service Date, and Physician.

![Assigned Procedure Code](AssignedProcedure.png)

### Assigned CPT Codes

Listed beneath Assigned Procedure Codes are the Assigned CPT Codes in code sequence order. The list includes the CPT code, description, Service Date, and Physician.

![Assigned CPT Code](AssignedCPT.png)

#### Print Summary
If a printer is configured for the computer, click on this button to print a copy of the abstract for this account. 

#### Claim Ownership
Use the Claim Ownership feature based on the organization’s requirements and procedures. Consult your {{%icon icon="user-tie"%}} manager for more information on claiming ownership of a chart. 


## Final Code Summary

![Final Code Summary Viewer](FinalCodeSumViewer.png)

The Final Code Summary will only be available once the facility Coder clicks the {{%button%}}Submit{{%/button%}} button. This provides transparency between CDI and physician coding teams (if also using Fusion CAC) as to what was coded. When a submitted chart is open again, users will see a new viewer under the navigation menu called the Final Code Summary. This will display what the coders coded along with code status details and sequencing. This data is viewable only for the role of [‘CDI’](https://dolbeysystems.github.io/fusion-cac-web-docs/cdi-user-guide/).  

![Final Code Summary](FinalCodeSummary.png)

Clicking on the header will expand the selection to display the codes that were coded and DRG/APC, if applicable. Any codes with a plus (+) sign indicates the code has not been added to the account. The plus (+) sign *does not indicate* that the code needs to be added. It is for the user to quickly add the code if they determine it is needed using coding judgment and supporting documentation. If applicable, the code’s HCC designation will show the HCC number and its version.


## Physician Coding Summary

The Physician Code Summary will display if the *Physician Coders* are also coding within Fusion CAC, and they submit the chart. This provides transparency between the facility and physician coding teams as to what was coded.

![Physician Coding Summary](PhysicianCodeSummary.png)

Clicking on the header will expand the selection to display the codes that were coded. Any codes with a plus (+) sign indicates the code has not been added to the account. The plus (+) sign *does not indicate* that the code needs to be added. It is for the user to quickly add the code if they determine it is needed using coding judgment and supporting documentation.

