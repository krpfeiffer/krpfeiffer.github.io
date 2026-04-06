![project logo](./assets/icon-128x128.png)

# setupDev

Wordpress plugin to convert a site to a development site.

## Description

This works for either a clean install or a copied site.

If this is a copied site, it updates settings and moves content to relevant user.
It replaces users and settings from that site to appropriate development requirements.

On a clean site it only sets the development site parameters.

### Features
* Can only be run once for a site.
* If needed, it creates a devmaster user as administrator.
* Move any webmaster content to devmaster.
* Remove any subscribers, keeping only those identified as allowed.
* Update settings in wp_options.
* Import pNet dev settings.
* All setup is done by the plugin activation function.
* Plugin deactivates itself on completion.

## Instructions
### Clean install
* Update config.php to use any development site settings.
* Login as site administrator.
* Activate the plugin.

### Copied site install
* Update config.php to use any development site settings.
* Login as 'webmaster' using source site credentials.
* Activate the plugin.
* Set 'devmaster' password.
* Logout and log back in as 'devmaster' using newly created credentials.
* Delete 'webmaster' user.

Note that all copied users will have the same credentials as they use on the source site.

## Dependencies
None.
