## Ansible Systemconfig
Ansible Runbooks for various components.

## Tech used

<b>Built with</b>
- [Ansible 2.7.6.1-2](https://www.ansible.com)



## Installation

Install ansible
```
sudo echo 'deb http://ppa.launchpad.net/ansible/ansible/ubuntu trusty main' > /etc/apt/sources.list.d/ansible.list
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 93C4A3FD7BB9C367
sudo apt-get update
sudo apt-get install ansible python3-apt sshpass apt-transport-https socat tor -y --allow-unauthenticated
```

Paket is the connection for tor network hosts

Install git
```
sudo apt-get install git -y
sudo rm -Rf /etc/ansible/*
sudo git clone https://github.com/Gemmers0n/ansible /etc/ansible/
```

## License
This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

MIT © [Gemmers0n]()
