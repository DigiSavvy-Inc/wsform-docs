# Using FooGallery with WS Form - WS Form

> **Source**: [https://wsform.com/knowledgebase/using-foogallery-with-ws-form/](https://wsform.com/knowledgebase/using-foogallery-with-ws-form/)


The FooGallery WordPress plugin provides a shortcode for embedded a gallery on a page. This shortcode can be used in WS Form.

WS Form supports WordPress shortcodes in forms using fields types such as Text Editor or HTML.

To enable the gallery to display, a small piece of JavaScript is required:

```
jQuery('.foogallery').foogallery();
```

This JavaScript needs to run on form load. This can be done very simply by using some conditional logic as shown below:

You can also use your own custom JavaScript to run scripts when a form loads. See: Run JavaScript on Form Load
