# ansible-role-laniakea-galaxy

Ansible Role to install Galaxy 20.01

Minimal playbook:       
	---

	- hosts: galaxyservers
  	  become: true
  	  roles:
	    - ansible-role-laniakea-galaxy
