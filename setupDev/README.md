![project logo](./assets/icon-128x128.png)

# setupDev

Wordpress plugin to convert a site to a development site.

## Description

This works for either a clean install or a copied site.

If this is a copied site, it updates settings and moves content to relevant user.
It replaces users and settings from that site to appropriate development requirements.

On a clean site it only sets the development site parameters, including creating a devmaster user, if needed.

### Features

* Will only permit only one run for a site.
* Most setup is done within the plugin activation function. Some post-activation activity to handle users is required. See instructions below.
* If needed, it creates a devmaster user as administrator.
* Moves any webmaster content to devmaster.
* Removes subscribers, keeping only those identified as allowed.
* Updates settings in wp_options.
* Imports pNet dev settings.
* Plugin deactivates itself on completion.

## Instructions

### Clean install

* Update config.php to use any development site settings.
* Login as site administrator.
* Activate the plugin.
* Resolve any administrator issues. Manually delete devmaster and move content, OR, remove exisiting site administrator.

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
