# Styler - WS Form

> **Source**: [https://wsform.com/knowledgebase/styler/](https://wsform.com/knowledgebase/styler/)


The Styler allows you to design an unlimited number of styles that can be applied to any WordPress form built with WS Form with ease. Whether you want to maintain consistent branding across your WordPress site or tailor the appearance of individual forms for specific purposes, the Styler offers the flexibility to create, design, and manage styles effortlessly.

For developers, the Styler provides access to over 400 customizable settings, all easily managed using CSS variables for maximum flexibility and control. For beginners, creating styles is a breeze with intuitive options for adjusting colors, sizes, and other design elements, no coding required.

## What is a Style?

A style in WS Form is a structured hierarchy of CSS variables, beginning with high-level settings like the color palette and typography. These foundational elements cascade down to progressively more specific settings, including sections, fields, and even individual field types, ensuring a consistent and customizable design throughout your forms.

## How to Edit a Style

There are two ways to open the Styler to edit a style.


The Form category in the Styler can be used to change the majority of the styling in a form and provides a quick way of getting the bulk of your form styled. For example, changing the Base color will change other elements on the form such as label colors, help text and input colors automatically.

The Form category includes the following style settings:

Setting
Type
Default
Description

Border
Color
Color
`transparent`
The border color. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/border-color).

Radius
Size
`0px`
The border radius. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/border-radius).

Width
Size
`0px`
The border width. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/border-width).

Style
Text
`solid`
The border style. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/border-style).

Color Palette
Background
Color
`transparent`
The form background color.

Base
Color
`#000000`
Main color used for labels, inputs and help text.

Base – Contrast
Color
`#ffffff`
Contrast color used for checkmarks, button text, etc.

Accent
Color
`#205493`
Used for checked and styled checkboxes and radio fields, range slider thumb, etc.

Neutral
Color
`#767676`
Used for neutral tones on the form such as the file upload button.

Primary
Color
`#205493`
Used for the form submit button and any elements configured to use the Primary color.

Secondary
Color
`#5b616b`
Default color used for other buttons.

Success
Color
`#2e8540`
Used for success messages.

Information
Color
`#02bfe7`
Used for information messages.

Warning
Color
`#fdb81e`
Used for warning messages.

Danger
Color
`#bb0000`
Used for error messages and invalid feedback.

Spacing
Grid Gap
Size
`20px`
The spacing between fields.

Padding – Horizontal
Size
`0px`
Horizontal form padding.

Padding – Vertical
Size
`0px`
Vertical form padding.

Transition
Speed
Text
`200ms`
The time for transitions it takes for general transitions to run on the form.

Timing Function
Text
`ease-in-out`
The CSS timing function used for transitions. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/transition-timing-function)

Typography
Font Family
Text
`inherit`
The base font family used throughout the form.

Font Size
Size
`16px`
The base font size used throughout the form.

Font Size – Small
Size
`14px`
This is primarily used on field help text.

Font Size – Large
Size
`18px`
This is primarily used on legends.

Font Style
Text
`inherit`
Defines italic or normal text style. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/font-style).

Font Weight
Text
`inherit`
Controls text boldness or lightness. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/font-weight).

Letter Spacing
Text
`inherit`
Adjusts space between text characters. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/letter-spacing).

Line Height
Sixe
`1.4`
Sets spacing between text lines. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/line-height).

Text Decoration
Text
`inherit`
Adds lines, styles, or colors. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/text-decoration).

Text Transform
Text
`inherit`
Changes text casing styles. [Learn more](https://developer.mozilla.org/en-US/docs/Web/CSS/text-transform).

These settings may vary slightly for conversation styles where font sizes and spacing are increased for legibility.

## How to Save a Style

Once you have finished making changes to a style, click the Save  icon. This will immediately publish the style ready for use on the website.

## The Styler Sidebar

The Styler will open on the left and side of your form by default.

### Style Name

The Style Name is shown at the top of the Styler. To edit the style name click the Settings icon at the top, change the name, then click the Save icon.


You can search for settings in a variety of ways:

Simply enter keywords into the search (minimum 2 characters) and the setting hierarchy will be filtered.

### Style Categories

The top level style categories are:

To open a category and view the sub-categories click the category name.

Use the Form category to change the main colors, sizes and typography settings for your form.


### Style Setting

There are various types of Style Setting.

#### Color

Color settings allow you to pick any color for a form element.

To use the color picker to choose a color, simply click the Swatch.

The following values can be entered into the color Setting Value.

Color Model
Example
Description

Hex
`#ff0000`
Hexadecimal as `#rrggbb`.

Hex 8
`#ff000088`
Hexadecimal with alpha as `#rrggbbaa`.

RGB
`rgb(255, 0, 0)`
Red, green, blue as `rgb(r, g, b)`.

RGBA
`rgba(255, 0, 0, 0)`
Red, green, blue, alpha as `rgba(r, g, b, a)`.

HSL
`hsl(0, 100%, 50%)`
Hue, saturation and lightness as `hsl(h, s, l)`.

HSLA
`hsla(0, 100%, 50%, 0.533)`
Hue, saturation and lightness as `hsla(h, s, l, a)`.

var()
`var(--accent-color)`
CSS variable.

### Size

Size settings allow you to set the size of a form element.

The following values can be entered into the color Setting Value.

Unit of Measurement
Example
Type
Description

px
`16px`
Absolute
Pixels: A fixed unit, most commonly used.

em
`1.5em`
Relative
Relative to the font size of the element.

rem
`1.5rem`
Relative
Root em: Relative to the font size of the root element.

%
`90%`
Relative
Percentage: Relative to the parent element’s size.

var()
`var(--font-size-base)`

CSS variable.

We recommend a base pixels size of at least 16 pixels to help with the accessibility of your form.

### Other Settings

Other settings include:

These values have text inputs that support a CSS value or variable.

### Style Undo

Any changes made during a given editing session can be undone by clicking the Style Undo  icon. This will reset all of the settings in the style those the values that were present when the Styler was opened.

If you want to fully reset a style to the system defaults, you can do that from the Styles admin page by clicking the Reset link.

### Settings

The settings panel allows you change the style name and also enable the alternative colors scheme. To access the settings panel click the Settings  icon.

### Save

The Save  icon is used to publish the changes you have made to the style so that they are committed to the live version of any form using that style.

If you are making significant changes to a style, consider cloning it or exporting a backup prior to doing so.

## Repositioning the Styler

You can temporarily move the Styler by clicking and dragging the WS Form logo. If the Styler is position at the left or right of the screen, WS Form will attempt to lock it in position and introduce left or right margin to the body element to provide you with a better view of your form.
