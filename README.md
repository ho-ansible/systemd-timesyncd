# Ansible role: systemd-timesyncd
Keep system time synchronized with NTP servers.

## Requirements
Only tested on Debian stable, for now.

## Role Variables
+ `ntp_fallback_pool` (default: "0.pool.ntp.org 1.pool.ntp.org"):
  space-separated list of upstream NTP servers.
  Any NTP servers assigned by DHCP on any interface managed by
  systemd-networkd will take precedence over these.

## Playbooks
+ `main.yml`: apply role

## Dependencies
None.

## License
MIT

## Author Information
Sean Ho, https://github.com/ho-ansible/
