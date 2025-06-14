# Ansible Role: Alacritty

[![CI](https://github.com/pluggero/ansible-role-alacritty/actions/workflows/ci.yml/badge.svg)](https://github.com/pluggero/ansible-role-alacritty/actions/workflows/ci.yml) [![Ansible Galaxy downloads](https://img.shields.io/ansible/role/d/pluggero/alacritty?label=Galaxy%20downloads&logo=ansible&color=%23096598)](https://galaxy.ansible.com/ui/standalone/roles/pluggero/alacritty)

An Ansible Role that installs a basic configuration of the Alacritty Terminal.

## Requirements

Requires a compatible Rust toolchain to build Alacritty from source; Recommended role: `pluggero.rustup`.
Requires a compatible font; Recommended role: `pluggero.nerdfonts`.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
alacritty_version: "x.x"
```

The version of alacritty to install can be defined in the variable `alacritty_version`.

```yaml
alacritty_install_method: "dynamic"
```

The method used to install alacritty can be defined in the variable `alacritty_install_method`.
The following methods are available:

- `source`: Installs alacritty from source
- `package`: Installs alacritty from the package manager of the distribution
  - **NOTE**: This method installs the latest version available in the package manager and not the version defined in `alacritty_version`.
- `dynamic`: Installs alacritty from package manager if available in the correct version, otherwise installs from source

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
