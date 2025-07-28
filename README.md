# Cisco Router Ansible Automation

This project contains Ansible inventory and playbooks to automate configuration and testing of Cisco routers using SSH.

## 🌐 Network Topology

- **Ansible Automation Platform (AAP)**: `10.32.20.14`
- **Cisco Router**: `10.32.20.210`
- **User**: `ansible`
- **SSH**: Passwordless (public key auth)

---

## 📁 Project Structure

├── inventory.yml # Ansible inventory with host/group variables
├── ping_pong.yml # Playbook to test ping from Cisco router
├── README.md # This documentation
---

## ⚙️ Requirements

- Cisco router with SSH enabled and accessible
- SSH key-based authentication (`ansible@10.32.20.210`)
- Cisco user with privilege 15
- Cisco IOS collection installed:
  
```bash
ansible-galaxy collection install cisco.ios
