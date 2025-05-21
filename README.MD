# Ansible Playbook Suite – Dissertation Artifact

This folder contains the Ansible playbooks developed and evaluated as part of the dissertation project:

**"Evaluating the Effectiveness and Limitations of Ansible Automation in Cross-Platform System Administration"**

## 📦 Contents

| Filename                   | Target OS         | Description                                                                 |
|----------------------------|-------------------|-----------------------------------------------------------------------------|
| `apache2.yml`              | Linux (Ubuntu)    | Installs and starts Apache2, opens ports 80/443 via UFW.                   |
| `iis.yml`                  | Windows Server    | Enables the IIS role and configures Windows Defender Firewall rules.       |
| `lin_security_harden.yml`  | Linux (Ubuntu)    | Applies updates, installs `fail2ban`, and configures unattended upgrades.  |
| `lin_user_management.yml`  | Linux (Ubuntu)    | Creates a sudo-enabled `Admin` user with a hashed password.                |
| `win_user_management.yml`  | Windows Server    | Creates an Admin user and disables the built-in `Administrator` account.   |
| `win_enable_updates.yml`   | Windows Server    | Installs all available Windows updates and reboots if required.            |


## 🛠️ Usage Instructions

1. Ensure you have Ansible installed on your control node (e.g. Linux).
2. Configure target hosts in the Ansible inventory file.
4. Ensure SSH access is configured on the target machines.
5. Run playbooks using:

```bash
ansible-playbook -i playbook_name.yml --ask-become-pass
```

## 📄 Reference
These playbooks were developed as part of the dissertation project and are intended for educational purposes. For more details, refer to the dissertation document particularly the Implementation and the 'Results and Evaluation' sections.
