Role Name
=========

This role checks the version of ansible installed on your machine.

Requirements
------------

None

Role Variables
--------------

This is a very simple role. Tell the role what the minimum version of Ansible is that it's expected to work on. It will fail if it's not running that version... which means that you can then provision a virtualenv with the *right* version of Ansible :)

Dependencies
------------

None

Example Playbook
----------------

    - hosts: localhost
      tasks:
      - include_role:
          name: JonTheNiceGuy.version-check
        vars:
          my_ansible_version_major_min: 2
          my_ansible_version_minor_min: 2
          my_ansible_version_point_min: 2
          my_ansible_version_debug: true

License
-------

The Unlicense

Author Information
------------------

https://jon.sprig.gs | https://keybase.io/JonTheNiceGuy
