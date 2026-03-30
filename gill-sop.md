# Standard Operating Procedure (SOP)

**Student Name:** Balbhader Singh Gill  
**Instructor:** Felix  
**Course:** Systems and Network Administration  
**Date:** March 30, 2026  

---

# Standard Operating Procedure  
## Creating a New Virtual Machine in VMware vSphere 7.0

---

## Purpose
The purpose of this document is to describe the process of creating a new Virtual Machine (VM) using VMware vSphere 7.0.  
Following this SOP helps ensure that virtual machines are created correctly, securely, and consistently within the organization.

---

## Audience
This document is intended for:
- System Administrators
- IT Support Team
- Virtualization Team
- Other IT staff involved in VM deployment

---

## Approval Table

| Version | Date | Name | Role |
|--------|------|------|------|
| 1.0 | March 30, 2026 | Balbhader Singh Gill | Author |
| 1.1 | March 30, 2026 | Jay Dixit | Reviewer |
| 1.2 | March 30, 2026 | Bobbi Plante | Reviewer |
| 1.3 | March 30, 2026 | Marni Russell | Approver |

---

## Scope / Objectives
This SOP explains the full process of creating a virtual machine, including:

- Planning the VM requirements  
- Configuring the virtual machine  
- Installing the operating system  
- Testing the system  
- Documenting the VM  

The goal is to make the process easy to follow and reduce setup errors.

---

# Accountability Matrix

| Task / Steps | Responsible Person / Team | Emergency Contact | Non-Emergency Contact | Review / Approval |
|--------------|---------------------------|------------------|----------------------|------------------|
| Pre-creation Planning and Assessment | System Administrator | +1 431-555-2145 | sysadmin-support@balbhader.ca | Jay Dixit |
| Configuration of Virtual Machine | Virtualization Team | +1 431-555-3278 | virtualization@balbhader.ca | Bobbi Plante |
| Installation of Guest OS | System Administrator | +1 431-555-4412 | os-install@balbhader.ca | Jay Dixit |
| Post-creation Verification and Testing | QA Team | +1 431-555-5689 | qa-team@balbhader.ca | Marni Russell |
| Documentation of Virtual Machine | Documentation Team | +1 431-555-6723 | documentation@balbhader.ca | Marni Russell |

---

## Definitions

**Virtual Machine (VM)**  
A virtual computer that runs on a physical server using virtualization technology.

**VMware vSphere**  
A platform used to manage and deploy virtual machines.

**ISO File**  
An installation file used to install an operating system on a virtual machine.

**Datastore**  
Storage location where VM files are stored.

---

# Procedure Steps

## Step 1: Identify the Purpose of the Virtual Machine
Determine why the Linux VM is needed:
- Web server
- Database server
- Testing environment
- Application deployment

---

## Step 2: Gather System Requirements
Check required resources.

Linux command to check system information (after install):

```bash
uname -a
lscpu
free -h
df -h
```

---

## Step 3: Check Host Capacity in VMware
Before creating the VM, ensure resources are available.

Commands to verify disk and memory after VM deployment:

```bash
top
htop
```

---

## Step 4: Access VMware vSphere Client
Login to vSphere and navigate to the server.

After Linux installation, confirm login:

```bash
whoami
hostname
```

---

## Step 5: Create a New Virtual Machine
Configure:
- VM name
- CPU
- RAM
- Disk
- Network

Verify network interface in Linux:

```bash
ip a
ip link
```

---

## Step 6: Configure Linux System
Update the system after installation.

```bash
sudo apt update
sudo apt upgrade -y
```

Set hostname:

```bash
sudo hostnamectl set-hostname linux-vm01
```

Check OS version:

```bash
cat /etc/os-release
```

---

## Step 7: Install Required Packages
Example packages commonly installed:

```bash
sudo apt install net-tools -y
sudo apt install curl -y
sudo apt install wget -y
sudo apt install git -y
```

Verify installations:

```bash
git --version
curl --version
```

---

## Step 8: Perform System Tests

### Network Test
Check internet connectivity:

```bash
ping -c 4 google.com
```

### Check IP Address

```bash
ip addr show
```

### Check Running Services

```bash
systemctl list-units --type=service
```

### Disk Usage Test

```bash
df -h
```

### Memory Usage Test

```bash
free -m
```

### Check Open Ports

```bash
ss -tuln
```

### Firewall Status

```bash
sudo ufw status
```

---

## Step 9: Document the Virtual Machine
Record the system details using:

```bash
hostnamectl
ip a
df -h
free -h
```

Save the information in system documentation.

Example:

```bash
echo "VM documentation saved successfully"
```

# Reference or Related Documents

Below are some helpful resources related to this SOP:

VMware Documentation  
https://docs.vmware.com/en/VMware-vSphere/index.html

VMware vSphere Installation Guide  
https://docs.vmware.com/en/VMware-vSphere/latest/vsphere-installation-guide.html

GitHub Markdown Guide  
https://docs.github.com/en/get-started/writing-on-github

Instructor Website  
https://felixliang.org/

# Revision History

| Version | Date | Updated By | Changes |
|--------|------|-----------|--------|
| 1.0 | March 30, 2026 | Balbhader Singh Gill | Initial document created |
| 1.1 | March 30, 2026 | Jay Dixit | Document review completed |
| 1.2 | March 30, 2026 | Bobbi Plante | Minor updates and improvements |
| 1.3 | March 30, 2026 | Marni Russell | Final approval |

---

