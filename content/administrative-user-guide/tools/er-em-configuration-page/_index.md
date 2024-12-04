+++
title = 'ER E/M Configuration Page'
weight = 110
+++

>[!Note] The organization must have ER E/M Configuration enabled to use this feature. If this is not currently enabled, please contact your account representative for more information.

Once the E/M Configuration has been enabled, the initial setup must be completed by the Dolbey Team. After this setup is finalized, your organization can make any desired changes directly or contact the SME Team at smeteam@dolbey.com for additional support.

Below is a reference guide to assist with setting up or modifying the configuration as needed.

The ER E/M Configuration can be found within the Tools menu. If enabled, it will be seen beneath Validation Management. 

![](2024-11-22_EMConfig.png)

When you click on the ER E/M Configuration, a page will open and should appear similar to the image below.

![](2024-11-22_EMConfigPg.png)

The configuration page allows you to set up the E/M Level Matrix and other related components. If a user has Facility Mapping, the E/M Configuration can be copied across different facilities.

When Facility Mapping is available, a new option will appear in the top-right corner of the screen, enabling you to select a facility. Once a facility is selected, the levels associated with that facility will be displayed. A Copy button will also appear at the top of the Levels section.

![](2024-11-22_Facility.png)

Clicking the Copy button opens a dialog box where you can choose a destination facility to copy the current levels to. Facilities available for copying will be listed in a dropdown menu. For example, if you are working in Dolbey South – Cincinnati, selecting the Copy button will allow you to pick another facility to replicate the levels.

![](2024-11-22_CopyFacility.png)

This option will overwrite and copy the current levels that are onscreen to the facility that is selected.

>[!Note] If an organization does not have Facility Mapping, and only has one facility, the copy options will be hidden.

## Configuring the E/M Matrix

The table below illustrates how the E/M Matrix will appear to end users. 
You can customize the text displayed in this table to tailor the information shown to end users.

![](2024-11-27_EMMatrix.png)

The E/M Level matrix features horizontal columns that display the levels across the top. Below each level are the criteria that define it,
organized into several categories. By default, these categories include the topics listed below; however, the topics are fully configurable
based on the specific needs of each facility. 

1. Mode of Arrival
2. Disposition
3. Testing
4. Medication
5. Behavioral
6. Procedures
7. Other Criteria

Each topic under the levels includes a list of items relevant to that topic and its corresponding level. 
The E/M Matrix configuration allows you to customize the content within each field under the respective E/M Level, 
enabling your facility to tailor the listed items for each code to meet its specific requirements.

To make changes to the default options, can click on of the grey numbers to open the matrix configuration.

![](2024-11-27_EMChanges.png)

After opening the number, you will see each E/M Level along with its corresponding codes. Under the Level Topic section,
you will find a "+Add" button next to each level. Clicking this button allows you to add a new criteria selection. An open
text field will appear where you can enter your facility's criteria. 

![](2024-11-27_EMAdd.png)

To remove any criteria selections, under each topic and level, simply click on the X button next to the criteria. 

![](2024-11-27_EMRemove.png)

To change or udpate the verbiage of the criteria selection, place the cursor into the level item field and change the text. 

![](2024-11-27_EMTextBefore.png)

![](2024-11-27_EMTextAfter.png)

## Configuring Charging Options and CDM

Below the E/M Level matrix configuration you will see a section for “Other”. The "Other" section allows you to add
in charging components attached to your facility's charge master. To make changes to the default, you can click on
the grey number to open the charge and CDM configuration.

The Effective Date field specifies the date when the CDM Table and its associated new charges will take effect. This feature allows you to schedule updates to the CDM Table, ensuring that future changes are staged and ready for the Coding Team when needed.

## Updating the CDM

Click on the green “Edit CDM Table” button to the right of the effective date.

![](2024-12-02_Options.png)

Clicking the button will open up the "Edit CDM Table" window where you can paste the CDM colmns directly from your Excel
spreadsheet.

![](2024-12-02_CDMTable.png)

The best practice is to paste in the column for the CDM code, then the description, and finally the CPT code. This step is
extremely important because any assigned CDM code will need to be sent in the outbound interface;
therefore, your CDM table needs to match whatever is going to be downstream from Dolbey.

After you paste in the information, click on the OK button to continue.

There is also a way to add a CDM code manually. To do this, click on the "+Add CDM Manually" button. This will create a new row with free text fields to add the CDM code, the description, and the CPT code. 

![](2024-12-02_AddCDM.png)

Once the CDM table is populated, you can edit the categories within the "Option" section. The default options available are:

- Trauma
- No charges
- Medication quantity
- Medication time/modifier
- Additional charges

Like the E/M Level matrix, these categories can be customized to suit your facility's specifc needs.

To edit an option, click the gray date tab to open the options and make changes. If certain options are not relevant to your facility, you can remove all items under those sections simply by clicking on the "Delete" button. Once emptied, the section will no longer appear for your users. 

## Trauma Section

When you open the trauma section, you will have an item name. Some data will be defaulted here. Each
of these items have a CDM attached per E/M level, including critical care. Ensure that the CDM
underneath each of the levels corresponds to what your CDM table indicates.

![](2024-12-02_Trauma.png)

For your end users this will appear as a drop-down menu. For example, when the user
selects **Pre-Hospital Notification**, they are not required to manually choose the E/M level. Based 
on the matrix and their selection, the system will automatically populate the corresponding CDM code associated 
with the assigned level.

![](image-529.jpg)

> [!caution]
If your CDM changes, you will need to update this table as well.

## No Charge Section

Once you have reviewed the Trauma section you can then click on the gray date next to the "No Charge" option. The "Item" field will be the verbiage that you want to correspond to the CPT code in the CPT column to the right of the Item column. 

![](image-527.jpg)

For your end users, this will appear as a drop-down menu. The user will choose the item and the outbound interface
will contain both the CPT code and the corresponding CDM code that you have listed in this table.

![](image-528.jpg)

## Medication Quantity

Once you have reviewed the "No Charge" option you can then click on the gray date next to the "Medication
Quantity" option. In this section, you can list item names, for which we have provided default descriptions. These items will
align with their corresponding CPT and CDM codes.

![](image-530.jpg)

The medication quantity as well as the medication time modifier is not about the medication, but rather the
way the medication was administered. This allows you to charge for any injections, infusions, IV pushes,
immunizations, and hydration. The medication administration quantity allows you to define how many
of each occurred on a particular date, if the ER visit occurred over more than one day, and other
modifiers which can be added as needed.

To the end-user this looks like a table where they can pick all the medication administrations to apply
and provide dates and modifiers. There is a section for the end users to enter a note to keep everything
in line so that they can indicate which medications they have already charged for. This helps the end-
user keep their thought process together, and also provides information in the event that there is an
audit.

![](image-531.jpg)

## Medication Time/Modifier

Medication administration time/modifier is very similar to the medication administration quantity. The
only difference is that you are able to indicate that there are, for example, multiple infusions. If there
are different drugs involved you can copy the individual lines so that you can add in the durations of
each medication along with the date and modifier if the modifiers are different.

Some organizations like to have medication administration quantity and medication administration
time/modifier, however, other organizations will relocate all of the items within the medication
administration to the medication administration time/modifier section so that all medications are within
the same section.

Within this section, you can list item names, for which we have provided default descriptions. These items will
align with their corresponding CPT and CDM codes.

![](image-532.jpg)

To the end-user, this looks like a table where they can pick all the medication administrations to apply
and provide date and modifiers. There is also a section for the end users to enter a note to keep
everything in line so that they can indicate which medications that they have already charged for. This
helps the end-user keep their thought process together, but also provides information if there is an
audit. There is also a copy button to the left of the note that allows the end user to copy if there are
more than one medication that needs to be considered.

![](image-533.jpg)

## Additional Charges

The "Addtional Charges" option allows you to enter items that are commonly charged in the ER. By default, we have 
identified four common items; however, you can easily add more by clicking the "+Add" button. If any of the default
items are not applicable to your facility, you can remove them by selecting the "Delete" button next to the item.

Within this section, you can list item names, for which we have provided default descriptions. These items will
align with their corresponding CPT and CDM codes.

![](2024-12-02_Additional.png)

To the end-user this looks like a table where they can quickly add a quantity, date, and modifier if any of
the default charges are applicable.

![](2024-12-02_AdditionalForUser.png)
