# wsf_render_media_button - WS Form

> **Source**: [https://wsform.com/knowledgebase/wsf_render_media_button/](https://wsform.com/knowledgebase/wsf_render_media_button/)


## Contents

## Description

The wsf_render_media_button filter allows you to control whether or not the Add Form button is added to the classic editor when editing a post.

## Usage

```
add_filter( 'wsf_render_media_button', 'my_hook_function', 10, 2 );
```

## Parameters

## Example

```
// Callback function for the wsf_render_media_button filter hook
function my_hook_function( $render_media_button, $post_type ) {
	
	// Your code here ...

	// Return value
	return false;
}

// Add a callback function for the wsf_render_media_button filter hook
add_filter( 'wsf_render_media_button', 'my_hook_function', 10, 2 );
```

## Source File

This hook can be found in: `<plugin root>/admin/class-ws-form-admin.php`

## More Resources
