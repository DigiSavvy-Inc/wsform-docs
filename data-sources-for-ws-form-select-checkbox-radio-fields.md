# Data Sources for WS Form Select, Checkbox & Radio Fields

> **Source**: [https://wsform.com/knowledgebase/data-sources/](https://wsform.com/knowledgebase/data-sources/)


Data sources are used to automatically populate Select, Checkbox and Radio fields as well as any other fields that support data lists (e.g. text fields).

### Demo

[Download Demo](https://wsform.com/plugin-support/form-download.php?id=13618)
Examples of using data sources include:

You’ll find the data source option at top of all field data grids.

By default, the data source will be Off. The Off setting allows you to manually edit the data grid to control which items appear in your field.

Here’s how to use a data source:

## 1. Select Data Source

The following data sources can be selected:

Once you have selected a data source, the settings for that data source will be displayed.

## 2. Configure The Data Source

Each data source has its own settings. The Preset data source simply requires that you choose a preset. Other data sources such as Post have many more options that allow you to control and filter the data retrieved.

## 3. Get Data

Once you have configured the data source, you need to retrieve the data. To do this simply click on the Get Data button.

Once the data is retrieved it will be displayed in a preview data grid:

In the above example, we retrieved a list of countries using the Preset data source. Because this data is static, WS Form will change the Data Source dropdown to Off and then allows you to edit the data grid. Other data sources such as Post or Term are not editable because they update dynamically according to the posts or terms you have created in WordPress.

WS Form updates data sources in real-time. This means that if you create a select field that lists all users, it will keep that list up to date with all the users you have in your WordPress admin. Likewise if you create a field that lists all of your posts, it will keep that list up to date with all the posts you create.

It is possible to make any data source static and no-longer update automatically by choosing Off as the Data Source . Note that when Off is selected, the data grid will not update automatically if the original source data is changed.

## 4. Column Mapping (Optional)

Once you are happy with the data you have retrieved you should ensure your column mapping is correct. The column mapping settings are shown underneath the data grid.

There are three column mappings to consider:

By default, WS Form will use the first column for each of these settings.

Each time you retrieve new data you should ensure the column mappings are correct.

## 5. Save

Click Save & Close (or Save if you wish to make further edits) to save your data source settings.

## 6. Preview

Click the Preview button at the top of the layout editor to preview the form and test the field contain your data source settings.
