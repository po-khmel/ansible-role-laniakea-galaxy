Laniakea Galaxy
===============

Ansible role to install Galaxy 20.05 using roles developed by the Galaxy community.

Requirements
------------

Required roles:
 
- src: galaxyproject.galaxy
  version: 0.9.6
- src: galaxyproject.nginx
  version: 0.6.4
- src: galaxyproject.postgresql
  version: 1.0.2
- src: natefoo.postgresql_objects
  version: 1.1
- src: geerlingguy.pip
  version: 1.3.0
- src: uchida.miniconda
  version: 0.3.0
- src: usegalaxy_eu.galaxy_systemd
  version: 0.1.2

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
