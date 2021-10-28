Configure Local Postfix for Forwarding
=========


[![Build Status](https://github.com/Rheinwerk/ansible-role-local_postfix/actions/workflows/ci.yml/badge.svg)](https://github.com/Rheinwerk/ansible-role-local_postfix/actions/workflows/ci.yml)

Requirements
------------

Upstream mailserver.


Role Variables
--------------

There is one main variable that drives this role: `_local_postfix`. It is a map that contains all configuration and settings for this role.
Please see `defaults/main.yml` for details.

Dependencies
------------

None.


Example Playbook
----------------

The general contract of this role is to take the variables map `_local_postfix` from `defaults/main.yml` as a template for your configuration and pass that configuration as a parameter to this role.

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      var:
        LOCAL_POSTFIX
          ...
      roles:
         - { role: local_postfix, tags: [ 'local_postfix' ], _local_postfix: "{{ LOCAL_POSTFIX }}" }

License
-------

Please see LICENSE.

Author Information
------------------

Original author is [Daniel Schneller](https://github.com/dschneller) as member of the [Rheinwerk](https://github.com/Rheinwerk) project.

