# Ansible Collection for Gnome

[![Gitlab pipeline status](https://img.shields.io/gitlab/pipeline/alvistack/ansible-collection-gnome/master)](https://gitlab.com/alvistack/ansible-collection-gnome/-/pipelines)
[![GitHub release](https://img.shields.io/github/release/alvistack/ansible-collection-gnome.svg)](https://github.com/alvistack/ansible-collection-gnome/releases)
[![GitHub license](https://img.shields.io/github/license/alvistack/ansible-collection-gnome.svg)](https://github.com/alvistack/ansible-collection-gnome/blob/master/LICENSE)
[![Ansible Collection](https://img.shields.io/badge/galaxy-alvistack.gnome-blue.svg)](https://galaxy.ansible.com/alvistack/gnome)

Ansible collection for deploying Gnome.

This Ansible collection provides Ansible playbooks and roles for the deployment and configuration of an [Gnome](https://www.gnome.org/) environment.

## Requirements

This collection require Ansible community package 4.2 or higher.

This collection was designed for:

  - Ubuntu 18.04, 20.04, 20.10, 21.04
  - CentOS 7, 8 Stream
  - openSUSE Leap 15.2, Leap 15.3, Tumbleweed
  - Debian 10, 11
  - Fedora 33, 34
  - RHEL 7, 8

## Quick Start

### Bootstrap Ansible and Roles

Start by cloning the repository, checkout the corresponding branch, and init with `git submodule`, then bootstrap Python3 + Ansible with provided helper script:

    # GIT clone the development branch
    git clone --branch develop https://github.com/alvistack/ansible-collection-gnome
    cd ansible-collection-gnome
    
    # Setup Roles with GIT submodule
    git submodule init
    git submodule sync
    git submodule update
    
    # Bootstrap Ansible
    ./scripts/bootstrap-ansible.sh
    
    # Confirm the version of Python3, PIP3 and Ansible
    python3 --version
    pip3 --version
    ansible --version

### AIO

All-in-one (AIO) build is a great way to perform an Gnome build for:

  - A development environment
  - An overview of how all the Gnome services fit together
  - A simple lab deployment

Simply execule our default Molecule test case and it will deploy all default components into your localhost:

    # Run Molecule test case
    molecule test -s default

### Molecule

You could also run our [Molecule](https://molecule.readthedocs.io/en/stable/) test cases if you have [Vagrant](https://www.vagrantup.com/) and [Libvirt](https://libvirt.org/) installed, e.g.

    # Bootstrap Vagrant and Libvirt
    ./scripts/bootstrap-vagrant.sh
    
    # Run Molecule on Ubuntu 20.04
    molecule converge -s ubuntu-20.04

Please refer to [.travis.yml](.travis.yml) for more information on running Molecule.

## License

  - Code released under [Apache License 2.0](LICENSE)
  - Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

## Author Information

  - Wong Hoi Sing Edison
      - <https://twitter.com/hswong3i>
      - <https://github.com/hswong3i>
