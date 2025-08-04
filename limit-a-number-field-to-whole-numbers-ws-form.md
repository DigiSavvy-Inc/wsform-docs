# Limit a Number Field to Whole Numbers - WS Form

> **Source**: [https://wsform.com/knowledgebase/limit-a-number-field-to-whole-numbers/](https://wsform.com/knowledgebase/limit-a-number-field-to-whole-numbers/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings-- Using RegEx Pattern Attributes on Field Inputs-- How Hidden Fields Work-- How to Add Help Text to Forms-- Customize the Visual Editor Toolbar-- Limit a Number Field to Whole Numbers-- Translate Forms-- Create Floating Inside Field Labels With CSS-- Create a Field Prefix or Suffix-- Change Required Field Indicators-- Find the ID of a Field- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Limit a Number Field to Whole Numbers

HTML number fields enable a user to enter any floating point number. Number fields have a variety of validation features such as min, max and step but these are only assessed when the form is submitted. Therefore you could set a step of 0 (which means no decimal places) but the user could still enter ‘1234.56’ and that won’t be trapped until the form is submitted.

A trick to getting a number field to only allow the entry of a whole number is as follows.

## Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13666)
## Tutorial

First, edit the number field by clicking the settings icon.

Next click on the Advanced tab in the settings sidebar and then scroll down to ‘Custom Attributes’.

Tip: Click the expand  icon (top right) to make the sidebar the full width of the page.

Click the add  icon to add a new custom attribute.

In the ‘Name’ column enter:

onkeypress

In the ‘Value’ column enter:

```
return (event.charCode == 8 || event.charCode == 0 || event.charCode == 13) ? null : (event.charCode >= 48 && event.charCode <= 57)
```

The finished custom attribute will look like this:

Then click Save at the bottom of the sidebar.

You should now find that the number field only allows a whole number to be entered.

The custom attributes setting allows you to add additional attributes to any field. In this case, it adds an onkeypress attribute to the field which checks the charCode of the keypress. If the keypress is a numeric character, it is added to the field, otherwise the character is discarded.

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

