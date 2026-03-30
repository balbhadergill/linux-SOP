# Standard Operating Procedure (SOP)

## Virtual Linux Server Setup for Web Application Testing

---

## 1. Purpose

This document explains how to set up a virtual Linux server for testing web applications. It ensures that the setup process is consistent and easy to follow.

---

## 2. Scope

This SOP is used by students and system administrators who need to create a Linux-based test environment.

---

## 3. Requirements

### Hardware

* Minimum 4 GB RAM
* 20 GB Storage
* Virtualization platform (Proxmox / VMware / VirtualBox)

### Software

* Ubuntu Server ISO
* SSH client

---

## 4. Steps

### Step 1: Create Virtual Machine

Create a new VM with the following settings:

* Name: web-server-01
* OS: Ubuntu Linux (64-bit)
* RAM: 2 GB
* CPU: 2 cores
* Disk: 20 GB

---

### Step 2: Install Ubuntu Server

* Attach ISO file
* Start VM
* Follow installation steps
* Set username and password

---

### Step 3: Update System

```bash
sudo apt update
sudo apt upgrade -y
```

---

### Step 4: Install Apache Web Server

```bash
sudo apt install apache2 -y
```

Start service:

```bash
sudo systemctl start apache2
sudo systemctl enable apache2
```

---

### Step 5: Configure Firewall

```bash
sudo ufw allow OpenSSH
sudo ufw allow 'Apache'
sudo ufw enable
```

---

### Step 6: Check Server

Find IP address:

```bash
ip a
```

Open browser and enter:
http://your-server-ip

---

### Step 7: Install Additional Packages

```bash
sudo apt install mysql-server -y
sudo apt install php libapache2-mod-php -y
```

Restart Apache:

```bash
sudo systemctl restart apache2
```

---

### Step 8: Enable SSH

```bash
sudo apt install openssh-server -y
sudo systemctl status ssh
```

Connect using:

```bash
ssh username@server-ip
```

---

## 5. Verification

* Web server is running
* SSH connection works
* Firewall is enabled

---

## 6. Troubleshooting

Restart Apache:

```bash
sudo systemctl restart apache2
```

Restart SSH:

```bash
sudo systemctl restart ssh
```

Check logs:

```bash
sudo journalctl -xe
```

---

## 7. Conclusion

This SOP provides a simple way to set up a Linux server for testing web applications in a virtual environment.

---
