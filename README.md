# Ansible playbook "wordpress-nginx-letsencrypt"
This playbook is based on [ansible-examples](https://github.com/ansible/ansible-examples/blob/master/wordpress-nginx), and [Original licence](https://github.com/ansible/ansible-examples/blob/master/wordpress-nginx/LICENSE.md).

# Overview
Ansible playbook to Install WordPress, MariaDB, PHP7, Nginx on Ubuntu Server.  
Set to HTTPS on "Let's Encrypt" module.

# Usage
Edit group_vars/all.yml.example and Save as group_vars/all.yml file.  
Edit production.example and Save as production.yml file.  

First step ONLY.  
$ ansible-playbook -i production ansible-user-setup.yml  

To setup server  
$ ansible-playbook -i production site.yml

Easy to setup WordPress!

[Blog](https://ak1211.com/4968)
