# Deploy LAMP with Ansible
This repository contains Ansible playbooks for practicing the deployment of LAMP (Linux, Apache, MariaDB, PHP) on RHEL 9.

## Requirements
* ansible-core 2.14+
* Control Node: RHEL 8.8+
* Managed Nodes: RHEL 9.2+

## Quick Start
1. Download the community.mysql collection.
```bash
$ ansible-galaxy collection install community.mysql -p ./collections
```
2. Modify the inventory.
```bash
$ vim inventory/hosts.ini
```
3. Run the Ansible playbooks.
```bash
$ ansible-playbooks -i inventory/hosts.ini lamp.yml
```