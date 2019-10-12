# Ansible playbooks for Kubernetes setup

## Prerequisites

* [Ansible](https://ansible.com)
* VM or real machine with freshly installed [Debian](https://www.debian.org/distrib/) OS

## Setup a cluster

1. Setup SSH connection to master and worker nodes
2. Add nodes hosts to the `/etc/ansible/hosts`:

```ini
[master_nodes]
master-node-host ansible_user=kubernetes

[worker_nodes]
worker-node-host1 ansible_user=kubernetes
worker-node-host2 ansible_user=kubernetes
worker-node-host3 ansible_user=kubernetes
```

3. Run `kubernetes-cluster.yml` playbook to setup Kubernetes cluster:

```shell script
ansible-playbook kubernetes-cluster.yml
```

## Setup a single-node cluster

```shell script
ansible-playbook kubernetes-cluster-single-node.yml -e target=master-node-host -u kubernetes
```
