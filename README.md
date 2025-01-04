# Ansible Role: Alacritty

[![CI](https://github.com/pluggero/ansible-role-alacritty/actions/workflows/ci.yml/badge.svg)](https://github.com/pluggero/ansible-role-alacritty/actions/workflows/ci.yml) [![Ansible Galaxy downloads](https://img.shields.io/ansible/role/d/pluggero/alacritty?label=Galaxy%20downloads&logo=ansible&color=%23096598)](https://galaxy.ansible.com/ui/standalone/roles/pluggero/alacritty)

An Ansible Role that installs a basic configuration of the Alacritty Terminal.

## Requirements

Requires a compatible Rust toolchain to build Alacritty from source; Recommended role: `pluggero.rustup`.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

## Dependencies

None.

## Example Playbook

```yaml
- hosts: all
  roles:
    - pluggero.alacritty
```

## License

MIT / BSD

## Author Information

This role was created in 2025 by Robin Plugge.
