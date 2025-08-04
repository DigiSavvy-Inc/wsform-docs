# wsf_form_stat_add_count - WS Form

> **Source**: [https://wsform.com/knowledgebase/wsf_form_stat_add_count/](https://wsform.com/knowledgebase/wsf_form_stat_add_count/)


## Contents

## Description

The wsf_form_stat_add_count filter allows you to enable or disable form statistics gathering.

## Usage

```
add_filter( 'wsf_form_stat_add_count', 'my_hook_function', 10, 1 );
```

## Parameters

## Example

```
// Callback function for the wsf_form_stat_add_count filter hook
function my_hook_function( $add_count ) {
	
	// Your code here ...

	// Return value
	return false;
}

// Add a callback function for the wsf_form_stat_add_count filter hook
add_filter( 'wsf_form_stat_add_count', 'my_hook_function', 10, 1 );
```

## Source File

This hook can be found in: `<plugin root>/includes/core/class-ws-form-form-stat.php`

## More Resources
