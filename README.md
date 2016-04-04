[![Build Status](https://travis-ci.org/bytepark/ansible-bytepark-base.svg?branch=master)](https://travis-ci.org/bytepark/ansible-bytepark-base)

ansible-bytepark-base
=========

Ansible role to install the base for every bytepark host

Requirements
------------

No further requirements

Role Variables
--------------

Available variables are listed below, along with default values:

	bytepark-base.server_packages: []
	bytepark-base.server_locale: de_DE.UTF-8
	bytepark-base.timezone: Europe/Berlin # UTC
	bytepark-base.timezone_dir: /etc/localtime

Dependencies
------------

No dependencies

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: bytepark.bytepark-base }
      vars:
        bytepark-base.server_packages: [ "screen", "cowsay"]
        bytepark-base.server_locale: de_DE.UTF-8
        bytepark-base.timezone: UTC

License
-------

MIT

Author Information
------------------

bytepark / 2016.