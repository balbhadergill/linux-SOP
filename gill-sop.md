# Assignment 2 – Standard Operating Procedure (SOP)

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

## Step 1: Pre-Creation Planning and Assessment

### Step 1.1 Identify Purpose and Requirements
Determine the purpose of the virtual machine such as:
- Web server
- Database server
- Application server

Also define the required resources:
- CPU cores
- RAM
- Storage space
- Network configuration

### Step 1.2 Plan Resource Allocation
Check the host server capacity and available resources.  
Select appropriate datastore and plan CPU and memory allocation.

### Step 1.3 Communicate with Stakeholders
Discuss the VM requirements with the requesting team and confirm the specifications before creating the VM.

---

## Step 2: Configuration of Virtual Machine

### Step 2.1 Access VMware vSphere Client
1. Open the vSphere Client.
2. Connect to the vCenter Server.

### Step 2.2 Create a New Virtual Machine
1. Navigate to the host or cluster.
2. Right-click and select **New Virtual Machine**.
3. Choose the deployment type.

### Step 2.3 Configure Virtual Machine Settings
Set the following configuration:
- VM name and location
- Operating system
- CPU allocation
- Memory allocation
- Network settings
- Storage configuration

---

## Step 3: Installation of Guest Operating System

### Step 3.1 Attach Installation ISO
Attach the ISO file that contains the operating system installation media.

### Step 3.2 Install Guest OS
1. Power on the virtual machine.
2. Follow the installation steps for the operating system.
3. Configure administrator credentials and system settings.

### Step 3.3 Configure Networking
Set up:
- IP address
- DNS settings
- Network connectivity

---

## Step 4: Post-Creation Verification and Testing

### Step 4.1 Verify Installation
Confirm that the operating system has been installed successfully.

### Step 4.2 Functional Testing
Perform testing such as:
- Logging into the system
- Testing network connectivity
- Checking required services

### Step 4.3 Security Compliance
Apply security configurations including:
- Firewall rules
- System updates
- Security policies

---

## Step 5: Documentation of Virtual Machine

Record the following information:
- VM name
- CPU and RAM allocation
- Storage size
- Network configuration
- Purpose of the VM


---
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

