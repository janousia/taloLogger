# taloLogger-role
Ansible role for installing olammi's taloLogger. Tested to work on Debian
squeeze (SPARC) and Raspbian (ARM) with latest ansible available from pip.

Implemented:
 - Download of taloLogger packages
 - Installation of MySQL datastore
 - Installation of taloLogger
 - Installation of taloLoggerGraph, initially for dummy data 

To-do:
 - Installation of remaining datastores
 - Configuring serial I/O data source (in separate role)
 - Split taloLoggerGraph into separate role
 - Configure graphs for additional data sources
 - nginx

# Example playbook

```
---
- hosts: all
  sudo: yes
  roles:
    - taloLogger-role
```
