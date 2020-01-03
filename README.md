
[![Build Status](https://travis-ci.org/rkm/ansible-role-dotnet-core.svg?branch=master)](https://travis-ci.org/rkm/ansible-role-dotnet-core)
[![Ansible Galaxy](https://img.shields.io/ansible/role/45475.svg)](https://galaxy.ansible.com/rkm/dotnet_core)


# Ansible Role: .Net Core SDK/Runtime

Installs the [.NET Core SDK/Runtime](https://www.microsoft.com/net). For supported systems, see [here](meta/main.yml).


## Role Variables

Available variables are listed below, along with [default values](defaults/main.yml):

```yaml
dotnet_package: "3.0"
microsoft_key_url: "https://packages.microsoft.com/keys/microsoft.asc"
```

Currently supported SDK versions are:

- `2.1`
- `2.2`
- `3.0`

Generally, these should not be changed, but if this role is out of date, or if you need a very specific version, these can be overridden.

## Dependencies

None.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - rkm.dotnet_core
```

## License

MIT / BSD

## Author Information

This role was originally created by [Iuri Gagnidze](https://www.github.com/ocha), and modified by [Ruairidh MacLeod](https://www.github.com/rkm).
