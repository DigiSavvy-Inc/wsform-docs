# Styling Forms with CSS - WS Form

> **Source**: [https://wsform.com/knowledgebase/styling-forms-with-css/](https://wsform.com/knowledgebase/styling-forms-with-css/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS-- Styling Forms with CSS-- How To Add Tooltips to Checkboxes and Radios-- Style Tabs-- Style Checkboxes-- Style Radios-- Vertical Range Sliders- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Styling Forms with CSS

Most styling of a form can be achieved using our responsive layout editor and customize tools, but sometimes you will want to apply more granular styling using some custom CSS (Cascading Style Sheet). This article describes how to use CSS to style forms created with WS Form.

If you need help understanding he HTML attributes used by WS Form, please see our HTML Form Attributes article.

If you require additional assistance understanding CSS, please see our Custom Project Development article.

## Contents

## Basic Examples

The following examples are for use with the WS Form framework. If you are using Bootstrap or Foundation please refer to the documentation for those frameworks.

### Labels

CSS selector: wsf-label

Example of making all labels white:

```
.wsf-form .wsf-field-wrapper .wsf-label {
    color: #FFFFFF;
}
```

### Fields

CSS selector: wsf-field

Example of giving fields a white background and black text:

```
.wsf-form .wsf-field-wrapper .wsf-field {
    background: #FFFFFF;
    color: #000000;
}
```

### Buttons

CSS selector: wsf-button

Example of making buttons red with white text:

```
.wsf-form .wsf-field-wrapper .wsf-button {
    background: #FF0000;
    color: #FFFFFF;
}
```

### Placeholders

CSS selector: wsf-field::placeholder

Example of making placeholder text gray:

```
.wsf-form .wsf-field-wrapper .wsf-field::placeholder {
    color: #999999;
}
```

### Help Text

CSS selector: wsf-help

Example of making help text white:

```
.wsf-form .wsf-field-wrapper .wsf-help {
    color: #FFFFFF;
}
```

## Targeting Forms

WS Form supports multiple forms per page. Each form on the page is called an instance.

Each instance on the page is given a unique ID. For example:

<form id="ws-form-1" data-id="123" class="wsf-form">

Let’s break those attributes down.

The id attribute is a unique identifier for the form. It has the format ws-form-<instance_id>. In this example it is referencing instance 1.

The data-id attribute indicates which form ID is being rendered. In this example it is rendering form ID 123.

The class attribute wsf-form appears on all forms. You can use it to target all forms rendered by WS Form.

### Selector Examples

.wsf-form Target all forms.

form[data-id="123"] Target form ID 123 on any page.

#ws-form-1 Target the first instance of a form on any page.

## Adding Classes to a Form

It is also possible to add classes to form elements so that you can target them with your own CSS.

### Form

To add a class to the form.

### Tabs (All)

Tabs are made up two components, the tab itself and the tab content. To add a class to these components:

The class(es) entered will be added to all tabs in the form.

### Tabs (Individual)

If you have more than one tab in your form, you can also add a class each tab content individually. To do this:

The class(es) entered will be added to the content for that tab.

### Sections (All)

To add a class to all sections in your form:

The class(es) entered will be added to all sections in the form.

### Section (Individual)

To add a class to a specific section in your form:

The class(es) entered will be added to that specific section.

### Fields (All)

Fields are made up of a wrapper and the field itself. To add wrapper or field classes to all fields on your form:

The class(es) entered will be added to all fields in the form.

### Field (Individual)

To add a class to a specific field in your form:

The class(es) entered will be added to that specific section.

### Setting the Form ID in a Shortcode

The format of the WS Form shortcode is very simple:

```
Unable to read published form data
```

… where 123 is equal to your form ID.

The shortcode also has an option element_id parameter which enables you to set the ID of the form element. For example:

```
Unable to read published form data
```

This is useful if you want to target your form using JavaScript.

## Learning CSS

Here are some great online resources for learning CSS:

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

