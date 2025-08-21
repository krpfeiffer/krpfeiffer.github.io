# Changelog

## Release 6.0.0
### Features
- Implement new UI.
- Implement new front page.
- Implement new site footer.

### Refactor
- Improve dark mode appearance.
- Improve CSS, js and icon asset handling.
- Fix asset dependencies and loading order.
- Use only GenerateBlocks v2 global styles.

## Release 5.12.0
### Features
- Add automated release notes generator

### Refactor
- Bump required php version to 8.2

## Release 5.11.0
* Reduced technical debt.

## Release 5.10.0
* Reduced technical debt.
	- Improved archive title handling.

## Release 5.9.0
* Reduced technical debt.
	- Consistent function naming.
	- Added assets include file to improve enqueueing.

## Release 5.8.0
* Deprecated repository-level QA tools (phpdoc, phpcs and phpmd). These are now run at Projects level.
* Improved dark mode appearance.

## Release 5.7.0
* Uses house style based on GenerateBlocks global styles.
* Dark mode added.

## Release 5.6.0
* Replaced namespace prefixes with PHP namespace.
* Changed internal package name.
* Improved phpdoc compatability.

## Release 5.5.0
* Technical debt reduction.
	- Changed namespace prefixes.
	- Changed text domain.
	- Renamed include files.
* PHP QA tools compatability.
	- PHP code sniffer (phpcs).
	- PHP mess detector (phpmd).
	- PHP documentor (phpdoc).

## Release 5.4.0
* Deprecated theme global colour handling to use standard GeneratePress functionality.
* Refactored to use Generatepress global colours and typography.
* Refactored CSS sylesheets to leverage Generateblocks global styles.
* General refactor to better leverage standard grid handling.
* Replaced include file functions with Generatepress elements and hooks.
* Improved XSS and CSRF protection.
* Improved WPCS compliance.

## Release 5.3.0
* Masonry display hook added to make plugins use theme settings.

## Release 5.1.0
* Added support for pSite and pNet plugin namespace.

## Release 5.0.0
* Deprecated Font Awesome.
* Improved responsive typography and spacing.
* Improved responsive images.
* Standardised colour palette.
* Improved image attachment page.
* Compatibility with GeneratePress 3.0.

## Release 4.0.0
* Version bump for consistency with plugins, themes and settings.
* Refactor to use RankMath plugin.
	- Disabled standard GeneratePress schema generation.
* Removed styles from style.css that override customiser settings.
* Added more image metadata and download button on attachment page.

## Release 1.2.0
* Added author archive page.
* Removed short page handling - now uses pNet plugin facility.

## Release 1.1.0
Minor refactor for consistency with pSite plugin. Mainly stylesheet changes.

## Release 1.0.1
Corrected LHS padding on mobile.

## Release 1.0.0
Initial release. Basic functionality.
