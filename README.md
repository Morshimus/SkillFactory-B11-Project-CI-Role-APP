Django
=========

Role for installing software Skillfactory

Requirements
------------

[Infrastructure](https://github.com/Morshimus/SkillFactory-B11-Project-CI-Role-INFRA)

Role Variables
--------------

**pg_fqdn**<br>  - *fully qulified domain name or ip address of pg instance| typr string*
</br>

**pg_port**<br> - *port of pg instance | type insteger*
</br>

**pg_db_user**<br> - *pg db user| type string*
</br>

**pg_db_user_password**<br> - *pg db user's password| type sensetive-string*
</br>

**pg_db_name** - *pg db name| type string*
</br>

**django_app_root**<br>  - *django app root folder| type string*
</br>

**django_app_static**<br> - *django app static folder| type string*
</br>

**django_app_templates** <br> - *djangi app templates folder| type string*
</br>

**pg_version**<br> - *pg instance version| type string*
</br>

**container_name**<br> - *docker container name| type string*
</br>

**container_port**<br> - *docker container port for expose| type integer*
</br>

**is_local**<br> - *type of installation, is pg instant locates locally ot remote?| typr boolean*
</br>

Dependencies
------------

[Infrastructure](https://github.com/Morshimus/SkillFactory-B11-Project-CI-Role-INFRA)

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: app
      roles:
         - role: django
           vars:
             pg_fqdn: "172.17.0.1"
             pg_port: "5432"
             pg_db_user: "django"
             pg_db_user_password: "test123"
             pg_db_name: "django_test"
             django_app_root: /srv/app/tst
             django_app_static: /srv/app/tst/static/polls
             django_app_templates: /srv/app/tst/templates/polls
             pg_version: "14"
             container_name : "sf_web_tst"
             container_port: "8001"
             is_local: true

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
