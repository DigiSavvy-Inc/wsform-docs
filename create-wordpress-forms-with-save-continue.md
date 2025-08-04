# Create WordPress Forms With Save & Continue

> **Source**: [https://wsform.com/knowledgebase/save-continue/](https://wsform.com/knowledgebase/save-continue/)


The WS Form save & continue feature allows someone completing a form to save their progress and then continue the form (resume) later. Each submission record has a hidden anonymized value called a hash that is used to identify the submission. It is this hash that WS Form uses to retrieve the submission in order that the user can continue their submission.

WS Form has two save & continue methods:

The cookie method is silent and allows someone to continue their form by simply returning to the original  web page containing the form. This must be done on the same device.

The link method provides a link to the user, typically in an email, that they can click to continue their form. The advantage of this method is that they can click the link on any device at any time to recall their form submission.

You can also use a combination of the cookie and link method if you wish.

This tutorial explains how to set up both save methods. By default, new forms are configured to use the cookie method.

## The Save Button

They key to the WS Form save & continue feature is the Save button.

To enable the save feature you simply need to add a save button to your form. To do this, drag or click the save button from the toolbox to your form. You can place the save button anywhere you wish on your form. You can also add as many save buttons as you wish.

## The Cookie Method

New forms are configured to use the cookie save & continue method, so by adding the save button your form will already allow progress to be saved.

If you do not wish to have the cookie method enabled, you can disable it from the Global Settings page under the Advanced tab. Simply uncheck the Enable Save Cookie setting and click Save.

## The Link Method

An easy way of seeing a demo of the link method is to try the Save & Continue demo template. To do this:

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13627)
### Tutorial

The most common way of providing a user with their save & continue link is to send an email. This provides them with a point of reference with which to retrieve the link to continue their form. You could also use other actions to inform the user about their link, such as showing a message. In this tutorial, we’ll send the link to the user in an email.

#### Add an Email Field

To do this you will require an Email field on your form which will be used to provide the email address the notification will be sent to. We recommend putting this field as early in your form as possible.

To add the email field, simply click or drag an Email field to your form. Click on the Email field settings and set it to Required, then click Save & Close.

#### Add a Save Button

You will also need to add a Save button to your form. When this is clicked, WS Form will create an In Progress submission record.

To add the save field, simply click or drag a Save field to your form.

#### Create a Save Email Action

When a form is saved or submitted, one or more actions can run. Actions allow you to send emails, show a message, redirect to another page or even integrate with third party systems such as MailChimp, Slack or Zapier.

For this tutorial we are going to create a Save Email action that runs when the Save button is clicked. The email will contain the link to return back to the form so that it can be continued.

#### Disable the Cookie Method (Optional)

If you do not wish to have the cookie method enabled, you can disable it from the Global Settings page under the Advanced tab. Simply uncheck the Enable Save Cookie setting and click Save.

#### All Done!

Your form will now email the user completing the form each time they click the Save button. When they click the Continue your submission link it will take them back to their form as they left off.

## Variables

The following submission related variables can be used in actions.

Name / VariableAdditional InformationAdmin Link`[#submit_admin_link](https://wsform.com/knowledgebase/submissions/)`Link to submission in WordPress admin. For more information about this variable, [click here](https://wsform.com/knowledgebase/submissions/).Admin URL`[#submit_admin_url](https://wsform.com/knowledgebase/submissions/)`URL to submission in WordPress admin. For more information about this variable, [click here](https://wsform.com/knowledgebase/submissions/).Date Added`[#submit_date_added](https://wsform.com/knowledgebase/submissions/)`Returns the date and time of the submission according to the Date Format setting found in WordPress Settings > General. For more information about this variable, [click here](https://wsform.com/knowledgebase/submissions/).Date Added Custom`[#submit_date_added_custom("format")](https://wsform.com/knowledgebase/the-date-time-cheat-sheet/)`Returns the submit date and time in the specified format (PHP date format). For more information about this variable, [click here](https://wsform.com/knowledgebase/the-date-time-cheat-sheet/).Hash`[#submit_hash](https://wsform.com/knowledgebase/submissions/)`Returns the anonymized hash ID of the submission. For more information about this variable, [click here](https://wsform.com/knowledgebase/submissions/).ID`[#submit_id](https://wsform.com/knowledgebase/submissions/)`Returns the ID of the submission. For more information about this variable, [click here](https://wsform.com/knowledgebase/submissions/).Link`[#submit_link](https://wsform.com/knowledgebase/submissions/)`Link to recall form with submission loaded. Used in conjunction with the 'Save' button. For more information about this variable, [click here](https://wsform.com/knowledgebase/submissions/).Status`[#submit_status](https://wsform.com/knowledgebase/submissions/)`draft = In Progress, publish = Submitted, error = Error, spam = Spam, trash = Trash. For more information about this variable, [click here](https://wsform.com/knowledgebase/submissions/).Status Label`[#submit_status_label](https://wsform.com/knowledgebase/submissions/)`Returns a nice version of the submission status. For more information about this variable, [click here](https://wsform.com/knowledgebase/submissions/).URL`[#submit_url](https://wsform.com/knowledgebase/submissions/)`URL to recall form with submission loaded. Used in conjunction with the 'Save' button. For more information about this variable, [click here](https://wsform.com/knowledgebase/submissions/).User ID`[#submit_user_id](https://wsform.com/knowledgebase/submissions/)`Returns the ID of the user who completed the form. For more information about this variable, [click here](https://wsform.com/knowledgebase/submissions/).
