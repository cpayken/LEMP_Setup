# LEMP_Setup
LEMP Stack for Ubuntu 22.04

# Customize Options
nano vars/default.yml

# vars/default.yml
---
###### mysql_root_password: the password for the MySQL root account.
###### http_host: your domain name, host name, or ip address.
###### http_conf: the name of the configuration file that will be created within nginx.
###### http_port: HTTP port, default is 80.
###### Uncomment lines 92-95 if you wish to use UFW.

# Run the playbook
ansible-playbook -l [target] -i [inventory file] -u [remote user] lemp-setup.yaml
