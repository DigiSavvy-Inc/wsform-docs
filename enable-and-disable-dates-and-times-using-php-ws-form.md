# Enable and Disable Dates and Times Using PHP - WS Form

> **Source**: [https://wsform.com/knowledgebase/enable-and-disable-dates-and-times-using-php/](https://wsform.com/knowledgebase/enable-and-disable-dates-and-times-using-php/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Enable and Disable Dates and Times Using PHPPRO

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

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

