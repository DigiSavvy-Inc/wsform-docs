# Push Form Submissions to a JetEngine Custom Content Type - WS Form

> **Source**: [https://wsform.com/knowledgebase/push-form-submissions-to-a-jetengine-custom-content-type/](https://wsform.com/knowledgebase/push-form-submissions-to-a-jetengine-custom-content-type/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content- WooCommerce

Search

# Push Form Submissions to a JetEngine Custom Content TypePRO

In this tutorial we’ll learn how to push a form submission to a Custom Content Type created with the popular Crocoblock plugin JetEngine by using the WS Form Webhook action.

## What is a JetEngine Custom Content Type?

A JetEngine Custom Content Type (CCT) is similar to a WordPress Custom Post Type except the data is stored in a separate table in the WordPress database. This offers improved performance given that a row of data is stored in a single database record as opposed to traditional WordPress post records which have separate post meta records for each field.

Each row of data in a CCT is made up of standard JetEngine custom fields.

JetEngine provides a REST API that enables you to add new CCT rows using an API endpoint. We’ll be interfacing with that API via the WS Form Webhook action.

## Create a Custom Content Type

If you don’t already have a CCT set-up, you’ll need to create one in JetEngine. We’ll refer to the JetEngine knowledge base for this step:

In this tutorial we have created a simple CCT containing three fields:

## Enable the REST API on the Custom Content Type

By default a CCT cannot be accessed by the WordPress REST API. In order to do that we’ll need to do the following:

## Create an Application Password

The next step is to create an application password for accessing the REST API. You’ll use the application password in conjunction with a WordPress username to authenticate the request to the REST API.

For hardened security, you may wish to create a dedicated WordPress user that has access capabilities that match those configured on your CCT (e.g. edit_posts). This provides you with the ability to delete the user in future if you need to.

Once you have decided which WordPress user will be used to access the CCT, you can then create the application password. To do this:

We now have everything we need to connect to the REST API:

## Connect Your Form to the JetEngine Custom Content Type

For this tutorial we’ve created a very simple form containing three fields:

To connect the form to the JetEngine CCT, we’re going to use the Webhook action. To do this:

## Test the Form

Click the Preview button at the top of the layout editor to test the form.

If you have the WS Form debug console open, click Populate & Submit and then you can check the response from the WordPress REST API in the Log tab. You should see a 200 success message in the log that indicates a record was added to the JetEngine CCT.

You should now see a new record added to your CCT in JetEngine.

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

