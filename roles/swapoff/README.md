Swapoff Role
=========

Disable swap, since Kubernetes will not run if it's enabled

Example Playbook
----------------

    - hosts: servers
      roles:
         - swapoff

License
-------

MIT
