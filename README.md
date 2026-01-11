# Ansible_Basic

# Ansible Basic – Nginx Playbook

This repository contains a simple Ansible playbook to install and start the Nginx web server on a Linux system.  
It is created for beginners who are learning Ansible basics.

Files included in this repository:
- `inventory` – defines the target host (localhost)
- `firstplaybook.yml` – Ansible playbook to install and start Nginx

Inventory configuration:
```ini
localhost ansible_connection=local
```

This playbook performs the following actions:

Installs Nginx using the apt module
Starts the Nginx service using the service module

How to run the project:
ansible -i inventory localhost -m ping
ansible-playbook -i inventory firstplaybook.yml


Expected result after running the playbook:

Nginx is installed on the system
Nginx service is running
Open http://localhost
in a browser to see the Nginx welcome page
