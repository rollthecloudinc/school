# Pulumi Role

This Ansible role installs Pulumi on Pop!_OS or other Debian-based systems.

## Requirements

- Ansible 2.9 or higher
- Root access to the target system

## Role Variables

None required by default.

## Example Playbook

```yaml
- hosts: localhost
  become: yes
  roles:
    - pulumi
