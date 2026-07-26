# Ansible Automation Projects Playbooks

## Ansible Project Directory

```
ansible-enterprise-admin/
├── group_vars/
│   ├── all.yml                 # Global variables (e.g., SMTP settings)
│   ├── windows.yml             # WinRM connection variables, Windows paths
│   └── linux.yml               # SSH connection variables, Linux paths
├── inventory.ini               # Infrastructure inventory file
├── site_linux.yml              # Main orchestrator for Linux hosts
├── site_windows.yml            # Main orchestrator for Windows hosts
└── roles/
    ├── os_patching/            # Handles yum/apt and win_updates
    ├── server_hardening/       # Enforces CIS benchmarks / PCI-DSS compliance
    ├── ssl_management/         # Health checks and Let's Encrypt / AD renewal
    ├── db_health_check/        # Probes Oracle and MongoDB instances
    └── db_backup/              # Executes automated snapshots/dumps
```
