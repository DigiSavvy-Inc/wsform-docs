# The Campaign Monitor Add-On

> **Source**: [https://wsform.com/knowledgebase/campaign-monitor/](https://wsform.com/knowledgebase/campaign-monitor/)


This knowledge base article relates to the WS Form Campaign Monitor add-on.
Included with the Freelance & Agency editions or buy separately for the personal edition.

The Campaign Monitor add-on lets you push new subscribers using an action, pull subscriber data using the WS Form autocomplete feature, and create new forms from your lists in a single click on the add form page.

## Installation

The Campaign Monitor plugin is installed in the same way as installing the WS Form PRO plugin.

Once installed you will need to activate the license for the plugin. When you purchase the Campaign Monitor plugin, you will be given a license key. If you have lost your license key(s), click here.

To activate your license key:

If your license key fails to activate, please ensure you are using the correct license key and not your WS Form PRO license key.

## Connecting to Campaign Monitor

In order to use the add-on, you need to connect it to Campaign Monitor. Connecting is easy!

If you do not have a Campaign Monitor account, you can create a new account here.

## Creating a Form for Campaign Monitor

### Automatically

WS Form can create a form for any of our Campaign Monitor lists in a single click. This process not only creates a form but also fully configures WS Form so that the form is ready to use immediately.

To create a Campaign Monitor form in WS Form:

That’s it! Your form will be created and is ready to add to your website.

If your list does not appear, click the refresh icon in the Campaign Monitor tab.

### Manually

It is also possible to use any form created in WS Form and add an action so that it is submitted to Campaign Monitor when a user saves or submits their form.

To add a Campaign Monitor action:

As with all sidebars in WS Form, click to the Save button at the bottom to save your changes, or click Cancel to disregard your changes.

The Campaign Monitor action settings are as follows:

#### When Should This Action Run?

You can choose to run the Campaign Monitor action when the form is saved, submitted, or both.

#### Campaign Monitor List

Choose the Campaign Monitor List you would like subscribers to be added, updated or removed from. If you have created a new list since viewing this screen, you can click the refresh icon to retrieve the new list.

#### Method

Select the Campaign Monitor method you would like to call when the action runs. Choose from:

#### Opt-In Field

Use this setting to select which of your fields to act as the opt-in field. We recommend adding a checkbox field with a single checkbox. It is always recommended that you have an unchecked opt-in checkbox on your forms to ensure you comply with GDPR requirements.

#### Name Mask

The name mask determines how the name field for a subscriber is determined. We recommend using text field variable for this setting. For example:

#field(1)

#### Field Mapping

Field mapping tells WS Form which of your form fields relate to the corresponding fields in Campaign Monitor. For example you would want to map your Email field to the Email field in Campaign Monitor.

To map a field:

## Populate Forms Using Campaign Monitor

As well as pushing form data with this add-on, you can also retrieve subscriber data and populate the fields on your form.

This feature is only available if a website visitor is signed in and their WordPress email address matches the email address of a subscriber in Campaign Monitor.

To enable this feature:

Note that if you created your form using a Campaign Monitor template the field mappings will automatically be created for you. You can also map tags (Campaign Monitor interests).
