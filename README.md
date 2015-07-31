# Atomic Enterprise Ansible

This repo contains Ansible code for Atomic Enterprise.

## Setup
- Install base dependencies:
  - Fedora:
  ```
    yum install -y ansible rubygem-thor rubygem-parseconfig util-linux
  ```
   - OSX:
  ```
    # Install ansible and python 2
    brew install ansible python
    # Required ruby gems
    gem install thor parseconfig
  ```
- Setup for a specific cloud:
  - [AWS](README_AWS.md)
  - [GCE](README_GCE.md)
  - [local VMs](README_libvirt.md)

- Bring your own host deployments:
  - [Atomic Enterprise](README_AEP.md)

- Build
  - [How to build the atomic-enterprise-ansible rpms](BUILD.md)

- Directory Structure:
  - [bin/cluster](bin/cluster) - python script to easily create Atomic Enterprise clusters
  - [docs](docs) - Documentation for the project
  - [filter_plugins/](filter_plugins) - custom filters used to manipulate data in Ansible
  - [inventory/](inventory) - houses Ansible dynamic inventory scripts
  - [playbooks/](playbooks) - houses host-type Ansible playbooks (launch, config, destroy, vars)
  - [roles/](roles) - shareable Ansible tasks

## Contributing
