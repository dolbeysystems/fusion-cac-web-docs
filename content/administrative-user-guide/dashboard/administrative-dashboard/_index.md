+++
title = 'Administrative Dashboard'
weight = 30
+++

## Administrative Dashboard

The administrative dashboard is only available for those users with the administrator role. This dashboard
displays data at a glance. Clicking on any of the blue numbers will open a grid to display the data
that goes into that number.

![Administrative Dashboard](AdminDash.png)

The dashboard can be filtered by facility. Leaving the filter blank will combine all facilities and all patient types. 

![Facilites Filter](FacilitesFilter.png)

### Users Online

This displays the users online or offline broken out user type. The blue numbers are links to view the
user detail behind the number you selected.

![Users Online](UsersOnline.png)

![Users Online Detail](CodersOnline.png)

Users can right click on the grid to export to CSV.

### Open Queries

This section displays open, unanswered, and answered queries per role along with average turn around time (TAT) and provider
response rate.

![Open Queries](OpenQueries.png)

Click on any of the blue numbers to see the data behind that number. Right clicking on the
grid provides the option to export to CSV.

### Top 10 Queries in Last 30 Days

This displays the 10 most used query templates within the last 30 days.

![Top 10 Queries](Top10Queries.png)

Click on any of the blue numbers to see the data behind that number. Right clicking on the
grid provides the option to export to CSV.

### AutoClose Daily Stats

This section displays AutoClose stats, including charts autoclosed and rejected on the current day. It also includes data for
month to date. 

![AutoClose Daily Stats](ACDailyStats.png)

Click on any of the blue numbers to see the data behind that number. Right clicking on the
grid provides the option to export to CSV.

### Coder Productivity

This displays the coders productivity by charts submitted and those that are pending.

![Coder Productivity](CoderProductvity.png)

Click on any of the blue numbers to see the data behind that number. Right clicking on the
grid provides the option to export to CSV.

### Coding Trends per Day

Coding Trends per day combines "Average Daily Coded" and "Average TAT to Submit" to show
averages over the last 7, 30, and 90 days compared to the prior 7, 30, or 90 days, grouped by category.

![Coding Trends Per Day](TrendsPerDay.png)

### Discharge Not Final Coded (DNFC)

This section provides the admin staff the ability to see where the organization is in regards to the outstanding sum of total charges. The data broken down by total outstanding charges per charts outstanding for the current month also known as discharge not final
coded. The admin staff can also see if the team is meeting their goal for how many charts are
outstanding at the end of the month. A comparison is displayed to show total charges for the current
month compared to the previous month. Next to each value should be a number in blue that represents the number of charts that make up the
dollar value. Users can click these numbers to drill down and display the chart details

![Discharge Not Final Coded](DNFCSection.png)

|Term     |Definition|
|---------|----------|
|Available|All patients discharged and not submitted within a coding worklist per either the “current month” or “previous month” depending on the column reported. **Workgroup Type must equal coding**.|
|Unavailable|Defined as all patients discharged and not submitted and not within a coding worklist per either the “current month” or “previous month” depending on the column reported. **Workgroup Type *not* equal coding**.|
|Total|The total of both available and unavailable for coding.|
|Goal|The target goal set per organization for the discharge not final coded. Users can set the goal by clicking on the red **{{%button%}}Add Goal {{%/button%}} ** button. ![Editing DNFC Goals](DNFCGoals.png)|
|Difference|The difference between the goal and actual. For visual clarity, the number will be displayed in green if the difference is less than or equal to the goal. If the total is greater than the goal, the difference will be displayed in red.|

### Work Available Queue

This section will show how much work is in the queue to code for any given day. This allows users with the role of Coder to plan their workload based on availability and frees up management from having to monitor and communicate with the coding staff. Clicking on any of the blue numbers, will display the data behind that number. Right-clicking on the grid allows the user to export to csv.

![Work Available Queue](WorkAvailable.png)

### Patient Daily Census

This displays the patient daily census on patients discharged or still inhouse. Clicking on any of the blue numbers, will display the data behind that number. Right-clicking on the grid allows the user to export to csv.

### Case Mix Index

This section will display the case mix for the Last 7, 30, 90, and 180 Days

![Case Mix Index](CMI.png)

### Top 10 Final DRGs

This displays the 10 most coded DRG’s within the current month, prior month, or last 6 months.

![Top 10 Final DRGs](Top10DRG.png)