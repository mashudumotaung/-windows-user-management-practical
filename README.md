# -windows-user-management-practical
#💻 Course-3
# windows-user-management-practical

## 📌 Overview
This project demonstrates practical Windows operating system administration using PowerShell. The lab focuses on user and group management, file system permissions, and software installation using a command-line package manager.

The objective of this exercise was to apply operating system concepts in a real-world administrative environment.

---

## 🎯 Objectives
- Create and manage local users
- Assign users to security groups
- Configure NTFS folder permissions
- Install software using command-line tools
- Verify system configuration changes

---

## 🛠️ Tools & Technologies Used
- Windows PowerShell
- `net user`
- `net localgroup`
- `icacls`
- Chocolatey (Windows package manager)

---

## 🧩 Tasks Performed

### 1️⃣ User Creation
Created a new local user account using:

```
net user PowerUser1 <password> /add
```

---

### 2️⃣ Group Assignment
Added the user to the Administrators group:

```
net localgroup Administrators PowerUser1 /add
```

---

### 3️⃣ Folder Creation
Created a project directory:

```
mkdir C:\Users\Public\PowerProjects
```

---

### 4️⃣ Permission Configuration
Granted full NTFS permissions to the user:

```
icacls "C:\Users\Public\PowerProjects" /grant "PowerUser1:(OI)(CI)F"
```

Verified permissions using:

```
icacls "C:\Users\Public\PowerProjects"
```

---

### 5️⃣ Package Installation
Installed software using Chocolatey:

```
choco install notepadplusplus -y
```

Verified installation by launching the application.

---

## 📸 Screenshots
<img width="675" height="128" alt="image" src="https://github.com/user-attachments/assets/7e6af090-9469-4e20-bf8f-48134edb6d9b" />
<img width="450" height="381" alt="image" src="https://github.com/user-attachments/assets/acf635cc-d724-45ae-9b91-aaa19810fce9" />
<img width="574" height="52" alt="image" src="https://github.com/user-attachments/assets/65c2bf99-3e99-4e5c-a035-6a33192aadbe" />
<img width="751" height="202" alt="image" src="https://github.com/user-attachments/assets/296cf35e-09c4-4703-b312-defc62d862c1" />
<img width="816" height="208" alt="image" src="https://github.com/user-attachments/assets/74568304-b660-4811-9f87-e25900ffbcf3" />
<img width="943" height="142" alt="image" src="https://github.com/user-attachments/assets/dd8835b0-89fd-48e7-a3eb-f92aeb52c390" />
<img width="1316" height="222" alt="image" src="https://github.com/user-attachments/assets/1d07aa00-1df2-484c-9c35-1ed6df859694" />
<img width="1345" height="408" alt="image" src="https://github.com/user-attachments/assets/03abd953-3429-463f-8c7e-d2331c931988" />
<img width="510" height="49" alt="image" src="https://github.com/user-attachments/assets/1d2722b9-e226-4fce-86bd-f2b3cfbbe1e1" />
<img width="1193" height="185" alt="image" src="https://github.com/user-attachments/assets/046b2246-1ae9-4215-9e20-8c0079838864" />



---

## 💡 Skills Demonstrated
- Windows user and group management
- NTFS file permission configuration
- Command-line system administration
- Package management using Chocolatey
- Basic system verification and troubleshooting

---

## 🚀 Relevance
This lab demonstrates foundational system administration skills relevant to:

- IT Support
- System Administration
- Cloud Engineering
- DevOps

---

## ✅ Conclusion
This project strengthened my understanding of Windows operating system internals, user access control, and software management. It reflects practical, hands-on administrative skills using command-line tools in a Windows environment.
