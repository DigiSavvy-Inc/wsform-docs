# Using Cascading Fields to Filter Posts by Terms - WS Form

> **Source**: [https://wsform.com/knowledgebase/using-cascading-fields-to-filter-posts-by-terms/](https://wsform.com/knowledgebase/using-cascading-fields-to-filter-posts-by-terms/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Using Cascading Fields to Filter Posts by Terms

Cascading fields can be used to filter a list of posts by terms. For example you could filter a list of blog articles by category, or filter a list of custom post types by a custom taxonomy term.

## Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13706)
In the above demo we are filtering knowledge base articles by their assigned categories.

There are two fields used to do this:

## Term Select

To configure the first select field to use terms, we configure the options to use the Terms data source. The screenshot below shows how the select field is configured to do this:

Choose a taxonomy applicable to the post type you want to filter. Use the default columns configured for the Terms data source (ID, Name & Slug). Finally we configure the column mapping and choose the Name column for the option labels and the Slug column for the value. The value column mapping will be passed to the cascade filtering of the next field.

## Post Select

To configure the second select field to use posts, we configure the options to use the Posts data source. The screenshot below shows the select field is configured to do this:

Choose a post type that is associated with the taxonomy chosen in the first field. Use the default columns configured for the Posts data source (ID, Title, Status, Slug, Date, Terms), or optionally just keep the the ID and Title and Terms columns. Configure the column mapping and choose the Title column for the option labels and the ID column for the option values. Cascading is enabled and we choose the Terms column as the Filter Column. It is possible a post will be assigned to more than one term, so we’ll check the Filter Column – Comma Separate setting to handle it. Finally we choose the first field as the Filter Value.

And that’s it! Your form will now enable to choose a term which will filter the posts in the second field.

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

