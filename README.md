Role Name
=========

Role vector

Requirements
------------

Role Variables
--------------

  The version of vector:
    vector_version: 0.21.1
  
  Change server name:
      vector_conf_endpoint: http://{{ hostvars['vector-01'].ansible_default_ipv4.address }}:8123

Dependencies
------------

Example Playbook
----------------


    - name: Install Vector
      hosts: vector
      roles:
        - vector

License
-------

MIT

Author Information
------------------

Matemaaan
