+++
title = 'Worksheet Designer'
weight = 150
+++

![Worksheet Designer](WorksheetDesigner.png)

Worksheet designer is used to create custom worksheets for users, which are used to collect data and/or take notes.

Access to worksheets can be restricted by user role:
- Audit
- CDI
- Coding
- Physician Coder

Alternatively, worksheets can be shared. A **Shared Worksheet** is a worksheet that can be utilized by Auditors, CDI Specialists, and Coders unlike the "CDI Worksheet" and "Coder Worksheet" which are exclusive to CDI and Coding, respectively.

## Creating a New Worksheet

To add a workheet, simply click on the {{%button%}}+Add{{%/button%}} button in the desired section. 

![Add New Worksheet](AddWorksheet.png)

A blank template will appear on screen. The first step is to enter a unique a document name. Each worksheet must have a unique name for reporting purposes. A document name must exist before the template can be saved. 

![Blank Template](BlankTemplate.png)

To start with a document that has already been created, copy the text and paste it into the form
designer. Changes to the formatting may be needed once pasted depending on the original document format.

Text copied or typed directly into the worksheet will be read-only for the end user(s) working with the form. This text is often used as labels and to direct users on completing the template. 

![Static Text](StaticText.png)


However, you can
create fields that they can enter information into the form by clicking
on Add Field will present an updated dialog that includes a new
"Account Field" type.

![](image-550.jpg)

In this dialog, the field name should be unique, so you can do reporting.
You can also make fields required by checking the box or not if it’s
optional. After clicking OK, another dialog will appear to
select the field to display. After selecting a field, a box will display in Form Designer as a
placeholder for the field that you selected. Chose the type of field that makes sense
based on the form.

![](image-551.jpg)

In the Physician Query Dialog or in a manually added worksheet within an account, the
placeholder will be replaced with bolded text representing the field's actual value

![](image-548.jpg)


## Creating Dynamic Sections

What is a Dynamic Section? This allows users to create a template for the user creating the query to
customize the query by removing sections as needed from the template or to
rearrange the order of information.

![](image-554.jpg)

The Field Name will be displayed in the template above its section. Text and
fields can be inserted into a section; sections cannot be inserted in other sections.
When the template is added to a query, each section will now show an up and
down arrow for movement, along with an X to delete that section from the query.

Once sections are created, they will look like the below within form designer:

![](image-555.jpg)

Once sections are created, they will look like this when a user created a query within an account

![](image-556.jpg)

A user can move sections up or down, or remove sections. If you remove a section you will be presented
with an undo button to place it back into the query.

## Creating Internal Notes

Internal only notes can now be added to Physician Query templates from
the form designer. On a template, clicking the Insert dropdown will now
show a new option of Add Internal Note. The Internal note is only
displayed for the user filling out the query and is not set to the provider
receiving the query.

![](image-560.jpg)

Selecting this option will add a highlighted free text line to the
document.

![](image-557.jpg)

When adding a physician query the user will see the highlighted section in the query when that template
is selected.

![](image-558.jpg)

After sending the query, this note will no longer be seen unless the user has the privilege of ‘Edit Open
Queries to resend’ in Role Management. An Edit checkbox will show on the date line, and checking it
will show the query with the internal note.

![](image-559.jpg)

In user reports, the following
reports will display the "Query For" field in the same field as the "Query Template" column separated
with a colon:

- Outstanding Queries
- Query Impact by Discharge Date
- Query Impact Report
- Query TAT by Author Report
- Query Template Volume Overview

Form Designer will create a history for changes made to templates in Form Designer. Once a change is
made on a form and saved, a Show History button will show in the top right of the worksheet. Clicking
on it will bring up a notes box, just like in Workflow Management.

![](image-561.jpg)

