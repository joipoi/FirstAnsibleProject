# Environment
I am running Virtualbox on my windows laptop. I currently have 1 VM to be the Ansible Controller and 1 VM to be an Ansible host. Both are running rhel.

I set up 2 network adapters, one is host-only so i can ssh between the VMs and one is NAT for normal internet connections.

I am using ssh keys for authentication

# Playbooks
* **master.yml:** The main playbook that defines hosts, vars, and imports other playbooks
* **ssh.yml:** Playbook for changing ssh settings to make it more secure
* **handlePrograms.yml:** Playbook for installing/updating/removing programs or services

# Todo(possibilities)
* Create an ansible role for this project
* Add Cronjobs for scheduled tasks or playbooks, including vulnerability scans and AIDE integrity checks
* Send logging data to the ansible controller(rsyslog)
* Add custom fapolicyd rules
* Keylime
* LUKS

# To Learn
* Ansible lookup (to include files)
* How to view task progress in Ansible output (for example if you install something  and it is taking a long time)
* Using other peoples Ansible roles
* Event driven ansible

# Sources
* [redhat.com article - locking-down-sshd](https://www.redhat.com/sysadmin/locking-down-sshd)
* [redhat.com article - 5 ways to harden a new system with Ansible](https://www.redhat.com/sysadmin/harden-new-system-ansible)
* [Red hat Security hardening documentation](https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/9/html-single/security_hardening/index) 
* [Ansible docs, list of modules](https://docs.ansible.com/ansible/latest/collections/index_module.html#ansible-builtin)  
