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
<img width="531" height="135" alt="Picture1" src="https://github.com/user-attachments/assets/c7d93a7b-0a5d-48bb-be8d-be5be5cd1344" />
<img width="488" height="387" alt="Picture2" src="https://github.com/user-attachments/assets/37d705c5-8cca-4799-bfc4-19cd0925c57f" />
<img width="602" height="52" alt="Picture3" src="https://github.com/user-attachments/assets/a6f89d23-b1f5-4031-a305-73fa4f9086ed" />
<img width="602" height="163" alt="Picture4" src="https://github.com/user-attachments/assets/5dbb8904-4832-417a-b4e5-e1642a28e131" />
<img width="602" height="110" alt="Picture5" src="https://github.com/user-attachments/assets/8a03623c-4193-4f02-8d55-839c98bd82ac" />
<img width="602" height="48" alt="Picture6" src="https://github.com/user-attachments/assets/4aab241b-7551-42a1-ab84-951c05613e57" />
<img width="602" height="77" alt="Picture7" src="https://github.com/user-attachments/assets/76720942-eb3a-4aed-bae7-f8a6866478c5" />
<img width="602" height="110" alt="Picture8" src="https://github.com/user-attachments/assets/dbadd047-5d4d-4fda-a3ab-9b049f05d0fa" />
<img width="602" height="236" alt="Picture9" src="https://github.com/user-attachments/assets/9623de06-143d-4510-9b3d-9d63e03dab47" />
<img width="254" height="41" alt="Picture10" src="https://github.com/user-attachments/assets/9d8f1f73-d83c-4bbd-a49b-9c872341cb47" />
<img width="602" height="157" alt="Picture11" src="https://github.com/user-attachments/assets/afdb3f84-1751-490d-8f7c-23d3db7703f5" />

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
