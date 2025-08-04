# Vertical Range Sliders - WS Form

> **Source**: [https://wsform.com/knowledgebase/vertical-range-sliders/](https://wsform.com/knowledgebase/vertical-range-sliders/)


HTML 5 does not provide a native way of displaying a vertical range slider. Instead you have to use a CSS class.

Note: We are unable to provide support for this. The CSS class below is experimental and included here for any users who require vertical sliders. Rotated range sliders have cross browser compatibility issues.
[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13615)
To create a vertical slide, edit the range slider field and in the advanced tab enter wsf-range-vertical into the Classes –> Field Wrapper setting.

Add the following custom CSS to your website to adjust the height of the range slider. It is possible to add this using a WS Form HTML field with the CSS wrapped in <style> tags.

Change the CSS variable --wsf-range-vertical-height (line 2) to any height you wish. It is set to 200 pixels by default.

```
.wsf-range-vertical {
    --wsf-range-vertical-height: 200px !important;
}
```
