# Active-Directory-Dipesh-Lab
Active Directory Lab with VMware workstation and Windows Server 2022, OUs, Users/Groups, AGDLP Access control, GPOs

# Active Directory Home Lab (What I Built)

This repo documents exactly what I configured to demonstrate skills relevant to a **Technology Officer** role: working in a virtualized environment, deploying Active Directory, and performing core identity and access tasks (users, groups, and departmental structure).

## Summary 
- **Virtualization & OS install:** Built a Windows Server 2022 VM in VMware Workstation and managed its resources.
- **Directory services:** Promoted the server to a domain controller for **DipeshAD.local**.
- **Identity & access basics:** Created users and both **security** and **distribution** groups.
- **Department structure:** Designed **Organizational Units (OUs)** for multiple departments like **ICT**, **Mental Health**, **Rehab**, with sub‑OUs for **Computers**, **Server**, and **Users**.
- **Administration tools:** Used **Active Directory Users and Computers (ADUC)** to provision and organize objects.
- **Verification:** Signed in with the domain’s **Administrator** account (screenshot evidence).

## Lab Details
- **Host:** VMware Workstation
- **VM (Server):** Windows Server 2022
  - Memory: **4 GB**
  - vCPU: **2**
  - Disk: **60 GB**
  - Network: **NAT**
- **Domain:** `DipeshAD.local`

## What I Configured (Step List)
1. **Created the VM in VMware** and allocated resources (4 GB RAM, 2 vCPU, 60 GB disk, NAT).  
2. **Installed Windows Server 2022** and configured it as a **Domain Controller** for `DipeshAD.local`.  
3. **Opened ADUC** and built a department‑based **OU structure**:
   - **ICT**, **Maternity**, **Mental Health**, **Rehab**, **Food Services**, **Emergency Department**
   - Each department includes sub‑OUs: **Computers**, **Server**, **Users**
4. **Created user accounts** (example: **Dipesh Thapa** using my own username within SCUH) in the relevant department OU.
5. **Created groups** to model access and communication:
   - **Security groups:** e.g., *Engineers*, *Tech officers*, *Cybersecurity*
   - **Distribution group:** e.g., *ICT community*
   - (Where applicable I selected appropriate **group scopes** such as **Global**/**Universal**.)
6. **Verified domain login** at the Windows sign‑in screen as `DIPESHAD\Administrator`.

## Achievements from the Lab
- **Core AD administration:** user provisioning, group management, and OU design.
- **Environment setup:** building and operating Windows Server inside VMware.
- **Departmental separation:** prepares for role‑based access and policy application by area.
- **Operational readiness:** clean structure that supports join, policy, and access workflows used in service desks and endpoint teams.
  
## Evidence (Screenshots)
- `Vm storage and configuration.png` — VMware resources (4 GB RAM, 2 vCPU, 60 GB, NAT)
- `DipeshAD.png` — Domain sign‑in (`DIPESHAD\Administrator`) confirmation
- `Organisational Units.png` — Department OUs created
- `Ou and users.png` — Sub‑OUs (**Computers/Server/Users**) per department
- `ICT users.png` — Users in ICT OU (example: **Dipesh Thapa**)
- `Security Groups.png` — Security and distribution groups (Engineers, Tech officers, Cybersecurity, ICT community)
- `Dipesh User ICT.png` — New User wizard with UPN/SAM details




