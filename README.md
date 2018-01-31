# sonarqubedeploy
Automation around sonarqube deployment. Vagrantfile + ansible provisioning
to easily deploy a Vagrant system for local use.

The scripts create a virtual machine (in Virtualbox) that has 2GB of RAM
and 10GB of disk space. Sonarqube 6.7.1 is installed on the host, along 
with postgresql. Edit playbook.yml to change the sonarqube version or
the database password. Installation roughly follows the steps on
https://www.vultr.com/docs/how-to-install-sonarqube-on-ubuntu-16-04

Use at your own risk!

# requirements
The following packages are required to be present:
* Vagrant
* Ansible
* Virtualbox
* Virtualbox additions for vagrant:
  vagrant plugin install vagrant-hostmanager vagrant-vbguest

