# Windows NT Legacy NT6 Installer

---

## 🧠 What is it?

**Windows NT Legacy NT6 Installer** is a custom Windows PE-based setup environment that allows you to install legacy versions of Windows NT—**Windows NT 3.51**, **Windows NT 4.0**, and **Windows 2000**—on modern systems using the Windows 10 (NT 6.x) setup infrastructure. Windows 2000 is installed with the Windows 10 setup, and Windows NT 3.51 and Windows NT 4.0 are installed with DISM.

This tool is designed to **bypass the traditional text-mode setup phase**, offering a modernized, semi-automated deployment method using `.WIM` images and basic DISKPART scripting.

---

## ✅ Supported Operating Systems

- Windows NT 3.51  
- Windows NT 4.0  
- Windows 2000 (NT 5.0)

> 🚫 Windows XP and newer are not included, as other tools already exist for those. 

---

## ⚠️ Disclaimer

This project is **in development** and may not work correctly on all systems or configurations.  
Expect instability, driver limitations, and incompatibility with modern hardware.  
Use at your own risk. No warranty is provided.

---

## 📥 Download
https://drive.google.com/file/d/1JQKF3b4ueRGR47BmzS1lNWkkzjQC1G-j/view?usp=drive_link 

---

## 🔧 Features

- Disk partitioning and formatting via DiskPart
- File system selection (FAT/FAT32/NTFS)
- WIM-based OS deployment using DISM
- NTLDR bootloader configuration
- Optional reboot into installed legacy system

---

## 🖥️ Requirements

- This ISO
- Legacy-compatible BIOS system (UEFI with CSM or legacy mode. CSMWrap might work as well but no guarantee.)

---


## 🚀 How to Use

1. **Burn the ISO onto a CD or USB with Rufus or a similar tool**
   - Use a USB or ISO with your custom environment.

2. **Follow the prompts**
    - Select NT version
    - Choose disk, partition size, and file system. **The program will wipe the disk you choose to install Windows on. You can install manually if you'd like if you do not want to wipe your drive.**
    - Installation begins and configures boot files

3. **Done!**
   - Reboot and boot into your installed legacy OS

---

## 🧪 Future Goals

 - Support for unattended installs 
 - VHD deployment support
 - Windows 2000 semi-automated deployment
 - Driver deployment
 - ACPI deployment
 - UEFI support (Quibble, CSNWrap, Freeldr, Vista 5219 UEFI files)
 - Windows 10 setup support for Windows NT 3.51 and 4.0

---

## ✨ Credits
 - 2W10 / Techonus – Lead developer
 - ages2001 - for Windows NT 4.0 & Windows 2000 installs
 - archeYR/Illen - for Windows NT 3.51 installs
 - win3x.org - for FAT32 driver for NT 3.51 and NT 4.0
 - VBEMP project
 - George King and XP2ESD - for inspiration
 - Thanks to the retrocomputing & NT dev communities for inspiration

