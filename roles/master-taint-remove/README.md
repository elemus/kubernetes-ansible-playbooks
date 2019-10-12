Master-Taint-Remove Name
=========

Allow scheduling pods on master nodes

Dependencies
------------

* kubectl-install

Example Playbook
----------------

    - hosts: master_nodes
      roles:
         - master-taint-remove

License
-------

MIT
