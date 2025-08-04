# Learn More About Date Formats

> **Source**: [https://wsform.com/knowledgebase/date-formats/](https://wsform.com/knowledgebase/date-formats/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers- Add File Types to File Upload Fields in WordPress- CommandUI- Variables Helper- HTML Form Attributes- How to Get the Post ID after Creating a Post- Performance Plugin Considerations- Clearing the Session ID Using the Debug Console- Custom Project Development- Database Tables- How To Delete Submission Records Using MySQL- Debug Console - Testing and Debugging Forms- Writing Custom HTML for Email Content and PDF Templates- Run JavaScript on Form Load- Variables Reference- Cookies- User Capabilities- Performance- Javascript Events- Input Masks- Date Formats E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials

Search

# Date Formats

Date formatting in WS Form follows the same conventions used when formatting PHP dates. For a list of available formatting string options, see the PHP date manual page.

Variables that use date formatting strings are as follows:

#field_date_format(field_id, "formatting string")
#post_date_custom("formatting string")
#server_date_custom("formatting string")
#blog_date_custom("formatting string")
#client_date_custom("formatting string")

For example:

#server_date_custom("m/d/Y H:i:s")

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

