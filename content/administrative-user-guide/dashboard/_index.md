+++
title = 'Dashboard'
weight = 30
+++

A user with administrative rights is provided with overviews of Coder and CDI activity. The administrative
user can also select to look specifically at Coder or CDI information by selecting the appropriate
dashboard button.

The dashboard is shown when the user logs in and after login, it can be accessed by 
- Clicking on Fusion CAC/CDI in the top left corner of the application
  
![Fusion CAC](FusionCAC.png)

- Clicking on the reporting menu item and selecting dashboard
  
![Reporting Menu Dashboard](Dashboard.png)

The software has 6 main dashboards with drill down data:

1. Administrative Dashboard
2. Coder Personal Dashboard
3. CDI Management Dashboard
4. CDI Personal Dashboard
5. Audit Management Dashboard
6. Audit Personal Dashboard

### Administrative Dashboard

The administrative dashboard is only available for those users with the administrator role. This dashboard
displays data at a glance. Clicking on any of the blue numbers will open a grid to display the data
that goes into that number.

![Administrative Dashboard](AdminDash.png)

#### Users Online

This displays the users online or offline broken out user type. The blue numbers are links to view the
user detail behind the number you selected.

![Users Online](UsersOnline.png)

![Users Online Detail](CodersOnline.png)

Users can right click on the grid to export to CSV.

#### Open Queries

This section displays open, unanswered, and answered queries per role along with average turn around time (TAT) and provider
response rate.

![Open Queries](OpenQueries.png)

Click on any of the blue numbers to see the data behind that number. Right clicking on the
grid provides the option to export to CSV.

##### Top 10 Queries in Last 30 Days

This displays the 10 most used query templates within the last 30 days.

![Top 10 Queries](Top10Queries.png)

Click on any of the blue numbers to see the data behind that number. Right clicking on the
grid provides the option to export to CSV.

#### AutoClose Daily Stats

This section displays AutoClose stats, including charts autoclosed and rejected on the current day. It also includes data for
month to date. 

![AutoClose Daily Stats](ACDailyStats.png)

Click on any of the blue numbers to see the data behind that number. Right clicking on the
grid provides the option to export to CSV.

#### Coder Productivity

This displays the coders productivity by charts submitted and those that are pending.

![Coder Productivity](CoderProductvity.png)

Click on any of the blue numbers to see the data behind that number. Right clicking on the
grid provides the option to export to CSV.

#### Coding Trends per Day

Coding Trends per day combines "Average Daily Coded" and "Average TAT to Submit" to show
averages over the last 7, 30, and 90 days compared to the prior 7, 30, or 90 days, grouped by category.

![Coding Trends Per Day](TrendsPerDay.png)

#### Discharge Not Final Coded (DNFC)

This section provides the admin staff the ability to see where the organization is in regards to the outstanding sum of total charges. The data broken down by total outstanding charges per charts outstanding for the current month also known as discharge not final
coded. The admin staff can also see if the team is meeting their goal for how many charts are
outstanding at the end of the month. A comparison is displayed to show total charges for the current
month compared to the previous month.

![Discharge Not Final Coded](DNFCSection.png)

##### Filtering Discharge Not Final Coded (DNFC)

This section can be filtered by facility and/or category. By leaving the filters blank it will combine all
facilities and all patient types. You can use the filter to filter by a facility by clicking on the drop down
or you can also include a category so that it only displays inpatient information.

![Filtering DNFC](image-347.jpg)

###### Available

Defined as all patients discharged and not submitted within a coding worklist (Workgroup Type must
equal coding) per either the “current month” or “previous month” depending on the column reported.
Next to each value should be a number in blue that represents the number of charts that make up the
dollar value. Users can click these numbers to drill down and display the chart details

###### Unavailable

Defined as all patients discharged and not submitted and not within a coding worklist (Workgroup Type
not equal to coding) per either the “current month” or “previous month” depending on the column
reported. Next to each value should be a number in blue that represents the number of charts that
make up the dollar value. Users can click these numbers to drill down and display the chart details. In
the drill down it would be helpful to pivot the list first on the Workgroup Type and then by Pending
Reason.

###### Total

This will be the total of both available and unavailable for coding.

###### Goal

This section of the dashboard allows you to set a target goal for your discharge not final coded. You can
set the goal by clicking on the red button that indicates “Add Goals”.

By clicking on “Add Goals” you can set the goals per facility and per category.

![Filtering DNFC](image-349.jpg)

###### Difference

The difference between the goal and actual (Goal - Total DNFC). For visual clarity, the number will be
displayed in green if the difference is less than or equal to the goal. If the total is greater than the goal,
the difference will be displayed in red.

### Work Available Queue

This section will show how much work is in the queue to code for any given day. This allows the Coder
User to plan their workload based on availability and frees up management from having to monitor and
communicate with the coding staff. If you click on any of the blue numbers, you can see the data behind
that number. If you right-click on the grid you can export to csv.

![Filtering DNFC](image-350.png)

### Patient Daily Census

This displays the patient daily census on patients discharged or still inhouse. If you click on any of the
blue numbers, you can see the data behind that number.

![Patient Daily Census](image-351.png)

If you click on any of the blue numbers you can see the data behind that number. If you right click on the
grid you can export to csv.

![Patient Daily Census](image-352.jpg)

### Case Mix Index

This section will display the case mix for the Last 7 Days, Last 30 Days, Last 90 Days and Last 180 Days

![Case Mix Index](image-353.png)

### Top 10 Final DRGs

This displays the 10 most coded DRG’s within the last 30 days

![Top 10 Final DRGs](image-354.png)

## Coder Personal Dashboard

The Coder dashboard is only available for users with a coder role. This dashboard displays quick data at a
glance personal statistic. Clicking on any of the numbers in blue will open a grid to display the data that
goes into the number displayed.

![Coder Personal Dashboard](image-355.jpg)

## CDI Management Dashboard

The CDI Management Dashboard is available for management users with CDI role and can be deployed
with a special role to CDI users if they have a need to see a team view of what all CDI users are doing.
This dashboard displays at a glance team statistics. Clicking on any of the numbers in blue will open a
grid to display the data that goes into the number displayed.

![CDI Management Dashboard](image-356.jpg)

## CDI Personal Dashboard

The CDI Personal Dashboard is available users with CDI role for users to see their personal statics
separate from the team view. This dashboard displays at a glance personal statistics. Clicking on any of
the numbers in blue will open a grid to display the data that goes into the number displayed.

![CDI Management Dashboard](image-357.jpg)

## Audit Management Dashboard

The Audit Management Dashboard is available to users with Auditor role to see team view of what all
Auditor users are doing. This dashboard displays quick data at-a-glance team statistics. Clicking on any of
the numbers in blue will open a grid to display the data that goes into the number displayed.

![Audit Management Dashboard](image-358.jpg)

## Audit Personal Dashboard

The Audit Personal Dashboard is available to users with Auditor .U to see their personal statistics
separate from the team view. This dashboard displays quick data at-a-glance personal statistics. Clicking
on any of the numbers in blue will open a grid to display the data that goes into the number displayed.

![Audit Personal Dashboard](image-359.jpg)
