# Word and Character Counts in Help Text - WS Form

> **Source**: [https://wsform.com/knowledgebase/word-and-character-counts-in-help-text/](https://wsform.com/knowledgebase/word-and-character-counts-in-help-text/)


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
