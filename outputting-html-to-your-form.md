# Outputting HTML To Your Form

> **Source**: [https://wsform.com/knowledgebase/html/](https://wsform.com/knowledgebase/html/)


The HTML field is used to output raw HTML on your form. HTML is entered using the standard WordPress HTML editor.

## Adding an HTML Field

To learn how to add, edit, clone, move, resize, offset, or delete an HTML field, please click here.

## Field Settings

To edit the settings for this field type, click the settings  icon on the field itself. Click the Save & Close or Save button to save your changes. If you do not want to save your changes, you can click the Cancel button or click any other form element to close the field settings sidebar.

## Basic

The basic tab contains settings that the majority of WS Form users will need to control a field. The settings are as follows:

### Label

The label is used solely for identifying the text editor field when editing your form. The label is not shown to the website visitor.

### Hidden

If checked the field will be hidden on the form. It can be shown again using conditional logic or your own JavaScript.

### HTML

Enter the text you want to display into this WordPress visual editor.

### Exclusions

#### Exclude From Emails

By default, WS Form uses the #email_submission variable in email templates. This provides a simple way of displaying all of the submitted fields in emails. Sometimes there might be a need to exclude a field from an email, for example, you might want to not include some introductory copy on a form, or hide a field you’re using with conditional logic to show or hide an element.

To hide a field from emails, check this box.

Other WS Form add-ons may add exclusions in this section too, such as the WooCommerce add-on which allows you to exclude certain fields from the cart entries.

## Advanced

The advanced tab contains additional form attribute settings that provide further control over how a field is rendered.

### Styles

Use the Styles settings to change the design of the HTML field.

#### Vertical Alignment

The vertical alignment option allows you to choose how this field will be vertically aligned in relation to fields in the same row. The options are:

### Classes

For developers WS Form allows you to add your own classes to fields.

#### Field Wrapper

The wrapper CSS class setting enables you to add a class (or classes) to a field wrapper. Field wrappers are sections of HTML added around a field to position them on the page. To add multiple classes, add a space between the class names.

### Restrictions

#### User Status

Choose from one of the options to filter which user status can see this field:

If you choose Has User Role or Capability, additional settings will appear that enable you to choose one or more roles or capabilities.

### Breakpoints

The breakpoint settings define the width of a field and also what the offset (how many columns from the left-hand side of the form or the previous field) of a field is for each breakpoint. For more information about the breakpoint settings and capabilities of WS Form, click here.
