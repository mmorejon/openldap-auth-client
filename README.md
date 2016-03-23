openldap-auth-client
=========

[![Ansible Role](https://img.shields.io/badge/ansible--galaxy-mmorejon.openldap--auth--client-blue.svg)](https://galaxy.ansible.com/mmorejon/openldap-auth-client)
[![Build Status](https://travis-ci.org/mmorejon/openldap-auth-client.svg?branch=master)](https://travis-ci.org/mmorejon/openldap-auth-client)

Ansible role for clients authentication into OpenLdap.

Requirements
------------

Currently working with Debian/Ubuntu.

Role Variables
--------------

### base
The distinguished name of the search base.

### uri
Another way to specify your LDAP server is to provide an url.

### rootbinddn
The distinguished name to bind to the server with if the effective user ID is root. Password is stored in /etc/ldap.secret (mode 600)

### port
The port by default is 389.


Dependencies
------------

No.

Example Playbook
----------------

Here's an example playbook.

    - hosts: all
      roles:
         - { role: mmorejon.openldap-auth-client }

License
-------

GPLv2

Author Information
------------------

Created by Manuel Morejón. 
