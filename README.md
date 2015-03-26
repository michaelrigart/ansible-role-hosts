Ansible Hosts Role
==================
[![Build Status](https://travis-ci.org/michaelrigart/ansible-role-hosts.svg?branch=master)](https://travis-ci.org/michaelrigart/ansible-role-hosts)

An ansible role for configuring the /etc/hosts file. It will automatically set your default ipv4 and ipv6 address using the inventory_hostname and inventory_hostname_short variables.
All extra hosts need to be listed in the variables below.

Role Variables
--------------

```yaml
- hosts_ipv4: array of ipv4 hosts containing a dict with the IP and FQDN
- hosts_ipv6: array of ipv6 hosts containing a dict with the IP and FQDN
```

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
     - { role: MichaelRigart.hosts, sudo: Yes }
```

License
-------

GPLv3

Author Information
------------------

Michaël Rigart <michael@netronix.be>