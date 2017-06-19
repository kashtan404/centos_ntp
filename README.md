centos_ntp
=========

This role can be used for install and configure ntp daemon.

Requirements
------------

This role requires Ansible 1.2 or higher, and platform requirements are listed in the metadata file.

Role Variables
--------------

ntp_servers:
  - "0.pool.ntp.org"
  - "1.pool.ntp.org"
  - "2.pool.ntp.org"
  - "3.pool.ntp.org"

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: centos_ntp, time_zone: "Europe/Moscow", ntp_servers: [0.pool.ntp.org, 1.pool.ntp.org]  }

License
-------

MIT

Author Information
------------------

Aleksey Demidov