# Ansible_Basic

Ansible Basic – Nginx Playbook

This repository contains a simple Ansible playbook to install and start the Nginx web server on a Linux system.  
It is intended for beginners learning Ansible fundamentals.

---

 📁 Files
- `inventory` – Defines the target host (localhost)
- `firstplaybook.yml` – Ansible playbook to install and start Nginx

---

 📄 Inventory
```ini
localhost ansible_connection=local


📜 Playbook Actions
The playbook performs the following tasks:
Installs Nginx using the apt module
Starts the Nginx service using the service module

▶️ How to Run
ansible -i inventory localhost -m ping
ansible-playbook -i inventory firstplaybook.yml


✅ Expected Result
Nginx is installed
Nginx service is running
Open http://localhost to see the Nginx welcome page
