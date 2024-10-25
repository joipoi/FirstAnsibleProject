# Ansible RedHat Security Hardening
This is a collection of Ansible roles that are supposed to do security hardening on a Linux RHEL machine.
It is not complete nor perfect, i am still working on it.
There are specific variables and readmes for each role.
## Example Playbook
This is what a playbook would look like if you used none of the role vars.

  ```yaml
---
- hosts: webservers
  become: true
  roles:
    - managePrograms
    - firewall
    - aide
    - auditd
    - ssh
```
