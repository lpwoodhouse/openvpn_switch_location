# Ansible playbook: openvpn_switch_location
![GitHub last commit](https://img.shields.io/github/last-commit/lpwoodhouse/playbook_openvpn_switch_location)
![GitHub repo file count](https://img.shields.io/github/directory-file-count/lpwoodhouse/playbook_openvpn_switch_location)
![GitHub top language](https://img.shields.io/github/languages/top/lpwoodhouse/playbook_openvpn_switch_location)

## Purpose

This play is for switching ExpressVPN connection locations configured on the linux openvpn client

## Requirements

None

## Role Variables

Available variables are listed below, along with default values (see ```defaults/main.yml```)
```shell
service: openvpn-client@client #openvpn@client on debian based distros
config_file: /etc/openvpn/client/client.conf #/etc/openvpn/client.conf on debian based distros

location: <expressvpn_connection_location>
# location examples include: usa-sanfrancisco, usa-washingtondc, usa-denver, canada-montreal, uk-london, switzerland, hongkong-1, india-sg, malaysia
```
## Dependencies

None

## Example Playbook
```yaml
    - hosts: all
      roles:
        - switch_location
```

## License

[![GitHub](https://img.shields.io/github/license/lpwoodhouse/playbook_openvpn_switch_location)](LICENSE)

## Author Information

This playbook was created in 2022 by [Lee Woodhouse](https://www.leewoodhouse.com/)
