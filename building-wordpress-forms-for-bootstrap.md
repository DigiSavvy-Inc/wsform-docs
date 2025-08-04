# Building WordPress Forms for Bootstrap

> **Source**: [https://wsform.com/knowledgebase/building-wordpress-forms-for-bootstrap/](https://wsform.com/knowledgebase/building-wordpress-forms-for-bootstrap/)


Bootstrap is a popular, free and open-source CSS framework directed at responsive, mobile-first front-end web development. It contains CSS- and (optionally) JavaScript-based design templates for typography, forms, buttons, navigation, and other interface components. Many popular WordPress themes use Bootstrap.

If your WordPress theme uses the Bootstrap framework, WS Form can output forms that contain  HTML markup that is native to that framework. This means that WS Form physically changes the HTML so that your form dovetails seamlessly into your theme.

In addition to output native markup, WS Form will also change the breakpoint selector to match the available breakpoints in Bootstrap. This feature is only available in WS Form PRO.

All of the available WS Form field types are fully compatible with Bootstrap.

## Demo

To view a demo of a WS Form outputting a form for the Bootstrap framework, click here.

## Supported Versions

WS Form supports the following versions of Bootstrap:

## Configuring WS Form to Use Bootstrap Framework

### Automatic

When you first install WS Form, it will scan your theme files and if Bootstrap is detected it will automatically output your form using Bootstrap markup.

### Manual

To manually select Bootstrap as your framework:

## Sample Output

An example of the HTML output for a tel field is shown below (includes some additional markup required by WS Form).

```
<div class="col-6 col-md-3 form-group" id="wsf-1-field-wrapper-6" data-id="6" data-type="tel">
	<label id="wsf-1-label-6" for="wsf-1-field-6">Phone</label>
	<input type="tel" id="wsf-1-field-6" name="field_6" class="form-control" aria-labelledby="wsf-1-label-6">
	<div id="wsf-1-invalid-feedback-6" class="invalid-feedback">Please provide a valid phone number.</div>
</div>
```
