Kubernetes-Init-Flannel Role
=========

Initialize Kubernetes cluster with Flannel pod network

Dependencies
------------

* swapoff
* kubernetes-install
* docker-install

Example Playbook
----------------

    - hosts: servers
      roles:
         - swapoff
         - kubernetes-install
         - kubernetes-init-flannel

License
-------

MIT
