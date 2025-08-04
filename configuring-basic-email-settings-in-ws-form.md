# Configuring Basic Email Settings in WS Form

> **Source**: [https://wsform.com/knowledgebase/email-configuration/](https://wsform.com/knowledgebase/email-configuration/)


When a form is saved or submitted, WS Form can send one or more emails. You can change who an email is sent to by changing the To and From email addresses in the Send Email action settings.

To change your email settings:

This will show the following email settings:

## From

Each email has a From email address and a display name. You can change this to any email address and display name you wish. You will notice that by default it uses #blog_admin_email and #blog_name for these values. WS Form converts these variables  to the WordPress General Settings email address and site title respectively.

You could also set this to the value of one of your fields. For example, if you have an email field with an ID of 123, you could enter:

#field(123)

… into the From Email Address setting and WS Form will put the email address entered in the form as the from email address.

Some email platforms require that emails are sent from a registered / validated email address. In that case, we would recommend using the Reply To setting to enter the email address (or #field(123) variable) into. That way when you reply to an email acknowledgement it will prompt your email software to send the email to the Reply To address as opposed to the registered / validated email address.

## To

You can add any number of To email addresses for the email. Typically this will be to you or perhaps to the website visitor to acknowledge their inquiry. To add a To email address:

You can enter straight text or use a WS Form variable in this field. For more information about WS Form variables, click here.

By default, WS Form uses #blog_admin_email and#blog_name which will enter the email address and the name of your website you have configured in the WordPress Settings > General page.

Tip: Some email clients do not like emails that are sent to and from the same email address. We would recommend changing the from email address to something like do.not.reply@yourdomain.com to ensure these are different. Also some email gateways require you to register sender email addresses before you can use them. Ensure you have registered all from addresses if that is the case.

To learn more about the available settings for the Send Email action, click here.
