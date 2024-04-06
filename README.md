# ArcanumVPN-WireGuard-Ansible
This Ansible playbook is designed for the automated setup and maintenance of WireGuard Arcanum VPN servers. It performs a series of tasks to ensure the servers are up-to-date, secure, and optimized for performance.

### Playbook Description

This Ansible playbook is designed for setting up VPN servers with a comprehensive initial configuration that includes system updates, installation of the WireGuard VPN software, and daily cleanup routines. Additionally, it disables and removes system logging to enhance privacy and security.

### Key Features:

- **System Update and Upgrade**: Ensures all packages are up-to-date.
- **WireGuard VPN Installation**: Automatically installs the Outline VPN server.
- **Logging Disablement**: Stops and disables `rsyslog` and `syslog`, and removes existing log files.
- **Daily Cleanup and Reboot**: Schedules a daily task for system cleanup and reboot.

### Installation on a New Server:

1. **Update and Upgrade the System**
```
sudo apt update && sudo apt upgrade -y
```

2. **Install Ansible**
```
sudo apt install ansible -y
```

3. **Run the Playbook**
   - Ensure you have an inventory file ready (e.g., `/path/to/your/inventory/file`).
   - Execute the playbook:
```
ansible-playbook -i /path/to/your/inventory/playbook.yaml
```
