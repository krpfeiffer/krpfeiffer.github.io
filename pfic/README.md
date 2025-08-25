![project logo](./assets/icon-128x128.png)

# setupDev

Wordpress plugin to convert a WordsPress site to a development site.

## Description

This works for either a clean install or a copied site.

If this is a copied site, it updates settings and moves content to relevant user.
It replaces users and settings from that site to appropriate development requirements.

On a clean site it only sets the development site parameters.

### Features
* Can only be run once for a site.
* If needed, it creates a devmaster user as administrator.
* Moves any webmaster content to devmaster.
* Removes any subscribers, keeping only those identified as allowed.
* Updates settings in wp_options.
* Imports pNet dev settings.
* All setup is done by the plugin activation function.
* Plugin deactivates itself on completion.

## Instructions
### Clean install
* Update config.php to use any development site settings.
* Activate the plugin.

### Copied site install
* Update config.php to use any development site settings.
* Login as 'webmaster' using source site credentials.
* Activate the plugin.
* Set 'devmaster' password.
* Logout and log back in as 'devmaster' using newly created credentials.
* Delete 'webmaster' user.

## Dependencies
None.

