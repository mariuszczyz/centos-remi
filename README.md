# CentOS 7 REMI Repository Install Role

Install REMI repository.

## Requirements

None.

## Role Variables

None

## Dependencies

EPEL repository.

Can be installed via Ansible Galaxy:

`ansible-galaxy install mariuszczyz.centos-epel`

## Example Playbook

Fetch this role from Ansible Galaxy:

`ansible-galaxy install mariuszczyz.centos-remi`

In playbook.yml:

```bash
- hosts: servers
  roles:
    - { role: mariuszczyz.centos-remi, tags: ['centos-remi'] }
```

Run it:

`ansible-playbook -i hosts playbook.yml --user root --ask-pass --limit=servers`

Optionally, run just this role:

`ansible-playbook -i hosts playbook.yml --user root --ask-pass --limit=servers --tags=centos-remi`

## License

BSD

## Author Information

Author: Mariusz Czyz

Date: 09/2018
