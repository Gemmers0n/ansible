# Ansible

Ansible Runbooks for various components

Ansible Version: 2.2.1.0-2
needed Packages: 
    python-apt (python 2)
    python3-apt (python 3)
    aptitude (before 2.4)


execute: ansible-playbook testservers.yml --ask-become-pass

#as user
ansible -m shell -a 'free -m' testservers
#change to root
ansible --su --su-user=root --ask-su-pass -m shell -a 'free -m' testservers

