# Populate the Default Value of a Field Using ACF Option Values - WS Form

> **Source**: [https://wsform.com/knowledgebase/populate-the-default-value-of-a-field-using-acf-option-values/](https://wsform.com/knowledgebase/populate-the-default-value-of-a-field-using-acf-option-values/)


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
