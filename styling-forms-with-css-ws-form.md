# Styling Forms with CSS - WS Form

> **Source**: [https://wsform.com/knowledgebase/styling-forms-with-css/](https://wsform.com/knowledgebase/styling-forms-with-css/)


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
