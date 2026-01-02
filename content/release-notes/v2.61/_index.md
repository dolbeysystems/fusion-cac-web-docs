+++
title = 'V2.61 (Jan 2026)'
+++

{{< release-notes-header version="V2.61.9477" date="01/09/26" >}}

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add ability to schedule a report per day of the week.

**CACTWO-5976 and CACTWO-7233** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

When creating a scheduled report, the user will now have the ability to schedule a report for a certain day of the week such as ‘first Tuesday of the month’ or ‘last Friday of the month’.  This has also been added to the scheduling window of the Account Search, along with the ability to report hourly. 

### Replace PSI 04 with a new failure to rescue measure.

**CACTWO-6787** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}** 

A new failure to rescue code of ISCMR will now show concurrently with PSI 04 when it applies, but it will be completely replacing PSI 04 in the future. 

### Allow scheduled reports to be restricted to particular domains

**CACTWO-7138** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new setting will now stop scheduled reports from going out to emails that are not in the configured domain.  As an example, if my setting is marked for ‘dolbey.com’, then if I put an aol.com address in the email for a scheduled report, I will be alerted that the address is not valid for the domain.

 [!info] Additional Configuration Required
Please contact Support to enable this feature.

