![project logo](./assets/icon-128x128.png)

# pfic
WordPress plugin to provide functionality for the pfeiffer cookbook website.

## Description
This plugin supports the GP-Cookbook theme without being dependent upon it.

Integrates with WP Recipe Maker to deliver recipe-related functionality.

### Features
* Chapter taxonomy to organise recipes for printed cookbook.
* Ingredient custom post type.
* Cookbook printing:
	- Print all recipes in chapter sequence.
	- Print a table of contents.
	- Print post content, including recipe, for a chapter.
	- Print post content, including recipe, within a date range.
* WP Recipe Maker taxonomy enablement and extension.
* Custom RSS feeds for automatic social media posting using IFTTT.

## Upgrades
Some upgrades may require changes to the contents of the database.
There is a file in the root folder which will handle the required changes.
You are advised to create a backup before running the script.
The script will abort if used on a production site.

Run the script from the command line, using the command:

`wp eval-file upgrade-db.php`

## Dependencies
* WP Recipe Maker plugin
* WP Recipe Maker Premium plugin (Pro Bundle)
* [pNet plugin](https://github.com/krpfeiffer/pnet)
