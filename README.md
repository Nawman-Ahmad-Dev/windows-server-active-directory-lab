# 🖥️ Windows Server Active Directory + IIS Website Lab

This project simulates a real corporate IT environment using **Windows Server 2019** and **Windows 10/Windows 11** virtual machines.  
It demonstrates how to deploy and manage an **Active Directory domain**, **DNS**, **Group Policies**, and a **hosted intranet website** using IIS.

---

## 🧱 Lab Setup

**Environment**
- **Virtualization:** Oracle VM VirtualBox  
- **VMs Used:**
  - 🧩 Windows Server 2019 — Domain Controller + DNS + IIS
  - 💻 Windows 10/11 — Domain-joined Staff
- **Network:** Bridged Adapter (same LAN)
- **IP Setup:** Static IP on Server, DHCP on Staff

**Lab Topology**
[Windows 10 Staff] ↔ [Windows Server 2019 Domain Controller + DNS + IIS]
192.168.x.10 192.168.x.9 (nawlab.local)

## ⚙️ Key Tasks Completed

1. **Installed and configured Windows Server 2019**
   - Promoted server to **Domain Controller**
   - Installed and configured **Active Directory Domain Services (AD DS)**
   - Set up **DNS** for domain resolution

2. **Active Directory Management**
   - Created **Organizational Units (OUs)** for departments
   - Added **users** and **security groups**
   - Set password policies and login restrictions via **Group Policy**

3. **Client Domain Join**
   - Joined Windows 10/11 machine to `nawlab.local` domain
   - Verified user login through AD

4. **Website Hosting (IIS + Node.js)**
   - Installed **Node.js** for project dependencies
   - Deployed static site to IIS folder `C:\inetpub\wwwroot`
   - Verified internal website accessibility at `http://192.168.x.9`

5. **Testing & Troubleshooting**
   - Confirmed **connectivity** via ping between VMs
   - Validated **DNS and Group Policy** functionality
   - Documented full setup and IP configuration

---

## 🧠 Skills Demonstrated

- Windows Server 2019 administration  
- Active Directory, DNS, and Group Policy  
- IIS web hosting and Node.js deployment  
- Virtualization and networking configuration  
- System troubleshooting and documentation  
