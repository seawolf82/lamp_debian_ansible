# lamp_debian_ansible

To install lamp on debian 11 run:

ansible-playbook -i hosts site.yaml

To uninstall lamp on debian 11 run:

ansible-playbook -i hosts deprovision.yaml

Adding Tags to permit run only specific task of playbook

Tags:

upgrade
package
ntp
apache2
mariadb
php


For example, to launch only task regarding upgrade os, run:
 
ansible-playbook -vv --tags "upgrade" -i hosts site.yaml
# lamp_debian_ansible
