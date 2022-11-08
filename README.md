# LEMP_Setup
LEMP Stack for Ubuntu 22.04

# Customize Options
nano vars/default.yml

#vars/default.yml
---
mysql_root_password: "mysql_root_password"
http_host: "your_domain"
http_conf: "your_domain.conf"
http_port: "80"

# mysql_root_password: the password for the MySQL root account.
# http_host: your domain name.
# http_conf: the name of the configuration file that will be created within nginx.
# http_port: HTTP port, default is 80.

# Run the playbook
ansible-playbook -l [target] -i [inventory file] -u [remote user] lemp-setup.yaml
