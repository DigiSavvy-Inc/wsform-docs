# Learn More About Date Formats

> **Source**: [https://wsform.com/knowledgebase/date-formats/](https://wsform.com/knowledgebase/date-formats/)


Date formatting in WS Form follows the same conventions used when formatting PHP dates. For a list of available formatting string options, see the PHP date manual page.

Variables that use date formatting strings are as follows:

#field_date_format(field_id, "formatting string")
#post_date_custom("formatting string")
#server_date_custom("formatting string")
#blog_date_custom("formatting string")
#client_date_custom("formatting string")

For example:

#server_date_custom("m/d/Y H:i:s")
