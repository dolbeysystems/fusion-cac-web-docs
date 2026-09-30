<!--
Shared snippet: filter operator tables.
Shown on BOTH Account Search (Operators section) and Workflow Management (Workflow Operators section)
Edit here once; both pages update.
Shortcodes such as button or rawhtml do not work inside a snippet; use plain Markdown or HTML.
-->

**Matching a Single Value**

| Operator             | Description | Example |
| -------------------- | ----------- | ------- |
| Equals               | The field must match your value exactly (nothing more, nothing less). Uppercase/lowercase matters. |Setting Equals → "Inpatient" will only match accounts where the field says exactly "Inpatient," not "inpatient" or "Inpatient Chart."|
|Not Equal             | The field must not match your value. Uppercase/lowercase matters. |Not Equal → "Inpatient" matches every account except those marked exactly "Inpatient."|

**Comparing Numbers or Amounts**

| Operator             | Description | Example |
| -------------------- | ----------- | ------- |
| < (less than)        | The field's value must be smaller than the number you enter.|< 5 matches 4, 3, 0, not 5 itself. |
| > (greater than)     | The field's value must be larger than the number you enter.|> 5 matches 6, 7, 100, not 5 itself. |
| <= (less than or equal to) | The field's value must be smaller than or the same as the number you enter. |<= 5 matches 5, 4, 3.|
| >= (greater than or equal to) | The field's value must be larger than or the same as the number you enter. |>= 5 matches 5, 6, 7.|

**Matching Against Several Possible Values**

| Operator             | Description | Example |
| -------------------- | ----------- | ------- |
| In List              | The field must exactly match one of the values you list (the whole field, not part of it). |In List → [Return to CDI, Return to Coding] matches an account only if the field's entire value is exactly one of those two phrases.|
| Not In List          | The field must not exactly match any of the values you list. |Not In List → [Return to CDI, Return to Coding] excludes accounts where the field is exactly one of those two phrases.|

**Searching Within Text**

| Operator             | Description | Example |
| -------------------- | ----------- | ------- |
| Starts With           | Matches if the field begins with the characters you enter. Useful for codes or document type prefixes.|Starts With → "I10" matches "I10.9," "I10.0," "I10-related note," etc.|
| Contains             | Matches if your word or phrase appears anywhere in the field, even if it's only part of a longer value, not the whole thing. |Contains → "Blue Cross" matches "Blue Cross of Ohio," "Anthem Blue Cross," or a note that simply mentions "Blue Cross" partway through.|
| Only Contains        | Matches only if every value in the field comes from your list; nothing extra is allowed. |If an account has codes A, B, and C, "Only Contains → [A, B, C]" matches. If the account also has code D, it does not match.|

**Checking Whether a Field Has Any Value**

| Operator             | Description | Example |
| -------------------- | ----------- | ------- |
| Exists               | Matches if the field has anything in it; it just can't be blank. No value needs to be entered for this operator. |Exists on "Discharge Date" matches any account that has a discharge date recorded, regardless of what that date is.|
| Does not Exist       | Matches if the field is blank. No value needs to be entered for this operator. |Does Not Exist on "Discharge Date" matches accounts with no discharge date yet (i.e., still admitted).|

**Working with Dates**

| Operator             | Description | Example |
| -------------------- | ----------- | ------- |
| More Than            | Only for date fields. Matches if the date is more than X days ago. You enter a number of days, not a calendar date, since this needs to stay relative to "today." |More Than → 30 (days ago) on Admit Date matches accounts admitted over a month ago.|
| Less Than            | Only for date fields. Matches if the date is less than X days ago. Again, you enter a number of days, not a calendar date. |Less Than → 7 (days ago) on Admit Date matches accounts admitted within the last week.|
| Later Than           | Only for date fields. Matches if the date is later than one specific, fixed calendar date you choose. |Later Than → 01/01/2026 matches any account dated after January 1, 2026.|
| Is On                | Matches an exact calendar date. Rarely used, since most searches and workflows need to stay relative to "today." |Is On → 03/15/2026 matches only accounts dated exactly March 15, 2026.|
| Weekday In           | Matches if the date falls on one of the specific days of the week you select. |Weekday In → [Saturday, Sunday] matches accounts admitted on a weekend.|
| Hour In Range        | Matches if the time (admit or discharge) falls within a range of hours you set. |Hour In Range → 8:00 AM–5:00 PM matches accounts admitted during standard business hours.|
| Hour In              | Matches if the time falls on one specific hour you select. |Hour In → 2:00 PM matches accounts admitted between 2:00–2:59 PM.|
| Last Month           | Matches records from the previous calendar month. In Workflow Management, this is mainly used for Audit workflows. |If today is any day in August, Last Month matches everything dated in July.|
| This Month           | Matches records from the current calendar month. In Workflow Management, this is mainly used for Audit workflows. |If today is any day in August, This Month matches everything dated in August.|

**Matching Against Multiple Values at Once (Lists Within a Field)**

| Operator             | Description | Example |
| -------------------- | ----------- | ------- |
| Includes Each Of     | The field must contain all of the values you list, but it's okay if it has other values too.|Includes Each Of → [A, B] matches an account with codes A, B, and C, because A and B are both present. It would not match an account with only A.|
| Includes Any Of      | The field must contain at least one of the values you list. | Includes Any Of → [A, B] matches an account with just A, just B, or both.|
| Does not Include     | This operator isn't available on its own. If you need "must not contain any of these values," use **Not In List** instead. |N/A|

>[!Note]Operator Values
>Unless an operator does not require a value, the value field must be filled in to save the criteria.
