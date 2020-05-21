ansible-role-firewalld-forward-port
===================================

An ansible role that configures firewalld for port forwarding.

Requirements
------------

None.

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------

```yml
- name: Forward traffic to port 80 to another host
  hosts: localhost
  gather_facts: yes
  roles:
  - name: bit_kitchen.firewalld_forward_port
    self_port: 80
    dest_addr: 10.20.30.40
    dest_port: 80
    protocol: tcp
```

License
-------

[MIT](LICENSE)

Author Information
------------------

[bit.kitchen](https://github.com/bit-kitchen)
