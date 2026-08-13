<div align="center">
  <img src="./assets/icon.svg" width="128" alt="project logo">
</div>

# ubuntu server

Scripts and configuration data for the main LAN server.

## Description

Settings and scripts to configure main LAN server.
It assume that the ubuntu common scripts and configuration data has been applied.

This repository is to be added to and overwrite existing configuration souce files for the target machine.

### Features

* Consistent with host git push-to-deploy.
* postfix mail server for LAN.
* Periodic system monitoring.
* chrony time server host.
* dnsmasq host for local DNS and DCHP.

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
