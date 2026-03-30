# Assignment 2 – SOP Document

**Student Name:** Balbhader Singh Gill  
**Instructor:** Felix  Liang

**Course:** Systems and Network Administration  
**Date:** March 30, 2026  

---

## Standard Operating Procedure
### Creating a New Virtual Machine (VM) in VMware vSphere 7.0

---

## Purpose
The purpose of this document is to explain how to create a new Virtual Machine (VM) using VMware vSphere 7.0.  
This process helps make sure that all virtual machines are created properly, securely, and in the same way every time.

---

## Scope
This SOP is mainly for:
- System administrators
- IT support staff
- Virtualization team members

It explains the steps from planning the VM to testing and documenting it.

---

## Objectives
The main goals of this SOP are:
- To create virtual machines correctly
- To avoid mistakes during setup
- To follow security practices
- To keep proper records of all virtual machines

---

## Who is Responsible

| Task | Responsible Team |
|------|------------------|
| Planning the VM | System Administrator |
| Configuring the VM | Virtualization Team |
| Installing Operating System | System Administrator |
| Testing the VM | QA Team |
| Documenting the VM | Documentation Team |

---

## Important Terms

**Virtual Machine (VM):**  
A computer that runs inside another computer using virtualization.

**VMware vSphere:**  
A platform used to create and manage virtual machines.

**ISO File:**  
A file used to install an operating system.

---

## Procedure

### Step 1: Planning the Virtual Machine
Before creating the VM, we need to understand why it is needed.

Things to decide:
- What the VM will be used for
- How much CPU is required
- How much RAM is needed
- Storage space
- Network requirements

After deciding this, confirm everything with the team requesting the VM.

---

### Step 2: Creating the Virtual Machine
1. Open the VMware vSphere Client.
2. Log in to the vCenter Server.
3. Go to the host or cluster.
4. Click **New Virtual Machine**.
5. Enter the VM name.
6. Select the operating system.
7. Assign CPU and memory.
8. Configure storage and network.

---

### Step 3: Installing the Operating System
1. Attach the OS installation ISO file.
2. Start the virtual machine.
3. Follow the installation steps on the screen.
4. Set administrator username and password.
5. Configure network settings.

---

### Step 4: Testing the Virtual Machine
After installation:
- Check if the system starts correctly
- Test login
- Check internet/network connectivity
- Verify applications if required

---

### Step 5: Documentation
Finally, record the VM details such as:
- VM name
- CPU and RAM
- Storage
- IP address
- Purpose of the VM

This helps future management and troubleshooting.

---

## Revision History

| Version | Date | Author | Description |
|--------|------|--------|-------------|
| 1.0 | March 30, 2026 | Balbhader Singh Gill | First version of the SOP |

---
