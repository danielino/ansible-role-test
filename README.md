## ansible_role_test


simple role that show the conditional execution of role dependencies defined in meta/main.yml


Role Name
=========

ansible-role-test

Requirements
------------

- Enterprise Linux

Role Variables
--------------

- execute_dependencies (enable run of dependencies in meta/main.yml[dependencies]

Dependencies
------------

- ioggstream.debug 

	this role is executed only when variable **execute_dependencies** is defined and it value is true

Example Playbook
----------------

```
- hosts: test
  gather_facts: no
  roles:
    - danielino.ansible_role_test
```


