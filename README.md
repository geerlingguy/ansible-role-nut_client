# Ansible Role: NUT Client

[![CI](https://github.com/geerlingguy/ansible-role-nut_client/actions/workflows/ci.yml/badge.svg)](https://github.com/geerlingguy/ansible-role-nut_client/actions/workflows/ci.yml)

Installs NUT client on Linux servers for Network UPS Tools power control.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
nut_client_ups: nut-server
nut_client_server: 127.0.0.1
nut_client_username: observer
nut_client_password: password_here
```

Controls the `nut-client` primary server access options.

```yaml
nut_client_state: started
nut_client_enabled: true
```

Controls the `nut-client` service options.

## Dependencies

None.

## Example Playbook

    - hosts: servers
      become: true
      roles:
        - geerlingguy.nut_client

## License

GPLv3

## Author Information

This role was created in 2025 by [Jeff Geerling](https://www.jeffgeerling.com/), author of [Ansible for DevOps](https://www.ansiblefordevops.com/).
