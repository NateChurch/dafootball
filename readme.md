# daFootball

This is the build script for a desktop computer converted to a ubuntu 18.04 server to be used as a collaboration platform for a data and analytics charity hackathon by Chevron Modeling and Analytics team for [BakerRipley](https://bakerripley.org/). Special thanks to Microcenter(in Houston) for giving the Chevron Modeling and Analytics team a discount on the computer which we dontated to the team at BakerRipley after the event was complete. The computer was used as a network server for Chevron employees to create and share the work done with Baker Ripley.

As of September 2024, I am marking this as archive because you shouldn't be using Ubuntu 18.04 any more. 

## Target
- Docker
- Shiny with R Server
- Anaconda with Jupyter
- Microsoft SQL Server for Linux

## Install Method
On a 18.04 Bionic Beaver, install ansible and then run an ansible pull

## Commands Run on server
```console       

sudo apt install ssh
service ssh status
hostnamectl
sudo hostnamectl set-hostname dafootball
ls /etc/cloud/cloud.cfg
ls /etc/cloud/
hostnamectl
sudo nano /etc/hosts
sudo apt-get install software-properties-common
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible
ssh-keygen -t rsa -b 4096
cat /home/ds/.ssh/id_rsa.pub
sudo ansible-pull -U https://github.com/NateChurch/dafootball.git --full -vvvv pullrequirements.yml
sudo ansible-pull -U https://github.com/NateChurch/dafootball.git --full -vvvv
   ```

## Ansible Roles
Installing a copy of geerlingguy\ansible-role-docker (https://github.com/geerlingguy/ansible-role-docker)
