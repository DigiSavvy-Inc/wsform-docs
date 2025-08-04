# Duplicate / Copy Field Values With #text - WS Form

> **Source**: [https://wsform.com/knowledgebase/duplicate-copy-field-values-with-text/](https://wsform.com/knowledgebase/duplicate-copy-field-values-with-text/)


The #text(...) variable is used to duplicate the value of field(s) in real-time.

## Examples

Example
Output

`#text(#field(1))`
Field 1 Content

`#field_label(1): #text(#field(1))`
Field 1 Label: Field 1 Content

`#field_label(1): #text(#field(1) #field(2))`
Field 1 Label: Field 1 Content Field 2 Content

## Demo

## Usage

#text can be used in the following field settings:

An example of how to configure a text field with ID 2 to duplicate the value of field ID 1 is shown below:
