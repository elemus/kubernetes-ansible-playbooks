Cluster-Init Role
=========

Initialize Kubernetes cluster

Dependencies
------------

* swapoff
* docker-install
* kubernetes-install
* kubectl-install

Example Playbook
----------------

    - hosts: servers
      roles:
         - cluster-init

License
-------

MIT
