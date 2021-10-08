# msys2-ansible

A real basic ansible playbook to configure msys2 environment

## Context

Sometimes you work in a very constrained environment (windows) without admin rights on your machine.

You cannot use WSL2 (forbidden by your company policies) but you would still like using common Linux/GNU tool.

You are also alergic to Putty and prefer the command line for SSH into your favorites servers.

## Installation

### Requirement

- Ansible >= 2.9
- [msys2](https://www.msys2.org/) on your local folder
- `python3` and `pip3` packages

```
pacman -S ansible python3 python3-pip
```

### Install roles

```shell
cd ansible
ansible-galaxy role install -r galaxy.yml --force -p roles
```