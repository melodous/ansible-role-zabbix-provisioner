Welcome to zabbix-provisioner Ansible Role’s documentation!
===========================================================

Zabbix provisioner
------------------

This role initialize a zabbix server environment, for example uploading
templates

### Requirements

Zabbix server running

### Dependencies

-   Docker

### Example Playbook

    - hosts: servers
      roles:
        - { role: zabbix-provisioner }

zabbix-provisioner ansible role default variables
-------------------------------------------------

#### Sections

-   zabbix management
-   zabbix configurations

### zabbix management

`zabbix_user`

> Zabbix server user login to access the API

    zabbix_user: Admin

`zabbix_password`

> Zabbix password for login to API

    zabbix_password: zabbix

`zabbix_server`

> Zabbix server url
>
>     zabbix_server: http://localhost

### zabbix configurations

`zabbix_templates`

> List with all templates to upload

    zabbix_templates:
      - zbx_export_redis.xml
      - zbx_export_os_project.xml
      - zbx_export_logstash.xml
      - zbx_export_es_env.xml
      - zbx_export_es_app.xml
      - zbx_export_postgres.xml

Changelog
---------

**zabbix-provisioner**

This project adheres to Semantic Versioning and human-readable
changelog.

### zabbix-provisioner master - unreleased

##### Added

-   First addition

##### Changed

-   First change

### zabbix-provisioner v0.0.3 - 2017/07/17

##### Added

-   Added potsgresql templates

### zabbix-provisioner v0.0.2 - 2017/07/13

##### Added

-   Fixed ansible-lint warnings

### zabbix-provisioner v0.0.1 - 2017/07/12

##### Added

-   Initial version

Copyright
---------

zabbix-provisioner

Copyright (C) DATE Raúl Melo &lt;<raul.melo@opensolutions.cloud>&gt;

LICENSE
