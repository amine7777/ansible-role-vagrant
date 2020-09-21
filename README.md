Ansible role: Vagrant
=========

This role helps you to install vagrant on your linux machine.


|Travis|CircleCI|GitHub|Quality|Downloads|Version|
|------|--------|------|-------|---------|-------|
|[![travis](https://travis-ci.com/amine7777/ansible-role-vagrant.svg?branch=master)](https://travis-ci.com/amine7777/ansible-role-vagrant)|![circleci](https://circleci.com/gh/amine7777/ansible-role-vagrant.svg?style=svg)|[![github](https://github.com/amine7777/ansible-role-vagrant/workflows/CI/badge.svg)](https://github.com/amine7777/ansible-role-vagrant/actions)|[![quality](https://img.shields.io/ansible/quality/50864)](https://galaxy.ansible.com/amine7777/vagrant)|[![downloads](https://img.shields.io/ansible/role/d/50348)](https://galaxy.ansible.com/amine7777/vagrant)|[![Version](https://img.shields.io/github/release/amine7777/ansible-role-vagrant.svg)](https://github.com/amine7777/ansible-role-vagrant/releases/)|

![](vagrant.jpg)

Requirements
------------
- Linux machine
- Ansible 2.9

Role Variables
--------------
These variables helps to manage vagrant installation.

You can specify your vagrant version in this variable.
```yaml
vagrant_version: 2.2.2
```
This is the url where vagrant will be downloaded.
```yaml
vagrant_download_url: https://releases.hashicorp.com/vagrant/{{ vagrant_version }}/{{ vagrant_package_name }}
```
This is vagrant the package name.
```yaml
vagrant_package_name: vagrant_{{ vagrant_version }}_x86_64
```

Example Playbook
----------------

```yaml
- hosts: all
  roles:
     - amine7777.vagrant
```


Author Information
------------------

- [Amine Kahlaoui](https://github.com/amine7777), DevOps engineer.
