# Show a Loader During Form Processing - WS Form

> **Source**: [https://wsform.com/knowledgebase/loader/](https://wsform.com/knowledgebase/loader/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders-- Show a Loader During Form Processing- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Show a Loader During Form ProcessingPRO

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

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

