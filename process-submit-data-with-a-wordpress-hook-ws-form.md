# Process Submit Data with a WordPress Hook - WS Form

> **Source**: [https://wsform.com/knowledgebase/handling-submit-data-with-your-own-code/](https://wsform.com/knowledgebase/handling-submit-data-with-your-own-code/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Process Submit Data with a WordPress Hook

You can use the Run WordPress Hook action in combination with some simple code to intercept submission data and use it in your own PHP scripts. By using a WordPress filter you can return the submit object back to WS Form for use in other actions.

To do this:

```
// Add filter
add_filter('wsf_filter_tag', 'wsf_filter_function', 10, 2);

// Filter function
function wsf_filter_function($form, $submit) {

    // Set meta key for field ID 123 (Change this to your field ID)
    $meta_key = 'field_123';

    // Get value submit object
    $field_value_old = $submit->meta[$meta_key]['value'];

    // Do something with $field_value_old (This is just an example)
    $field_value_new = str_replace('replace_this', 'with_this', $field_value_old);

    // Set value in submit object
    $submit->meta[$meta_key]['value'] = $field_value_new;

    // Return the submit object back to WS Form
    return $submit;
}
```

When the filter is fired, the form and submit data are passed to it.

In the example above, you would change field_123 to match the field ID on your form. For example, if the field you want to obtain has an ID of 321 in the WS Form layout editor, you would enter field_321 as the $meta_key variable.

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

