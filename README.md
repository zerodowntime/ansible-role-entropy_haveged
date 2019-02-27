# entropy_haveged

Increase the entropy available in the system

## Installation

```yaml
   ansible-galaxy install zerodowntime.epel_repo
   ansible-galaxy install zerodowntime.entropy_haveged
```

## Requirements

This role requires Ansible 2.5 or higher.

Supported platforms:

```yaml
  platforms:
    - name: EL
      versions:
        - 7
    - name: Ubuntu
      versions:
        - xenial
```

## Default role variables

| Variable name                  | Required? |  Type  | Description             |
|:------------------------------ |:---------:|:------:|:----------------------- |
| entropy_haveged__package_state |    yes    | string | installed package state |

**All variables are described in [defaults/main.yml](defaults/main.yml) file.**

## Static role variables

| Variable name                 |  Type  | Description            |
|:----------------------------- |:------:|:---------------------- |
| entropy_haveged__package_name | string | installed package name |
| entropy_haveged__service_name | string | service name           |

**All static variables are described in [vars/main.yml](vars/main.yml) file.**

## Example Playbook

```yaml
- hosts: all
  become: true
  roles:

  - role: zerodowntime.entropy_haveged
```

## License

[Apache License 2.0](LICENSE)

## Support

ansible@zerodowntime.pl
