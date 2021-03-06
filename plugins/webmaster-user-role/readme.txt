=== Webmaster User Role ===
Contributors: tylerdigital, croixhaug
Tags: admin, users, webmaster, capabilities, administrator, editor, permissions, roles, user roles
Requires at least: 3.5
Tested up to: 3.9.1
Stable tag: 1.3

Adds a new "Admin" user role between Administrator and Editor. Perfect for clients and those who know just enough to be dangerous.

== Description ==
This plugin creates a new role named "Admin" that is the same as "Administrator" with the following changes:

= In WP-Admin =
* Hide / Remove Settings menu
* Hide / Remove Plugins menu
* Hide / Remove Tools menu
* Hide / Remove Users menu
* Disable theme installation
* Disable theme switching
* Hide / Remove Appearance > Editor
* Disable WP core updates
* Hide non-essential dashboard items

= 3rd party plugin compatibility =

* Advanced Custom Fields (Elliot Condon) - hide ACF menu, only admins/developers should be modifying ACF definitions/rules/fields
* Contact Form 7 - user can only read contact form submissions
* Gravity Forms (RocketGenius) - user can view form entries but not edit forms or create new ones
* iThemes Security - hide iThemes security menus
* Sucuri Scanner (Sucuri) - hide security scan information
* TablePress - Show/Edit/Import/Export TablePress content (all tabs except plugin options)
* Ultimate Branding (WPMU Dev) - hide branding menu
* Yoast SEO - hide Yoast SEO menu & metabox when editing pages/posts

== Screenshots ==

1. Adds a role to fit nicely between Administrator and Editor
2. Easily remove administrative menu items, while leaving content-related items like Menus and Wigets

== Installation ==
Install and activate, there are no settings in the UI

== Changelog ==
= v 1.3 =
* Hide Users menu (often requested, and really the webmaster user couldn't do much in this screen anyway)
* Add support for ACF5 (hide Custom Fields Menu compatible with new version)
* Add support for Contact Form 7
* Add support for iThemes Security

= v 1.21 =
* Add support for TablePress [http://wordpress.org/plugins/tablepress/]

= v 1.2 =
* Multisite bugfix: Prevent webmaster from removing users from individual sites
* Multisite bugfix: Stop removing Settings & Tools from network administrator

= v1.1.1 =
* Now hides non-essential dashboard items
* Fixes a conflict with Mizzo theme (thanks djesch)

= v1.1 =
* Add support for Sucuri Scanner [http://wordpress.org/plugins/sucuri-scanner/]
* Add support for Advanced Custom Fields [http://wordpress.org/plugins/advanced-custom-fields/]
* Remove tools menu – so webmaster users can't import/export/migrate/find&replace

= v1.0.9 =
* Add support for Ultimate Branding [http://premium.wpmudev.org/project/ultimate-branding/]

= v1.0.8 =
* Add Gravity Forms edit_forms capability as an option (only allows entry viewing by default) via filter:
add_filter( 'td-webmaster-user-roleoption_cap_gravityforms_edit_forms', __return_true );

= v1.0.7 =
* Remove settings menu from wp-admin

= v1.0.5 =
* Remove capability to delete users

= v1.0.4 =
* Add "editor" cap for role so plugins checking for "editor" explicitly work

= v1.0.3 =
* Remove capabiilty to add, edit, promote users
* Remove capability to update core

= v1.0.2 =
* Initial Release