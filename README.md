# Ansible playbooks for Kubernetes setup

## Prerequisites

* [Ansible](https://ansible.com)
* VM or real machine with freshly installed [Debian](https://www.debian.org/distrib/) OS

## Usage examples

* Setup a single node Kubernetes:

        ansible-playbook kubernetes-single-node.yml -e target=<remote-server-ip> -u <remote-user>
