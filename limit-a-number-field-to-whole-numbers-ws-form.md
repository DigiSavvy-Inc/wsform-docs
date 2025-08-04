# Limit a Number Field to Whole Numbers - WS Form

> **Source**: [https://wsform.com/knowledgebase/limit-a-number-field-to-whole-numbers/](https://wsform.com/knowledgebase/limit-a-number-field-to-whole-numbers/)


HTML number fields enable a user to enter any floating point number. Number fields have a variety of validation features such as min, max and step but these are only assessed when the form is submitted. Therefore you could set a step of 0 (which means no decimal places) but the user could still enter ‘1234.56’ and that won’t be trapped until the form is submitted.

A trick to getting a number field to only allow the entry of a whole number is as follows.

## Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13666)
## Tutorial

First, edit the number field by clicking the settings icon.

Next click on the Advanced tab in the settings sidebar and then scroll down to ‘Custom Attributes’.

Tip: Click the expand  icon (top right) to make the sidebar the full width of the page.

Click the add  icon to add a new custom attribute.

In the ‘Name’ column enter:

onkeypress

In the ‘Value’ column enter:

```
return (event.charCode == 8 || event.charCode == 0 || event.charCode == 13) ? null : (event.charCode >= 48 && event.charCode <= 57)
```

The finished custom attribute will look like this:

Then click Save at the bottom of the sidebar.

You should now find that the number field only allows a whole number to be entered.

The custom attributes setting allows you to add additional attributes to any field. In this case, it adds an onkeypress attribute to the field which checks the charCode of the keypress. If the keypress is a numeric character, it is added to the field, otherwise the character is discarded.
