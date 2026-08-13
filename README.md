# 💻 Cybersecurity Lab Environment Setup# 
Student: Francis Saviour Ahianyo
---
Course: Cybersecurity
---
Lab:Week 1 – Cybersecurity Lab Setup
---
Platform: Oracle VirtualBox
---
Guest OS: Kali Linus
---
Instructor: Waqas Karim(CCIE)
---

---
**The Purpose of this lab**
---
The purpose of this lab is to build a controlled and isolated cybersecurity laboratory using Oracle VirtualBox and Kali Linux.

The laboratory environment will provide a safe platform for practicing networking, Linux administration, ethical hacking, vulnerability assessment, and other authorized cybersecurity exercises.

---

# 🖥️ Lab Environment

| Component               | My Configuration              |
| ----------------------- | ----------------------------- |
| Host Operating System   | Windows 11                    |
| Processor               | **Core   i5**        |
| RAM                     | **16gb**              |
| Storage                 | **1TB** |
| Virtualization Platform | Oracle VirtualBox             |
| Guest Operating System  | Kali Linux                    |
| Network Type            | NAT Network                   |
| Network CIDR            | **10.0.0.0/24**     |
| Kali Linux IP Address   | **10.0.0.2**        |
| Gateway                 | **10.0.0.1**   |
| DNS                     | **8.8.8.8**              |
---

# 🔗 Tools Used

* 7-Zip
* Oracle VirtualBox
* Kali Linux
* Windows 11
* Linux networking tools

---

# 🛡️ Lab Setup Workflow

The laboratory setup consists of the following stages:

1. Install 7-Zip
2. Install Oracle VirtualBox
3. Configure the VirtualBox NAT Network
4. Download and import Kali Linux
5. Configure Kali Linux networking
6. Test network connectivity
7. Create a VirtualBox snapshot
8. Document the completed laboratory

---

# 🚀 Phase 01 — Lab Setup

## 1️⃣ 7-Zip Installation

### What I Did

I installed 7-Zip on my Windows 11 host computer to extract and manage compressed virtual-machine files.

### Why

Kali Linux virtual-machine files may be distributed in compressed formats. 7-Zip provides the tools required to extract these files before importing them into VirtualBox.

### Evidence

**Screenshot:** Add screenshot of 7-Zip installation here.

`![7-Zip Installation](screenshots/01-7zip-installation.png)`

### Result

**Status:** ✅ Completed

---

# 2️⃣ Oracle VirtualBox Installation

### What I Did

I installed Oracle VirtualBox on my Windows 11 computer.

### Why

VirtualBox provides the virtualization platform required to create and run the Kali Linux virtual machine.

### Evidence

**Screenshot:** Add VirtualBox installation or main interface screenshot.

`![VirtualBox](screenshots/02-virtualbox.png)`

### Result

**Status:** ✅ Completed

---

# 3️⃣ NAT Network Configuration

### What I Did

I created a dedicated NAT Network in Oracle VirtualBox for the cybersecurity laboratory.

### Why

A dedicated virtual network allows the laboratory machines to communicate within a controlled environment.

### Network Configuration

```text
Network Type : NAT Network
Network CIDR : 10.0.0.0/244
DHCP         : Enabled
```

### Evidence

**Screenshot:** Add your VirtualBox NAT Network configuration screenshot.

`![NAT Network](screenshots/03-nat-network.png)`

### Result

**Status:** ✅ Completed

---

# 4️⃣ Kali Linux VM Setup

### What I Did

I downloaded/imported Kali Linux into Oracle VirtualBox and connected the virtual machine to my configured NAT Network.

### VM Configuration

```text
Operating System : Kali Linux
Virtualization   : Oracle VirtualBox
Network          : NAT Network
RAM              : 2070
CPU              : 2
```

### Evidence

**Screenshot:** Add screenshot showing the Kali Linux VM in VirtualBox.

`![Kali Linux VM](screenshots/04-kali-vm.png)`

### Result

**Status:** ✅ Completed

---

# 5️⃣ Kali Linux Network Configuration

### What I Did

I configured and verified the network interface inside Kali Linux.

### Network Information

```text
IP Address : 10.0.0.2
Subnet     : 24
Gateway    : 10.0.0.1
DNS        : 8.8.8.8
```

### Commands Used
1. ifconfig
2. sudo ifconfig eth0 down
3. sudo ifconfig eth0 up
4. ping google.com

### Connectivity Test

I used ping to verify that Kali Linux could communicate with the network.

### Evidence

**Screenshot:** Add terminal screenshot showing the IP configuration and successful connectivity test.

`![Kali Network Configuration](screenshots/05-kali-network.png)`

### Result

**Status:** ✅ Completed

---

# 6️⃣ VirtualBox Snapshot

### What I Did

After completing the initial Kali Linux configuration, I created a VirtualBox snapshot.

### Why

The snapshot provides a restore point that can be used if the virtual machine becomes incorrectly configured during future cybersecurity exercises.

### Snapshot Name

```text
Week1-Cybersecurity-Lab-Baseline
```

### Evidence

**Screenshot:** Add screenshot showing the VirtualBox snapshot.

`![VirtualBox Snapshot](screenshots/06-snapshot.png)`

### Result

**Status:** ✅ Completed

---

# 🧪 Connectivity Verification

The laboratory network was tested using standard Linux networking commands.

### IP Address

```bash
ifconfig
```

### Routing Table

```bash
ip route
```

### Connectivity Test

```bash
ping 8.8.8.8
```

### Result

```text
IP configuration:     PASS
Routing:              PASS
Network connectivity: PASS
```

> The results above should only be marked PASS after I have personally performed the tests and captured the evidence.

---

# 🧠 Key Learning

During this laboratory exercise, I gained practical experience in:

* Installing virtualization software
* Creating a virtual machine
* Installing and configuring Kali Linux
* Configuring a NAT Network
* Understanding IPv4 addressing
* Understanding subnet configuration
* Checking Linux network interfaces
* Checking routing information
* Testing network connectivity
* Creating virtual-machine snapshots
* Maintaining an isolated cybersecurity laboratory

---

# 🔐 Security and Ethics

This laboratory is intended strictly for educational and authorized cybersecurity practice.

All security testing will be performed only against systems, virtual machines, applications, and networks that I own or have explicit permission to test.

The laboratory provides an isolated environment where cybersecurity concepts can be studied without intentionally targeting unauthorized systems.

---

# 📸 Evidence

The following screenshots document my completed laboratory:

| No. | Evidence                   | File                       |
| --- | -------------------------- | -------------------------- |
| 1   | 7-Zip Installation         | `01-7zip-installation.png` |
| 2   | VirtualBox                 | `02-virtualbox.png`        |
| 3   | NAT Network                | `03-nat-network.png`       |
| 4   | Kali Linux VM              | `04-kali-vm.png`           |
| 5   | Kali Network Configuration | `05-kali-network.png`      |
| 6   | VirtualBox Snapshot        | `06-snapshot.png`          |

---

---

# ✅ Completion Status

| Task                      | Status      |
| ------------------------- | ----------- |
| 7-Zip Installation        | ✅ Completed |
| VirtualBox Installation   | ✅ Completed |
| NAT Network Configuration | ✅ Completed |
| Kali Linux Installation   | ✅ Completed |
| Network Configuration     | ✅ Completed |
| Connectivity Testing      | ✅ Completed |
| VirtualBox Snapshot       | ✅ Completed |
| Documentation             | ✅ Completed |

---

## 📚 Reference

The structure of this laboratory follows the Week 1 Cybersecurity Lab Setup exercise provided by the class.

The original reference repository is available on [GitHub](https://github.com/syedbilalahmed-cyber/networkwalks-B082-week1-Cybersecurity-lab-setup/blob/main/README.md?utm_source=chatgpt.com).

---

**Prepared by:** Francis Saviour Ahianyo
