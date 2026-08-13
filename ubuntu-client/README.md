<div align="center">
  <img src="./assets/icon.svg" width="128" alt="project logo">
</div>

# ubuntu client

Scripts and configuration data for ubuntu linux machines that are not the main LAN server..

## Description

Settings and scripts to configure LAN linux machines.
This assumes that the basic server requirements have set from the ubuntu server repository.

This repository is to be added to any existing configuration souce files for the target machine.

### Features

* Consistent with host git push-to-deploy.
* postfix null client.
* chrony client.

## Instructions

* Follow the instructions in the [ubuntu-common]( https://github.com/krpfeiffer/ubuntu-common/) README.md to clone the target host configuration source repository.
* Update the target host configuration to include the unbuntu-common settings.
* Copy the relevant files into this host configuration repository. Overwrite if required.
* Carefully remove any artefacts. These will be deleted or renamed files.
* Commit and push changes.
* Changes on the "main" branch will trigger an automatic deployment to /usr/local/src/config.d

## Dependencies

* Ubuntu 20.04
* [Ubuntu common](https://github.com/krpfeiffer/ubuntu-common)
* Public key ssh login to target machine.
