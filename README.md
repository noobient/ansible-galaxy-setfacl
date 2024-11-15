# noobient.setfacl

## Synopsys

This role lets you set the file access control list (ACL) on the specified directory.

## Parameters

| Name | Required | Example | Description |
|---|---|---|---|
| `path` | yes | `/var/www/html` | Directory to apply the ACL on. |
| `acl` | yes | `u::rwx,g::rwx,o::---,d:u::rwx,d:g::rwx,d:o::---` | ACL to apply on the directory. |

## Examples

```yml
- include_role:
    name: noobient.setfacl
  vars:
    path: '/var/www/htdocs'
    acl: 'u::rwx,g::rwx,o::---,d:u::rwx,d:g::rwx,d:o::---'
```

## Return Values

N/A

## Support

| Platform | Support | Status |
|---|---|---|
| Linter | ✅ | [![Lint](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/lint.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/lint.yml) |
| AlmaLinux 8 | ✅ | [![AlmaLinux 8](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/almalinux-8.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/almalinux-8.yml) |
| AlmaLinux 9 | ✅ | [![AlmaLinux 9](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/almalinux-9.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/almalinux-9.yml) |
| Fedora 40 | ✅ | [![Fedora 40](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/fedora-40.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/fedora-40.yml) |
| Fedora 41 | ✅ | [![Fedora 41](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/fedora-41.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/fedora-41.yml) |
| Ubuntu 20.04 | ✅ | [![Ubuntu 20.04](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/ubuntu-20.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/ubuntu-20.04.yml) |
| Ubuntu 22.04 | ✅ | [![Ubuntu 22.04](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/ubuntu-22.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/ubuntu-22.04.yml) |
| Ubuntu 24.04 | ✅ | [![Ubuntu 24.04](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/ubuntu-24.04.yml/badge.svg)](https://github.com/noobient/ansible-galaxy-setfacl/actions/workflows/ubuntu-24.04.yml) |
