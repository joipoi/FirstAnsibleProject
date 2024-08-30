# Environment
I am running Virtualbox on my windows laptop. I currently have 1 VM to be the Ansible Controller and 1 VM to be an Ansible host. Both are running rhel.

I set up 2 network adapters, one is host-only so i can ssh between the VMs and one is NAT for normal internet connections.

I am using ssh keys for authentication

# Playbooks
* **master.yml:** The main playbook that defines hosts, vars, and imports other playbooks
* **ssh.yml:** Playbook for changing ssh settings to make it more secure
* **handlePrograms.yml:** Playbook for installing/updating/removing programs or services

# Questions
* How should i divide up plays, is this too split up?
* How do i keep track of problems on the hosts, should i use event-driven ansible?
* Are the following relevent for this project or important to learn: polkit, PKCS #11, System-wide cryptographic policies, FIPS, USBGuard
* When to use others Ansible roles/collections and when to use your own
* Is it bad practice to share your inventory.ini on github with all the ip-adresses?


# Todo(possibilities)
* Create a ansible role for this project
* Add Cronjobs for scheduled tasks or playbooks, including vulnerability scans and AIDE integrity checks
* send logging data to the ansible controller(rsyslog)
* Add custom fapolicyd rules
* Keylime
* LUKS

# To Learn
* Ansible lookup (to include files)
* How to view task progress in Ansible output (for example if you install something  and it is taking a long time)
* Using other peoples Ansible roles
* Event driven ansible

# Sources
* [ssh settings](https://www.redhat.com/sysadmin/locking-down-sshd)
* [disabling software & restricting ports](https://www.redhat.com/sysadmin/harden-new-system-ansible)
* [AIDE, auditd, and more](https://docs.redhat.com/en/documentation/red_hat_enterprise_linux/9/html-single/security_hardening/index) 
* [Ansible modules](https://docs.ansible.com/ansible/latest/collections/index_module.html#ansible-builtin)  
