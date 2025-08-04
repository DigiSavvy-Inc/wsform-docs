# Make Add-On - WS Form

> **Source**: [https://wsform.com/knowledgebase/make/](https://wsform.com/knowledgebase/make/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons- Make Add-On- Airtable Add-On- Google Sheets Add-On- AI- CRM- Cloud Storage- Communication- Databases- Email Marketing- Gallery- Hosting- Integration- PDF- Payment Gateways- Spam- Spreadsheets- Support Platforms- WooCommerce- WordPress Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials

Search

# Make Add-OnPRO

This knowledge base article relates to the WS Form Make add-on.
Included with the Freelance & Agency editions or buy separately for the personal edition.

The Make WS Form add-on allows you to integrate form submissions with thousands of apps. Make was formerly called Integromat.

## Installation

The WS Form Make plugin is installed in the same way as installing the WS Form PRO plugin.

Once installed you will need to activate the license for the plugin. When you purchase the Make plugin, you will be given a license key. If you have lost your license key(s), click here.

To activate your license key:

If your license key fails to activate, please ensure you are using the correct license key and not your WS Form PRO license key.

Note: You will require one published form and at least one submission in order to create a Make scenario.

Note: The WordPress REST API must be enabled and accessible to Make in order for this add-on to work. Make pulls data from WS Form and therefore it must have access to your website.

### Adding the WS Form Make App

### Creating a Scenario

To create a WS Form scenario:

## Fields

In addition to your form fields, the following submission fields are made available to Make for use in filters or mappings:

Identifier
Name
Description

`id`
ID
A unique identifier for the record. If a form is saved, this will be prefixed with `-<count_submit>` where `count_submit` is a number representing the number of times the form has been saved. This ensures zaps are re-assessed when a save occurs.

`submit_id`
Submission ID
The ID of the WS Form submission.

`form_id`
Form ID
The ID of the WS Form form.

`hash`
Hash
The hash (session ID) of the WS Form submission.

`duration`
Duration
The time it took in seconds from the initial form render to the last save or submit.

`count_submit`
Count
The number of times the form was saved or submitted.

`status`
Status
The status of the submission. `draft` represents an In Progress (saved) submission. `publish` represents a completed submission.

`preview`
Preview
A true or false value indicating if the form was saved or submitted in preview mode.

`spam`
Spam Level
A true or false value indicating if the form was saved or submitted in preview mode (Blank if no spam level available).

`date_added`
Date Added
The date / time the submission was created.

`date_updated`
Date Updated
The date / time the submission was updated.

`date_expire`
Date Expires
The date / time the submission will be purged (Blank for no expiry).

`admin_url`
Admin URL
The URL to view the submission in the WordPress admin.

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

