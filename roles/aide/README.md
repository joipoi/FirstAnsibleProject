Aide
=========
Installs and configures AIDE.
Also creates a cronjob to run "aide --check"

Role Variables
--------------
```yaml
aide_DBDIR: /var/lib/aide
aide_LOGDIR: /var/log/aide
aide_cron_hour: "4"
aide_cron_weekday: "*"
```

Dependencies
------------
This role is expected to be used with the other roles in this github repo.
It might not work as a standalone role

Files
-------
The aide.conf file was taken from github user virtadpt at: https://github.com/virtadpt/rhel-hardening/blob/master/7/aide.conf