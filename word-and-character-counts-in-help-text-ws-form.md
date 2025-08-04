# Word and Character Counts in Help Text - WS Form

> **Source**: [https://wsform.com/knowledgebase/word-and-character-counts-in-help-text/](https://wsform.com/knowledgebase/word-and-character-counts-in-help-text/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials- How to Extract First and Last Names from a Full Name- Create a Form Recipient Selector Using PHP- How to Set a 'Reply To' When Sending Emails- Number Rounding Examples- Add Custom Templates to the Template Library- Enable and Disable Dates and Times Using PHP- Create a State / Province by Country Selector- Push Form Submissions to a JetEngine Custom Content Type- Build a WordPress Form with the JetEngine Plugin- Using Cascading Fields to Filter Posts by Terms- Build a WordPress Form With the Toolset Plugin- Build a WordPress Form with the Pods Plugin- Form Abandonment - Saving Partial Form Submissions- Build a WordPress Form with the Meta Box Plugin- Redirect Existing Users by Role During Registration- Redirect Users by Role After Login- Change Form Submission Limit Settings Using PHP- Translate Forms- Assign a Form to a WooCommerce Product- Custom Server-Side Form Validation- Create a Form Summary- Writing Custom HTML for Email Content and PDF Templates- Make a Field Read-Only- Save & Continue- Send File Attachments in an Email- Add Select2 to a WS Form Select Field- Email Address Validation- Duplicate / Copy Field Values With #text- Run JavaScript on Form Load- Add Row Numbers to Repeatable Sections- Use Repeatable Section Count in Calculations- Process Submit Data with a WordPress Hook- Style Radios- Create a Customizable T-Shirt Product- Populate a Form With Post Data- Build a WordPress Form with the Advanced Custom Fields (ACF) Plugin- Vertical Range Sliders- Populate Select, Checkbox and Radio Fields Using PHP- Create an 'Other' Option- Create Floating Inside Field Labels With CSS- Create a Field Prefix or Suffix- Combine First and Last Name Fields into a Full Name Field- Change Required Field Indicators- Create a Contact Form in WordPress- Create Select, Checkbox, and Radio Cascading Lookups- Create a File Upload Progress Bar- Create Random Values- Populate a Form With User Data- Create a Redirect Selector- Use Shortcodes In Forms- Show Select, Checkbox and Radio Labels in Emails- Extract Select, Checkbox & Radio Labels- Use Fields To Change Repeatable Section Row Counts- Display Checkboxes or Radios in Columns- Create a Form Recipient Selector Using Conditional Logic- Find the ID of a Field- Populate a Field With Query String Data- ACF- ACPT- AI- Abandonment- Calculated Fields- Cascading- Checkbox Fields- Conditional Logic- Date/Time- E-Commerce- Email Addresses- Email Notifications- Field Settings- File Uploads- Geolocation- JavaScript- JetEngine- Loaders- Meta Box- PHP Examples- Pods- Population- Post Management- Radio Fields- Redirecting- Repeatable Sections- Select Fields- Spam- Styling & CSS- Tabs- Templates- Toolset- Translation- User Management- Validation- Variables & Dynamic Content-- How to Extract First and Last Names from a Full Name-- Variables Helper-- Calculating Minimum and Maximum Field Attributes-- Calculate Character and Word Counts for a Form Field-- How to Enable File Previews in Emails and PDF Templates-- Formatting Numbers Using #number_format-- Dynamic Label, Placeholder and Help Text With #text-- Using #field With Delimiter and Column Parameters-- Transforming Strings-- The Variable Cheat Sheet-- Create a Form Summary-- Duplicate / Copy Field Values With #text-- Combine First and Last Name Fields into a Full Name Field-- Create Random Values-- Word and Character Counts in Help Text- WooCommerce

Search

# Word and Character Counts in Help Text

WS Form can add word or character counters to all types of text fields and in any format you wish.

Word and character counters are added to the Help Text setting of a field.

To determine how the word or character count is displayed, you simply add some WS Form variables in the help text setting of a field. To do this:

## Examples

Here are some examples of how these variables can be used in the Help Text setting.

#character_count #character_count_label / #word_count #word_count_label
Example output: 15 characters / 3 words

#character_count #character_count_label
Example output: 123 characters

#word_count #word_count_label
Example output: 12 words

#word_count #word_count_label (Maximum: #word_max #word_max_label)
Example output: 1 word (Maximum: 12 words)

You have #word_remaining #word_remaining_label remaining.
Example output: You have 5 words remaining.

## Word & Character Count Variables

The word and character count variables are as follows:

#### Character

Name / VariableAdditional InformationCount`[#character_count](https://wsform.com/knowledgebase/word-and-character-count/)`Returns the total character count. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Count Label`[#character_count_label](https://wsform.com/knowledgebase/word-and-character-count/)`Returns 'character' or 'characters' depending on the character count. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Maximum`[#character_max](https://wsform.com/knowledgebase/word-and-character-count/)`Returns the maximum character length that you set for a field. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Maximum Label`[#character_max_label](https://wsform.com/knowledgebase/word-and-character-count/)`Returns 'character' or 'characters' depending on the maximum character length. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Minimum`[#character_min](https://wsform.com/knowledgebase/word-and-character-count/)`Returns the minimum character length that you set for a field. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Minimum Label`[#character_min_label](https://wsform.com/knowledgebase/word-and-character-count/)`Returns 'character' or 'characters' depending on the minimum character length. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Count Remaining`[#character_remaining](https://wsform.com/knowledgebase/word-and-character-count/)`If you set a maximum character length for a field, this will return the total remaining character count. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Count Remaining Label`[#character_remaining_label](https://wsform.com/knowledgebase/word-and-character-count/)`If you set a maximum character length for a field, this will return the total remaining character count. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).#### Word

Name / VariableAdditional InformationCount`[#word_count](https://wsform.com/knowledgebase/word-and-character-count/)`Returns the total word count. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Count Label`[#word_count_label](https://wsform.com/knowledgebase/word-and-character-count/)`Returns 'word' or 'words' depending on the word count. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Maximum`[#word_max](https://wsform.com/knowledgebase/word-and-character-count/)`Returns the maximum word length that you set for a field. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Maximum Label`[#word_max_label](https://wsform.com/knowledgebase/word-and-character-count/)`Returns 'word' or 'words' depending on the maximum word length. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Minimum`[#word_min](https://wsform.com/knowledgebase/word-and-character-count/)`Returns the minimum word length that you set for a field. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Minimum Label`[#word_min_label](https://wsform.com/knowledgebase/word-and-character-count/)`Returns 'word' or 'words' depending on the minimum word length. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Count Remaining`[#word_remaining](https://wsform.com/knowledgebase/word-and-character-count/)`If you set a maximum word length for a field, this will show the total remaining word count. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).Count Remaining Label`[#word_remaining_label](https://wsform.com/knowledgebase/word-and-character-count/)`If you set a maximum word length for a field, this will show the total remaining word count. For more information about this variable, [click here](https://wsform.com/knowledgebase/word-and-character-count/).

 

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

