# Use Fields To Change Repeatable Section Row Counts - WS Form

> **Source**: [https://wsform.com/knowledgebase/how-to-use-fields-to-change-repeatable-section-row-counts/](https://wsform.com/knowledgebase/how-to-use-fields-to-change-repeatable-section-row-counts/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Use Fields To Change Repeatable Section Row CountsPRO

WS Form can set the number of rows in a repeatable section by using the value from another field. In the example below we are using the numeric value of a range slider to set the number of rows in the repeatable section. Instead of a range slider, this could be any other field that can accommodate a numeric value.

## Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13577)
## Conditional Logic: Set Row Count

The demo above is achieved by using conditional logic. When selecting a section in a THEN or ELSE statement, you can select Set row count as an option. Note that this will only work with the section is set up as repeatable. We are using #field(field_id) to get the value of the range slider and using that to set the row count of the repeatable section People.

The conditional logic used in this demo to change the row count to match the range slider value is as follows:

## Variable: #section_row_count(section_id)

You can also use the variable #section_row_count(section_id) to obtain the current number of rows in a repeatable section. You would set section_id to be the ID of the section you want to get row count from.

The conditional logic used in the demo to update the Number of Rows field is as follows:

The ELSE statement above ensures that the Number of Rows field is initially updated with the row count before any interaction occurs. The THEN statement then updates the value after the People row count changes.

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

