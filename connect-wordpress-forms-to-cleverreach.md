# Connect WordPress Forms to CleverReach

> **Source**: [https://wsform.com/knowledgebase/cleverreach/](https://wsform.com/knowledgebase/cleverreach/)


This knowledge base article relates to the WS Form CleverReach add-on.
Included with the Agency edition or buy separately for other editions.

The CleverReach add-on lets you push new subscribers using an action, pull subscriber data using the WS Form autocomplete feature, and create new forms from your lists in a single click on the add form page.

## Installation

The CleverReach plugin is installed in the same way as installing the WS Form PRO plugin.

Once installed you will need to activate the license for the plugin. When you purchase the CleverReach plugin, you will be given a license key. If you have lost your license key(s), click here.

To activate your license key:

If your license key fails to activate, please ensure you are using the correct license key and not your WS Form PRO license key.

## Connecting to CleverReach

In order to use the add-on, you need to connect it to CleverReach. Connecting is easy!

If you do not have a CleverReach account, you can create a new account here.

## Creating a Form for CleverReach

### Automatically

WS Form can create a form for any of our CleverReach lists in a single click. This process not only creates a form but also fully configures WS Form so that the form is ready to use immediately.

To create a CleverReach form in WS Form:

That’s it! Your form will be created and is ready to add to your website.

If your list does not appear, click the refresh icon in the CleverReach tab.

### Manually

It is also possible to use any form created in WS Form and add an action so that it is submitted to CleverReach when a user saves or submits their form.

To add a CleverReach action:

As with all sidebars in WS Form, click to the Save button at the bottom to save your changes, or click Cancel to disregard your changes.

The CleverReach action settings are as follows:

#### When Should This Action Run?

You can choose to run the CleverReach action when the form is saved, submitted, or both.

#### CleverReach List

Choose the CleverReach List you would like subscribers to be added, updated or removed from. If you have created a new list since viewing this screen, you can click the refresh icon to retrieve the new list.

#### Method

Select the CleverReach method you would like to call when the action runs. Choose from:

#### Opt-In Field

Use this setting to select which of your fields to act as the opt-in field. We recommend adding a checkbox field with a single checkbox. It is always recommended that you have an unchecked opt-in checkbox on your forms to ensure you comply with GDPR requirements.

#### Double Opt-In

When checked, a double opt-in email will be sent to the recipient to confirm their subscriptions. This is useful for confirming a users email address as well as adhering to GDPR requirements.

You will also need to enter a CleverReach form ID to associate with the double opt-in with. Enter this in the Form ID setting, see below.

The following data will be sent to CleverReach as part of the double opt-in request:

We recommend informing your website users that this information will be shared with CleverReach as part of your privacy policy.

#### Form ID

If you choose double opt-in you will be required to enter a form ID to associate it with. Learn how to find your form ID.

#### Field Mapping

Field mapping tells WS Form which of your form fields relate to the corresponding fields in CleverReach. For example you would want to map your Email field to the Email field in CleverReach.

To map a field:

#### Custom Mapping

Custom mapping allows you to set a CleverReach field to any value you wish, including the use of WS Form variables. For example you might want to map a lead source (e.g. #blog_name) to the source field in CleverReach.

To add a custom mapping:

## Populate Forms Using CleverReach

As well as pushing form data with this add-on, you can also retrieve subscriber data and populate the fields on your form.

This feature is only available if a website visitor is signed in and their WordPress email address matches the email address of a subscriber in CleverReach.

To enable this feature:

Note that if you created your form using a CleverReach template the field mappings will automatically be created for you.
