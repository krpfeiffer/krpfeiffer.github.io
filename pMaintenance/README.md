
![project logo](./assets/icon-128x128.png)

# pMaintenance

WordPress plugin to inform visitors that site is in maintenance mode.

## Description

Prohibits site fontend display and shows an "under maintenance" page, whilst allowing administrator login.

From version 6.5.0 this plugin no longer tracks the same version number as the pNet plugin.

### Features

* Shows an "under maintenance" page to all visitors.
* Shows the date that maintenance started.
* Allows administrator login to the site.
* Sends a 503 "temporarily unavailable" header.

## Usage

* Activate the plugin to enable maintenance mode.
* Access the login page by going to {site-url}/wp-login.php
* Only administrators will be able to successfully login.
* Deactivate the plugin when maintenance is complete.
