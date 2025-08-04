# wsf_render_media_button - WS Form

> **Source**: [https://wsform.com/knowledgebase/wsf_render_media_button/](https://wsform.com/knowledgebase/wsf_render_media_button/)


Category

Select...
 Getting Started Accessibility Actions Add-Ons Building Forms Calculated Fields Conditional Logic Custom Field Plugins Data Grids Developers E-Commerce Fields Front-End Frameworks GDPR Hooks- wsf_action_email_css- wsf_name_suffixes- wsf_name_prefixes- wsf_submit_block_ips_message- wsf_submit_block_keywords_message- wsf_submit_block_ips_message_type- wsf_submit_block_keywords- wsf_submit_block_ips- wsf_action_redirect_url- wsf_pre_render- wsf_populate- wsf_config_parse_variables- wsf_action_webhook_payload- wsf_action_webhook_http_headers- wsf_field_invalid_feedback_text- wsf_submit_hidden_fields- wsf_form_checksum_check- wsf_submit_validate- wsf_action_pdf_template_path- wsf_action_pdf_filename- wsf_enqueue_script_strategy_defer- wsf_enqueue_script_in_footer- wsf_action_user_signon_error- wsf_action_user_lostpassword_error- wsf_enqueue_scripts- wsf_enqueue_styles- wsf_submit_export_csv_row- wsf_submit_field_validate- wsf_submit_export_csv_header- wsf_conversational_enqueue_styles- wsf_config_frameworks- wsf_form_create_meta_data- wsf_loaded- wsf_submit_status- wsf_activate- wsf_submit_post_complete- wsf_settings_update- wsf_form_stat_add_count- wsf_pre_render_<form_id>- wsf_dropzonejs_image_size- wsf_action_email_email_validate- wsf_action_email_headers- wsf_action_email_message- wsf_action_email_subject- wsf_action_email_to- wsf_action_email_template- wsf_action_email_attachments- wsf_action_email_bcc- wsf_action_email_reply_to- wsf_action_email_cc- wsf_currency_default- wsf_api_call_timeout- wsf_api_call_verify_ssl- wsf_debug_enabled- wsf_option_set- wsf_option_get- wsf_submit_export_file_size_zip- wsf_submit_export_page_size- wsf_api_submit_response_data- wsf_dropzonejs_upload_path- wsf_settings_button- wsf_settings_static- wsf_table_submit_column_actions- wsf_table_submit_field_type_list- wsf_render_media_button- Actions- Filters Licensing Migration PHP Functions Populating Forms Publishing Forms Reporting Sections Security Spam Protection Statistics Styling Forms Submissions Tracking Troubleshooting Tutorials

Search

# wsf_render_media_button

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

[Knowledge Base](https://wsform.com/knowledgebase/)

Search

