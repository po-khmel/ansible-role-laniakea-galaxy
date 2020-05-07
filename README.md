# ansible-role-ma_galaxy

Ansible Role to install Galaxy 20.01

Minimal playbook:
	---

	- hosts: galaxyservers
  	  become: true
  	  roles:
	    - ansible-role-ma_galaxy
