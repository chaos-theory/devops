Install Ansible
=============

Mac:
----
Install Python setuptools: https://pypi.python.org/pypi/setuptools#installation-instructions

If you prefer not to install packages to your global `site-packages` you can install and use virtualenv: http://virtualenv.readthedocs.org/en/latest/

``` shell
sudo easy_install pip
```

``` shell
sudo pip install paramiko PyYAML jinja2 passlib
```

``` shell
sudo pip install ansible
```

Then, if you're going to update ansible later, just do:

``` shell
sudo pip install ansible --upgrade
```

Other:
------
http://www.ansibleworks.com/docs/intro_installation.html

Install VirtualBox and Extension Pack
======================================
https://www.virtualbox.org/wiki/Downloads

Install Vagrant
===============
http://docs.vagrantup.com/v2/installation/

Install [vagrant-cachier plugin](https://github.com/fgrehm/vagrant-cachier) to speed up apt with a shared cache between boxes:

``` shell
vagrant plugin install vagrant-cachier
```

Install [vagrant-hostmanager plugin](https://github.com/smdahlen/vagrant-hostmanager) to manage the /etc/hosts file on guest machines and the host:

``` shell
vagrant plugin install vagrant-hostmanager
```

Clone this repo, and start the virtual machines:

``` shell
git clone https://github.com/steinim/devopscon-zero-downtime-ansible.git
cd devopscon-zero-downtime-ansible
vagrant up
```

Provision with Ansible
=======================
``` shell
ansible-playbook site.yml
```
