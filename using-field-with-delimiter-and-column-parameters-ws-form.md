# Using #field With Delimiter and Column Parameters - WS Form

> **Source**: [https://wsform.com/knowledgebase/using-field-with-delimiter-and-column-parameters/](https://wsform.com/knowledgebase/using-field-with-delimiter-and-column-parameters/)


The #field variable takes the following parameters:

#field(field_id, delimiter, column)

The column parameter is compatible with select, checkbox and radio fields.

Example: #field(123, ",", "Width")

In order to the use the column parameter the Value column mapping must contain unique values. For Select fields, any AJAX settings should be disabled to ensure option values are always present.

## Demo

This demo uses a checkbox field that has the following data grid:

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13687)
## Column Mapping

When using the column parameter of the #field variable, you must ensure the column mapped to Values contains unique values.

## Examples

Example
Description

`#text(#field(123))`
Dynamically returns the value of field ID 123 and update it if field ID 123 changes.

`#text(#field(123, "/"))`
Dynamically returns the value of field ID 123, separating multiple values with the / character and update it if field ID 123 changes.

`#text(#field(123, "/", "Width"))`
Returns the value found in the Width column of field ID 123, separating multiple values with the / character.

`#text(#field(123, "/", 2))`
Dynamically returns the value found in column index 2 (third column) of field ID 123, separating multiple values with the / character and update it if field ID 123 changes.

## Using #calc with Multiple Columns

You can use the #calc variable with #field variables containing the column parameter.

For example: #calc(#field(123, ",", "Width") * #field(123, ",", "Length"))

Note how the delimiter parameter is simply set to its default value "," and is essentially ignored in this example because the radio field only returns one value (row).

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13688)
