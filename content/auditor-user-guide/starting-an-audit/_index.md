+++
title = 'Starting an Audit'
weight = 20
+++

1. Ensure you have the role of an auditor and chart access of auditor.
   ![Audit Rolle and Chart Access](AuditAccess.png)
2. Open a chart that has been submitted by a coder, you may get this chart from a worklist
or, by manually typing in an account number.
3. On the navigation tree you will notice a viewer called “Audit Worksheet”, click {{%button%}}+Add Audit{{%/button%}} to begin ![Add Audit](AddAudit.png)

>[!info]DRG Required
> A DRG must be computed by a user before an audit can be started

4. Select the appropriate audit type from the dropdown. This will be used for reporting on the types of audit performed and can also be used for workflow purposes. ![Audit Types](AuditTypes.png)
   
5. The codes in the assigned code tree are the same codes initially submitted by the
coder, allowing the auditor to start the audit with the codes from the coder. The audit
viewer can be popped out onto a separate screen, allowing the auditor to have a screen
for reviewing the chart. Selecting “Show All” codes in the unassigned code tree and then clicking on the codes assigned, the
auditor will load the documentation supporting that code. This will help
streamline the audit process. ![Show All Button](ShowAll.png)

6. Once the auditor has made changes and is completed with the audit, they can click “Update Codes”
  which automatically calculates and populates the audit statistics section. There is a comment bubble
  next to each code as well as the DRG for the auditor to enter any comment(s). A symbol may display next to the codes.
    - A green ‘plus’ sign will show if the code was added. ![Green Plus](GreenPlus.png)
    - A red ‘minus’ sign will show if a code was deleted. ![Red Minus](RedMinus.png)
    - A orange up or down ‘arrow’ sign will appear if the code location has been changed, as
    in a primary and secondary are swapped. ![Orange Arrow](OrangeArrow.png)

7. Although audit statistics have been automatically calculated and populated, the auditor must 
manually enter in the “total errors” which then automatically calculates the “Error Rate”.

>[!note]
>Because of its importance, and to include principal diagnosis changes in the error rate, changing the principal diagnosis counts as **two errors intentionally**. 
>- One error for changing a diagnosis code
>- A second error if the principal diagnosis is wrong 
>
>For an account with only two diagnosis codes, the error rate when the principal code is changed is 2 out of 3.
>If on the same account the auditor says the principal is correct and only changes the secondary code, the error rate is 1 out of 3.

8. Complete the additional sections, (abstracting and training recommendations) if applicable.

![Abstracting](Abstracting.png)
![Training Recommendations](TrainingRecs.png)

9. The auditor can then re-submit the chart or route it back to the coder of record by using the
“Route to Coder” button in the top right corner of the audit worksheet. This will route the chart to
the coder’s **You** worklist for them to review and re-submit.

![Route to Coder](RouteToCoder.png)
