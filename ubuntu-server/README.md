<div align="center">
  <img src="./assets/icon.svg" width="128" alt="project logo">
</div>

# ubuntu common

Scripts and configuration data for all ubuntu linux machines.

## Description

Settings and scripts to configure a ubuntu server.

This repository is to be added to existing configuration files for the target machine.

### Features

* Consistent with host git push-to-deploy.
* apt package management.
* iptables firewall settings.
* logwatch log monitoring.
* Periodic system monitoring.
* ssh and sshd configuration.
* sysctl.d settings.
* Common mail aliases.
* crontab configuration.
* hostname - this will need to be changed on every machine.
* git hooks.
* The standard bash library.
* The required kernel modules.
* The scripts to deploy the settings.

## Instructions

* Ensure public key ssh login for the target machine is enabled.
Set .ssh/config to contain the following entry:
	- Where {user name} is your name on the host. Ensure this has read/write access to the git configuration repository.
	- Where {host name} is the name of the host, and is usually used for the {alias}.
```
Host {alias}
	HostName	{host name}
	User		{user name}
		IdentityFile	~/.ssh/id_ed25519_pnet
		IdentitiesOnly	yes
```

* Go to the projects folder and clone the target machine configuration repository.
```
cd Projects
git clone {alias}:/srv/git/config.git {host name}.config
```

* Copy the relevant files into this host configuration repository. Overwrite if required.
* Carefully remove any artefacts. These will be deleted or renamed files.
* Commit and push changes.
* Changes on the "main" branch will trigger an automatic deployment to /usr/local/src/config.d

## Dependencies

* Ubuntu 20.04
* Public key ssh login to target machine.
