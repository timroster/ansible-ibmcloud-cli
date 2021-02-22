IBM Cloud CLI - 2021
=========

This role installs the full IBM Cloud CLI and some of the most commonly used plugins for the provided user. For more information on what is installed, please see [installing the IBM Cloud CLI](https://cloud.ibm.com/docs/cli?topic=cli-getting-started)

Requirements
------------

Tested on CentOS 8 stream. Presumes linux and systemd platforms in general. This role can be run as the target user (see `user` variable) on the managed system iff the user can sudo to root.

Role Variables
--------------

An **existing** OS platform user for installing the plugins must be provided for the `user` variable.

Dependencies
------------

None

Example Playbook
----------------

Apply this role using:

    - hosts: servers
      roles:
         - { role: timroster.ibmcloud_cli, user: youruser }

License
-------

Apache

Author Information
------------------

Tim Robinson, IBM
