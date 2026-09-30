# Shared snippets

Each file in this folder is text that appears on more than one guide page.
Edit the text here once and every page that includes it updates.

| Snippet | Shown on |
|---|---|
| filter-operators.md | Account Search (Operators), Workflow Management (Workflow Operators) |
| designer-field-types.md | Query Designer, Worksheet Designer (Field Type) |
| designer-make-required.md | Query Designer, Worksheet Designer (Make Required) |
| designer-field-width.md | Query Designer, Worksheet Designer (Changing Field Width) |

A page shows a snippet with this line:

    {{% include "snippets/filter-operators.md" %}}

Notes:
- Screenshots named in a snippet are loaded from the folder of the page that shows it, so each page keeps its own screenshots under the same file name.
- Shortcodes such as `{{%button%}}` do not work inside a snippet. Use plain Markdown, or copy the HTML a shortcode produces (see the Edit Dropdown button in designer-field-types.md).
- This folder is not published as pages; readers only see the snippets inside the pages that include them.
