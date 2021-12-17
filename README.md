Ansible Role: webmin
=========
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

Description
------------

Webmin installation for Debian.

Requirements
------------

- Ansible >= 2.7

Role Variables
--------------

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) and are listed in the table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| webmin_version | 1.983 | Webmin package version.  Also accepts latest as parameter.|
| webmin_port | 10000 | TCP port on which webmin will listen |


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }