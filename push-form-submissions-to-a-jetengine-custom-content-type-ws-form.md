# Push Form Submissions to a JetEngine Custom Content Type - WS Form

> **Source**: [https://wsform.com/knowledgebase/push-form-submissions-to-a-jetengine-custom-content-type/](https://wsform.com/knowledgebase/push-form-submissions-to-a-jetengine-custom-content-type/)


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
