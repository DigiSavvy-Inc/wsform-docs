# Calculated Fields - WS Form

> **Source**: [https://wsform.com/knowledgebase/calculated-fields/](https://wsform.com/knowledgebase/calculated-fields/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields- Calculate Character and Word Counts for a Form Field- Number Rounding Examples- Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials

Search

# Calculated FieldsPRO

The #calc calculated fields function in WS Form PRO makes it easy to create calculate field values that are updated in realtime. It can handle everything from simple addition to more complex trigonometric functions.

## Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13588)
[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13584)
[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13590)
[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13589)
[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13797)

## Features

## How To Create A Calculated Field

Common field types you might use a calculated field in include:

You can put calculated values in the following settings of a field:

To create a calculated field value for the default value of a field, click the field settings  icon and then enter a #calc(...) variable in the Default Value setting.

Anything within the brackets will be calculated in realtime on your form and used as the value of your field.

You can create calculations such as:

#calc(1 + 2)

You can include values from other fields on your form, for example, multiplying field ID 123 value by 5:

#calc(#field(123) * 5)

You can use WS Form math variables (listed at the end of this document) to perform more complex calculations, for example, rounding the previous example to two decimal places:

#calc(#round(#field(123) * 5, 2))

You could even create a calculated field that works out the sum of all values of a field in a repeatable section. The syntax is easy:

#calc(#field(123))

… where field ID 123 is a field in a repeatable section. WS Form PRO automatically sums the values together.  The #section_row_count(456) function (where 456 is the section ID) can be used to calculate the average value of those values:

#calc(#field(123) / #section_row_count(456))

There is an easier way of creating these calculations … the calculator!

### Calculator

WS Form PRO includes a calculator feature that helps creating calculated values for fields.

The calculator will then appear directly below:

The cursor will automatically position itself within the #calc() function. In addition to the normal numeric and arithmetic buttons, the calculator has the following additional buttons:

Insert Field – Click this to insert a #field() variable into your calculated field. It lists all of the fields on your form that are compatible with the calculated field feature.

del – Deletes a character

AC (All Clear) – Deletes the entire calculation

f – Inserts a math variable into your calculation such as #pi, #cos(...) or #sin(...) (See below)

Note that whilst the calculator will do its best to maintain a suitable cursor position, you can always click on the default value itself to reposition the cursor.

### Source Field Rules

If a field used in a calculation is an e-commerce type (e.g. price, price select etc), the input value is assumed to be a currency and WS Form will therefore correctly interpret the price according to your currency symbol, decimal and thousand separator settings and will convert that to a floating point number.

If a field used in a calculation is not an e-commerce type (e.g. number, text, select etc), the input value should follow standard conventions used for evaluating numbers in JavaScript, i.e.

For example: 123.45

### Display Calculations as Prices

If you wish to show a calculation as a price using your currency settings, you can use the ecommerce_price variable, for example:

#ecommerce_price(#calc(#field(1) + #field(2)))

### JavaScript Floating Point Rounding

WS Form calculations are assessed using standard JavaScript. In some cases this can result in floating point numbers such as:

123.40000000000001 instead of 123.4

This is actually perfectly normal in the computing world! If you’re interested here is an explanation.

In order to get a neater looking number, simply use the #round variable, for example:

#round(#calc(#field(1) + #field(2)), 1)

The last parameter is the number of decimal places you would like to use.

### Variables

In addition to #field(...), the following variables can be used inside with #calc(...).
MathNumberRandom NumbersSeconds#### Math

Name / VariableAdditional InformationAbsolute#abs(number)Returns the absolute value of a number. For more information about this variable, click here.Inverse Cosine#acos(number)Returns the inverse cosine of a number in radians. For more information about this variable, click here.Inverse Sine#asin(number)Returns the inverse sine of a number in radians. For more information about this variable, click here.Inverse Tangent#atan(number)Returns the inverse tangent of a number in radians. For more information about this variable, click here.Average#avg(number)Returns the average of all the input numbers. For more information about this variable, click here.Ceiling#ceil(number)Rounds a number up to the next largest whole number. For more information about this variable, click here.Cosine#cos(radians)Returns the cosine of a radian number. For more information about this variable, click here.Euler's#exp(number)Returns E to the power of a number. For more information about this variable, click here.Floor#floor("number")Returns the largest integer value that is less than or equal to a number. For more information about this variable, click here.Logarithm#log(number)Returns the natural logarithm of a number. For more information about this variable, click here.Maximum#max(number)Returns the maxiumum value of the supplied numbers. For more information about this variable, click here.Minimum#min(number)Returns the lowest value of the supplied numbers. For more information about this variable, click here.Negative#negative(number)Returns 0 if positive, or original value if negative. For more information about this variable, click here.PI#piReturns an approximate value of PI. For more information about this variable, click here.Positive#positive(number)Returns 0 if negative, or original value if positive. For more information about this variable, click here.Base to the Exponent Power#pow(base, exponent)Returns the base to the exponent power. For more information about this variable, click here.Round#round(number, decimals)Returns the rounded value of a number. For more information about this variable, click here.Sine#sin(radians)Returns the sine of a radian number. For more information about this variable, click here.Square Root#sqrt(number)Returns the square root of the number. For more information about this variable, click here.Tangent#tan(radians)Returns the tangent of a radian number. For more information about this variable, click here.#### Number

Name / VariableAdditional InformationFormat Number#number_format(number, decimals, "decimal_separator", "thousand_separator")Returns a number with grouped thousands. Same as the PHP number_format function.#### Random Numbers

Name / VariableAdditional InformationRandom Number#random_number(min, max)Outputs an integer between the specified minimum and maximum attributes. This function does not generate cryptographically secure values, and should not be used for cryptographic purposes. For more information about this variable, click here.#### Seconds

Name / VariableAdditional InformationSeconds in a day#seconds_dayReturns the number of seconds in a day. For more information about this variable, click here.Seconds since Epoch#seconds_epochReturns the number of seconds since the Unix Epoch (January 1 1970 00:00:00 GMT). For more information about this variable, click here.Seconds since Epoch at midnight#seconds_epoch_midnightReturns the number of seconds since the Unix Epoch (January 1 1970 00:00:00 GMT) to the closest previous midnight. For more information about this variable, click here.Seconds in an hour#seconds_hourReturns the number of seconds in an hour. For more information about this variable, click here.Seconds in a minute#seconds_minuteReturns the number of seconds in a minute. For more information about this variable, click here.Seconds in a week#seconds_weekReturns the number of seconds in a week. For more information about this variable, click here.Seconds in a year#seconds_yearReturns the number of seconds in a common year. For more information about this variable, click here.

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

