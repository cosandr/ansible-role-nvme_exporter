# ansible-role-nvme_exporter

![GitHub](https://img.shields.io/github/license/cosandr/ansible-role-nvme_exporter) ![GitHub last commit](https://img.shields.io/github/last-commit/cosandr/ansible-role-nvme_exporter) ![GitHub issues](https://img.shields.io/github/issues-raw/cosandr/ansible-role-nvme_exporter)

**Ansible role for setting up [nvme_exporter](https://github.com/cosandr/nvme_exporter).**

## Supported Platforms

| OS Family | Distribution  | Latest | Supported Version(s) | Comment |
|-----------|---------------|--------|----------------------|---------|
| RedHat    | RHEL          | :heavy_check_mark: | 9 | |
|           | RockyLinux    | :heavy_check_mark: | 8, 9 | |
|           | AlmaLinux     | :heavy_check_mark: | 8, 9 | |
|           | Fedora        | :heavy_check_mark: | 35, 36, 37 | |

## Requirements

Ansible 2.12 or higher.

## Variables

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `nvme_exporter_version` | latest | Set specific version, without `v` prefix |
| `nvme_exporter_listen_address` | :9998 | Set exporter listen address |


## Example Playbook

```yaml
---

- hosts: all
  become: true
  gather_facts: true
  roles:
    - role: ansible-role-nvme_exporter
```

## Author

[Andrei Costescu](https://github.com/cosandr/)
