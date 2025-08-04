# Send Email Action

> **Source**: [https://wsform.com/knowledgebase/send-email/](https://wsform.com/knowledgebase/send-email/)


Category

Select...
 Getting Started Accessibility Actions- Actions- Advanced- Basic-- Send Email Action-- Save Submission Action-- Show Message Action-- Redirect Action Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials

Search

# Send Email Action

The Send Email action lets you send any number of emails to recipients when a form is saved or submitted.

This action is fully configurable and allows you to:

* You can dynamically set these values with WS Form variables too. So you could even set one of these as the email address someone entered onto your form.

Tip: To ensure WS Form is fully compatible with WordPress, we use the standard wp_mail function to send emails. We recommend using an email gateway such as Amazon SES, MailGun, or SendGrid to send emails and using a WordPress plugin to add support for these gateways. You will then find that email sending is a lot more efficient than relying on raw emails being sent from your hosting provider.

## Adding This Action

To add a Send Email action:

As with all sidebars in WS Form, click the Save button at the bottom to save your changes, or click Cancel to disregard your changes.

The Send Email action settings are as follows:

### When Should This Action Run?

You can choose to send an email when the form is saved, submitted, or both.

### From Email Address

Enter the From email address in this field. You can either enter an email address directly or use a WS Form variable in this field. For more information about WS Form variables, click here.

This field defaults to #blog_admin_email which will enter the email address you have configured in the WordPress Settings > General page.

### From Display Name (optional)

You can enter a display name for your email for the from field. This will show the display name instead of the email address in most email clients.

You can either enter a name or use a WS Form variable in this field. For more information about WS Form variables, click here.

This field defaults to #blog_name which will enter the name of the website you have configured in the WordPress Settings > General page.

### To

You can add any number of To email addresses for the email. Typically this will be to you or perhaps to the website visitor to acknowledge their inquiry. To add a To email address:

You can enter straight text or use a WS Form variable in this field. For more information about WS Form variables, click here.

This field defaults to #blog_admin_email and#blog_name which will enter the email address and the name of your website you have configured in the WordPress Settings > General page.

Tip: Some email clients do not like emails that are sent to and from the same email address. We would recommend changing the from email address to something like do.not.reply@yourdomain.com to ensure these are different. Also some email gateways require you to register sender email addresses before you can use them. Ensure you have registered all from addresses if that is the case.

### Round Robin

The round robin feature is used to send notifications to each recipient in your To list according to the percentages you set in the Round Robin % column. To enable round robin, check this box. A third column will then appear in the To repeater above.

The Round Robin % column defaults to Auto. WS Form will automatically calculate a percentage for that row. For example, if you have two recipients, each recipient will receive 50% of the notifications if the column is set to Auto. If you enter a percentage, e.g. 25, that row will receive 25% of the notifications and the other Auto row will receive 75%.

The sum of the percentages entered for all the rows should not exceed 100.

### CC

The CC field lets you send a carbon copy of the email to recipients. Use the same method as adding values to the To field (see above) to complete this section. This field is optional.

### BCC

The BCC field lets you send a blind carbon copy of the email to recipients. Use the same method as adding values to the To field (see above) to complete this section. This field is optional. BCC recipients will receive a copy of the email, but other recipients will not see that they received it.

### Reply To Email Address

By default replies to an email are sent to the From email address. You can override this by entering an email address into this field.

For multiple reply to email address, separate email addresses with a comma.

You can enter straight text or use a WS Form variable in this field. For more information about WS Form variables, click here.

### Subject

Enter the subject line of your email here.

You can enter straight text or use a WS Form variable in this field. For more information about WS Form variables, click here.

This field defaults to #form_label which enters the label of your form as the subject line.

### Message

Enter the content of your email here.

You can enter straight text and also use WS Form variables in this field. For more information about WS Form variables, click here. There are various email-specific variables that can be used in this field.

This field defaults to:

#email_subject
#email_submission

This will add the subject of the email and the contents of the form submission to the email.

Some frequently used variables are as follows:

#### Email

Name / VariableAdditional InformationCharacter set`[#email_charset](https://wsform.com/knowledgebase/send-email/)`Returns the email character set. For more information about this variable, [click here](https://wsform.com/knowledgebase/send-email/).Content type`[#email_content_type](https://wsform.com/knowledgebase/send-email/)`Returns the email content type. For more information about this variable, [click here](https://wsform.com/knowledgebase/send-email/).E-Commerce Values`[#email_ecommerce](https://wsform.com/knowledgebase/introduction-e-commerce/)`Returns a list of the e-commerce transaction details such as total, transaction ID and status fields. For more information about this variable, [click here](https://wsform.com/knowledgebase/introduction-e-commerce/).Logo`[#email_logo](https://wsform.com/knowledgebase/send-email/)`Returns the email logo specified in WS Form Settings > Variables. For more information about this variable, [click here](https://wsform.com/knowledgebase/send-email/).Subject`[#email_subject](https://wsform.com/knowledgebase/send-email/)`Returns the email subject line. For more information about this variable, [click here](https://wsform.com/knowledgebase/send-email/).Submitted Fields`[#email_submission(tab_labels, section_labels, field_labels, blank_fields, static_fields)](https://wsform.com/knowledgebase/send-email/)`Returns a list of the fields captured during a submission. You can either use: `#email_submission` or provide additional parameters to toggle tab labels, section labels, blank fields and static fields (such as text or HTML areas of your form). Specify 'true' or 'false' for each parameter, for example: `#email_submission(true, true, false, true, true)` For more information about this variable, [click here](https://wsform.com/knowledgebase/send-email/).Tracking data`[#email_tracking](https://wsform.com/knowledgebase/send-email/)`Returns a list of all the enabled tracking data that was captured when the form was submitted. For more information about this variable, [click here](https://wsform.com/knowledgebase/send-email/).#### Tracking

Name / VariableAdditional InformationAgent`[#tracking_agent](https://wsform.com/knowledgebase/tracking/)`Stores the website visitors agent (browser type). For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).Duration`[#tracking_duration](https://wsform.com/knowledgebase/tracking/)`Stores the duration it took to complete the form in seconds. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).Location (By browser)`[#tracking_geo_location](https://wsform.com/knowledgebase/tracking/)`If a website visitors device supports geo location (GPS) this option will prompt and request permission for that data and store the latitude and longitude to a submission. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).URL Hash`[#tracking_hash](https://wsform.com/knowledgebase/tracking/)`Hash of the URL. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).Hostname`[#tracking_host](https://wsform.com/knowledgebase/tracking/)`Stores the server hostname. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).City (By IP)`[#tracking_ip_lookup_city](https://wsform.com/knowledgebase/tracking/)`If checked, WS Form will perform an IP lookup and obtain the city located closest to their approximate location. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).Country (By IP)`[#tracking_ip_lookup_country](https://wsform.com/knowledgebase/tracking/)`If checked, WS Form will perform an IP lookup and obtain the country located closest to their approximate location. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).Location (By IP)`[#tracking_ip_lookup_latlon](https://wsform.com/knowledgebase/tracking/)`This will obtain an approximate latitude and longitude of a website visitor by their IP address. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).Region (By IP)`[#tracking_ip_lookup_region](https://wsform.com/knowledgebase/tracking/)`If checked, WS Form will perform an IP lookup and obtain the region located closest to their approximate location. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).Time Zone (By IP)`[#tracking_ip_lookup_time_zone](https://wsform.com/knowledgebase/tracking/)`If checked, WS Form will perform an IP lookup and obtain the time zone closest to their approximate location. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).Operating System`[#tracking_os](https://wsform.com/knowledgebase/tracking/)`Stores the website visitors operating system. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).URL Pathname`[#tracking_pathname](https://wsform.com/knowledgebase/tracking/)`Pathname of the URL. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).URL Query String`[#tracking_query_string](https://wsform.com/knowledgebase/tracking/)`Query string of the URL. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).Referrer`[#tracking_referrer](https://wsform.com/knowledgebase/tracking/)`Stores the web page address a website visitor was on prior to completing the submitted form. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).Remote IP Address`[#tracking_remote_ip](https://wsform.com/knowledgebase/tracking/)`Stores the website visitors remote IP address, e.g. 123.45.67.89 For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).URL Full`[#tracking_url](https://wsform.com/knowledgebase/tracking/)`Full URL. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).UTM Campaign`[#tracking_utm_campaign](https://wsform.com/knowledgebase/tracking/)`This can be used to store the UTM (Urchin Tracking Module) campaign parameter. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).UTM Content`[#tracking_utm_content](https://wsform.com/knowledgebase/tracking/)`This can be used to store the UTM (Urchin Tracking Module) content parameter. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).UTM Medium`[#tracking_utm_medium](https://wsform.com/knowledgebase/tracking/)`This can be used to store the UTM (Urchin Tracking Module) medium parameter. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).UTM Source`[#tracking_utm_source](https://wsform.com/knowledgebase/tracking/)`This can be used to store the UTM (Urchin Tracking Module) source parameter. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).UTM Term`[#tracking_utm_term](https://wsform.com/knowledgebase/tracking/)`This can be used to store the UTM (Urchin Tracking Module) term parameter. For more information about this variable, [click here](https://wsform.com/knowledgebase/tracking/).
To view all available variables, click here.

### Message Editor

Use this setting to choose which type of editor to use for your message content. The available options are:

### Field Attachments

If you have file upload or signature fields in your form, you can attach them using this setting. To add a field attachment:

### Media Attachments

You can attach files from your media library to your email. To add a media attachment:

### Link to Files

If file uploads are included in the email submission, then enabling this checkbox will link the file names to the files.

### Wrap Messages in Header and Footer

This setting is checked by default. It wraps your message in a simple header and footer including some basic styling to make email sending quick and easy. If you want more control over your email content, you can uncheck this setting and the content of your message will sent without this wrapper.

### Clear Hidden Fields

When this setting is checked, WS Form will clear the value of any fields that are hidden on the form before they are processed by this action. This is useful if you only want to include completed fields a user could see at the time the form was submitted or saved. Note that fields that are of the hidden type are always included.

### Content Type

Choose Plain text or HTML for your email type. We recommend using HTML, which will enable you to better format your email and include images if you wish.

### Headers

You can use this setting to add custom headers to your email.

### Character Set

Enter the character set of the email here if you wish to change it.

You can enter straight text or use a WS Form variable in this field. For more information about WS Form variables, click here.

This field defaults to #blog_charset which enters the character set of your website.

### 

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

