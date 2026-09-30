<!--
Shared snippet. Shown on both Query Designer and Worksheet Designer.
Edit here once; both pages update. Screenshots come from each page's own folder.
Shortcodes such as button or rawhtml do not work inside a snippet; use plain Markdown or HTML.
-->

#### Make Required

![Make Field Required](MakeRequired.png)

Fields can be made required by checking the box. Leaving the box unchecked means the field is optional and the template can be completed even if that field is left blank. 

When the template is added to a chart, required fields will have a light red background to indicate action must be taken. Additionally, the user will be presented with a red toast message if they try to save the chart without completing all required fields. The toast message will include the fields that need to be completed. 

![Required Field Red Background](RedRequiredField.png)

Clicking OK, will add the selected field to the template with the specified settings. A box will then display in the designer as a
placeholder for the selected field with the field name. The fields are not interactive from the designer. Once the template has been added to a chart, the field name will be replaced with instructions for the end user. 

![Fields From the Front End](FrontEndFields.png)
