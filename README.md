[![Build Status](https://travis-ci.org/fireeye-ops/ansible-role-base.svg?branch=master)](https://travis-ci.org/fireeye-ops/ansible-role-base)
[![Galaxy Role](https://img.shields.io/badge/ansible--galaxy-base-blue.svg)](https://galaxy.ansible.com/fireeye-ops/base/)

fireeye-ops.base
=========

Base configuration for FireEye Labs Linux hosts

Role Variables
--------------

|Name|Type|Description|Default|
|----|----|-----------|-------|
`base_packages`|List|OS Packages to install|[]
`base_edit_hosts`|Boolean|Inserts an entry into /etc/hosts for host's public IP|false

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      roles:
         - { role: fireeye-ops.base, base_packages: [ 'ngrep' ] }
