# How to Build a WordPress Form Using the ACF Plugin

> **Source**: [https://wsform.com/knowledgebase/how-to-build-a-wordpress-form-with-the-advanced-custom-fields-acf-plugin/](https://wsform.com/knowledgebase/how-to-build-a-wordpress-form-with-the-advanced-custom-fields-acf-plugin/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Build a WordPress Form with the Advanced Custom Fields (ACF) PluginPRO

This knowledge base article relates to the WS Form Post Management add-on.
Included with the Agency edition or buy separately for other editions.

Advanced Custom Fields (ACF) is a plugin that allows you to create custom fields for any post type. WS Form can be fully integrated with custom fields created using ACF.

To obtain the official free or PRO version of ACF, please refer to this ACF blog article:

In this tutorial, we’ll show you how to integrate WS Form PRO with the ACF plugin. You’ll learn how to create a form that can create a WordPress post that contains custom fields configured in ACF.

ACF has basic form functionality built-in that enables you to place the same ACF form you find in the WordPress admin onto the frontend of your website. However, this form has a fixed layout and design.

By using WS Form you can develop powerful, mobile friendly forms that have any layout in place of this basic functionality.

In this tutorial we’re going to create a form that will create a new blog post when it is submitted. These same instructions can be used to create any other post types such as pages or products.

When used with the WS Form Post Management Add-On you can:

ACF repeater fields are fully supported when creating, populating and submitting forms.

## Prerequisites

For this tutorial you will need the following plugins:

## Create Fields in ACF

First, we’re going to create some custom fields that will appear when we edit a post in WordPress. We can choose any of the field types that ACF offers, including groups and repeaters.

You can find some helpful resources on how to configure ACF here.

The following ACF field types are supported in WS Form:

Basic

Content

Choice

Relational

jQuery

Layout

If you add a Repeater field in ACF, that field will be converted to a repeatable section in WS Form. When that form is submitted the repeated rows will be populated in the post at rows in ACF. WS Form supports all field types in repeatable sections.

## Create a Form

Next, we’re going to create a form in WS Form. To do this, we click on Add New in the WS Form menu.

Because we have the Post Management add-on installed, you’ll see that we have a Post Management tab. If we click on that tab it will show us templates for each post type registered in WordPress. We’re going to choose the Post template.

After you click on a template, WS Form automatically creates a form for you. WS Form will:

At the top of the form is a section that includes standard fields we would expect to see for a post, such as the title, content an excerpt. In addition to that it has created fields and sections for all of the custom fields we created with ACF. WS Form sets the width of fields to match your ACF configuration settings.

You can edit the form in exactly the same way as you would any other form. For example, you can resize fields, resize sections and even split the form up across multiple tabs. All of the functionality of the WS Form layout editor is available to you.

## Field Mapping (Optional)

When the form is submitted, the fields on your form are used to create a post in WordPress. WS Form automatically creates field mappings for you if you use a template.

The fields are mapped to either WordPress or ACF fields by using a Post Management action.

To edit the field mappings:

Fields such as selects, checkboxes and radios pull their choices dynamically from ACF. This means that if you change a choice in ACF it will automatically update on your form.

Likewise, relational fields in ACF such as Post Object and User fields are also updated dynamically.

## Preview The Form

Now let’s test the form. To do that we simply click the Preview button.

You’ll notice in our preview window that we have the WS Form debug console open. This is a really great feature for testing forms and allows you to populate a form in a single click. Every time you click Populate the form is populated with different data. There’s even a Populate & Submit button which lets you populate the form with data and submit it.

## View The Post

Now that the form is submitted, let’s take a look at how that looks in WordPress.

First, we’ll click back to the WordPress admin. Then we’ll click on Posts in the WordPress menu.

And there is our new post that was created by WS Form.

If we click on the post, we can see that the post title, excerpt and content have been populated from the form. Below that you can see the custom fields created in ACF that have also been populated.

WS Form supports integration with all of the core ACF field types.

## Pre-Populating a Form with ACF Custom Fields

In addition to creating posts, WS Form can also pre-populate forms using ACF custom fields. To demonstrate this, we’ll go back to the layout editor for the form we just created. Next, we click on the form settings icon at the top of the layout editor.

Then we click on the data tab. From here we configure WS Form to populate the form using the data from an existing WordPress post. In this example, we’ll set WS Form to use the ID of the post we just created.

Below that, you will find the field mappings.

These allow you specify which post and ACF fields will be mapped to which WS Form field. You’ll notice that because we created this form from a template, all of the fields are already mapped for us, so all we need to do is click Save & Close. Then we click Preview to view the form.

The form has been populated with the data from the post and is ready for editing.

And that’s how easy it is to integrate WS Form with ACF!

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

