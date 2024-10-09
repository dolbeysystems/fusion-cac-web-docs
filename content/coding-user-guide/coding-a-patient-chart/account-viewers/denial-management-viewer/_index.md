+++
title = 'Denial Management Viewer'
weight = 160
+++

Denial management tracking involves monitoring cases where a patient's submitted billing chart is
rejected by the payer. Various reasons, such as medical necessity, code, or DRG assignment, could lead
to these denials. This tool is designed to comprehensively record the specifics related to denial
management and tracking. It is capable of documenting multiple denials for each chart, with the ability
to log and categorize them for the purpose of tracking, managing workflows, and generating reports.

![Denial Management Viewer](image-208.jpg)

If an account is submitted, a new "Denial Management" viewer will appear in the Navigation tree.
Clicking on this viewer presents a form with several fields to be filled in when an account has been
denied payment. If the desired the user can create validation rules on input.

Mutiple denial sheets can be created within the viewer, if applicable.o

![Denial Management](image-209.jpg)

Sheets can be removed from the account by clicking on the red X to the right of each denial heading. For
reporting within Account Search, a Denials drilldown is available. This drilldown only reports on the first
denial on the account.

Dropdown items have a default, but mappings with the following IDs can customize the dropdown
entries:

- DenialType
- DenialStatus
- DenialOutcome
- DenialAppealRoute
- DenialReason
- DenialCodeChangeNeeded
- DenialDRGChangeNeeded

![Denial Management](image-210.jpg)

All values are saved in a new separate "DenialManagement" object on the account. Each field (except
Comments) can be added to Grid Column Management for display in Account Search, these fields can
also be used in workflow if necessary.

![Denial Management](image-211.jpg)