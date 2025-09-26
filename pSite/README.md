![project logo](./assets/icon-128x128.png)

# pSite
WordPress plugin to provide functionality for the pfeifferNet website.

## Description
This plugin supports the GP-pfeifferNet theme without being dependent upon it.

### Features
* Post series functionality. Allows associated posts to be grouped in a time-based set.
* Self service member functionality.
	- A member is a direct family member. A page with their name is created as their web presence.
	- Maintain contact details.
	- Maintain preferred image.

## Upgrades
Some upgrades may require changes to the contents of the database.
There is a file in the root folder which will handle the required changes.
You are advised to create a backup before running the script.
The script will abort if used on a production site.

Run the script from the command line, using the command:

`wp eval-file upgrade-db.php`

## Dependencies
* [pNet plugin](https://github.com/krpfeiffer/pnet)
