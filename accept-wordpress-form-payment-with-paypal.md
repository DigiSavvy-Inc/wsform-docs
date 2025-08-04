# Accept WordPress Form Payment with PayPal

> **Source**: [https://wsform.com/knowledgebase/paypal_checkout/](https://wsform.com/knowledgebase/paypal_checkout/)


This knowledge base article relates to the WS Form PayPal Checkout add-on.
Included with the Freelance & Agency editions or buy separately for the personal edition.

The PayPal Checkout add-on allows you to accept PayPal or credit card payments from your forms. You can either charge a fixed amount using the button in isolation, or you can use the WS Form E-Commerce fields to produce more advanced cart options.

The PayPal Checkout button uses the latest client-side payment process offered by PayPal described here.

Note: When a PayPal Checkout transaction is completed, WS Form PRO will store the transaction ID with the form submission. This transaction ID is a credit transaction ID. Your customer will receive a debit transaction ID. Although these IDs are different, you can still search using either transaction ID in PayPal.

Note: You must serve the page containing the payment form over HTTPS. The address of the page containing PayPal Checkout must start with https:// rather than just http://.

## Installation

The WS Form PayPal Checkout add-on is installed in the same way as installing the WS Form PRO plugin.

Once installed you will need to activate the license for the plugin. When you purchase the PayPal Checkout add-on, you will be given a license key. If you have lost your license key(s), click here.

To activate your license key:

If your license key fails to activate, please ensure you are using the correct license key and not your WS Form PRO license key.

## Configuring PayPal Checkout

In order to use the PayPal Checkout button, you first need to enter your PayPal client IDs.

If you do not yet have a PayPal account, register for a new account.

To obtain your client IDs:

To enter your client IDs:

Once configured, the PayPal Checkout button will appear under the E-Commerce section of the toolbox when editing a form.

## Adding The PayPal Checkout Button

To learn how to add, edit, clone, move, resize, offset, or delete a PayPal Checkout button field, please click here.

When editing a custom button field, the field settings sidebar will appear. This contains the following tabs:

You can edit any of the settings in each of these tabs and then click the Save button to save your changes. If you do not want to save your changes, you can click the Cancel button or click any other form element to close the field settings sidebar.

For a full explanation of the configuration options for the PayPal Checkout button, click here.

## Basic

The basic tab contains settings that the majority of WS Form users will need to control a field. The settings are as follows:

### Label

This label is used to identify the custom button in the WS Form form builder.

### Transaction

#### Amount To Charge

By default this field is blank, and the PayPal Checkout button will charge the amount calculated by the e-commerce fields on your form (the same as entering #ecommerce_cart_total). For example, you might have a single price field for making a donation, or a more elaborate form with prices, quantities, and subtotals.

You can also enter a fixed amount into this field.

WS Form variables can be entered into this field.

#### Description

Enter the description of the transaction in this field. For example: Payment To My Blog.

WS Form variables can be entered into this field.

### Billing Address

#### First Name

You can use this field to pre-populate the payers first name.

WS Form variables can be entered into this field.

#### Last Name

You can use this field to pre-populate the payers first name.

WS Form variables can be entered into this field.

#### Email

You can use this field to pre-populate the payers email address.

WS Form variables can be entered into this field.

#### Phone Type / Phone

You can use this field to pre-populate the payers phone number. First use a phone type, e.g. Mobile, then enter their phone number.

WS Form variables can be entered into this field.

#### Billing Address Mapping

This field is optional. Billing Address Mapping tells WS Form which of your form fields relate to the corresponding billing (payer) fields in PayPal Checkout. When using this feature, the following fields MUST be mapped:

To map a field:

### Shipping Address

#### Recipient Name

You can use this field to pre-populate the recipient name when used in conjunction with the shipping mapping fields.

#### Shipping Address Mapping

This field is optional. Shipping Address Mapping tells WS Form which of your form fields relate to the corresponding shipping fields in PayPal Checkout. When using this feature, the following fields MUST be mapped:

To map a field:

### Disabled Payment Methods

Check which payment methods you would like to disable.

## Advanced

The advanced tab contains additional form attribute settings that provide further control over how the PayPal Checkout button is rendered.

### Button

#### Layout

This setting determines the button layout when multiple buttons are available. Choose from horizontal or vertical.

#### Color

Select the button color you would like to use. The default and recommended color is gold.

### Shape

Select the button color you would like to use. The default and recommended shape is rectangle.

#### Height

Height is optional. Leave this field blank, or enter a value in pixels (typically between 25 and 55) to specify a button height. Different button sizes have different limitations on height.

#### Label

Select the style of button you would like to create by changing this setting. The available options are:

#### Tagline

When enabled the PayPal tagline will appear under the button. This option is only available for the horizontal layout.

### Classes

For developers WS Form allows you to add your own classes to fields.

#### Field Wrapper

The wrapper CSS class setting enables you to add a class (or classes) to a field wrapper. Field wrappers are sections of HTML added around a field to position them on the page. To add multiple classes, add a space between the class names.

### Transaction

#### Breakdown Mapping

This field is optional. Breakdown Mapping tells WS Form which of your cart detail form fields relate to the corresponding detail fields in PayPal Checkout. When using this feature, the following fields are available for mapping:

Note: The mapped fields MUST add up to the cart total.

To map a field:

#### Zero Amount

You can configure how WS Form should handle zero amounts for PayPal Checkout buttons. In some cases you may wish to show an error message (e.g., a donation amount is set to zero). In other cases you may wish to still submit the form (e.g., if something is determined to be free). Select the appropriate action from the pull-down list.

#### Zero Amount Message

If you opt to show an error message, enter the error message you would like be shown here.

#### Messages

WS Form PRO processes any error messages as standard WS Form messages. The error message settings match those of the Show Message action. You can configure these settings to change how the error messages are displayed to users.

### Breakpoints

The breakpoint settings define the width of a field and also what the offset (how many columns from the left-hand side of the form or the previous field) of a field is for each breakpoint. For more information about the breakpoint settings and capabilities of WS Form, click here.
