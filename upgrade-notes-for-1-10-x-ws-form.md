# Upgrade Notes for 1.10.x - WS Form

> **Source**: [https://wsform.com/knowledgebase/upgrade-notes-for-1-10-x/](https://wsform.com/knowledgebase/upgrade-notes-for-1-10-x/)


Release date: January 2, 2025.

Version 1.10.x of WS Form introduces a new Styler system that provides greater control for WordPress form design.

The new system is designed to be backward compatible with earlier versions of WS Form with minimal changes to the underlying HTML used to render forms. However, there are a few improvements that you should consider when upgrading to 1.10.x.

## First Things, First!

Whenever you upgrade a plugin, theme or core in WordPress:


Version 1.10.x introduces some new accessibility features that may have a subtle effect on your forms.

## New CSS

1.10.x includes a rewrite of the CSS used in WS Form to support CSS variables. You can check the CSS Variables Reference to see all of the available CSS variables.

CSS is now dynamically loaded by field type to reduce redundancy.

### Custom CSS Considerations

If you have implemented any custom CSS yourself this should still work provided your selectors are specific enough to WS Form elements.

We recommend prefixing all CSS selectors with:

.wsf-form

This is per our original Styling Forms with CSS documentation.

For example:

.wsf-form .wsf-field-wrapper .wsf-label

Whilst not necessary, we would recommend using the new Styler to implement your customizations. You can, of course, implement any further customizations you need using custom CSS. Consider using the WS Form CSS variables to customize form elements.

## New HTML

Revised HTML has been implemented to improve the presentation / customization of some field types. These should not present any styling issues but have been included here for transparency.

### Date / Time Fields

All icons in the date / time picker have now been replaced with pure CSS icons. This allows for easier resizing and coloring.

### Password Fields

Password fields now have the following markup added as a sibling to the password input element if the password strength meter is enabled:

<ul><li /><li /><li /></ul>

This replaces an SVG that was used for the strength meter and improves the ability for you to recolor the meter if required by using pure CSS icons.

### Select Fields

The dropdown arrow on Select fields has been converted from an SVG file to a pure CSS icon. This allows for easier resizing and coloring.
