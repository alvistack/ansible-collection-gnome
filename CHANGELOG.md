# Ansible Collection for Gnome

## YYYYMMDD.Y.Z - TBC

### Major Changes

  - Upgrade minimal Ansible support to 4.0.0
  - Support Fedora 34
  - Support Ubuntu 21.04

## 20210313.1.1 - 2021-03-13

### Major Changes

  - Bugfix [ansible-lint `namespace`](https://github.com/ansible-community/ansible-lint/pull/1451)
  - Bugfix [ansible-lint `no-handler`](https://github.com/ansible-community/ansible-lint/pull/1402)
  - Bugfix [ansible-lint `unnamed-task`](https://github.com/ansible-community/ansible-lint/pull/1413)
  - Install Python package with `pipx`
  - Simplify Python dependency with system packages
  - Support RHEL 8 with Molecule
  - Support RHEL 7 with Molecule
  - Remove CentOS 8 support
  - Support CentOS 8 Stream
  - Support openSUSE Tumbleweed
  - Migrate base Vagrant box from `generic/*` to `alvistack/*`

## 4.6.0 - 2020-12-28

### Major Changes

  - Simplify Molecule scenario for vagrant-libvirt
  - Migrate from Travis CI to GitLab CI
  - Support Fedora 33
  - Remove Fedora 32 support
  - Support Ubuntu 20.10

## 4.5.0 - 2020-08-26

### Major Changes

  - Upgrade minimal Ansible Lint support to 4.3.2
  - Upgrade Travis CI test as Ubuntu Focal based
  - Upgrade minimal Ansible support to 2.10.0
  - Support openSUSE Leap 15.2

## 4.4.0 - 2020-08-12

  - Ininitial release for Ansible 2.9 or higher
  - This role was designed for:
      - Ubuntu 18.04/20.04
      - RHEL/CentOS 7/8
      - openSUSE Leap 15.1
      - Debian 10
      - Fedora 32
