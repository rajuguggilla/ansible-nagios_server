# ansible-nagios_server
Deploying nagios server using ansible from source tar ball
### hosts
--------
This file is located at /etc/ansible/hosts

This hosts file contains the IP address, username, key-pair path of the instance to connect and deploy the nagios server.

To execute the playbook

ansible-playbook install-nagios.yml

If we don't mention these details such as username and key-pair in the hosts file. 
      We have to provide these details while executing the playbook.

To execute with passing key-pair and username      

ansible-playbook install-nagios.yml --private-key=<PRIVATE_KEY_FILE> --user=<REMOTE_USER>
