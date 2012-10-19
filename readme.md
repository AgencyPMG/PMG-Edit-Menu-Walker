# Menu Edit Walker

A simple plugin to replace the default menu edit walker with one that provides a
few `do_action` calls:

    <?php
    do_action('nav_menu_item_settings_before', $item_id, $item);

    // snip snip ...

    do_action('nav_menu_item_settings_after', $item_id, $item);

This exists to make it easier to add custom fields to nav menu items. You can
use the actions in conjuction with `wp_setup_nav_menu_item` and
`wp_update_nav_menu_item`.
