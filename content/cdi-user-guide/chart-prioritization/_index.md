+++
title = 'CDI Alerts and Chart Prioritization'
weight = 20
+++

The software has a feature called CDI Alerts which are automated messages generated by the software
that can be used to prioritize your CDI workflow. CDI Alerts are used to detect potential inaccuracies,
inconsistencies and or discrepancies in clinical documentation. These Alerts help CDI teams to prioritize
the charts based on potential query opportunities available.

The software provides real-time Alerts when potential query opportunities are identified. Which will
then allow CDI staff to prioritize charts based upon those potential opportunities.

## What is a CDI Alert Topic?

CDI Alert topics are the diagnosis that is being targeted by the Alert. The Topic encompasses a broad
range of diagnoses that address various issues being targeted by our system. These diagnoses then
branch out into more specific types known as Alerts. These are based on the type of issue being
Targeted.

## What is a CDI Alert Message?

The Alert message is a specific message that details what is missing, incomplete and/or inaccurate
documentation that is missing with the Diagnosis/Topic that is being targeted.

## CDI Alert Types

CDI Alerts branch out into 4 types of Alerts.

| Alert Type                                      | Description |
| ----------------------------------------------- | ----------- |
| **No Documentation but, Clinical Indicators**   | This Alert type is when the provider did not document a Diagnosis but, there are Clinical Indicators that support “Possible Diagnosis”.|
| Documentation but lack of Clinical Indicators   | This is where the provider documented the diagnosis but there is a lack of Clinical Indicators that support the diagnosis. For example, if Sepsis was documented by the provider but, it's not supported by Clinical Indicators. This Alert helps to ensure that diagnoses are audit proof. Ensuring that the supporting evidence requiered for a proper diagnsosis validation is present within the patients chart. |
| **Documentation but Not Fully Specified           | This is where the provider documented a diagnosis but, it was not documented to its Full Specificity. For example, Heart Failure Unspecified; the diagnosis is not documented to the Full Specificity. This CDI Alert is helpful for ensuring that Diagnoses are documented to their full extent in order to combat denials. |
| Conflicting Diagnosis                           | This Alert looks at if there are two or more Fully Specified versions of a diagnosis that maybe potentially conflicting. For example, if the provider or providers in one location documented that a patient had Acute Diastolic Heart Failure and the other location of the patients record it was Acute on Chronic Systolic Heart Failure, this Alert helps to make sure that the proper diagnosis is present to have an accurate patient picture for all care providers involved. |


## Setting up CDI Alerts

In order to set up CDI Alerts you must reach out to the SME Team (smeteam@dolbey.com) for
assistance there is a module that must be deployed in conjunction with set up within the workflow
management editor.

## Workgroup Prioritization

Once the CDI Alerts are setup you will see within the workgroup there is a column named “criteria
group” it may be named something different depending on your setup you should check the grid column
configuration if you do not see this field to see if its viewable or has a different name.
These criteria groups are used to indicate a “potential” query opportunities based upon the algorithms.
Once the algorithms meet the criteria to initiate a CDI Alert then it will be matched on in workflow and if
it’s the only Alert it will display as the “ Criteria Group”.

![Workgroup Prioritization](image-279.jpg)

In cases where multiple Alerts match during workflow execution, the displayed criteria group name will
be determined by the hierarchical list. This hierarchical list is established by your management team
using the workflow management editor. The management team has the ability to rearrange the order of
the Alerts based on priority and initiatives at your hospital, ensuring the Alerts are organized from
highest to lowest priority.

There is also a second grid column called “Active Matched Criteria Groups”. This column will display the
actual number of active CDI Alerts on the account not just the Alert it matched first going through the
workflow list. This column represents the total number of “potential” query opportunities in a patient
record.

You have these two columns available, namely the “Criteria Group” and “Active Matched Criteria
Groups”, which can be utilized to prioritize the worklist. Among these columns, the most valuable one
we feel is the “Active Matched Criteria Groups”. It enables you to concentrate your team's efforts on the
charts that require the most significant improvement, allowing you to prioritize your resources
effectively.

It’s important to note that the only Alerts that affect the Priority Criteria Group name and number of
Active Matched Criteria Groups are Active Alerts. Once an Alert is closed it will not be used in these
columns for prioritization. This helps to make sure we are putting the charts with the most priority in
front of the CDIS. As Alerts are closed these numbers will be updated in real time.

## Viewing CDI Alerts

To access and view CDI Alerts within a patient's chart, you can locate them in the
Navigation Pane positioned above the Documents Pane. Below that, you will find
the "CDI Alerts” viewer. By clicking on the CDI Alerts viewer, you will notice a box
with an arrow next to CDI Alerts tab in the navigation pane.

![CDI in Nav Tree](image-280.jpg)

Clicking on this box will detach the CDI Alerts Viewer, opening it in a separate
page. This feature allows the end user to move the viewer to a second monitor,
which can be advantageous when toggling through the evidence hyperlinks listed within the CDI Alerts
Viewer. This allows you to easily review the evidence provided without having to continously go back to
the Alerts viewer.

## Navigating the CDI Alerts Viewer

Once in the CDI Alerts Viewer you will notice two headings in the dark blue bars “Active Alerts” and
“Completed Alerts”. When you click on the either of these headings you can either expand or collapse
that section and hide or view any alerts present under those sections

![Navigating the CDI Alerts Viewer](image-281.jpg)

### Active Alerts

The section “Active Alerts” are Alerts that the system found and no action has been taken meaning
closed by the specialist or queried on.With each Active Alert you’ll notice a word(s) prior to a dash,
which correspond to the CDI Alert Topic..

The words after the dash are a brief description of what the system found to be missing, incomplete or
possibly inaccurate also known as the CDI Alert Message.

After that you will notice and @ sign with a date and time following. This date and time is when the
system found compelling evidence of something missing, incomplete, or possibly inaccurate information
leading to a CDI Alert being iniated. This information is tracked for reporting so you can see how quickly
the system is triggering an Alert.

### Completed Alerts

The section “Completed Alerts” are alerts that have been closed by either the system Auto-Resolving the
Alert or by the end user taking action either by initating a query or by clicking the close button which is
the red x. You will notice the @ sign with a date and time following. The date and time present is when
the CDI Alert was closed by the system or the end user. You will also see a message after which depicts
how the alert was closed.

| Resolved Type                   | Definition                                                                      |
| ------------------------------- | ------------------------------------------------------------------------------- |
| CDI Audit Education Opportunity | This is an opportunity for education.                                           |
| Insufficient Clinical Evidence  | The abstracted evidence was insufficient to support the alert.                  |
| Documentation already present   | Documentation for the condition related to the alert is present on the account. |
| Handled with query              | A physician query was opened for this alert.                                    |

### CDI Alert Notes

Next to each of the Alerts in either the Active or Completed Alerts section is a paper icon.

![CDI Alert](image-282.jpg)

When you click on that paper icon it will launch you into a notes page. This can be used by a CDIS to
leave a note if they don’t feel the Alert currently doesn’t have enough evidence to build a query but isn’t
necessarily ruled out or seems to be trending towards the diagnsosis Alerted.

![CDI Alert Notes](image-283.jpg)

Instead of closing the Alert prematurely if you aren‘t sure if the Alert isn‘t correct it may be useful to
wait and provide a note on why you are waiting becasue new information may present. Once a note is
typed in it will leave the date/time and along with the CDIS name so if another CDIS enters the chart
they will be able to clearly see who chose to monitor the Alert
at this time and why.

![Active Alerts](image-284.jpg)

![Active Alerts](image-285.jpg)

Upon adding the note the paper icon will turn red, notifying the next user that is reviewing the CDI Alerts
that there is a note present on the Alert.

### CDI Alert Editor Function

Adjacent to the Alert message, you'll find a pencil icon. Clicking on it will open an editor,
enabling you to rearrange and customize the placement of evidence using a drag-and-drop functionality.
This feature empowers CDIS professionals to organize their items in a personalized manner, aligning
with their specific querying requirements.

### Reviewing Clinical Evidence

Each CDI Alert contains clinical evidence extracted from the patient's chart. There are four different
types of evidence you will see. First are words and phrases within documentation such as signs and
symptoms, and medications. Second are value abstractions from the documentation such as vital signs
or laboratory findings within physical documents. The third are code abstractions from the
documenation. Fourth are discrete values such as laboratory studies and vital signs found in the
flowsheets, medications from the medication viewer and other flowsheet data. Finally, there are links to
documents. These links consist of the document name and connect directly to the respective document.
This feature proves valuable when referencing specific CT Scan documents that may be pertinent to a
particular Alert. This evidence is categorized into sections such as Laboratory Studies, Clinical Evidence,
Vital Signs, and Intake and oOutput Data.

![Reviewing Clinical Evidence](image-286.png)

The blue text serves as a hyperlink. Furthermore, following the abstraction, you will observe word for
phrase in quotes. That is the words or phrases that then engine found in the documentation or values.
Subsequently, either the document name and document date are considered if derived from a
document, or the result date and time are used if obtained from flowsheets. In the case of medication
discrete abstraction, the medication name, dosage, route, and the date and time of administration are
presented.. This helps provide the necessary context. When evidence with a document type and date is
selected it will hyperlink you to the place in the document that abstraction was found and highlight that
yellow. You will also note that there is green highlights with words or phrases in the documentation.
Those are abstractions that are specific to CDI Alerts. They are just like code abstraction, but are what
we use for CDI rules. When you hover your mouse over the green abstraction it will provide you with an
understanding of which Alert the evidence is being used for if there are multiple Alerts present.

![Reviewing Clinical Evidence Document](image-287.jpg)

![Reviewing Clinical Evidence Code](image-288.jpg)

When you click on a hyperlinked evidence that is folled by result date and time, indicating a discrete
value abstracted from the flowsheets, it will automatically take you to the corresponding location in the
flowsheets and highlight the respective row.

![Reviewing Clinical Evidence Discrete Value](image-289.jpg)

Another noteworthy capability within Clinical Evidence is the ease with which a CDIS can incorporate
additional evidence. While reviewing documentation and flowsheets, if CDIS identifies items deemed
crucial for inclusion in the CDI Alerts as supporting evidence for a query, they can effortlessly highlight
words or phrases in a document, up to a maximum of 1000 characters, and perform a right-click. This
action triggers a menu presenting various options, including one that reads "Copy to CDI Alert." Clicking
on this option reveals a pop-out menu displaying available Alerts to which the evidence can be added

![Copy to CDI Alert](image-290.jpg)

Upon selecting the desired Alert, the system opens the Evidence Editor, allowing the CDIS to specify
where the evidence should be attached. If the CDIS clicks on existing evidence, the new evidence will be
attached below it. Therefore, it is crucial to ensure that, when determining the placement, the CDIS
selects the appropriate location by clicking above. Once the evidence is copied over, the system
provides details such as the evidence itself, the name of the document, and the date. For Laboratory
Studies, it includes the result date and time.

After incorporating the evidence into the designated alert, any highlighted evidence will be displayed in
the document in purple, accompanied by the phrase "MANUALLY_ADDED" in green at the end. This
informs the user that the evidence was added manually. Similar to other evidence, hovering over the
green-highlighted section will provide information about the CDI Alert to which the item was applied.

![Evidence Editor](image-291.jpg)

Next when going back to the CDI Alerts viewer you will notice check boxes present next to the evidence
which serves two purposes. Firstly, if you initiate a query, any evidence marked with a check mark will
be automatically be copied to your clipboard, enabling you to conveniently paste it into your query. This
copying action occurs when you click on the envelope icon


Secondly, unchecking any of the clinical evidence will put a strike through the text and it will prevent it
from being copied over. Additionally, any unchecked evidence will be reported back to Dolbey's clinical
team if an Alert is closed due to it having invalid clinical indicator, insuffiecient clinical evidence or
documentation is already present.

![Unchecking Evidence](image-292.jpg)

### How to initiate a Query

In the right hand corner of the Alert you will see a blue envelope icon next to a red x icon. When you
click on the blue envelope it will launch you into the query.

### Query

Once in the query you will notice that a template will autoload for the specific Alert. These autoloaded
templates can be set by the management staff templates specific to each site and what they use as
querys.

The evidence previously examined on the Alerts viewer page can now be effortlessly incorporated into
the query. When the query button is pressed, the selected evidence will be automatically copied to the
clipboard. You can then paste it using a simple process, either by pressing the "ctrl" and "v" keys, the
standard Windows keyboard shortcut for copying, or by performing a right-click and choosing the paste
option. After the query is submitted, the corresponding CDI Alert will transition from the Active Alerts
section to the Closed Alerts section.

Once that query has been submitted that CDI Alert will move from the Active Alerts section down to the
Closed Alerts section.

![Unchecking Evidence](image-293.jpg)

## Autoresolve

The Alerts have the ability to autoresolve themselves if documentation comes in that would satisfy the
Alert. Once an Alert is Autoresolved it will move to the Close Alert section. This will ensure that we are
only putting Alerts to the end-user that require attention. We don’t want them to have Alerts that need
no action.

## Closing Alert without Querying

If a CDIS chooses that an alert needs closed not by a query being initiated by the envelop button. This is
done by clicking the red x and it provides several choices for closing an Alert. There are several options
to state why an Alert is being close without query being sent or placed. There is a section at the bottom
for additional notes that we encourage the specialist to provide a deeper understanding of why the
closed.

![Closing Alert without Querying](image-294.jpg)

## Documentation Reviews

If your site does different styles of CDI reviews or want to track management reporting different than
how our default tracks, you can use the documentation review viewer to track reviews by topic. Other
organizations have used this if there CDI team would like to do a utilization management type review
and it doesn’t fit the typical initial or follow up review.

By default, documentation reviews by design have a free form text field however, you can also create
forms within the form designer for each of these reviews.

If your site does not have documentation reviews enabled, and you wish to track reviews different than
the default contact us at smeteam@dolbey.com we can show you a demo and discuss if this is a good fit
for your organization.

![Documentation Review](image-296.jpg)

By clicking on “+ Add Review” you can select the type of review that you wish to complete. 

> [!tip] Review Type List Configuration
The list of review types presented here are configurable by a site administrator through
[Mapping Configuration.]({{< ref "../../administrative-user-guide/mapping-configuration" >}})

![Documentation Review](image-297.jpg)

Then, type in your notes.  Finally, click Ok to save.

![Documentation Review](image-298.png)

Each review is saved, there are custom management reports to report out specific reviews and the CDI
Management and CDI Personal Dashboard will all change to accommodate these custom reviews, if you
do not have this enabled custom review info will be hidden since its not appliable.


