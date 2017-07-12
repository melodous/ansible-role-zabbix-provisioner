Zabbix provisioner
==================

This role initialize a zabbix server environment, for example uploading templates

Requirements
------------

Zabbix server running

Dependencies
------------

- Docker

Example Playbook
----------------

.. code::

  - hosts: servers
    roles:
      - { role: zabbix-provisioner }
