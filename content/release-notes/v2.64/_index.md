+++
title = 'V2.64 (Oct 2026)'
+++

{{< release-notes-header version="V2.63.9680" date="07/06/26" >}}

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Ability for the end User to add Custom Subheadings in the CDI Alerts Editor

**CACTWO-6448** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Previously, subheadings such as Clinical Evidence, Laboratory Studies, and Vital Signs only appeared in the CDI Alerts Evidence Editor when evidence already existed under them, so users had no way to add a subheading that was missing. A new Add button has been added to the Evidence Editor that lets users select and add a subheading from a configured mapping list. Once added, the subheading can be dragged and dropped to resequence it, and evidence can be moved into it or added to it from an abstraction, discrete value, or medication. A new mapping with the ID "CdiAlertTopicSubHeaders" must be created in Mappings Configuration to populate the list of available subheadings.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Allow an end User to Manually add a CDI/Clinical Alert

**CACTWO-7161** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

Previously, a CDI/Clinical Alert topic could only appear on an account if the system automatically triggered it, so users had no way to open an alert for a topic that hadn't yet been flagged. Users can now manually add a new CDI/Clinical Alert from a preselected list of topics, using a mapping called "CdiAlertTopicHeaders." Manually added alerts will show ‘Manually added’ next to the name, along with a person and plus sign icon. All Alert Topics can no longer have their name edited in the Evidence Editor, the edit icon has been removed. If the system later automatically detects the same topic, it will still create its own active alert, since the automated version pulls in additional data and subcategory information. When closing a manually added alert, the "Insufficient clinical evidence," "Documentation already present," and "Other" outcome choices are not available, and a "Created by accident" choice is available only for manually added alerts, allowing users to remove ones opened in error.

> [!info] Additional Configuration Required
Please contact Support to enable this feature.

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add a Days from Discharge column to Account Search

**CACTWO-7533** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

A new "Days from Discharge" column has been added for use in Account Search. When added to a grid through Grid Column Maintenance, it displays the number of days between today and the account's discharge date. If an account has a blank discharge date, the value is treated as zero. This field is intended for display only.  This column is also supported in scheduled Account Search reports run through JSReport. 

<hr style="height:1px;border-width:0;color:gray;background-color:black">

### Add Charge and Abstraction Audit Columns to the Outpatient Coder Scorecard

**CACTWO-7989** **{{< rawhtml >}}<span style="color:#1F497D">(Enhancement)</span>{{< /rawhtml >}}**

The Audit Outpatient Coder Scorecard report has been updated to add up to six new columns. When the site configuration setting "ShowAuditCharges" is enabled, Charge Audit, Charge Errors, and Charge Accuracy Rate columns appear after the CPT related columns. Abstraction Audit, Abstraction Errors, and Abstraction Accuracy Rate columns always appear before the Training Topics column. These fields match the values shown in Audit Management for an outpatient account, and no Accuracy Rate value displays when the Audit count is zero.

