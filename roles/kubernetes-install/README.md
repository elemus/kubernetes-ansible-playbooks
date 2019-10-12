Kubernetes-Install Role
=========

Install kubelet, kubeadm, kubectl and kubernetes-cni network plugin

Dependencies
------------

* common
* swapoff

Example Playbook
----------------

    - hosts: servers
      roles:
         - kubernetes-install

License
-------

MIT
