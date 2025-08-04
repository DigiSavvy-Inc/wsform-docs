# The Date/Time Cheat Sheet - WS Form

> **Source**: [https://wsform.com/knowledgebase/the-date-time-cheat-sheet/](https://wsform.com/knowledgebase/the-date-time-cheat-sheet/)


Dates in WordPress forms can be complex! On this page we provide a variety of Date/Time field examples. You can download any of the examples below and import them into a blank form to review them further. You can even drag and drop them into your section library to use in any other form.

In the demos below we are using the following WordPress date and time format settings:

When using date variables, there are three types of date/time you can reference:

## Default to Today’s Date

The date/time field will default to your visitors date/time when the picker is opened, but it will not show this as the default value. To set the default value to today’s date, the following variables can be used:

These variables are added in the Default Value setting of the field:

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13668)
## Default to Today’s Date with Custom Formatting

You can change the format of a date using the following variables:

For example:

#blog_date_custom("m/d/Y")

The date format follows the date format as the PHP date function. Learn more.

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13669)
## Default to Today’s Date with Offset

You can offset a date/time using the offset parameter:

The offset is the number of seconds to add (or subtract) from the current date.

For example:

#blog_date_custom("m/d/Y", #seconds_year)

This would offset today’s date by a year and then format the date as m/d/Y (e.g. 12/31/2022)

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13670)
### Seconds Constant Variables

As well as entering your own offset, you can use the following variables for several helpful constants that represent durations in seconds.

Variable
Output
Description

`#seconds_minute`
60
Seconds in a minute

`#seconds_hour`
3600
Seconds in an hour

`#seconds_day`
86400
Seconds in a day

`#seconds_week`
604800
Seconds in a week

`#seconds_year`
31536000
Seconds in a year

## Default to Current Time

If you are using a date/time field with a type of Time, you can also pre-populate the time. To set the default value to the current time, the following variables can be used:

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13671)
## Offset a Date

The #field_date_offset variable can be used to insert the value of date field that has been offset by a value in seconds.

The syntax is #field_date_offset(field_id, offset_in_seconds, format)

The parameters are:

You can put this variable in the default value of a date field as well as the minimum and maximum settings should you wish to dynamically adjust the available date range.

By wrapping the variable in #text(...) you can ensure the value updates whenever the source date is changed.

### Demo (Default Value)

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13677)
### Demo (Default Value + Date Range)

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13678)
## Setting Minimum and Maximum Date Offsets

When the date picker is opened, you can limit the dates shown to the visitor. You can set the minimum and maximum dates available to choose by using the following date/time field settings (these can be found in the advanced tab):

There are two formats you can enter in this date:

### Offset Examples

Offsets can be in the future or past by using the + or - as the first character and have an origin of 1970-01-01, for example:

+1970-01-01 (Future)

or

-1970-01-01 (Past)

If you want to set the minimum date to todays date minus 2 days, you would enter:

-1970-01-03

If you want the maximum date to be todays date plus 2 days, you would enter:

+1970-01-03

If you want the maximum date to be todays date plus 1 month, you would enter:

+1970-02-01

If you want the maximum date to be todays date plus 1 year and 6 months, you would enter:

+1971-07-01

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13672)
## Setting Minimum and Maximum Time Offsets

When the date picker is opened and the field is configured to use Time only, you can limit the time shown to the visitor. You can set the minimum and maximum times available to choose by using the following date/time field settings (these can be found in the advanced tab):

The time entered into these fields must be in 24 hour clock notation, for example:

You can also configure these settings using dynamic values. For example, if you had From and To time fields and you wanted the To field to not offer times before the From time you could enter the following into the Minimum Time setting in the To field:

#text(#field_date_format(123, "H:i:s"))

… where 123 is the ID of the From field.

### Demo

## Disabling Week Days

You can disable any week day in the date/time picker by using the Disabled Week Days setting in the Advanced tab.

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13674)
## Disabling Dates

You can disable dates in the date/time picker by using the Disabled Dates setting in the Advanced tab.

To add a date to disable:

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13673)
## Enabling Dates

You can enable dates and exclude all others  in the date/time picker by using the Enabled Dates setting in the Advanced tab.

To add a date to enable:

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13675)
## Setting the Minimum and Maximum Year

By default, the minimum and maximum year in the date/time picker will be 1950 – 2050. You can change this range by using the following settings in the Advanced tab:

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13676)
## Calculated Dates

It is possible to use dates in calculated fields.

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13587)
