# 🛡️ Wazuh Installation (All-in-One)

Repository ini berisi script otomatis untuk install Wazuh (All-in-One) yang mencakup:

- Wazuh Server (Manager)
- Wazuh Indexer (OpenSearch)
- Wazuh Dashboard

Script ini mempermudah proses instalasi tanpa perlu setup manual satu per satu.

---

## 📦 Requirements

Pastikan server memenuhi minimum requirement:

- OS: Ubuntu / Debian / CentOS / AlmaLinux
- RAM: Minimal 4 GB (Recommended 8 GB)
- CPU: 2 Core (Recommended 4 Core)
- Disk: Minimal 20 GB

---

## 🚀 Installation Steps

### 1. Clone Repository

```bash
git clone https://github.com/syahrulrzk/security_wazuh.git
cd security_wazuh


'''
root@homelab:/home/wazuh# ./wazuh-install.sh -a
01/04/2026 10:23:12 INFO: Starting Wazuh installation assistant. Wazuh version: 4.14.4
01/04/2026 10:23:12 INFO: Verbose logging redirected to /var/log/wazuh-install.log
01/04/2026 10:23:36 INFO: Verifying that your system meets the recommended minimum hardware requirements.
01/04/2026 10:23:36 INFO: Wazuh web interface port will be 443.
01/04/2026 10:23:45 INFO: --- Dependencies ----
01/04/2026 10:23:45 INFO: Installing debhelper.
01/04/2026 10:24:49 INFO: Wazuh repository added.
01/04/2026 10:24:49 INFO: --- Configuration files ---
01/04/2026 10:24:49 INFO: Generating configuration files.
01/04/2026 10:24:50 INFO: Generating the root certificate.
01/04/2026 10:24:50 INFO: Generating Admin certificates.
01/04/2026 10:24:51 INFO: Generating Wazuh indexer certificates.
01/04/2026 10:24:51 INFO: Generating Filebeat certificates.
01/04/2026 10:24:52 INFO: Generating Wazuh dashboard certificates.
01/04/2026 10:24:53 INFO: Created wazuh-install-files.tar. It contains the Wazuh cluster key, certificates, and passwords necessary for installation.
01/04/2026 10:24:53 INFO: --- Wazuh indexer ---
01/04/2026 10:24:53 INFO: Starting Wazuh indexer installation.
01/04/2026 10:28:11 INFO: Wazuh indexer installation finished.
01/04/2026 10:28:11 INFO: Wazuh indexer post-install configuration finished.
01/04/2026 10:28:11 INFO: Starting service wazuh-indexer.
01/04/2026 10:29:15 INFO: wazuh-indexer service started.
01/04/2026 10:29:15 INFO: Initializing Wazuh indexer cluster security settings.
01/04/2026 10:29:29 INFO: Wazuh indexer cluster security configuration initialized.
01/04/2026 10:29:29 INFO: Wazuh indexer cluster initialized.
01/04/2026 10:29:29 INFO: --- Wazuh server ---
01/04/2026 10:29:29 INFO: Starting the Wazuh manager installation.
01/04/2026 10:34:46 INFO: Wazuh manager installation finished.
01/04/2026 10:34:54 INFO: Wazuh manager vulnerability detection configuration finished.
01/04/2026 10:34:54 INFO: Starting service wazuh-manager.
01/04/2026 10:35:29 INFO: wazuh-manager service started.
01/04/2026 10:35:29 INFO: Starting Filebeat installation.
01/04/2026 10:38:41 INFO: Filebeat installation finished.
01/04/2026 10:39:19 INFO: Filebeat post-install configuration finished.
01/04/2026 10:39:19 INFO: Starting service filebeat.
01/04/2026 10:39:21 INFO: filebeat service started.
01/04/2026 10:39:21 INFO: --- Wazuh dashboard ---
01/04/2026 10:39:21 INFO: Starting Wazuh dashboard installation.
01/04/2026 11:26:20 INFO: Wazuh dashboard installation finished.
01/04/2026 11:26:22 INFO: Wazuh dashboard post-install configuration finished.
01/04/2026 11:26:22 INFO: Starting service wazuh-dashboard.
01/04/2026 11:26:39 INFO: wazuh-dashboard service started.
01/04/2026 11:26:41 INFO: Updating the internal users.
01/04/2026 11:28:52 INFO: A backup of the internal users has been saved in the /etc/wazuh-indexer/internalusers-backup folder.
01/04/2026 11:29:59 INFO: There was an error accessing the API. Retrying...
01/04/2026 11:30:41 INFO: The filebeat.yml file has been updated to use the Filebeat Keystore username and password.
01/04/2026 11:32:18 INFO: Initializing Wazuh dashboard web application.
01/04/2026 11:32:18 INFO: Wazuh dashboard web application not yet initialized. Waiting...
01/04/2026 11:32:37 INFO: Wazuh dashboard web application not yet initialized. Waiting...
01/04/2026 11:32:52 INFO: Wazuh dashboard web application not yet initialized. Waiting...
01/04/2026 11:33:17 INFO: Wazuh dashboard web application not yet initialized. Waiting...
01/04/2026 11:33:32 INFO: Wazuh dashboard web application initialized.
01/04/2026 11:33:32 INFO: --- Summary ---
01/04/2026 11:33:32 INFO: You can access the web interface https://<wazuh-dashboard-ip>:443
    User: admin
    Password: S7oRgXNy*4k6teUaG?ylANgorrCXkp*8
01/04/2026 11:33:33 INFO: Installation finished.
root@homelab:/home/wazuh#
'''
