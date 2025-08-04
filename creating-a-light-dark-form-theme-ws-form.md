# Creating a Light / Dark Form Theme - WS Form

> **Source**: [https://wsform.com/knowledgebase/creating-a-light-dark-form-theme/](https://wsform.com/knowledgebase/creating-a-light-dark-form-theme/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms- How to Change Which Style a Form Uses- Upgrade Notes for 1.10.x- CSS Variables Reference- Creating a Light / Dark Form Theme- Styler- Styles- HTML Form Attributes- Setting Custom Breakpoint Sizes- Show a Loader During Form Processing- Responsive Forms- Style Checkboxes- Style Radios Submissions Tracking Troubleshooting Tutorials

Search

# Creating a Light / Dark Form ThemePRO

The WS Form Styler can create alternative color schemes for your WordPress forms. The most popular application for alternative color schemes is to build a light / dark theme.

Dark and light themes can improve accessibility by enhancing readability, reducing visual strain, accommodating diverse visual needs, and aligning with user preferences for a more inclusive and customizable experience. Of course, the effectiveness of alternative themes depends on the colors you choose. We encourage you to choose high contrast colors throughout to improve accessibility.

The WS Form alternative color scheme could, however, be used to switch to any other color scheme you wish. For example you could offer a monochromatic, higher contrast or larger font scheme.

This tutorial focusses on providing a light / dark theme for your website.

## Specifying Your Site Color Scheme

In order for WS Form to deliver the correct color scheme you should configure whether your website has a light or dark color scheme. To do this:

By choosing Light, WS Form will show the Base style if the users preferred color scheme is Light.

By choose Dark, WS Form will show the Base style if the users preferred color scheme is Dark.

If the alternative color scheme is not enable on a style, it will always use the Base style.

If you would like WS Form to attempt to automatically detect the preferred color scheme of your website visitors, check the Auto Color Scheme setting. You will need this to be enabled for testing your alternative color scheme.

## Enabling Alternative Color Themes

Each style can have a single or dual color scheme. By default all new styles have a single color scheme. To enable the alternative color scheme on a style:

## Modifying Alternative Colors

When the alternative color scheme is enabled, a scheme selector will appear at the top of the Styler sidebar.

There are three buttons:

## Picking Alternative Colors

When editing style colors in Alt or Both scheme mode, WS Form provides two helpers for picking alternative colors.

### Suggest an Alternative Color

WS Form can automatically suggest an alternative color. To do this, click the Magic Wand  icon.

### Use an Alternative Color Shade

WS Form will also suggest various shades of your base color in the color picker in the swatches. Simply click a swatch to use that color.

## Testing Alternative Color Schemes

To test your alternative color scheme:

## How WS Form Renders Alternative Schemes

When WS Form is using an alternative color scheme, the following class is added to the HTML element:

wsf-styler-scheme-alt

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

