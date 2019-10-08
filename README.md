# Ansible playbooks for Kubernetes setup

## Prerequisites

* [Ansible](https://ansible.com)
* VM or real machine with freshly installed [Debian](https://www.debian.org/distrib/) OS

## How to use

1. Setup SSH connection to master and worker nodes
2. Add nodes hosts to the `/etc/ansible/hosts`:

```ini
[master_nodes]
master-node-host

[worker_nodes]
worker-node-host1
worker-node-host2
worker-node-host3
```

3. Run `kubernetes-cluster.yml` playbook to setup Kubernetes cluster:

```shell script
ansible-playbook kubernetes-cluster.yml
```
