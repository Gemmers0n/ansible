# Ansible

Ansible Runbooks for various components

Ansible Version: 2.7.6.1-2

sudo echo 'deb http://ppa.launchpad.net/ansible/ansible/ubuntu trusty main' > /etc/apt/sources.list.d/ansible.list
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 93C4A3FD7BB9C367
sudo apt-get update
sudo apt-get install ansible python3-apt sshpass -y --allow-unauthenticated

sudo apt-get install git -y
sudo rm -Rf /etc/ansible/*
sudo git clone https://github.com/Gemmers0n/ansible /etc/ansible/


#as user
ansible -m shell -a 'free -m' testservers
#change to root
ansible --su --su-user=root --ask-su-pass -m shell -a 'free -m' testservers
#playbook run
ansible-playbook testservers.yml --ask-become-pass --ask-pass
