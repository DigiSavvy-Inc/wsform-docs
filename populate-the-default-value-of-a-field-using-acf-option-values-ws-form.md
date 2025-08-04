# Populate the Default Value of a Field Using ACF Option Values - WS Form

> **Source**: [https://wsform.com/knowledgebase/populate-the-default-value-of-a-field-using-acf-option-values/](https://wsform.com/knowledgebase/populate-the-default-value-of-a-field-using-acf-option-values/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF-- Populate the Default Value of a Field Using ACF Option Values-- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Populate the Default Value of a Field Using ACF Option Values

You can use WordPress filter hooks, WS Form functions, and ACF option page values to dynamically set the default value of fields.

## Example Code

Here is example code for setting the default value of the field with ID 321 in form ID 123 using a value from an ACF option page. You would put this code in your theme’s functions.php file (preferably in the child theme if one is present) or use a code snippet plugin.

```
<?php

// Add filter to change form ID 123 prior to rendering
add_filter( 'wsf_pre_render_123', 'populate_field_from_acf' );

// Function to populate the default value using ACF
function populate_field_from_acf($form) {

    // Get the value from the ACF option page
    $acf_value = get_field( 'your_acf_field_key', 'option' );

    // Get the field with ID 321
    $field = wsf_form_get_field( $form, 321 );

    // Set the default value of the field
    $field->meta->default_value = $acf_value;

    // Return the modified form
    return $form;
}
```

## Code Breakdown

### WordPress Filter

Before WS Form renders a form, a WordPress filter runs called wsf_pre_render_{form_id}, where {form_id} is the ID of your form. WS Form passes a form object to this filter function, which you can use to edit all elements of the form.

For example:

```
<?php

// Add filter to change form ID 123 prior to rendering
add_filter( 'wsf_pre_render_123', 'your_custom_function' );

// Your function to modify the form
function your_custom_function( $form ) {

    // Your custom code here

    return $form;
}
```

### Using ACF Option Page Values

To retrieve values from an ACF option page, use the get_field() function. When accessing option page values, you must specify 'option' as the second parameter of get_field(). Replace 'your_acf_field_key' with the field key you set in ACF.

```
$acf_value = get_field( 'your_acf_field_key', 'option' );
```

### Getting a Field

To modify a field in your form, use wsf_form_get_field($form, $field_id), where $form is the form object passed to your filter function by WS Form. $field_id is the ID of the field you want to retrieve. You can find the field ID in the layout editor. This function returns the field settings.

```
$field = wsf_form_get_field( $form, $field_id );
```

### Changing the Default Value

To update the default value of a field, assign a value to the default_value property of the field’s meta object.

```
$field->meta->default_value = $acf_value;
```

## Complete Example

Here’s the full example of dynamically setting a field value using an ACF option page value:

```
<?php

// Add filter to change form ID 123 prior to rendering
add_filter( 'wsf_pre_render_123', 'populate_field_from_acf' );

// Function to populate the default value using ACF
function populate_field_from_acf( $form ) {

    // Retrieve the value from ACF option page
    $acf_value = get_field( 'your_acf_field_key', 'option' );

    // Get the field with ID 321
    $field = wsf_form_get_field( $form, 321 );

    // Set the default value of the field
    $field->meta->default_value = $acf_value;

    // Return the modified form
    return $form;
}
```

This approach ensures your WS Form fields dynamically populate with values managed in the ACF option page, allowing for flexible and centralized value management.

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

