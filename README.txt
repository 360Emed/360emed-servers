This is the playbook for configuring server environment for 360emed.

ansible-playbook -u [your user name] -k -K -e 'host_key_checking=False' -i [inventory path] playbooks/server-preconfig.yml

ansible-playbook -u [your user name] -k -K -e 'host_key_checking=False' -i [inventory path] playbooks/webserver-config.yml

ansible-playbook -u [your user name] -k -K -e 'host_key_checking=False' -i inventory/emed-web playbooks/webserver-config.yml
ansible-playbook -u [your user name] -k -K -e 'host_key_checking=False' -i inventory/emed-mysql playbooks/mysql-config.yml