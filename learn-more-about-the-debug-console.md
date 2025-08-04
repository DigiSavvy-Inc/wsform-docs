# Learn More About the Debug Console

> **Source**: [https://wsform.com/knowledgebase/debug-console/](https://wsform.com/knowledgebase/debug-console/)


The debug console enables rapid testing and debugging of WordPress forms created with WS Form PRO when viewing a form.

It has a populate feature that automatically completes the fields on your form with appropriate data and, in most cases, will enable you to submit a test form in a single click!

The debug console features a wealth of information about your form, including performance data on how quickly it was rendered in the browser and how long a submission took on the server.

It is also the place to find useful logs and error messages about your form.

## Enabling the Debug Console

If you let us know you are a developer when you completed the welcome steps after installing the plugin, the debug tool will already be enabled.

If the debug tool is disabled and you want to enable it:

The Show always option is useful during the development of a website, but remember to switch this off prior to go live of a new website.

The Administrators only option is the best option to use if you want to see the debug tool whenever you are signed into WordPress as an administrator.

## Features of the Debug Console

### Resizing the Debug Console

The debug console can be resized by clicking and dragging the top bar. Adjust the debug console to your desired height and then release. You can also reset the height by clicking the + icon at the top right of the debug console, as well as minimizing the debug console by clicking the – icon.

### Instances

WS Form allows you to have multiple instances of the same or different forms on the same web page. This is useful if, for example, you want a newsletter form to appear in the header and footer of your website.

The instances of forms on a particular website are shown at the top of the debug console. Simply click an instance name to view information about that particular instance.

Each instance has its own independent set of tools and logs. To access the different features simply click the sub tabs found under the instance tabs. The different features are titled Tools, Log and Errors.

### Tools

The tools tab provides a variety of buttons along the top to help with testing a form instance as well as technical information about the form instance below that.

The tools are as follows:

#### Populate

By clicking the Populate button, WS Form will run through each of the fields on your form and attempt to complete them with random data that would qualify the form as validated. Each time you click the Populate button, the form will be re-populated with different data.

Note that some fields, such as the reCAPTCHA field, cannot be automatically populated and you will be required to complete them manually.

#### Submit

Click Submit to submit your form. WS Form will validate the form and, if validated, will submit your form and run your form actions.

#### Populate & Submit

As the title suggests, this populates the form with sample data and then submits the form in a single click.

#### Save

This performs the same action as the Save button.

#### Reload

This button will reload the form completely and set it up as if the page had just loaded.

#### Reset

This button resets the form fields to their initial state, including any default values.

#### Clear

This button will clear the form fields, regardless of their initial default values.

#### Identify

If you have a page with multiple instances of a form, clicking this will highlight the form on the page so that you can identify which form the debug instance tab relates to.

#### Edit

This will open the form builder for the form instance in a new browser tab.

#### Submissions

This will open the submissions page for the form instance in a new browser tab.

### Logs

The  logs tab provides useful information as events occur in your tab. Different types of log are color coded to make identifying certain types of log easier. You can consider anything in the Logs tab a successful event. The following types of event are logged here:

### Errors

Any server side errors that occur are captured here. This is useful for debugging errors such as email send issues or API connection issues with third parties such as MailChimp or ConstantContact if your key is incorrect.
