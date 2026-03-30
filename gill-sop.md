# Standard Operating Procedure (SOP)

**Student Name:** Balbhader Singh Gill  
**Instructor:** Felix  
**Course:** IT / System Administration  
**Date:** March 30, 2026  
**Document Type:** Markdown SOP Documentation  

---

# Standard Operating Procedure
## New Virtual Machine Creation on VMware vSphere 7.0

---

## Purpose
The purpose of this document is to describe the standard process for creating a new Virtual Machine (VM) using VMware vSphere 7.0.  
This ensures that all virtual machines are created consistently, securely, and according to organizational best practices.

---

## Scope
This SOP applies to:
- System Administrators
- IT Support Staff
- Virtualization Team
- IT Operations Team

This document covers:
- Planning the virtual machine
- Configuring the VM
- Installing the operating system
- Testing the VM
- Documenting the VM

---

## Objectives
The objectives of this SOP are:
- Ensure proper VM configuration
- Maintain system security
- Standardize VM deployment
- Reduce errors during VM setup
- Improve documentation and tracking

---

## Accountability Matrix

| Task | Responsible Person/Team | Approval |
|------|------------------------|----------|
| Planning VM Requirements | System Administrator | IT Manager |
| VM Configuration | Virtualization Team | IT Operations Manager |
| Operating System Installation | System Administrator | IT Manager |
| Testing and Verification | QA Team | QA Manager |
| Documentation | Documentation Team | Author |

---

## Definitions

**Virtual Machine (VM):**  
A virtual computer that runs inside a physical server.

**VMware vSphere:**  
A platform used to manage and deploy virtual machines.

**ISO File:**  
An installation image used to install operating systems.

**Datastore:**  
Storage location where virtual machine files are saved.

---

# Procedure Steps

## Step 1: Pre-Creation Planning

### Step 1.1 Identify Purpose
Determine why the VM is needed.  
Example:
- Web server
- Database server
- Application server

### Step 1.2 Define Requirements
Decide the resources required:
- CPU cores
- RAM
- Storage
- Network configuration

### Step 1.3 Confirm With Stakeholders
Communicate with the requesting team and confirm the specifications.

---

## Step 2: Configure Virtual Machine

### Step 2.1 Access vSphere Client
1. Open VMware vSphere Client.
2. Log in to vCenter Server.

### Step 2.2 Create New Virtual Machine
1. Navigate to the host or cluster.
2. Right-click and select **New Virtual Machine**.
3. Select deployment type.

### Step 2.3 Configure Settings
Set the following:
- Virtual machine name
- Operating system type
- CPU allocation
- Memory allocation
- Network settings
- Storage location

---

## Step 3: Install Guest Operating System

### Step 3.1 Attach Installation Media
Attach the ISO file containing the OS installer.

### Step 3.2 Start Installation
1. Power on the VM.
2. Follow OS installation instructions.
3. Configure system settings.

### Step 3.3 Configure Network
Set:
- IP address
- DNS settings
- Connectivity

---

## Step 4: Post-Creation Verification

### Step 4.1 Verify Installation
Check that the OS installed correctly.

### Step 4.2 Test System
Perform tests:
- Login test
- Network connectivity
- Application test

### Step 4.3 Security Configuration
Apply:
- Firewall settings
- Updates
- Security policies

---

## Step 5: Documentation

### Step 5.1 Record VM Details
Document:
- VM name
- CPU and RAM
- Storage
- Network configuration

### Step 5.2 Update System Records
Save the information in the company documentation system.

---

# Revision History

| Version | Date | Author | Description |
|--------|------|--------|-------------|
| 1.0 | March 30, 2026 | Balbhader Singh Gill | Initial Document |

---

