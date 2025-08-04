# wsf_submit_get_value_repeatable_by_field_class - WS Form

> **Source**: [https://wsform.com/knowledgebase/wsf_submit_get_value_repeatable_by_field_class/](https://wsform.com/knowledgebase/wsf_submit_get_value_repeatable_by_field_class/)


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
