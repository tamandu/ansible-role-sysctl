# ansible-role-sysctl

This role configures kernel parameters.

## Requirements

None.

## Role Variables

variable | required | default | choice | comment
-------- | -------- | ------- | ------ | -------------------
key      | yes      |         |        | name of kernel parameter
value    | yes      |         |        | value of kernel parameter

## Dependencies

None.

## Example Playbook

```yml
- hosts: servers
  roles:
    - sysctl
```

*Inside `vars/main.yml`*:  
Variables must be defined by dictionary.
```yml
sysctl:
  net.ipv6.conf.all.disable_ipv6: 1
```

## License

MIT

## Author Information
