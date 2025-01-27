+++
title = 'Baseline DRG'
weight = 70
+++

The baseline DRG is used for reporting CDI program impact. 

![Baseline DRG](BaselineDRG.png)

>[!Note] Not Used By All Organizations 
>This reporting style may not be used by your organization. The Fusion CAC system accommodates for it, if an organization chooses to use it. Please speak with your {{%icon icon="user-tie"%}} manager if you have questions about how your facility tracks impact. 

The baseline is defined as the DRG that would have been coded and billed if no CDI specialist reviewed the chart. Organizations can report the impact of a CDI specialist by measuring the difference between the baseline DRG and the billed DRG.

Two seperate styles of impact that can be reported:

1. Chart Impact - postivie, negative, or neutral
2. Query Impact - can be positive regardless of chart impact

Fusion CAC measures impact on the last known working *and* final DRGs, readjusting as needed, to accurately track impact throughout the patient stay.

While baseline DRG may seem like a simple concept, it can at times be difficult to determine. Here is
an example:

1.  A patient is admitted through the ER after presenting with *undiagnosed abdominal pain*, which
would result in {{% drg 392 %}} with an estimated reimbursed of {{% money "$5,008" %}}</span>.
1. After further testing, it is revealed the abdominal pain is the result of *acute cholecystitis*; this
changes the {{% drg 446 %}} (disorders of the biliary tract **without complication**) with an estimated
reimbursement of {{% money "$5,175" %}}.
1. CDI documents an increased creatinine and a decreased glomerular filtration rate and queries
the physician regarding the patient’s renal status. If the doctor provides proper documentation,
it could be possible to assign a code indicating a *complication for Stage IV chronic kidney disease*, which would
result in {{% drg 445 %}} (disorders of the biliary tract **with CC**) with an estimated reimbursement of {{% money "$7,464" %}}.
1. The patient undergoes a *laparoscopic cholecystectomy*, changing the DRG to {{% drg 418 %}} (laparoscopic
cholecystectomy with CC) with an estimated reimbursed of {{% money "$11,868" %}}.
1. Next, the patient develops shortness of breath, and the consulting cardiologist documents
*acute-on-chronic congestive heart failure*, changing the DRG to {{% drg 417 %}} (laparoscopic
cholecystectomy **with MCC**) with an estimated reimbursed of {{% money "$17,478" %}}.

Normally, instead of the baseline being {{% drg 392 %}} which is the first listed, would adjust to
would be readjusted to {{% drg 417 %}} once the patient goes to surgery. If the patient had not gone in for surgery the baseline
would have remained {{% drg 392 %}}. 

However, none of the CDI impact is lost though because queries are counted separately if you run the query report that CDI would:

- **Query Impact** (Difference between {{% drg 446 %}} and {{% drg 445 %}}= $2289)
- **Chart Impact** (Difference between Baseline {{% drg 417 %}} and Final {{% drg 4117 %}} = $0

The above is how *some* organizations choose to do reporting.

### Reminder

To remind the user that the baseline may need to be updated, a feature can be enabled to display a message when a CDI user saves a chart.

![Update Baseline DRG Prompt](UpdateBaseline.png)

Dolbey recommeneds to only move the baseline when the baseline needs reset, such as a patient going in for surgery. Constantly updating
the baseline will result in little to no impact.



