# Ansible role resolved

![GitHub](https://img.shields.io/github/license/jam82/ansible-role-resolved) ![GitHub last commit](https://img.shields.io/github/last-commit/jam82/ansible-role-resolved) ![GitHub issues](https://img.shields.io/github/issues-raw/jam82/ansible-role-resolved)

**Ansible role for setting up systemd-resolved.**

## Description

This role installs and configures systemd-resolved on the targeted host(s).


## Prerequisites

This role has no special prerequisites.

### System packages (Fedora)

- `python3` (Python 3.8 or later)

### Python (requirements.txt)

- ansible >= 2.15

## Dependencies (requirements.yml)

```yaml
collections:
  - community.general

roles: []
```

## Supported Platforms

| OS Family | Distribution | Version | Container Image |
|-----------|--------------|---------|-----------------|
| RedHat | AlmaLinux | latest | [jam82/molecule-almalinux:latest]( https://hub.docker.com/r/jam82/molecule-almalinux ) |
| Archlinux | Archlinux | latest | [jam82/molecule-archlinux:latest]( https://hub.docker.com/r/jam82/molecule-archlinux ) |
| Debian | Debian | latest | [jam82/molecule-debian:latest]( https://hub.docker.com/r/jam82/molecule-debian ) |
| RedHat | Fedora | latest | [jam82/molecule-fedora:latest]( https://hub.docker.com/r/jam82/molecule-fedora ) |
| Suse | openSUSE Leap | latest | [jam82/molecule-opensuse-leap:latest]( https://hub.docker.com/r/jam82/molecule-opensuse-leap ) |
| Debian | Ubuntu | latest | [jam82/molecule-ubuntu:latest]( https://hub.docker.com/r/jam82/molecule-ubuntu ) |

## Role Variables

No role default variables specified, see [defaults/main.yml](defaults/main.yml).

## Example Playbook

Example playbooks(s) that show how to use this role.

## Simple example playbook

A simple default example playbook for using jam82.resolved.
```yaml
---
# name: "jam82.resolved"
# file: "playbook_resolved.yml"

- name: "PLAYBOOK | resolved"
  hosts: "resolved_hosts"
  gather_facts: true
  roles:
    - role: "jam82.resolved"
```

## Author(s) and License

- :octocat:                 Author::    [jam82](https://github.com/jam82)
- :triangular_flag_on_post: Copyright:: 2024, Jonas Mauer
- :page_with_curl:          License::   [MIT](LICENSE)


---
