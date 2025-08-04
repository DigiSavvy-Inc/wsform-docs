# Run WordPress Hook Action

> **Source**: [https://wsform.com/knowledgebase/run-wordpress-hook/](https://wsform.com/knowledgebase/run-wordpress-hook/)


The Run WordPress Hook action runs a WordPress action or filter when a user saves or submits a form. Although simple this action is powerful and allows developers to run any PHP code when a website visitor submits a form.

## Adding This Action

To add a Run WordPress Hook action:

As with all sidebars in WS Form, click the Save button at the bottom to save your changes, or click Cancel to disregard your changes.

The Run WordPress Hooks action settings are as follows:

## When Should This Action Run?

You can choose to run the WordPress hook when the form is saved, submitted, or both.

## Type

Select the type of hook you would like to run:

## Hook Tag

Enter the tag name of the filter or action you want to run.

## Priority

Choose whether to run the hook before or after other actions. The options are:

If you want to manipulate field values before other actions run, select Before submission created or Before other actions.

If you want to use data other actions have created (For example, to obtain a Zendesk ticket ID), select After other actions.

## Writing Hooks

Click on a tab below to learn how to use this action for Filters and Actions.

### Filter

WS Form PRO will call the filter as follows:

apply_filters($tag_name, $form, $submit);

#### Return Values

The return from your PHP filter function will be processed as follows:

Return Type
Processed As

Object: `$submit`
$submit object will be replaced and passed to the next action.

Integer: 0 – 100
Spam level set
0 = Not spam, 100 = Spam.

Array
Return messages, field value setting or redirect to a different URL (See below).

Boolean: false
Action processing halted.

### Sample Code

#### Return a Submit Object

You can use the Run WordPress Hook action in combination with some simple code to intercept submission data and use it in your own PHP scripts. By using a WordPress filter you can return the submit object back to WS Form for use in other actions.

An example of how to do this is shown below:

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

When the filter runs, the form and submit data are passed to it.

In the example above, you would change field_123 to match the field ID on your form. For example, if the field you want to obtain has an ID of 321 in the WS Form layout editor, you would enter field_321 as the $meta_key variable.

#### Set a Field Value

You can use the Run WordPress Hook action in combination with some simple code to set the value of a field on your form.

An example of how to do this is shown below:

```
// Add filter
add_filter('wsf_filter_tag', 'wsf_filter_function', 10, 2);

// Filter function
function wsf_filter_function($form, $submit) {

    return array(

        array(

            'action' => 'field_value',
            'field_id' => 123,
            'value' => 'Test value',
        )
    );
}
```

The available parameters for the custom message return type array are as follows:

Name
Description
Values
Default
Required

`field_id`
The field ID to set the value in.
–
–
Yes

`value`
The field value to set.

No

`check`
Used to determine if a select, checkbox and radio row matching the value is checked or not.
true, false
true
No

`append`
For text based fields, whether to append the value to the existing value in the field.
true, false
false
No

`prepend`
For text based fields, whether to prepend the value to the existing value in the field.
true, false
false
No

`section_repeatable_index`
Use this to identify the row index if you want to target a field in a repeatable section.
Integer
0 = No section repeatable index
No

In the example above, you would change 123 to match the field ID on your form.

#### Return a Spam Level

If your filter is designed to check for spam, you can return a spam level. This is done by returning an integer between 0 (Not spam) and 100 (Spam).

To return a spam level, the return from your PHP filter can be set as follows:

```
// Add filter
add_filter('wsf_filter_tag', 'wsf_filter_function', 10, 2);

// Filter function
function wsf_filter_function($form, $submit) {

    // Perform your spam check here
    $spam_level = 100;

    // Return a spam level of 100
    return $spam_level;
}
```

#### Return a Custom Message

To return a custom message, the return from your PHP filter can be set as follows:

```
// Add filter
add_filter('wsf_filter_tag', 'wsf_filter_function', 10, 2);

// Filter function
function wsf_filter_function($form, $submit) {

    return array(

        array(

            'action' => 'message',
            'message' => __('My custom message')
        )
    );
}
```

The available parameters for the custom message return type array are as follows:

Name
Description
Values
Default
Required

`message`
Message to display.
–
–
Yes

`type`
Type of message.
success, information, warning, danger, none
success
No

`method`
Position.
before, after
before
No

`form_hide`
Hide form when shown.
true, false
true
No

`clear`
Clear other messages.
true, false
true
No

`duration`
Show duration (ms).

No

`scroll_top`
Scroll to top.
instant, smooth (Blank = Do not scroll)

No

`scroll_top_offset`
Scroll offset (pixels).

0
No

`scroll_top_duration`
Scroll Duration (ms).

400
No

`message_hide`
Hide message after duration.
true, false
false
No

`form_show`
Show form after duration.
true, false
false
No

The behavior of a custom message is the same as the Show Message action.

A more advanced example of returning a custom message array is shown below:

```
// Add filter
add_filter('wsf_filter_tag', 'wsf_filter_function', 10, 2);


// Filter function
function wsf_filter_function($form, $submit) {

    return array(

        array(

            'action' => 'message',
            'message' => __('My information message'),
            'type' => 'information',
            'method' => 'after',
            'form_hide' => false,
            'clear' => true
        )
    );
}
```

#### Return a Redirect

To return a redirect, the return from your PHP filter can be set as follows:

```
// Add filter
add_filter('wsf_filter_tag', 'wsf_filter_function', 10, 2);

// Filter function
function wsf_filter_function($form, $submit) {

    // Set your redirect URL
    $redirect_url = 'https://mysite.com/redirect-url/';

    // Redirect
    return array(

        array(

            'action' => 'redirect',
            'url' => $redirect_url
        )
    );
}
```

#### Return an Error Message

To return an error message, the return from your PHP filter can be set as follows:

```
// Add filter
add_filter('wsf_filter_tag', 'wsf_filter_function', 10, 2);

// Filter function
function wsf_filter_function($form, $submit) {

    return array(

        array(

            'action' => 'error',
            'message' => __('My error message')
        )
    );
}
```

#### Return a Halt Signal

To halt further action processing, the return from your PHP filter can be set as follows:

```
// Add filter
add_filter('wsf_filter_tag', 'wsf_filter_function', 10, 2);

// Filter function
function wsf_filter_function($form, $submit) {

    // Return false to halt action processing
    return 'halt';
}
```

### Action

WS Form PRO will call the action as follows:

do_action($tag_name, $form, $submit);

### Sample Code

#### Retrieve Field Data

The following code is an example of how to retrieve submitted field data from a form:

```
// Add action to process form data
add_action('wsf_action_tag', 'wsf_action_function', 10, 2);

// My function for action
function wsf_action_function($form, $submit) {

    // Get submit value (Change '123' to your field ID)
    $submit_value = wsf_submit_get_value($submit, 'field_123');

    // Do something with $submit_value here
    // ...
}
```

### Using Conditional Logic to Catch Submit and Save Errors

An example of how to catch a form submission error is shown below. Similar conditions exist for a form save error too. In the example below a previously hidden message field is made visible if a submit error occurs.
