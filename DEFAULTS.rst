.. vim: foldmarker=[[[,]]]:foldmethod=marker

zabbix-provisioner ansible role default variables
=================================================

.. contents:: Sections
   :local:

zabbix management
-----------------

.. envvar:: zabbix_user

   Zabbix server user login to access the API

::

  zabbix_user: Admin




.. envvar:: zabbix_password

   Zabbix password for login to API

::

  zabbix_password: zabbix




.. envvar:: zabbix_server

   Zabbix server url
   ::

     zabbix_server: http://localhost





zabbix configurations
---------------------

.. envvar:: zabbix_templates

   List with all templates to upload

::

  zabbix_templates:
    - zbx_export_redis.xml
    - zbx_export_os_project.xml
    - zbx_export_logstash.xml
    - zbx_export_es_env.xml
    - zbx_export_es_app.xml



