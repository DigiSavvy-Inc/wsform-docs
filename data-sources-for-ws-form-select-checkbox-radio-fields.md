# Data Sources for WS Form Select, Checkbox & Radio Fields

> **Source**: [https://wsform.com/knowledgebase/data-sources/](https://wsform.com/knowledgebase/data-sources/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields-- How To Make Checkboxes Required-- Data Sources: Google Sheets-- Create a Link in a Checkbox or Radio Label-- Data Grid Column Mapping-- Using #field With Delimiter and Column Parameters-- How To Add Tooltips to Checkboxes and Radios-- Data Grids-- Style Checkboxes-- Data Sources-- Populate Select, Checkbox and Radio Fields Using PHP-- Create Select, Checkbox, and Radio Cascading Lookups-- Show Select, Checkbox and Radio Labels in Emails-- Extract Select, Checkbox & Radio Labels-- Display Checkboxes or Radios in Columns- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Data Sources

Data sources are used to automatically populate Select, Checkbox and Radio fields as well as any other fields that support data lists (e.g. text fields).

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13618)
Examples of using data sources include:

You’ll find the data source option at top of all field data grids.

By default, the data source will be Off. The Off setting allows you to manually edit the data grid to control which items appear in your field.

Here’s how to use a data source:

## 1. Select Data Source

The following data sources can be selected:

Once you have selected a data source, the settings for that data source will be displayed.

## 2. Configure The Data Source

Each data source has its own settings. The Preset data source simply requires that you choose a preset. Other data sources such as Post have many more options that allow you to control and filter the data retrieved.

## 3. Get Data

Once you have configured the data source, you need to retrieve the data. To do this simply click on the Get Data button.

Once the data is retrieved it will be displayed in a preview data grid:

In the above example, we retrieved a list of countries using the Preset data source. Because this data is static, WS Form will change the Data Source dropdown to Off and then allows you to edit the data grid. Other data sources such as Post or Term are not editable because they update dynamically according to the posts or terms you have created in WordPress.

WS Form updates data sources in real-time. This means that if you create a select field that lists all users, it will keep that list up to date with all the users you have in your WordPress admin. Likewise if you create a field that lists all of your posts, it will keep that list up to date with all the posts you create.

It is possible to make any data source static and no-longer update automatically by choosing Off as the Data Source . Note that when Off is selected, the data grid will not update automatically if the original source data is changed.

## 4. Column Mapping (Optional)

Once you are happy with the data you have retrieved you should ensure your column mapping is correct. The column mapping settings are shown underneath the data grid.

There are three column mappings to consider:

By default, WS Form will use the first column for each of these settings.

Each time you retrieve new data you should ensure the column mappings are correct.

## 5. Save

Click Save & Close (or Save if you wish to make further edits) to save your data source settings.

## 6. Preview

Click the Preview button at the top of the layout editor to preview the form and test the field contain your data source settings.

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

