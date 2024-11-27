+++
title = 'Baseline DRG'
weight = 70
+++

The baseline DRG is used for reporting program impact. The baseline is defined as the DRG that would have been coded and billed if no CDI specialist reviewed the chart.

There are two styles of impact that can be reported:

1. Chart Impact
2. Query Impact

Both styles of reporting are separate, as query impact can be positive regardless of if the chart has
a positive, negative, or neutral impact.

Organizations can report the impact of a CDI specialist by measuring the difference between the baseline DRG and
the billed DRG. because of your organizations policy that the last know working and final DRG always
match, I we measure impact on last known working and final your impact would always be neutral if we
measure baseline which by default is the first DRG you calculate unless the baseline is readjusted you
may claim to much impact therefore the baseline throughout the patients stay is commonly readjusted.
While the baseline DRG may seem like a simple concept, it can at times be difficult to determine. Here is
an example:

1.  A patient is admitted through the ER after presenting with *undiagnosed abdominal pain*, which
would result in {{% drg 392 %}} with an estimated reimbursed of {{% money "$5,008" %}}</span>.
2. After further testing, it is revealed the abdominal pain is the result of *acute cholecystitis*; this
changes the {{% drg 446 %}} (disorders of the biliary tract **without complication**) with an estimated
reimbursement of {{% money "$5,175" %}}.
3. CDI documents an increased creatinine and a decreased glomerular filtration rate and queries
the physician regarding the patient’s renal status. If the doctor provides proper documentation,
it could be possible to assign a code indicating a *complication for Stage IV chronic kidney disease*, which would
result in {{% drg 445 %}} (disorders of the biliary tract **with CC**) with an estimated reimbursement of {{% money "$7,464" %}}.
4. The patient undergoes a *laparoscopic cholecystectomy*, changing the DRG to {{% drg 418 %}} (laparoscopic
cholecystectomy with CC) with an estimated reimbursed of {{% money "$11,868" %}}.
5. Next, the patient develops shortness of breath, and the consulting cardiologist documents
*acute-on-chronic congestive heart failure*, changing the DRG to {{% drg 417 %}} (laparoscopic
cholecystectomy **with MCC**) with an estimated reimbursed of {{% money "$17,478" %}}.

Normally, instead of the Baseline being {{% drg 392 %}} which is the first listed, would adjust to
would be readjusted to {{% drg 417 %}} once the patient goes to surgery. If the patient had not gone in for surgery the baseline
would have remained {{% drg 392 %}}. 

However, none of the CDI impact is lost though because queries are counted separately if you run the query report that CDI would:

- **Query Impact** (Difference between {{% drg 446 %}} and {{% drg 445 %}}= $2289)
- **Chart Impact** (Difference between Baseline {{% drg 417 %}} and Final {{% drg 4117 %}} = $0

The above is how *some* organizations choose to do reporting.

To remind the user that the baseline may need to be updated, a feature can be enabled to displays a message upon a save asking the CDI user if they would like to update the baseline DRG if the last computed working DRG is different than the baseline. It is recommened to only move the
baseline when the baseline needs reset, such as a patient going in for surger. Constantly updating
the baseline will little to no impact. The goal of baseline drg reporting is to show the impact of the CDI user's work.

![DRG](image-303.jpg)

>[!Note] Not Used By All Organizations 
>This reporting style may not be used by your organization. The Fusion CAC system accommodates for it, if an organization chooses to use it. Please speak with your {{%icon icon="user-tie"%}} manager if you have questions about how your facility tracks impact. 
