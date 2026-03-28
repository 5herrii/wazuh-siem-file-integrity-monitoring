# Wazuh SIEM File Integrity Monitoring Lab

Home lab built using Wazuh, an Ubuntu VM as the Wazuh Manager, and a Windows endpoint as the Wazuh Agent to monitor and detect file changes in real time.

## Overview
In this project, I built a Wazuh-based SIEM lab to monitor endpoint activity and detect unauthorized file changes using File Integrity Monitoring (FIM). The Wazuh Manager was deployed on an Ubuntu virtual machine, while a Windows machine was configured as the monitored endpoint.

The goal of this lab was to understand how endpoint telemetry is collected by a SIEM, how agents communicate with a manager, and how file creation, deletion, and modification events can be detected and investigated through Wazuh.

## What This Project Demonstrates
- SIEM setup and deployment using Wazuh
- Agent onboarding and manager-agent communication
- File Integrity Monitoring (FIM) using Wazuh Syscheck
- Real-time detection of file creation, deletion, and modification
- Log analysis using alert metadata such as rule IDs, hashes, timestamps, and file paths
 Basic network configuration and troubleshooting in a lab environment

## Architecture
Windows Endpoint (Wazuh Agent) → Ubuntu VM (Wazuh Manager) → Wazuh Dashboard


<img width="1200" height="1200" alt="Windows agent" src="https://github.com/user-attachments/assets/5b7a79c4-a747-41b4-bd1d-640d5f94b59b" />


## Highlights
- Deployed a working Wazuh SIEM lab with manager and agent integration
- Configured real-time monitoring for a target Windows directory
- Generated alerts for file creation, deletion, and modification events
- Reviewed detection data including rule ID 554, hashes, timestamps, user, and file path
- Resolved setup issues including agent communication and FIM configuration

## Detailed Walkthrough
Detailed explanation: `DETAILED-WALKTHROUGH.md`
