# vagrant_project_c

## Description:
This repository provides to you **2 Ubuntu Xenial Webservers and 1 Ubuntu Xenial Mysql Server** configured as follows:
- hostaname **web01**, **web02** and **mysql**
- **nginx** installed on web01 and web02 boxes
- **mysql-server** installed on mysql box

## Files:
- `Vagrantfile` - Contain all boxes configuration

## Requiered software:

- In order to use Vagrant you need to have **Virtualbox** tool installed.
- In order to use the already configured **Vagrantfile** you require **Vagrant** tool installed.

## Install Section:
**Note that following instructions have been tested in Ubuntu**

### Instructions HOW to install `Virtualbox`
- Go to [Virtualbox downloads](https://www.virtualbox.org/wiki/Linux_Downloads) choose **Virtualbox** package
- Type in your terminal: `sudo apt-get install -y virtualbox `

### Instructions HOW to install `Vagrant`
- Download **Vagrant** from [here](https://www.vagrantup.com/downloads.html)
- Click on following link: [Installing vagrant](https://www.vagrantup.com/docs/installation/)

### Instructions HOW to run this project on your computer
- Download the content of **berchev/vagrant_project_c** repository: `git clone https://github.com/berchev/vagrant_project_c.git`
- Change to downloaded **vagrant_project_c** directory: `cd vagrant_project_c`
- Type `vagrant up` and wait the command to finish (Note that it can take up to 10 minutes, depending on your internet connection)
- Type `vagrant status` in order to verify that all machines are running and ready for use. If everything is OK, you should see:
  ```
    Current machine states:

  web01                      running (virtualbox)
  web02                      running (virtualbox)
  mysql                      running (virtualbox)

  This environment represents multiple VMs. The VMs are all listed
  above with their current state. For more information about a specific
  VM, run `vagrant status NAME`
  ```
- Type `vagrant ssh <vm_name>` in order to connect to desired server via ssh.
- Type `exit` in order to close the ssh connection
- Type `vagrant halt <vm_name>` in order to power off desired Ubuntu Xenial Box
- Type `vagrant destroy` if this project is no longer needed

### TODO
