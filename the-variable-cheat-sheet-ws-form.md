# The Variable Cheat Sheet - WS Form

> **Source**: [https://wsform.com/knowledgebase/the-ws-form-variable-cheat-sheet/](https://wsform.com/knowledgebase/the-ws-form-variable-cheat-sheet/)


While you can achieve a whole lot in WS Form without using variables, you can create even more dynamic and powerful forms using them.

Variables can be used in a variety of places, including:

Below are some common variable combinations our customers use in WS Form.

## Fields

Example
Description
Where To Use

`#field(123)`
Returns the value of field ID 123.

`#field(123, "/")`
Returns the value of field ID 123, delimiting multiple values with the / character.
Learn more about the delimiter parameter.

`#field(123, "/", "Width")`
Returns the value found in the Width column of field ID 123, delimiting multiple values with the / character.
Learn more about the delimiter and column parameters.

`#field(123, "/", 2)`
Returns the value found in column index 2 (third column) of field ID 123, delimiting multiple values with the / character.
Learn more about the delimiter and column parameters.

`#text(#field(123))`
Dynamically returns the value of field ID 123. The value is updated whenever field ID 123 changes.
Learn more about the #text variable

`#calc(#field(123) + #field(321))`
Returns the sum of field IDs 123 and 321. The sum is updated whenever field ID 123 or 321 changes if it is used in field settings.
Learn more about the #calc variable

## Sections

Example
Description
Where To Use

`#section_row_count(123)`
Returns the number of repeatable rows in section ID 123.
Learn more about repeatable sections

`#calc(#section_row_count(123) * 10)`
Returns the number of repeatable rows in section ID 123 multiplied by 10. The value is updated whenever the number of rows in section ID 123 changes.
Learn more about repeatable sections

`#section_row_number`
Returns the current section row number. This is useful for numbering repeatable sections.
Learn more about repeatable sections

## Submissions

Example
Description
Where To Use

`#submit_id`
Returns the submission ID.

`#submit_hash`
Returns the submission hash.

`#submit_url`
Returns a URL that can be used to return back to a saved submission.
Learn more about save and continue

## #if … #endif

Example
Description
Where To Use

`#if(#field(123))You entered something in field ID 123#endif`
Returns You entered something in field ID 123 if field ID 123 is not blank.

`#if(#field(123) == "Option 1")You chose option 1#endif`
Returns You chose option 1 if field ID 123 equals Option 1.

`#if("#text(#field(123))" == "Option 1")You chose option 1#endif`
Dynamically returns You chose option 1 if field ID 123 equals Option 1. The value is updated whenever field ID 123 changes.
Learn more about the #text variable

`#if(#calc(#field(123)) > 10)Number greater than 10#endif`
Dynamically returns Number greater than 10 if field ID 123 contains a number greater than 10. The value is updated whenever field ID 123 changes.
Learn more about the #calc variable

## Blog

Example
Description
Where To Use

`#blog_name`
Returns the site title.

`#blog_admin_email`
Returns the administration email address.

`#blog_date`
Returns the current date using the site date format.

`#blog_time`
Returns the current time using the site time format.

## Selects, Checkboxes and Radios

Example
Description
Where To Use

`#field(123)`
Returns the value of a select, checkbox or radio for field ID 123.

`#select_option_text(123)`
Returns selected option text for field ID 123.

`#checkbox_label(123)`
Returns the checked checkbox(es) label(s) for field ID 123.

`#radio_label(123)`
Returns the checked radio label for field ID 123.

## Query Variables

Example
Description
Where To Use

`#query_var("post_id")`
Returns the value of the query variable `post_id`.
For example:

https://mysite.com/?post_id=123

This would return 123.

## Date/Time

Also see our Date/Time Cheat Sheet for more examples.

Example
Description
Where To Use

`#client_date`
Returns the users web browser local date in the format configured in WordPress. This variable can only be used in client-side.

`#client_time`
Returns the users web browser local time in the format configured in WordPress. This variable can only be used in client-side.

`#client_date_custom(format, seconds_offset)`
Returns the users web browser local date and time in a specified format (PHP date format)
Learn more about date formats

`#blog_date`
Returns the blog date in the format configured in WordPress.

`#blog_time`
Returns the blog time in the format configured in WordPress.

`#blog_date_custom(format, seconds_offset)`
Returns the blog date and time in a specified format (PHP date format).
Learn more about date formats

`#server_date`
Returns the server date in the format configured in WordPress.

`#server_time`
Returns the server time in the format configured in WordPress.

`#server_date_custom(format, seconds_offset)`
Returns the server date and time in a specified format (PHP date format).
Learn more about date formats

For a complete reference of all the available variables, click here.
