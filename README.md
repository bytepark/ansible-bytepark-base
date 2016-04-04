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

	bytepark_base_server_packages: []
	bytepark_base_server_locale: de_DE.UTF-8
	bytepark_base_timezone: Europe/Berlin # UTC
	bytepark_base_timezone_dir: /etc/localtime

Dependencies
------------

No dependencies

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: bytepark.bytepark-base }
      vars:
        bytepark_base_server_packages: [ "screen", "cowsay"]
        bytepark_base_server_locale: de_DE.UTF-8
        bytepark_base_timezone: UTC

License
-------

MIT

Author Information
------------------

bytepark / 2016.