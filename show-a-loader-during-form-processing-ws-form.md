# Show a Loader During Form Processing - WS Form

> **Source**: [https://wsform.com/knowledgebase/loader/](https://wsform.com/knowledgebase/loader/)


A form loader (spinner) is a used to indicate that a form is in the process of loading, submitting or processing data. It is used to provide visual feedback to users that their action (such as submitting a form) has been initiated, and that WS Form is working on processing the request.

WS Form supports a variety of customizable built-in loaders as well as being able to implement your own loader HTML.

WS Form makes adding a loader icon to your form easy.

## Demo

## Loader Styles

The following built-in loader styles are available:

Rotate 25 Gap

Rotate 25 Accent

Rotate Grow

Rotate Dots

Rotate Dots Tail

Circle Dots

Circle Dots Pulse

Horizontal Dots Pulse

Horizontal Dots Accent

Credit: The built-in lightweight CSS loaders were adapted from the cssloader github repo developed by Vineeth.TR.

## How to Enable the Loader

To enable the WS Form loader:

## Customizing the Loader

The loader can be fully customized using the settings in the Loader tab. The loader settings are as follows:

### Sprite

#### Type

Choose from the following types:

#### Size

The approximate size of the sprite. Note that due to how CSS loaders are rendered in the browser this may not be pixel perfect.

#### Color

Choose the color for the sprite.

#### Opacity

Choose the opacity for the sprite (0 = Transparent, 1 = Solid).

#### Accent Color

If the sprite type chosen supports an accent color (e.g. Rotate 25 Color), choose the color for the accent.

#### Accent Opacity

If the sprite type chosen supports an accent color (e.g. Rotate 25 Color), choose the opacity for the sprite (0 = Transparent, 1 = Solid).

#### Border Width

If the sprite type chosen utilizes a border width CSS attribute, choose the border width in pixels.

#### Always Visible

If checked WS Form will attempt to keep the loader always visible. If a form is taller than the web browser viewport, this feature can be useful to ensure the loader is seen by the user.

This setting is best suited to forms that are statically positioned and scroll with the page. If your form is rendered in a pop-up or is in an element that has been placed in a specific position on this page, we recommend disabling this setting.

#### Custom HTML

If you choose the Custom HTML option then an HTML editor will appear allowing you enter any custom HTML you wish for your sprite.

You can find a sample of other loader sprites in the cssloaders github repo.

We recommend adding any associated CSS to your theme as opposed to the Custom HTML setting.

### Text

Text can optionally be displayed below the sprite. Note that the text will always be present in the DOM for accessibility purposes.

#### Visible

If checked, the text will be displayed beneath the sprite.

#### Text

Text shown below the sprite.

### Overlay

When the loader is shown, an overlay is rendered over the top of the form. This is intended to fade out the form and indicate to the user that form processing is in progress.

#### Color

Choose the color for the overlay.

#### Opacity

Choose the opacity for the overlay (0 = Transparent, 1 = Solid).

#### Cursor

You also choose a cursor to show when the mouse pointer hovers over the overlay.

### Timing

#### Animation Duration

This is the total time in seconds one cycle of the sprite animation should take. The higher this value, the slower the sprite will animate.

#### Fade-In Duration

This is the total amount of time it should take for the animation to fade-in. Set to 0 for no fade-in.

#### Fade-Out Duration

This is the total amount of time it should take for the animation to fade-out. Set to 0 for no fade-out.

### Events

Use the events settings to determine when the loader should appear.

#### Submit

If checked, the loader will appear with the form is submitted. Use the slider beneath this setting if you would like to delay showing the loader.

#### Save

If checked, the loader will appear with the form is saved. Use the slider beneath this setting if you would like to delay showing the loader.

#### Action

If checked, the loader will appear when an action is run using conditional logic. Use the slider beneath this setting if you would like to delay showing the loader.

#### Render

#### If checked, the loader will appear while the form is being rendered. Use the slider beneath this setting if you would like to delay showing the loader.

#### Geolocate

#### If checked, the loader will appear while a geolocate (browser or IP) is in progress. Use the slider beneath this setting if you would like to delay showing the loader.
