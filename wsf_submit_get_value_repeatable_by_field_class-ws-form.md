# wsf_submit_get_value_repeatable_by_field_class - WS Form

> **Source**: [https://wsform.com/knowledgebase/wsf_submit_get_value_repeatable_by_field_class/](https://wsform.com/knowledgebase/wsf_submit_get_value_repeatable_by_field_class/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions- wsf_helper_get_object_meta_value- wsf_helper_get_object_property- wsf_submit_set_value_by_field_id- wsf_submit_set_value- wsf_submit_get_value_repeatable_by_field_class- wsf_submit_get_value_by_field_class- wsf_submit_get_value_repeatable- wsf_submit_get_value- wsf_submit_get_object- wsf_submit_get_by_hash- wsf_form_get_all_key_value- wsf_form_get_all- wsf_field_get_objects_by_class- wsf_field_get_objects_by_meta- wsf_field_get_objects_by_label- wsf_field_get_object- wsf_section_get_object- wsf_group_get_object- wsf_form_get_count_submit_by_id- wsf_form_get_label_by_id- wsf_form_get_object- wsf_config_get_field_types- Configuration- Fields- Forms- Helper- Sections- Submission- Tabs Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials

Search

# wsf_submit_get_value_repeatable_by_field_class

## Contents

## Description

The wsf_submit_get_value_repeatable_by_field_class PHP function returns a submitted field value by field class from a repeatable section.

This function is useful if you want to extract submission values by class name instead of field ID.

To add a class to a field, edit a field and then enter a class name in the Advanced tab under the Classes settings. You can add a class name in either the Field Wrapper or Field class settings.

When using this function you can specify a single class name even if you have entered multiple classes in a field. For example a field that has the classes my-class-1 my-class-2 my-class-3 will be picked up if you pass my-class-2 as the class to this function.

If one field matching the class name is found, the field value is returned. If more than one field matching the class name is found, an array of the field values is returned.

## Usage

```
wsf_submit_get_value_repeatable_by_field_class( $form_object, $submit_object, $class_name, $default_value, $protected );
```

## Parameters

## Return

`Array` [String](https://www.php.net/manual/en/language.types.string.php)An array of field value of the matching field class name, one element per repeatable row.

If more than one field matches the supplied class name, an array of values is returned per row.

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

