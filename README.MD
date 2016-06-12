# Apache Toolkit

This toolkit is designed to make virtual host management more easier from command line.

## What's inside
This toolkit contains 4 utilites:
* `create-host` - Create a new virtual host (it will prepare all config's and folder)
* `delete-host` - Delete a virtual host (including files and config)
* `edit-host` - Edit host's configuration in VIM.

## Installation
* Clone this repo or go to releases tab and download suitable version.
* Open nessesary distributive folder (currently Ubuntu or CentOS/RHEL)
* Run `install` file and follow instructions on screen.

## Builds
* **ubuntu** - Release for all Ubuntu-based products.
* **linux-common** - Rest Linux systems, include only common stuff.
* **darwin** - Soon. Will include OSX build.

## Support
* Ubuntu      - Supported.
* Debian      - Experimental, may work with ubuntu's package.
* RHEL/CentOS - Supported.
* Darwin/OSX  - Soon will be available. 

## Features
* Virtual host management
* Quick configuration edit
* Creating template for new hosts
* Create dns mask for all `.loc` and `.dev` domains (only Ubuntu) **optional**

### Create virtual hosts
To create virtual host, just run `sudo create-host site.com`.
Tool will create and enable config file and directory for the site.

### Delete vitrual hosts
To edit host, use `sudo delete-host site.com`.
Also you will be prompted if you want to delete a host directory.

### Edit virtualhost configuration
To edit configuration, use `sudo edit-host site.com`.

### Edit general host configuration template
General template is stored in `/etc/apache-cli/example.conf`.
To edit it, you have to use `sudo`.

### Edit Toolkit configuration
Configuration can be found in `/etc/apache-cli/config.sh`.

## Uninstall
To remove toolkit, just run `sudo apache-cli-remove`;
