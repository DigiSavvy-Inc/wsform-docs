# Using #field With Delimiter and Column Parameters - WS Form

> **Source**: [https://wsform.com/knowledgebase/using-field-with-delimiter-and-column-parameters/](https://wsform.com/knowledgebase/using-field-with-delimiter-and-column-parameters/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields-- How To Make Checkboxes Required-- Data Sources: Google Sheets-- Create a Link in a Checkbox or Radio Label-- Data Grid Column Mapping-- Using #field With Delimiter and Column Parameters-- How To Add Tooltips to Checkboxes and Radios-- Data Grids-- Style Checkboxes-- Data Sources-- Populate Select, Checkbox and Radio Fields Using PHP-- Create Select, Checkbox, and Radio Cascading Lookups-- Show Select, Checkbox and Radio Labels in Emails-- Extract Select, Checkbox & Radio Labels-- Display Checkboxes or Radios in Columns- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Using #field With Delimiter and Column ParametersPRO

The #field variable takes the following parameters:

#field(field_id, delimiter, column)

The column parameter is compatible with select, checkbox and radio fields.

Example: #field(123, ",", "Width")

In order to the use the column parameter the Value column mapping must contain unique values. For Select fields, any AJAX settings should be disabled to ensure option values are always present.

## Demo

This demo uses a checkbox field that has the following data grid:

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13687)
## Column Mapping

When using the column parameter of the #field variable, you must ensure the column mapped to Values contains unique values.

## Examples

Example
Description

`#text(#field(123))`
Dynamically returns the value of field ID 123 and update it if field ID 123 changes.

`#text(#field(123, "/"))`
Dynamically returns the value of field ID 123, separating multiple values with the / character and update it if field ID 123 changes.

`#text(#field(123, "/", "Width"))`
Returns the value found in the Width column of field ID 123, separating multiple values with the / character.

`#text(#field(123, "/", 2))`
Dynamically returns the value found in column index 2 (third column) of field ID 123, separating multiple values with the / character and update it if field ID 123 changes.

## Using #calc with Multiple Columns

You can use the #calc variable with #field variables containing the column parameter.

For example: #calc(#field(123, ",", "Width") * #field(123, ",", "Length"))

Note how the delimiter parameter is simply set to its default value "," and is essentially ignored in this example because the radio field only returns one value (row).

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13688)

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

