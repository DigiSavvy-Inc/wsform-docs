# Setting Custom Breakpoint Sizes - WS Form

> **Source**: [https://wsform.com/knowledgebase/setting-custom-breakpoint-sizes/](https://wsform.com/knowledgebase/setting-custom-breakpoint-sizes/)


WS Form supports fully responsive forms. In a responsive form, a breakpoint is a point (screen width) at which the form will adapt in a certain way in order to provide the best possible user experience. These are approximately the width of a screen you would find on different devices such as a phone, tablet, laptop, or desktop computer.

Breakpoints can be changed by using the wsf_config_frameworks filter hook. An example of changing the breakpoints for the WS Form framework can be found below:

```
// Add a callback function for the wsf_config_frameworks filter hook
add_filter( 'wsf_config_frameworks', 'my_hook_function', 10, 3 );

// Callback function for the wsf_config_frameworks filter hook
function my_hook_function( $frameworks, $framework, $public ) {

    // Get framework breakpoints
    $breakpoints = $frameworks['types'][$framework]['breakpoints'];

    // Extra small (ID: 25) always 0

    // Small (ID: 50)
    $breakpoints[50]['min_width'] = 576;    // Small breakpoint size in pixels

    // Medium (ID: 75)
    $breakpoints[75]['min_width'] = 768;    // Medium breakpoint size in pixels

    // Large (ID: 100)
    $breakpoints[100]['min_width'] = 992;   // Large breakpoint size in pixels

    // Extra large (ID: 150)
    $breakpoints[150]['min_width'] = 1200;  // Extra large breakpoint size in pixels

    // Set admin breakpoint settings so that sizes are reflected in layout editor
    $breakpoints[25]['admin_max_width'] = $breakpoints[50]['min_width'] - 1;
    $breakpoints[50]['admin_max_width'] = $breakpoints[75]['min_width'] - 1;
    $breakpoints[75]['admin_max_width'] = $breakpoints[100]['min_width'] - 1;
    $breakpoints[100]['admin_max_width'] = $breakpoints[150]['min_width'] - 1;

    // Set framework breakpoints
    $frameworks['types'][$framework]['breakpoints'] = $breakpoints;

    // Return frameworks with adjusted breakpoints
    return $frameworks;
}
```

Note that after adding this code, if you have Compile CSS enabled in WS Form > Settings > Advanced you may need to click Save on that admin page to force the CSS to recompile.
