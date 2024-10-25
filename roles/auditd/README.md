Auditd
=========
Installs and configures Auditd

Role Variables
--------------
```yaml
auditd_num_logs: 5
auditd_max_log_file: 8
auditd_max_log_file_action: ROTATE
```
Dependencies
------------

This role is expected to be used with the other roles in this github repo.
It might not work as a standalone role

Files
--------------
The Audit.rules file has been taken from @Neo23x0(Florian Roth) at https://github.com/Neo23x0/auditd/blob/master/audit.rules