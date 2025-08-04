# The Text Area Field Option

> **Source**: [https://wsform.com/knowledgebase/textarea/](https://wsform.com/knowledgebase/textarea/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields- Advanced- Basic-- Text Field-- Number Field-- Phone Field-- Email Field-- URL Field-- Text Area Field- Buttons- Choice- Consent- Content- E-Commerce- Mapping- Repeatable Sections- Spam Protection Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials

Search

# Text Area Field

The Text Area field creates a text area input for your form. This field is useful for storing larger volumes of text or text requiring multiple lines. For example you might want to use this field to store an inquiry or customer feedback.

## Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13536)
## Adding a Text Area Field

To learn how to add, edit, clone, move, resize, offset, or delete a text area, please click here.

## Field Settings

To edit the settings for this field type, click the settings  icon on the field itself. Click the Save & Close or Save button to save your changes. If you do not want to save your changes, you can click the Cancel button or click any other form element to close the field settings sidebar.

## Basic

The basic tab contains settings that the majority of WS Form users will need to control a field. The settings are as follows:

### Label

This is the label shown alongside the field. As well as entering a label into this field, you can also double click the label of the field in the editor. You should enter an easy-to-understand label for your field, for example, First Name or Email.

### Show Label

If enabled the label will be shown on your form. If you do not want the label to appear for a particular field, uncheck this box.

### Type

There are three types you can choose for your text area:

### Required

If checked this field will be required when the website visitor completes your form. Failure to complete the field if this is checked will result in a validation message appearing under the field prompting the user to complete the field correctly.

Required fields are indicated on your website with the word Required being adding to the label of the field. This can be changed in the form settings advanced tab.

### Hidden

If checked the field will be hidden on the form. It can be shown again using conditional logic or your own JavaScript.

### Default Value

The default value setting is used to populate the field with some default content. Unlike the placeholder text, default values are stored when the form is saved or submitted. An example default value could be #user_first_name to insert a logged-in user’s first name into a First Name text field.

WS Form variables can be entered into this field.

### Placeholder

Field placeholders are used to place text in a field prior to the website visitor completing the field. The web browser then removes the placeholder text when text is entered into the field. Placeholder text is typically used to provide an example of what should be entered into that field, such as Describe yourself here… for a text area field. If this field is left blank, a placeholder will not be added to the field.

Placeholder text is not stored when the form is saved or submitted.

WS Form variables can be entered into this field.

### Help Text

The help text setting enables you to add smaller text under the field to assist the website visitor in completing that field.

As well as inserting plain text into this field, WS Form also provides extensive functionality for adding character and word count information. Click here to learn more about this functionality.

WS Form variables can be entered into this field.

### Auto Complete

Web browsers sometimes have features for helping users fill forms in, for example pre-filling the user’s address based on earlier user input. The autocomplete content attribute can be used to hint to the web browser how to, or indeed whether to, provide such a feature.

Use this setting if you would like to specify the value of the autocomplete attribute. Use the off option to prevent auto complete on the field.

### Visual Editor Settings

#### Toolbar

Choose from a Full or Compact toolbar. You can also customize the Visual Editor toolbar using WordPress filter hooks.

#### Enable Add Media Button

If checked, logged in users that have the upload_files capability will see the Add Media button on the visual editor.

#### Paste as Text

This setting is used to set the default state of the Paste as Text button. If is set to off by default.

### Prefix / Suffix

The prefix and suffix settings allow you to add a prefix box and/or suffix box to the field.

For example, you could add a unit of measure as a suffix, or an @ symbol as a prefix.

### Accessibility

#### ARIA Label

Accessible Rich Internet Applications (ARIA) defines ways to make web content and web applications more accessible to people with disabilities.

This setting enables you to define what text is made available to ARIA applications. This would, for example, provide a screen reader with specific text to read to someone with a disability.

The value of this setting defaults to your field label. If you would like to change this, enter a new value.

WS Form variables can be entered into this field.

### Exclusions

#### Exclude From Emails

By default, WS Form uses the #email_submission variable in email templates. This provides a simple way of displaying all of the submitted fields in emails. Sometimes there might be a need to exclude a field from an email, for example, you might want to not include some introductory copy on a form, or hide a field you’re using with conditional logic to show or hide an element.

To hide a field from emails, check this box.

Other WS Form add-ons may add exclusions in this section too, such as the WooCommerce add-on which allows you to exclude certain fields from the cart entries.

### Hidden Behavior

#### Always Include in Actions

This setting allows you to change the behavior of a field if the hidden setting is checked (See above), or if you set a field as hidden using conditional logic.

The normal behavior for a field that has been hidden is that it will not be included if an action has a Clear Hidden Fields setting enabled. For example, if you have a Send Email action, WS Form will not include fields that are hidden.

If this setting is checked, this field will always be included in actions if it is hidden.

## Advanced

The advanced tab contains additional form attribute settings that provide further control over how a field is rendered.

### Styles

Use the Styles settings to change the design of the text area field.

#### Label Position

There are five positions you can choose from for your label:

The default position will place the label set in the form settings advanced tab. For new forms this will be the Top positioning.

Note that when using some frameworks some label positions may not be available.

#### Label Width

If your label position is set to left or right, you can specify how wide the label will be. You can consider the overall width of the label and the field to be 12 columns (or whatever value is set in Form Settings). By default, labels are rendered at 3 columns wide (1/4 width), which means the field itself is 9 columns wide (3/4 width). You can change the width of the label using this setting.

To change the default width of all labels in your form:

1. Click the form settings  icon.
2. Click the Advanced tab.
3. Scroll down to Default Label Width and change the setting.
4. Click Save at the bottom.

#### Vertical Alignment

The vertical alignment option allows you to choose how this field will be vertically aligned in relation to fields in the same row. The options are:

### Classes

For developers WS Form allows you to add your own classes to fields.

#### Field Wrapper

The wrapper CSS class setting enables you to add a class (or classes) to a field wrapper. Field wrappers are sections of HTML added around a field to position them on the page. To add multiple classes, add a space between the class names.

#### Field

To add a class to the actual field element itself, enter a class (or classes) to this setting. To add multiple classes, add a space between the class names.

### Restrictions

Field restrictions enable you to define what can or cannot be entered into the field.

#### Disabled

If checked the field will be disabled, and it cannot be interacted with. You can re-enable a field dynamically by using conditional logic.

#### Read Only

If checked the field will be read only. Read-only forms provide a way of showing a value in a field without giving the website visitor the opportunity to change the value.

#### Minimum Characters

This is the minimum number of characters that need to be entered into the field in order for it to be valid. Leaving this blank will set the minimum character length to zero. If the field is submitted without the minimum character length defined, a validation error will appear under the field.

This number can be used in conjunction with the character count variables.

#### Maximum Characters

This is the maximum number of characters that can to be entered into the field in order for it to be valid. Leaving this blank will set the maximum character length to infinity. If the field is submitted with more than the maximum character length defined, a validation error will appear under the field. Typing will typically be limited to this number of characters.

This number can be used in conjunction with the character count variables.

#### Minimum Words

This is the minimum number of words that need to be entered into the field in order for it to be valid. Leaving this blank will set the minimum word length to zero. If the field is submitted without the minimum number of words defined, a validation error will appear under the field.

This number can be used in conjunction with the word count variables.

#### Maximum Words

This is the maximum number of words that can be entered into the field in order for it to be valid. Leaving this blank will set the maximum number of words to infinity. If the field is submitted with more than the maximum word length defined, a validation error will appear under the field.

This number can be used in conjunction with the word count variables.

#### Input Mask

Input masks help the user with the input by ensuring a predefined format. This can be useful for fields such as dates, numerics and phone numbers.

Example input masks can be selected by clicking the hamburger icon .

Learn more about input masks.

#### Columns

Use this setting to specify how many columns of characters the text area should have. This field should only be used if you are not styling the text area. By default WS Form will automatically apply a width to your text area, so you can leave this setting blank.

#### Rows

Use this setting to determine how many rows of text the text area should have. This field should only be used if you are not styling the text area. By default WS Form will automatically apply a width to your text area, so you can leave this setting blank.

#### User Status

Choose from one of the options to filter which user status can see this field:

If you choose Has User Role or Capability, additional settings will appear that enable you to choose one or more roles or capabilities.

### Transform

#### Transform

The transform setting can be used to force the case of the characters that are entered in the field. For example, choosing Uppercase will convert any lowercase characters entered into the field to uppercase. There are four transform options:

To see examples of how the transform options work, you can learn more by reading our Transform Strings knowledge base article.

### Duplication

#### No Submission Duplicates

When checked, WS Form will check to see if a duplicate submission exists containing the same value for this field. If found, the submission will not be allowed and a message shown to the user completing the form.

#### Within

This setting lets you specify how recently WS Form should check for duplicates. The available options are:

Setting
Description

All Time
Check all submissions

Past Hour
Check submissions in the past hour

Past Day
Check submissions in the past 24 hours

Current Day
Check submissions since midnight

Past Week
Check submissions in the past 7 days (168 hours)

Past Month
Check submissions in the past month

Past Year
Check submissions in the past year

### Duplication Message

If a duplicate is found, this message will show.

### Validation

#### Show Invalid Feedback

Invalid feedback text is shown when a form is saved or submitted and the field has not been completed according to the field settings you have configured. For example if the minimum character count is 10 and you enter 5 characters and then submit the form, the field will be deemed invalid. If this setting is checked, invalid feedback is shown under the field.

#### Invalid Feedback Text

WS Form automatically builds invalid feedback text for all of your fields. If no text is entered into this field, the value shown in the field in light gray text will be shown. If you would like to specify alternative invalid feedback text, you can do enter it within this setting.

WS Form variables can be entered into this field.

### Custom Attributes

This setting is used to add custom attributes to the HTML of this field, such as data-my-attribute="1234". You can add as many custom attributes as you need.

To add a custom attributes key value pair:

### Breakpoints

The breakpoint settings define the width of a field and also what the offset (how many columns from the left-hand side of the form or the previous field) of a field is for each breakpoint. For more information about the breakpoint settings and capabilities of WS Form, click here.

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

