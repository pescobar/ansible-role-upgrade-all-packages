[![Build Status](https://travis-ci.org/pescobar/ansible-role-upgrade-all-packages.svg?branch=master)](https://travis-ci.org/pescobar/ansible-role-upgrade-all-packages)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-pescobar.upgrade_all_packages-blue.svg)](https://galaxy.ansible.com/pescobar/upgrade_all_packages)


ansible-role-upgrade-all-packages
=========

Upgrade all packages. Optionally reboot the system if a new kernel was installed.

The default is to reboot when a new kernel is installed unless you define `upgrade_all_packages_kernel_reboot: false`

*This role is not idempotent*

Role Variables
--------------

```
upgrade_all_packages_reboot: true
```

Dependencies
------------

none

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: pescobar.upgrade_all_packages }

License
-------

GPLv3

Author Information
------------------

Pablo Escobar Lopez
