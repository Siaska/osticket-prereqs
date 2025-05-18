# osTicket - Prerequisites and Installation Guide

## 🎯 Introduction
osTicket is a free and open-source support ticket system designed for managing customer inquiries. This guide walks through the setup on a Windows 10 virtual machine hosted on Microsoft Azure.

## 🎥 Video Demonstration
- [YouTube: How to Install osTicket with Prerequisites](https://www.youtube.com)

## 💻 Environments and Technologies Used
- Microsoft Azure (Virtual Machines)
- Remote Desktop Protocol (RDP)
- Internet Information Services (IIS)
- PHP
- MySQL/MariaDB

## 🖥️ Operating System
- Windows 10 (21H2)

---

## ✅ Prerequisites
- Azure account (permission to create virtual machines)
- Windows 10 VM deployed
- RDP access to the VM
- IIS installed and running
- PHP 7.4+ installed and configured
- MySQL or MariaDB installed
- osTicket installation files downloaded

---

## 🛠️ Installation Steps

### Step 1: Deploy the Windows 10 VM
1. Sign in to [Azure Portal](https://portal.azure.com)
2. Create a new VM using Windows 10 21H2
3. Configure networking and open port 3389 for RDP access

![Azure VM Creation](https://via.placeholder.com/800x400.png?text=Azure+VM+Creation)

---

### Step 2: Connect via Remote Desktop
1. Use Remote Desktop Connection on your local machine
2. Input the VM's public IP address and login credentials

![Remote Desktop](https://via.placeholder.com/800x400.png?text=Remote+Desktop+Connection)

---

### Step 3: Install IIS
1. Open **Control Panel > Programs > Turn Windows features on or off**
2. Check **Internet Information Services**
3. Restart and verify by visiting `http://localhost`

![IIS Installation](https://via.placeholder.com/800x400.png?text=IIS+Installation)

---

### Step 4: Install PHP
1. Download PHP 7.4 (non-thread safe) from the [official PHP site](https://windows.php.net/)
2. Extract to `C:\PHP`
3. Add PHP to system environment variables
4. Configure IIS to recognize `.php` file extension

![PHP Setup](https://via.placeholder.com/800x400.png?text=PHP+Configuration)

---

### Step 5: Install MySQL
1. Download and install [MySQL Community Edition](https://dev.mysql.com/downloads/)
2. Set a root password during setup
3. Create a new database for osTicket

![MySQL Setup](https://via.placeholder.com/800x400.png?text=MySQL+Installation)

---

### Step 6: Install osTicket
1. Download osTicket from [https://osticket.com/download](https://osticket.com/download)
2. Extract the folder into `C:\inetpub\wwwroot\osticket`
3. Set appropriate folder permissions
4. Open `http://localhost/osticket` and follow the web installer

![osTicket Web Setup](https://via.placeholder.com/800x400.png?text=osTicket+Web+Installer)

---

### Step 7: Finalize Setup
1. Rename or delete the `/setup` directory
2. Login to the osTicket admin panel to confirm setup was successful

![osTicket Dashboard](https://via.placeholder.com/800x400.png?text=osTicket+Dashboard)

---

## 🚀 Next Steps
- Configure SMTP/email piping
- Enable HTTPS via SSL certificate
- Create snapshots or backups for disaster recovery

---

**📝 End of Document**
