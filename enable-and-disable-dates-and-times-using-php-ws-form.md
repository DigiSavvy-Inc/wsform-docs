# Enable and Disable Dates and Times Using PHP - WS Form

> **Source**: [https://wsform.com/knowledgebase/enable-and-disable-dates-and-times-using-php/](https://wsform.com/knowledgebase/enable-and-disable-dates-and-times-using-php/)


You can disable and enable dates and times in Date / Time fields using the ‘Disabled Dates’, ‘Enabled Dates’ and ‘Enabled Times’ settings. These settings are available on the following Date / Time field types:

It is possible to dynamically set disabled and enabled dates and times using PHP.

Example code for doing this can be found below.

## Disabled Dates

In this example we disable two dates for form ID 123 and date/time field ID 321. Disabled dates are entered in the format yyyy-mm-dd.

```
<?php

  // Add filter to change form ID 123 prior to rendering
  add_filter('wsf_pre_render_123', 'my_pre_render_123');

  // My function for filter wsf_pre_render_123
  function my_pre_render_123($form) {

    // Get field ID: 321
    $field = wsf_form_get_field($form, 321);

    // Set the disabled dates
    $field->meta->disabled_dates = array(

        array('disabled_dates_date' => '2025-03-01'),
        array('disabled_dates_date' => '2025-03-03')
    );

    // Return the form
    return $form;
  }
```

## Enabled Dates

In this example we enable two dates for form ID 123 and date/time field ID 321. Enabled dates are entered in the format yyyy-mm-dd.

```
<?php

  // Add filter to change form ID 123 prior to rendering
  add_filter('wsf_pre_render_123', 'my_pre_render_123');

  // My function for filter wsf_pre_render_123
  function my_pre_render_123($form) {

    // Get field ID: 321
    $field = wsf_form_get_field($form, 321);

    // Set the enabled dates
    $field->meta->enabled_dates = array(

        array('enabled_dates_date' => '2025-03-01'),
        array('enabled_dates_date' => '2025-03-03')
    );

    // Return the form
    return $form;
  }
```

## Minimum and Maximum Dates

In this example we set the minimum and maximum date for form ID 123 and date/time field ID 321. Dates are entered in the format yyyy-mm-dd.

```
<?php

  // Add filter to change form ID 123 prior to rendering
  add_filter('wsf_pre_render_123', 'my_pre_render_123');

  // My function for filter wsf_pre_render_123
  function my_pre_render_123($form) {

    // Get field ID: 321
    $field = wsf_form_get_field($form, 321);

    // Set the minimum and maximum dates
    $field->meta->min_date = '2025-03-01';
    $field->meta->max_date = '2025-03-15';

    // Return the form
    return $form;
  }
```

## Enabled Times

In this example we enable two times for form ID 123 and date/time field ID 321. Enabled times are entered in the format hh:mm:ss.

```
<?php

  // Add filter to change form ID 123 prior to rendering
  add_filter('wsf_pre_render_123', 'my_pre_render_123');

  // My function for filter wsf_pre_render_123
  function my_pre_render_123($form) {

    // Get field ID: 321
    $field = wsf_form_get_field($form, 321);

    // Set the enabled times
    $field->meta->enabled_times = array(

        array('enabled_times_time' => '15:00:00'),
        array('enabled_times_time' => '16:00:00')
    );

    // Return the form
    return $form;
  }
```

## Minimum and Maximum Times

In this example we set the minimum and maximum time date/time field ID 321 on form ID 123. Times are entered in the format hh:mm:ss.

```
<?php

  // Add filter to change form ID 123 prior to rendering
  add_filter('wsf_pre_render_123', 'my_pre_render_123');

  // My function for filter wsf_pre_render_123
  function my_pre_render_123($form) {

    // Get field ID: 321
    $field = wsf_form_get_field($form, 321);

    // Set the minimum and maximum times
    $field->meta->min_time = '13:00:00';
    $field->meta->max_time = '18:00:00';

    // Return the form
    return $form;
  }
```
