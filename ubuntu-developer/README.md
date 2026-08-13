<div align="center">
  <img src="./assets/icon.svg" width="128" alt="project logo">
</div>

# ubuntu developer

Scripts and configuration data for ubuntu developer machines.

## Description

Settings and scripts to configure ubuntu machines for developer use.
It assumes that the ubuntu client configuration has been set.

This repository is to be added to the existing configuration souce files for the target machine.

### Features

* Consistent with host git push-to-deploy.
* Pull current codebase development versions.
* QA checks for the codebase.
	- Create release notes from developent branch conventional commits.
	- PHP coding standards checks.
	- PHP mess detection.
	- PHP version compatabilty checks.
	- Update documentation site with katest PHPDocs output.
* Run QA check tools periodically. Check if codebase has changed before running.
* Code beautifier. Meets WordPress coding standards.

## Instructions

* Follow the instructions in the [ubuntu-common]( https://github.com/krpfeiffer/ubuntu-common/) README.md to clone the target host configuration source repository.
* Update the target host configuration to include the unbuntu-common and ununtu-client settings.
* Copy the relevant files into this host configuration repository. Overwrite if required.
* Carefully remove any artefacts. These will be deleted or renamed files.
* Commit and push changes.
* Changes on the "main" branch will trigger an automatic deployment to /usr/local/src/config.d

## Dependencies

* Ubuntu 20.04
* [Ubuntu common](https://github.com/krpfeiffer/ubuntu-common)
* [Ubuntu client](https://github.com/krpfeiffer/ubuntu-client)
* Public key ssh login to target machine.
