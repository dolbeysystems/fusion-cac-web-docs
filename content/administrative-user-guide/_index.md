+++
title = 'Administrative'
weight = 22
+++


## Chat Room

A chat room feature is available in most administrative tools, including User Management, Workflow Management, Validation Management, Query Designer, and Worksheet Designer. This feature allows users to communicate in real-time while working within these tools.

![Chat Room](ChatRoom.png)

The chat room is only active when multiple users are simultaneously accessing one of the administrative tools to ensure that changes are not lost when multiple users are working in the same tool. When two users are in the same tool and one saves data, the other user will see a red button indicating that changes are out of sync. Clicking the button will refresh the page with the other user's changes.

![Changes out of Sync](OutOfSync.png)

>[!note]
>Please note that chat history resets upon logging off.

## Inactivity Timeout

A configurable "inactivity reason" prompt can be displayed upon login, if the user has been logged out for a specified amount of time. 

![Inactivity Reason Prompt](InactivityReason.png)

If the user attempts to log in after having logged out between the minimum and maximum minutes, the user must record an "inactivity reason". There is a default set of dropdown options for the reason, which can be customized in Mapping Configuration. 

![Inactivity Mapping Table](InactivityReasonsMapping.png)


Additionally, Role Management contains an option to exclude user roles from being prompted upon login.

![Exclude from Inactivity Prompt](ExcludeFromPrompt.png)

When enabled, this functionality allows management to track why users were idle during the day. The User Audit Trail report shows the inactivity reason that was selected. 

Please contact CAC Support (cacsupport@dolbey.com) to have the inactivity timeout enabeled. 




{{% children depth=999 %}}