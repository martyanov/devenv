Development environment
=======================

## Overview

As it's always cumbersome to manually setup development environment I've created this repository. It contains a number of configuration files to easily initialize and provision Ubuntu based development environment. Thanks to Vagrant and Ansible projects for great tools that made it possible.

## How to use

Assuming [Vagrant](http://docs.vagrantup.com/v2/installation/) and [Ansible](http://docs.ansible.com/intro_installation.html) are already installed it is as easy as cloning the repository and executing the following command:

```bash
vagrant up
```

Please review the contents of tasks directory to find out what's going under the hood.

Feel free to fork and edit to your needs.