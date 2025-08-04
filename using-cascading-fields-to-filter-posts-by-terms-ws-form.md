# Using Cascading Fields to Filter Posts by Terms - WS Form

> **Source**: [https://wsform.com/knowledgebase/using-cascading-fields-to-filter-posts-by-terms/](https://wsform.com/knowledgebase/using-cascading-fields-to-filter-posts-by-terms/)


Cascading fields can be used to filter a list of posts by terms. For example you could filter a list of blog articles by category, or filter a list of custom post types by a custom taxonomy term.

## Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13706)
In the above demo we are filtering knowledge base articles by their assigned categories.

There are two fields used to do this:

## Term Select

To configure the first select field to use terms, we configure the options to use the Terms data source. The screenshot below shows how the select field is configured to do this:

Choose a taxonomy applicable to the post type you want to filter. Use the default columns configured for the Terms data source (ID, Name & Slug). Finally we configure the column mapping and choose the Name column for the option labels and the Slug column for the value. The value column mapping will be passed to the cascade filtering of the next field.

## Post Select

To configure the second select field to use posts, we configure the options to use the Posts data source. The screenshot below shows the select field is configured to do this:

Choose a post type that is associated with the taxonomy chosen in the first field. Use the default columns configured for the Posts data source (ID, Title, Status, Slug, Date, Terms), or optionally just keep the the ID and Title and Terms columns. Configure the column mapping and choose the Title column for the option labels and the ID column for the option values. Cascading is enabled and we choose the Terms column as the Filter Column. It is possible a post will be assigned to more than one term, so we’ll check the Filter Column – Comma Separate setting to handle it. Finally we choose the first field as the Filter Value.

And that’s it! Your form will now enable to choose a term which will filter the posts in the second field.
