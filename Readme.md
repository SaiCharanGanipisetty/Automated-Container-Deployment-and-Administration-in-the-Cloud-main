# Docker Server Configuration with Ansible

This Ansible playbook configures an EC2 instance to install and run Docker automatically on boot.

## Prerequisites

- Ansible installed on the control node
- SSH access to the target EC2 instance
- `inventory.ini` file with EC2 IP and SSH key path

## Files

- `docker_setup.yml`: Ansible playbook for configuring Docker on the server
- `inventory.ini`: Inventory file with server details

## Instructions

1. Clone this repository and navigate to the folder.
2. Run the following command to apply the configuration:
   ```bash
   ansible-playbook -i inventory.ini docker_setup.yml
