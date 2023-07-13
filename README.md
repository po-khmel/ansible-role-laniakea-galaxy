# Laniakea Galaxy

Ansible role to install Galaxy 22.05 using roles developed by the Galaxy community.

## Requirements

Required roles:

- src: galaxyproject.galaxy
  version: 0.10.4
- src: galaxyproject.nginx
  version: 0.7.0
- src: galaxyproject.postgresql
  version: 1.0.3
- src: natefoo.postgresql_objects
  version: 1.1
- src: geerlingguy.pip
  version: 2.0.0
- src: uchida.miniconda
  version: 0.3.0
- src: usegalaxy_eu.certbot
  version: 0.1.5
- name: galaxyproject.tusd
  version: 0.0.1
- src: galaxyproject.cvmfs
  version: 0.2.13

### Ansible-version

**tested with** : Ansible core 2.11.12

## Role Variables

## Dependencies

## Example Playbook

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

## License

Apache Licence v2

http://www.apache.org/licenses/LICENSE-2.0

## Author Information

Pietro Mandreoli email: pietro.mandreoli@unimi.it
