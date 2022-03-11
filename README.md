init_client
===========

This ansible role init a client for ansible with python3.
It uses the raw module of ansible to check if pyhton3 is ready to use on the system. If not, it installes the package. At the end it checks if ansible is working on the system.
Hint: The playbook needs to run with "gather_facts: no", else it will fail (without python3).


Requirements
------------

This role has no special requirements.


Role Variables
--------------

This role has no variables.


Dependencies
------------

This role has no dependencies.


Example Playbook
----------------

This role can be used e.g. with the following playbook:
```
---
- name: init client for ansible with python3
  gather_facts: no
  hosts: server
  remote_user: root
  roles:
    - christian_becker.init_client
```


License
-------

MIT


Author Information
------------------

* **Christian Becker** - [christian-becker](https://github.com/christian-becker)  

