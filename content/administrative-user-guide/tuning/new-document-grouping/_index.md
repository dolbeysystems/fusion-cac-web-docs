+++
title = 'New Document Grouping'
weight = 32
+++

## New Document Grouping

New Document Grouping allows you to automatically put documents into folders. For example, if the
document name contains the word “consults” or “consultation”, you may want to file it within the
Consults folder and set the engine handling set to Do not Code Procedures.

By default, users with the Administrator role or the Tuning role have access to the "New Document
Grouping" page in the Tuning menu. In this page, users create a list of groups that should be created for
new document types:

- Group Name equals the name of an existing document group from Document Types
Management. Note that when one is selected, its Group Order automatically populates.
- Add equals click to add a new document group that is not in Document Types Management.
Users enter the document group name and its order number.
- Group Order = the sequence of the document grouping. Note this is copied from Document
Types Management but it can be edited, which would only affect new document types.
- Includes, Excludes, and NLP Handling = same functionality as in Document Types Management
- Documents = click to add string matching for new document types from the interface. Note that
there are four supported operators
- Sequencing buttons = new document types are processed through the groups in the order that
is displayed

### How to Create a New Automated Grouping

1. Click on + Add Group
2. Select the group name you are creating the automation for or click on the Add Button to
create a new group that doesn’t already exist.
![](image-572.jpg)

3. Select how you want the engine to handle these types of documents - you can either
have engine handling dropdown or use includes or excludes.

#### Engine Handling Drop Down

This drop down allows you to block certain code sets. But,if you need more targeted handling to
include or exclude certain codes, then consider using the includes or excludes method shown
below.

![](image-573.jpg)

#### Includes and Excludes

Using the includes or excludes allows you to override the settings and choose to either includeor
exclude certain code prefixes. The below figure shows that this group will only include codes
that begin with the prefix of A. To note you can not use both includes and excludes this is an
either or.

![](image-574.jpg)

4.  Once you have set the folder and the engine handling, then select the documents you
want to include in this group. Click on the edit button then select +Add. Then, choose
your operator. HINT: Contains will likely be the best choice. For example, if you want to
put all radiology documents into to a folder, you may consider that if it contains XR, NM,
MRA, MRI, US, CT, then those should go into the radiology folder. Use a comma to
separate multiple items. Click OK once complete.

![](image-575.png)

Once you have completed the new grouping, select Save All in the top right corner.

![](image-576.jpg)