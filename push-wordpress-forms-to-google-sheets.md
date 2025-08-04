# Push WordPress Forms To Google Sheets

> **Source**: [https://wsform.com/knowledgebase/google-sheets/](https://wsform.com/knowledgebase/google-sheets/)


This knowledge base article relates to the WS Form Google Sheets add-on.
Included with the Agency edition or buy separately for other editions.

The Google Sheets add-on lets you push form submissions as new rows in a Google Sheet and create new forms from your Google Sheets in a single click on the add form page.

Note: In order to use the Google Sheets add-on, you just need at least one sheet that has field headings in the columns of the first row. For example:

## Installation

The Google Sheets plugin is installed in the same way as installing the WS Form PRO plugin.

Once installed you will need to activate the license for the plugin. When you purchase the Google Sheets plugin, you will be given a license key. If you have lost your license key(s), click here.

To activate your license key:

If your license key fails to activate, please ensure you are using the correct license key and not your WS Form PRO license key.

## Connecting to Google Sheets

In order to use the add-on, you need to connect it to Google Sheets. Connecting is easy!

If you do not have a Google Sheets account, you can create a new account here.

## Creating a Form for Google Sheets

To add a Google Sheets action:

As with all sidebars in WS Form, click to the Save button at the bottom to save your changes, or click Cancel to disregard your changes.

The Google Sheets action settings are as follows:

#### When Should This Action Run?

You can choose to run the Google Sheets action when the form is saved, submitted, or both.

#### Spreadsheet ID

In this setting you will paste the spreadsheet ID. This can be obtained by looking at the URL of you sheet when in Google Sheets. For example, when editing your spreadsheet the URL might look like this:

https://docs.google.com/spreadsheets/d/1W3Gm5truVLbn0PZ8o6n2RrHCSwTMGsuP3cgNSYWcSqQ/edit?gid=0#gid=0

The spreadsheet ID is found after /d/ and /edit so in this example the spreadsheet ID would be:

1W3Gm5truVLbn0PZ8o6n2RrHCSwTMGsuP3cgNSYWcSqQ

Copy and paste this ID into the Spreadsheet ID setting. If the ID is entered correctly, WS Form will retrieve the available sheets and show them in the Sheet setting.

#### Sheet

Choose the Sheet within the Spreadsheet you want to push data to.

#### Opt-In Field

Use this setting to select which of your fields to act as the opt-in field. We recommend adding a checkbox field with a single checkbox. It is always recommended that you have an unchecked opt-in checkbox on your forms to ensure you comply with GDPR requirements.

#### Field Mapping

Field mapping tells WS Form which of your form fields relate to the corresponding column in Google Sheets. For example you would want to map your Email field to the Email column in Google Sheets.

To map a field:

#### Use URL for File Fields

If checked, mapped file and signature fields will be populated with URLs instead of the file name. This will be added as a =HYPERLINK formula if a single file is uploaded.

#### Custom Mapping

Custom mapping allows you to set a Google Sheets cell to any value you wish, including the use of WS Form variables. For example, you might want to map a lead source to a cell in your sheet.

To add a custom mapping:

#### Repeater to Rows

This setting allows you to push repeatable section rows as rows in the Google Sheet. Choose which repeater you want to use and WS Form will create a sheet row for each repeater row. Any fields outside of the repeater will be duplicated to each row.
