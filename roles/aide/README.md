Role Name
=========

A brief description of the role goes here.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

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

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

Files
-------
The aide.conf file was taken from github user virtadpt at: https://github.com/virtadpt/rhel-hardening/blob/master/7/aide.conf