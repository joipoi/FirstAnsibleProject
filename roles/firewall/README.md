firewalld
=========
Installs and configures firewalld.
Also gives option to configure a custom firewalld zone and set it as default

Role Variables
--------------
```yaml
use_custom_default_zone: false
custom_zone_name: custom_zone
custome_zone_services: []
custom_zone_ports: []
```
Dependencies
------------
This role is expected to be used with the other roles in this github repo.
It might not work as a standalone role