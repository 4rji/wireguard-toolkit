# WireGuard Toolkit

A collection of Bash scripts to manage WireGuard VPN connections efficiently.

## Scripts

### wginst (WireGuard Installer)

A script that:
- Automatically detects your Linux distribution
- Installs WireGuard and its dependencies
- Sets up WireGuard configuration
- Offers automatic connection recovery through cron jobs
- Supports multiple Linux distributions:
  - Debian/Ubuntu/Kali
  - CentOS/RHEL
  - Fedora
  - Arch Linux

Usage:
```bash
./wginst path/to/your/config.conf
```

<img width="1045" alt="Image" src="https://github.com/user-attachments/assets/0876e6eb-fdf4-4ec9-9ae6-680efc0efd8c" />






### wgc (WireGuard Controller)

An interactive menu-driven script to manage WireGuard connections. Features:
- Connect/Disconnect WireGuard interface
- Reconnect functionality
- Show connection status
- Modify configuration files
- Systemd-resolved service management

Usage:
```bash
./wgc <interface_name>
```
<img width="649" alt="Image" src="https://github.com/user-attachments/assets/80b18cd0-9ed6-4380-a3a5-1d8d79f5f715" />


## Requirements

- Linux-based operating system
- Root/sudo privileges
- WireGuard configuration file
- Nano text editor (for configuration editing)

## Security Notice

These scripts should only be used for authorized testing and educational purposes. Users are responsible for ensuring proper authorization before using these tools.

## Installation

1. Clone this repository
2. Make the scripts executable:
```bash
chmod +x wginst wgc
```
3. Run the installer first:
```bash
./wginst path/to/your/config.conf
```
4. Use the controller as needed:
```bash
./wgc your_interface_name
```