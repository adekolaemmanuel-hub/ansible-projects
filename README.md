# ansible-projects
# Ansible Projects

Configuration management using Ansible.

## Playbooks

### playbook.yml
Basic playbook that updates apt cache, installs curl,
creates a directory and file, and prints a success message.
Demonstrates idempotency — safe to run multiple times.

### nginx-playbook.yml
Installs nginx, starts the service and deploys a custom
HTML page to /var/www/html/index.html.

## How to run
ansible-playbook -i inventory.ini playbook.yml
ansible-playbook -i inventory.ini nginx-playbook.yml

## Key concept
Ansible only makes changes when needed. Running the same
playbook twice will not break anything already configured.
