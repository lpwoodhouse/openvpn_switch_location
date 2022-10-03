# Ansible play: switch_location

### <sub-heading>

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

MIT

## Author Information

This role was created in 2022 by [Lee Woodhouse](https://www.leewoodhouse.com/)
