# Using RegEx Pattern Attributes on Field Inputs - WS Form

> **Source**: [https://wsform.com/knowledgebase/using-regex-pattern-attributes-on-field-inputs/](https://wsform.com/knowledgebase/using-regex-pattern-attributes-on-field-inputs/)


The pattern attribute in HTML form inputs is used to define a regular expression (regex) that the input field’s value must match for the form to be submitted successfully. This attribute is particularly useful for validating the format of user input directly in the browser, without needing to rely on server-side validation.

The pattern attribute can be applied to several field types, such as Text, Date/Time, Email, and Phone. When a user enters data that doesn’t conform to the specified regex, the browser will block the submission of the form and WS Form will show invalid feedback against that field.

Learn more: mdn web docs: HTML attribute: pattern

## How To Set The Pattern Attribute in WS Form

In WS Form, the Pattern setting sets the pattern attribute on form inputs. You can find this setting in the Advanced tab in the Restriction section.

## Example Regular Expressions

The form below demonstrates the use of the Pattern attribute setting found in the Advanced tab of form input fields.

You can enter a value into any input to test the regular expression.

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13768)
