ansible-role-laniakea-galaxy
============================

Ansible role to install Galaxy 20.01 using roles developed by the Galaxy community.


Requirements
------------

Required roles:
 
- galaxyproject.galaxy
- galaxyproject.nginx
- galaxyproject.postgresql
- galaxyproject.proftpd
- geerlingguy.pip
- natefoo.postgresql_objects
- uchida.miniconda
- usegalaxy_eu.certbot
- usegalaxy_eu.galaxy_systemd

### Ansible-version

**tested with** : Ansible 2.9.10

Role Variables
--------------


Dependencies
------------


Example Playbook
----------------

     ---
     
     - hosts: galaxyservers
       become: true
       vars:
         GALAXY_ADMIN_USERNAME: ""
         GALAXY_ADMIN_PASSWORD: ""
         GALAXY_ADMIN_API_KEY: ""
         GALAXY_ADMIN_EMAIL: ""
       roles:
         - ansible-role-laniakea-galaxy



License
-------
Apache Licence v2

http://www.apache.org/licenses/LICENSE-2.0


Author Information
------------------
Pietro Mandreoli email: pietro.mandreoli@unimi.it
