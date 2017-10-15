# Ansible playbook "wordpress-nginx-letsencrypt"
This playbook is based on [ansible-examples](https://github.com/ansible/ansible-examples/blob/master/wordpress-nginx), and [Original licence](https://github.com/ansible/ansible-examples/blob/master/wordpress-nginx/LICENSE.md).

# Overview
Ansible playbook to Install WordPress, MariaDB, PHP7, Nginx on Ubuntu Server.  
Set to HTTPS on "Let's Encrypt" module.

# Requirements
Ansible 2.4 or newer.
Remote host where Ubuntu server is installed.

# Usage
Edit group_vars/all.yml.example and Save as group_vars/all.yml file.  
Edit production.example and Save as production.yml file.  
Set "ANSIBLE_PUBKEY" environment variable to public key file path.

Expects below commands before run playbooks.

```
$ ssh-agent bash  
$ ssh-add "PRIVATE KEY FILE"  
```

First step ONLY.  
```
$ ansible-playbook -i production ansible-user-setup.yml
```

To setup server  
```
$ ansible-playbook -i production site.yml
```

Easy to setup WordPress!

# Author
[Blog](https://ak1211.com/4968)
