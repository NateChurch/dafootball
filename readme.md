# daFootball

This is the build script for a desktop computer converted to a ubuntu 18.04 server to be used as a collaboration platform for a data and analytics charity hackathon by Chevron Modeling and Analytics team for BakerRipley. Special thanks to Microcenter(in Houston off safe) for giving us a discount on the computer.

## Target
- Docker
- Shiny with R Server
- Anaconda with Jupyter
- Microsoft SQL Server for Linux

## Commands Run on server
```console       

    1  sudo apt install ssh
    2  service ssh status
    3  hostnamectl
    4  sudo hostnamectl set-hostname dafootball
    5  ls /etc/cloud/cloud.cfg
    6  ls /etc/cloud/
    7  hostnamectl
    8  sudo nano /etc/hosts
    9  sudo apt-get install software-properties-common
   10  sudo apt-add-repository ppa:ansible/ansible
   11  sudo apt-get update
   12  sudo apt-get install ansible
   13  history
   14  ls
   15  cd /
   16  ls
   17  cd tmp
   18  ssh-keygen -t rsa -b 4096
   19  cat /home/ds/.ssh/id_rsa.pub
   20  history

   ```

## Ansible Roles
Installing a copy of geerlingguy\ansible-role-docker (https://github.com/geerlingguy/ansible-role-docker)