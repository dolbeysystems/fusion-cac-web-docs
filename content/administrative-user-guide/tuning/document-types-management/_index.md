+++
title = 'Document Types Management'
weight = 31
+++

## Document Type Management

![Document Types Management](DocTypesManagement.png)

### Filing Documents

To file documents:

- Open Document Type Management
- Sort on documents by clicking on the group name to display the documents currently not in a folder. Choose the documents that need to be filed
- Change the friendly name by double-clicking on the name and replacing it with another name **using a naming convention that new users will understand**

![Filing a Document](NewSort.png)

### Engine Handling

Engine Handling is set up after the documents have a friendly name. This set-up basically instructs the code suggesting engine what to do when it encounters the document. 

Depending on how the organization is configured, there may be a drop-down menu to select the type of handling the document receives. 

![]()

On the other hand, there can be two different fields - one called inclusion and one
called exclusion - that allows us to include or exclude certain code sets starting with a prefix.
For example, on a document called Newborn History and Physical, the engine should exclude O codes so that if the
documentation has mother documentation, the engine doesn’t get confused and try to suggest O codes
on a newborn chart.

![](image-570.jpg)

For further assistance setting up Engine Handling, contact the Tuning Team at results@dolbey.com
Once engine handling is set up, it’s now time to place the document into a folder by double-clicking the
empty space in the Group Name column and type in the name of the folder where the document should
be filed. If you’re not familiar with the folder structure that is already set up, go to the top of the group
name, hover over the column, and click on the three dashes to see all the group names that are
available.

### Cancels Pending Reason

“Cancels Pending Reason” is a field In Document Types Management, which can be used to cancel an
existing pending reason. By selecting this, the existing pending reason will remove the pending reason
and re-trigger workflow. If you don’t want to delete this because the original pending reason is used for
DNFC reporting and/or a user needs to know the original reason for pending, you don’t need to delete it.
Instead, there is another option to Add a Pending reason.

![](image-569.jpg)

### Add a Pending Reason

In Document Types Management, a field "Adds Pending Reason" now can contain the name of a
pending reason to add when the document type is added to an account with matching pending reasons
from the "Cancels Pending Reason" field.

Two important facts about the "Adds Pending Reason" field:

1. The presence of an "Adds Pending Reason" value overrides the functionality that cancels
pending reasons from the "Cancels Pending Reason" field. In other words, when a pending
reason exists on the account that matches the "Cancels Pending Reason" field, the pending
reason is not deleted when there is an "Adds Pending Reason" value present. The functionality is
designed to be one or the other – not both – but the account must have one of the "Cancels
Pending Reasons" to add the pending reason.
2. The "Adds Pending Reason" is intentionally free-form text. It can contain a value that is not
listed in the Pending Reasons mapping so that users cannot select it. Whatever value is recorded
in this field will be the pending reason name that the Script Engine will automatically add to the
account.

![](image-571.jpg)

> [!note] Enabling "Adds Pending Reason"
If you wish to use this functionality, you must perform a one-time step to add the **Adds Pending
Reason** column to the Document Types Management grid. This is done by clicking on the three dashes
in the column header column, clicking on the column list tab, and checking **Adds Pending Reason**.
In the grid, you double click in the field to edit the **Adds Pending Reason** field, but you must press
Enter to "commit" that value before saving (just like all other text fields in this grid). The "Mass Edit"
dialog in Document Types Management also supports the entry of the **Adds Pending Reason** field

### Caution Coding

Caution codea are suggested by the system but cannot be assigned by a coder because of the document type.

If a document is configured in Document Types management to be a caution code document it means the coder should not code from that but, be aware that the verbiage exists as it may
result in a possible query. For example, if a nurse indicates the patient was being treated for respiratory
failure but, the provider never mentioned it the caution code will help to ensure you aren’t missing
anything.

In Document Types Management, change the "Caution Coding" field of the Document Type to "All
Patient Types". Save your change, then load the account and that document. A "caution coding"
document is a document from which the user cannot assign codes, so the code suggestions within the
document have a "caution" background instead of the usual lavender background. The Unassigned Code
tree now displays the same caution background for those codes, and the right-click menu on those
codes prevent assigning or changing the caution code.

![](image-577.jpg)

In the Unassigned Codes pane, any code attached to that document will show in a yellow background,
and will not have the option to assign on the right click menu.

![](image-578.jpg)