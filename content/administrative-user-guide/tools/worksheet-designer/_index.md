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

A blank template will appear on screen. The first step is to enter a unique a document name. Each worksheet must have a unique name for reporting purposes. **A document name must exist *before* the template can be saved.**

![Blank Template](BlankTemplate.png)

To start with a document that has already been created, copy the text and paste it into the form
designer. Changes to the formatting may be needed once pasted depending on the original document format.

Text copied or typed directly into the worksheet will be read-only for the end user(s) working with the form. This text is often used as labels and to direct users on completing the template. 

![Static Text](StaticText.png)

### Adding Fields

Fusion CAC offers several types of fields that can be added to worksheet templates. These fields all end users to enter information into the worksheet. 

Add a new field by clicking {{%button%}}+Add Field{{%/button%}} in the template tool menu.

![Add Field](AddField.png)

![Add Field Dialogue](AddFieldDialogue.png)

#### Field Type

![Field Type](FieldType.png)

###### Single Input

![Single Input Field](SingleInput.png)

A single input field allows the end user to free type text. This field is best used for entering a concise amount of information, such as a name or short series of numbers. The box will grow horizontally as the user types to fit the data entered.

###### Multiple-Line Text

![Multiple-Line Text](MultiLineText.png)

A multiple-line text field allows the end user to free type text. This field is often used for entering a large amount of information, such as taking notes or providing detailed comments. The box will grow vertically as the user types to fit the data entered. 

###### Checkbox

![Worksheet Checkbox](Checkbox.png)

A checkbox allows the end user to indicate certain items are applicable. This field has been used to show that the worksheet is complete or as a way for users to select certain action items. 

###### Date/Datetime

![Date](Date.png) ![Datetime](Datetime.png)

These fields allow the end user to indicate the date and time of a response, test, or other item being tracked. 

###### Dropdown

###### Account Field

#### Field Name

![Unique Field Name](FieldName.png)

Each field should have a unique name for reporting purposes. 

Field names can repeat across worksheets, but **each field on a worksheet must be unique.** If a field name is repeated on a worksheet, whatever is entered into one field will be automatically duplicated into the other fields with the same name on that worksheet. 

#### Editable

![Editable](Editable.png)

Individual fields can be locked down per user role. This way Auditors, CDI Specialists, and Coders can add and view a shared worksheet to a chart, but only users with the specified role can edit certain fields. All users will be able to see the information in that field, but only the specified user role can edit the field. 

#### Make Required

![Make Field Required](MakeRequired.png)

Fields can be made required by checking the box. Leaving the box unchecked means the field is optional and the worksheet can be completed even if that field is left blank. 

When a worksheet is added to a chart, required fields will have a light red background to indicate action must be taken. Addiontally, the user will be presented with a red toast message if they try to save the chart without completing all required fields. The toast message will include the fields that need to be completed. 

![Required Field Red Background](RedRequiredField.png)

Clicking OK, will add the selected field to the template with the specified settings. A box will then display in Worksheet Designer as a
placeholder for the selected field with the field name. The fields are not interactive from Worksheet Designer. Once a worksheet has been added to a chart, the field name will be replaced with instructions for the end user. 

![Fields From the Front End](FrontEndFields.png)

## Show History

Worksheet Designer will create a history for changes made to templates in Form Designer. Once a change is
made on a form and saved, {{%button%}}Show History{{%/button%}} will appear in the top right of the worksheet. Clicking
on it will bring up a notes box, just like in Workflow Management.

![Show History Button](ShowHistory.png)

![Show History Changes Dialogue](ShowHistChanges.png)

