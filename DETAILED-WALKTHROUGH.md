# Detailed Walkthrough – Wazuh SIEM File Integrity Monitoring Lab

## 1. Network Configuration

Ubuntu VM and Windows machine were configured on the same network using bridged mode.

### Ubuntu IP
![Ubuntu IP](screenshots/ubuntu-ip.png)

### Windows IP
![Windows IP](screenshots/windows-ip.png)

---

## 2. Wazuh Manager Installation

Wazuh was installed on the Ubuntu VM using the official installation script.

![Wazuh Installation](screenshots/wazuh-server-installation.png)

---

## 3. Accessing the Dashboard

After installation, the Wazuh dashboard was accessed via browser.

### Login Page
![Dashboard Login](screenshots/dashboard-login.png)

### Dashboard Overview
![Dashboard](screenshots/dashboard.png)

---

## 4. Agent Setup (Windows)

The Wazuh agent was installed and configured on the Windows machine.

### Agent Configuration
![Wazuh Agent](screenshots/wazuh-agent-windows.png)

---

## 5. Agent Registration

Agent was registered using the manager.

### Manage Agents
![Agent Manager](screenshots/agent-manager-ossec.png)

### Extracted Key
![Agent Key](screenshots/connection.png)

---

## 6. Agent Connected

After configuration, the agent successfully connected and appeared as active.

![Agent Active](screenshots/agent-detail.png)

---

## 7. File Integrity Monitoring Configuration

File Integrity Monitoring (FIM) was enabled by editing the configuration file.

### Windows Configuration File
![OSSEC Config Windows](screenshots/ossec-conf-windows.png)

### FIM Directory Added
![OSSEC Config FIM](screenshots/ossec-conf-fm.png)

---

## 8. Test Scenario

A test file was created in the monitored directory to trigger alerts.

![Test File](screenshots/fm-testdoc.png)

---

## 9. File Integrity Monitoring Events

Wazuh detected file creation, deletion, and modification events in real time.

![FIM Events](screenshots/dashboard-event.png)

---

## 10. Log Analysis

Detailed logs were analyzed, including rule ID, hashes, and metadata.

### Log Details 1
![Log Details](screenshots/doc-details1.png)

### Log Details 2
![Log Details](screenshots/doc-details2.png)

### Log Details 3
![Log Details](screenshots/doc-details3.png)

---

## 11. Troubleshooting

During setup, an issue with incompatible agent version was encountered and resolved.

![Error Log](screenshots/error-log.png)

---

## Summary

- Successfully deployed Wazuh SIEM lab
- Connected Windows agent to Ubuntu manager
- Enabled File Integrity Monitoring (FIM)
- Detected file changes in real time
- Analyzed logs including hashes and rule IDs
- Resolved setup and compatibility issues
