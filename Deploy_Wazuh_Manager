
# Wazuh Manager (Server) Installation on Ubuntu

## Prerequisites

- Ubuntu Server
- Minimum **4 GB RAM** (8 GB recommended)
- Minimum **2 CPU cores** (8 cores recommended)
- Root or sudo privileges

---

## 1. Download the Wazuh Installer

```bash
curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh
```

---

## 2. Install Wazuh Components

Run the following command to install the Wazuh Indexer, Manager, and Dashboard:

```bash
sudo bash ./wazuh-install.sh -a
```

> **Note:** The installation may take several minutes.

---

## 3. Save the Login Credentials

After the installation completes, the script will display the **Dashboard username and password**.

Save these credentials, as they are required to log in to the Wazuh Dashboard.

---

## 4. Access the Wazuh Dashboard

Find the server IP address:

```bash
hostname -I
```

Open your browser and navigate to:

```
https://<SERVER_IP>
```

> **Note:** Since Wazuh uses a self-signed SSL certificate by default, your browser may display a security warning. Accept the warning and continue.

Log in using the credentials provided at the end of the installation.

---

# Starting Wazuh Services After a System Reboot

## On the Wazuh Manager (Ubuntu)

Check the Wazuh Manager status:

```bash
sudo systemctl status wazuh-manager
```

Start the required services if they are not running:

```bash
sudo systemctl start wazuh-indexer
sudo systemctl start wazuh-manager
sudo systemctl start wazuh-dashboard
```

Get the server IP address:

```bash
hostname -I
```

Access the dashboard:

```
https://<SERVER_IP>
```

---
