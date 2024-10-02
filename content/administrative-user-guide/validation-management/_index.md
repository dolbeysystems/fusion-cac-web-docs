+++
title = 'Validation Management'
weight = 100
+++

Validation management is a rule editor that is permission based and can be found under the Tools menu.

Validation rules allow the admin staff to create rules that show up on the code summary page to prevent
users from submitting a patient chart or provide a warning to simply warn the user that something may
need to be completed instead of preventing submission.

From the front end of the software, you can create simple rules such as:

- A user must have a discharge date to submit a patient chart that is inpatient.
- If the coder codes a newborn code, the newborn weight must exist.
- If a certain charge is on a chart and a diagnosis code is not present.

There are countless ways to use this validation rules editor to notify your end-user, whether they are
coder or a CDI specialist

## Creating a Validation Rule

You can create new rules by entering in a rule name in the top right-hand corner of the page and clicking
on +add rule.

![](image-495.jpg)

This adds the new validation rule and a number to the rule. This way when you are trying to
troubleshoot a rule that may not be doing quite what you were looking for, it will tell you what rule
number it happens to be to make it easier to target the rule in the validation rules editor.

![](image-491.jpg)

### Level Type

Once you have named a validation rule, you can then open the rule by clicking on the +. Once you have
done that, you now must define what you want the validation rule
to do. Start by selecting the level of the rule on the left-hand side.

![](image-497.jpg)

The levels are defined as:

- **Error** - This validation rule must be resolved before the
user can submit a chart. Typically, this type of rule only
applies to a coder because CDI specialists do not typically submit charts. This validation rule
appears in a red color, indicating there is a hard stop.
- **Critical** - This validation rule is the same as an error, with an additional warning. If, upon clicking
save, the end-user still has a critical error, they will get a pop-up box that indicates they still
have validation rules outstanding and asking if they wish to continue. This validation rule
appears in a red color, indicating there is a hard stop.
- **Warning** - This validation rule is a soft stop used to notify a user that there may be things that
they need to resolve. It does not prevent the user from submitting the chart. This validation
rules appears in a yellow color, indicating there is possible intervention needed.
- **Toast Message** - This is a notification that comes from the top right-hand corner of the browser
as a red notification that is presented for a few seconds. Toast messages do not stop the user
from submitting or saving a chart. It is simply a notification message to alert the user.
- **Disabled** – This will disable the validation rule and turn the rule within validation management
red to show it is not active.

### Defining the Criteria

Once you have selected the level of the validation rule you want to create, you must define what the
criteria is starting with the verbiage you want to display to the end user. For example, you can display an
error if a chart does not have a discharge disposition, so it doesn’t get submitted to billing without one.
Since we would want to warn the coder and not the CDI specialist, we would add another criterion input
so user role is not equal to CDI specialist. First, type in the display name, which is displayed for the user
on the code summary so keep it simple but provide how they fix the error.

Example: **D/C Disposition must be present** - The end user would know they have to add that to
continue.

![](image-498.jpg)


### Type of Criteria

Once you have created the rule name, click on **Add Criteria** to define how the system fires this rule.
Upon clicking on **Add Criteria**, you will be presented with types of criteria.

**Account** – Account type criteria allows you to select fields for a patient chart/account such as discharge
date discharge disposition, admit date, procedure codes, diagnosis codes, and many others.

**User** - User type criteria allows you to restrict the rule to a certain users role, such as a coder or a CDI
user role only. Commonly, an account criterion and a user role will be used together, however account
level criteria can be used independently from the user role. It does not, however, make sense to create a
rule on a user role and not define any other account level criteria.

![](image-499.jpg)

Once you have defined the type of criteria, you can then add the details.

Example: **ERROR: D/C Disposition must be present**

Building criteria for a validation rule is much like workflow. For this example, select account, then in the
field name find Discharge Disposition. Once you drop in the field name, it will then give you other fields.
In this example it allows you to select an operator.

![](image-500.jpg)

## AND/OR Criteria

Validation Rules, much like workflow, has two different options to create a validation rule.

1. AND criteria
2. OR Criteria.

### Example of AND Criteria

At the end of each criterion, you add an “AND” (see below). This criterion will cause the validation rule
to display if the patient has both a newborn Z code AND an admit type of 4.

![](image-498.jpg)

### Example of OR Criteria

At the end of each criterion, you add an “OR” (see below). When you add an OR criteria it will turn blue
to differentiate between the first and second statement. This criterion will cause the validation rule to
display if the patient has either a newborn Z code OR an admit type of 4.

![](image-501.jpg)

| Operator             | Description |
| -------------------- | ----------- |
| Equals               | This is used if you have one value, and it must equal the value. This is case sensitive. |
| >                    | This sign means that the value must be less than the value noted. |
| <                    | This sign means that the value must be greater than the value noted. |
| >=                   | This sign means that the value must be less or equal to than the value noted. |
| <=                   | This sign means that the value must be greater or equal to the value noted. |
| In List              | If you have more than one value, it could be any of the following. |
| Not In List          | If you have more than one value, you do not want it to equal. |
| Contains             | If you have a word, phrase or value that can contain it must have what you added exactly. This is common when including payors. |
| Only Contains        | Any one of the codes it is not needed to do all 3. |
| Exists               | This will search to see if anything “exists” in this field, if it’s not blank it will match. No value is needed after the operator. |
| Does not Exist       | This will search to see if anything “does exists” in this field if it’s blank it will match. No value is needed after the operator. |
| More Than            | This operator is only used with date fields, you will need to define “more than” how many days ago. You cannot add a date into the field as this field will need to be dynamic therefore days ago is used. |
| Less Than            | This operator is only used with date fields, you will need to define “less than” how many days ago. You cannot add in a date into the field as this field will need to be dynamic therefore days ago is used. |
| Later Than           | This operator is only used with date fields, you will need to define the exact date you do not wish to exceed. |
| Is On                | This is for an exact date, this is uncommon to use for workflow. |
| Includes Each Of     | If you have more than one value, it must contain all of the following. However, note the chart must have each of the values but can also have other values. |
| Includes Any Of      | If you have more than one value and it could be any of the following. |
| Does not Include     | If you have more than one value, you do not want it to equal you must use “Not In List” |



Once you have selected the field and your operator add a value.

Example: **ERROR: D/C Disposition must be present** We might select **Does Not Exist** as an operator. This would
mean if a discharge disposition does not exist, then this rule would display on the code summary and prevent 
the user from submitting the chart.

![](image-503.jpg)

Additionally, we may only want to display this rule if the user has a role of a coder. To constrain the rule further,
click on the **Add Criteria** again, select user, and then select “Is not CDI Specialist”. This will prevent the
rule from display to a user with a role of a CDI.

![](image-502.jpg)

### For Each Check Box

**For each** is used for fields that are repetitive. For example, a field like discharge disposition is a single
field (there are not multiple discharge dispositions on a patient chart) therefore, you do not need the
"for each" checkmark.

The **For Each** checkmark makes sense when you’re trying to create a rule that would have multiple
outcomes, such as checking if any diagnosis codes have a POA status of U. We don’t want to check only
the first diagnosis rather we want to check all diagnosis to see if it has a status of U. **For Each** can also be
used if you want to check if a procedure code has a date of service and/or provider attached. We don’t
want to just check the first procedure code for the date of service, we want to check each of them.

To use this field, first select **For Each** before defining a field. The system will open another drop-down
field to the right of **For Each** to indicate where you want to create the rule. There are only a handful of
fields the **For Each** field make sense for: charges, CPT codes, diagnosis codes, procedures, pending
reasons, and physicians.

Once you have selected a fields, you need to define the field you are looking for.
Example: Place an error reminding the coder to add the POA status on any diagnosis code that has a U
Click on **For Each**, then select diagnosis codes. Select POA from the field drop-down menu which will
allow you to review operators. For this example, use the operator of Equals. Once you select the
operator of Equals, then you have a field to fill in the value, which would e be “U” in this example.

![](image-504.jpg)

Then, because it makes sense to direct the coder to where the diagnosis code was validated or added,
we can then select Navigate to document code and it will take the end user back to the documentation
so they can review and assign the POA status appropriately.

### Adding fields to a rule

You can add fields to the rule to tell the user exactly what POA is triggering this rule so they don’t have
to look through all of the codes to determine which one has a U status.

You can inject a field within the rule that will be displayed for the end-user. Do this by putting the field
name in braces exactly like this {Code}. When the rule fires for the end-user, it will display the code with
the issue. If there are multiple, use the For Each
field to see each of the codes that are the issue as
an individual rule.

![](image-506.jpg)

### Navigate To

Once you have defined your rule, you will want to decide if it makes sense to take the end user
somewhere in the software to correct the issue based on the rule created. In the example of a discharge
disposition, it does make sense to direct the user to go to the account information
page as that is where they would likely change the disposition. Under where you
selected the level, there is a field for

![](image-505.jpg)

**Navigate** to (these are placed within the patient chart, under the navigation pane).

- **None** – Will not take the user anywhere if they click on the error/warning.
- **Charges** – Will take the user to the charges viewer.
- **Account Info** – Will take the user to the account information viewer.
- **Document Code** – Will take the user to where the code was validated/added.
- **Physicians & Queries** – Will take the user to the Physicians & Queries viewer.

### Pending Reason

![](image-508.jpg)

This field will have a dropdown with all available pending reasons.
If a rule is triggered on an account and it has a pending reason
attached, then the pending reason will be added and the user will
be able to see the number of the rule. Pending reasons that have a
physician or date requirement will NOT be available in this list. The
only way to remove a pending reason that was added by a rule is
to have that rule cleared

### Saving your Rule

Once you’ve completed adding criteria for your validation rule
remember to click on Save Rules in the top right-hand corner. It is
recommended that you test your validation rule by opening a chart that
fits the criteria of your validation rule

![](image-507.jpg)
