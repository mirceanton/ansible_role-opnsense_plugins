OPNsense: Plugins
=================

An ansible role to manage the installed plugins on an opnSense firewall. 

Requirements
------------

This role requires the `lxml` python package to be installed on the host system.

Role Variables
--------------

|     Variable     |     Type     |                 Description                 |
| :--------------: | :----------: | :-----------------------------------------: |
| opnsense_plugins | list(string) | List of plugin names to install and enable. |

Dependencies
------------

N/A.

Example Playbook
----------------

```yaml
- name: Configure the plugins on all firewalls
  hosts: opnsense

  roles:
    - role: mirceanton.opnsense_plugins
      vars:
        opnsense_plugins:
          - os-theme-cicada
          - os-iperf
```

License
-------

MIT

Author Information
------------------

A role developed by [Mircea-Pavel ANTON](https://www.mirceanton.com).
