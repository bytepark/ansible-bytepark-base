Role Name
=========

Ansible role to install the base for every bytepark host

Requirements
------------

No further requirements

Role Variables
--------------

Available variables are listed below, along with default values:

	server_packages: []
	server_locale: de_DE.UTF-8
	timezone: Europe/Berlin # UTC
	timezone_dir: /etc/localtime

Dependencies
------------

No dependencies

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: bytepark.bytepark-base }
      vars:
        server_packages: [ "screen", "cowsay"]
  		server_locale: de_DE.UTF-8
		timezone: UTC

License
-------

MIT

Author Information
------------------

bytepark / 2016.
