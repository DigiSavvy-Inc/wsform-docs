# Process Submit Data with a WordPress Hook - WS Form

> **Source**: [https://wsform.com/knowledgebase/handling-submit-data-with-your-own-code/](https://wsform.com/knowledgebase/handling-submit-data-with-your-own-code/)


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
