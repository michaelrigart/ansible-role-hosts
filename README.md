Ansible Hosts Role
==================

An ansible role for configuring the /etc/hosts file. It will automatically set your default ipv4 and ipv6 address using the inventory_hostname and inventory_hostname_short variables.
All extra hosts need to be listed in the variables below.

Role Variables
--------------

- hosts_ipv4: array of ipv4 hosts containing a dict with the IP and FQDN
- hosts_ipv6: array of ipv6 hosts containing a dict with the IP and FQDN

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: MichaelRigart.hosts }

License
-------

GPLv3

Author Information
------------------

Michaël Rigart <michael@netronix.be>