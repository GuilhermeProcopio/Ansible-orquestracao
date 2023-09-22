# Using Ansible and Vagrant to manage and create are VMs

## Vagrant Setup

Use the following command to install the Vagrant on your machine
```shell
wget -O- https://apt.releases.hashicorp.com/gpg | sudo gpg --dearmor -o /usr/share/keyrings/hashicorp-archive-keyring.gpg
echo "deb [signed-by=/usr/share/keyrings/hashicorp-archive-keyring.gpg] https://apt.releases.hashicorp.com $(lsb_release -cs) main" | sudo tee /etc/apt/sources.list.d/hashicorp.list
```
The currently version of the Vagrant in this project is ```Vagrant 2.3.7```
## What is the control node

## directorys structure
## What is the control node
## The app01 
### app01 VagrantFile and shell script
The VagrantFile from app01 create a virtual machine with CentOs 7, with a hostname called app01, with your ip address configured, fowarded ports and the path for the script to authenticate the controlnode machine to login with ssh.
## The db01
### What is the provision.sh script
### what the VagrantFile do
## how to startup the vagrant stuffs


You can follow the Vagrant installation documentation [here](https://developer.hashicorp.com/vagrant/docs/installation)



# Ansible 
## Ansible Setup  
The currently version of the Ansible in this project is ```Ansible 2.9.27```

you can install the ansible manually in the virtuak machines using :
```shell
sudo yum -y install epel-release
sudo yum -y install ansible
```
But in this project, we writed in the provision.sh to install the ansible and passed to VagrantFile to install this in the controlnode machine.
# To-do:

## Ansible directory structure
## Playbook explained
### the etc directory 
Contains the configurations to manage and control the service
### the handlers directory
### the roles directory
Contains a basic .yml file installing to install the git 
### the templates directory
Contains the application.properties for the springboot application, managing the database

### vars directory
Contains the environment variable for the application

### what the app.yaml do
Has few tasks to manage and configure the application, configuring your hosts, the dependencies installation for the application

### what the db.yaml do
Contains the database configuration tasks
