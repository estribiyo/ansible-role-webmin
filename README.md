# Ansible Role: webmin

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-artfulbodger.webmin-5bbdbf.svg)](https://galaxy.ansible.com/artfulbodger/webmin/)

## Description

Webmin installation for Debian.

## Requirements

### Ansible

* This role is developed and tested with versions 2.12
* You will need to run this role as a root user using Ansible's `become` parameter. Make sure you have set up the appropriate permissions on your target hosts.

## Installation

### Ansible Galaxy

Use `ansible-galaxy install artfulbodger.webmin` to install the latest stable release of the role on your system.

## Role Variables

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) and are listed in the table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| webmin_version | 1.983 | Webmin package version.  Also accepts latest as parameter.|
| webmin_port | 10000 | TCP port on which webmin will listen |


## Example Playbook

Use it in a playbook as follows:

    - hosts: webservers
      roles:
         - { role: artfulbodger.webmin, webmin_version: '1.970', webmin_port: '9000'}