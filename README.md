# ansible-ansible

This Ansible configuration automates the setup of a Python-based environment for running Ansible and related tools. It ensures all required system packages are installed, creates a dedicated Python virtual environment, installs and upgrades Ansible and essential Python packages, and sets up necessary Ansible collections. The playbook also generates a custom `ansible.cfg` configuration file and ensures the `/etc/ansible` directory exists.

## Features
- Installs required system packages (Python, pip, venv)
- Creates a Python virtual environment for Ansible
- Installs and upgrades Ansible and key Python libraries (kubernetes, jsonpatch, PyYAML)
- Installs Ansible collections (`ansible.posix`, `community.kubernetes`)
- Generates `/etc/ansible/ansible.cfg` from a template
- Ensures `/etc/ansible` directory is present
- Outputs the installed Ansible version for verification

This setup is ideal for preparing a consistent and reproducible Ansible control node environment.
