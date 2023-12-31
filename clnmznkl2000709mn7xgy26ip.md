---
title: "Linux Installation Fest: Guide to installing linux"
datePublished: Thu Oct 12 2023 09:39:41 GMT+0000 (Coordinated Universal Time)
cuid: clnmznkl2000709mn7xgy26ip
slug: linux-installation-fest-guide-to-installing-linux
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1697103514955/7f55650d-99d8-4595-ba4b-2ec5f2d03c20.jpeg
tags: ubuntu, operating-system, linux, opensource, linux-for-beginners

---

Greetings Freshers. Embarking on your university journey brings with it a whirlwind of experiences and opportunities. Among these is the chance to dive deep into the vast world of technology. And what better way to start than by immersing yourself in the world of Linux?

### **Why Linux for Freshers?**

Linux, unlike commercial operating systems, is all about freedom, flexibility, and community support. As a fresher:

1. **Learn & Experiment**: Get hands-on experience with real-world tech skills. Linux offers a safe environment to experiment and learn.
    
2. **Stand Out**: With Linux proficiency under your belt, you're setting yourself apart in the tech world.
    
3. **Community**: Linux isn't just an OS; it's a vibrant community of passionate tech enthusiasts. Being a part of this community aids in learning and networking.
    

Linux, an open-source operating system, offers an enticing blend of freedom, speed, and variety. Whether you’re looking for more customization capabilities, a more stable system, or merely the thrill of diving into something new – Linux is the answer.

---

### **Preparation: Essential Downloads and Checks**

**For Windows Users**:

1. **Ubuntu 22.04** - An efficient and user-friendly Linux distribution.
    
    * **Download**: [Ubuntu 22.04](https://ubuntu.com/download/desktop/thank-you?version=22.04.3&architecture=amd64)
        
2. **Pendrive**: Make sure you have an 8GB (or larger) Pendrive.
    
3. **VMware VirtualBox**: This tool allows you to run Linux virtually on your Windows system without affecting your primary OS.
    
    * **Download**: [VMware VirtualBox](https://download.virtualbox.org/virtualbox/7.0.10/VirtualBox-7.0.10-158379-Win.exe)
        
4. **Balena Etcher**: An application to flash the Ubuntu image onto your pendrive, making it bootable.
    
    * **Download**: [Balena Etcher](https://github.com/balena-io/etcher/releases/download/v1.18.11/balenaEtcher-Setup-1.18.11.exe)
        
5. **Disk Space**: Ensure you have at least 60GB (100GB recommended) free on your laptop.
    

**For Mac Users**:

1. **Ubuntu 22.04 for ARM64** - Tailored for Macs with ARM architecture.
    
    * **Download**: [Ubuntu 22.04 ARM64](https://cdimage.ubuntu.com/releases/22.04/release/ubuntu-22.04.3-live-server-arm64.iso)
        
2. **UTM**: A virtualization tool for Mac.
    
    * **Download**: [UTM](https://github.com/utmapp/UTM/releases/latest/download/UTM.dmg)
        
3. **Disk Space**: Ensure around 40-50GB of disk space is available.
    

---

### **Step-by-Step Installation Guide**

#### **Dual Boot with Windows**:

1. **Backup**: Always back up important files. While the installation is usually safe, it’s best to be prepared.
    
2. **Create a Bootable Pendrive**:
    
    * Install and run Balena Etcher.
        
    * Select the downloaded Ubuntu 22.04 ISO and your pendrive.
        
    * Click “Flash!” to create your bootable drive.
        
3. **Partition Your Drive**:
    
    * In Windows, open 'Disk Management'.
        
    * Shrink your primary partition by the desired amount (at least 60GB is recommended).
        
    * This will create an 'Unallocated' space where Linux will be installed.
        
4. **Install Linux**:
    
    * Restart your computer and boot from the pendrive (this often involves pressing F12, F2, or the DEL key during startup).
        
    * When presented with the Ubuntu setup, choose 'Install Ubuntu'.
        
    * When asked about installation type, select 'Install alongside Windows'.
        
    * Follow on-screen instructions, and select the 'unallocated' space when prompted for the installation location.
        
5. **GRUB Bootloader**:
    
    * Post-installation, your computer will use the GRUB bootloader. It allows you to choose between Windows and Linux at startup.
        

#### **Bootcamp for Mac**:

1. **Backup**: Ensure all your data is backed up using Time Machine or another backup solution.
    
2. **Install UTM**:
    
    * Download and run the UTM application.
        
3. **Setup a New Virtual Machine (VM)**:
    
    * Click “+” in UTM to create a new VM.
        
    * Name your VM, choose the OS type as Linux, and select the downloaded Ubuntu ARM64 ISO as your installation media.
        
4. **Allocate Resources**:
    
    * Assign at least 2 cores and 4GB RAM to your VM for optimal performance. Adjust the disk size based on your needs.
        
5. **Install Linux**:
    
    * Start the VM and follow the on-screen instructions to install Ubuntu.
        
6. **Accessing Ubuntu**:
    
    * Whenever you wish to use Linux, open UTM and run your VM.
        

### **Guidance and Support**

While our step-by-step guide is here to help, remember this: at the installation fest, you'll be surrounded by seniors and experts ready to assist. We've all been in your shoes, and we're eager to help you step into the Linux universe.

**Tips for the Fest**:

1. **Ask Questions**: No question is too small. If you're unsure about something, ask!
    
2. **Network**: This is a golden chance to interact with seniors who've been through the tech grind. They can offer insights and guidance, and might even have cool project opportunities.
    
3. **Stay Patient**: Installing a new OS is a significant step, and sometimes things can go awry. But with persistence and guidance, you'll get there!
    

---

**Pro Tip**: The beauty of Linux lies in its extensive community. If you stumble upon a roadblock, a quick search or a visit to Linux forums will often provide a solution.

---

### **What After the Installation?**

After you've successfully installed Linux, the real fun begins. Start exploring, customize your desktop, try out different software, and most importantly, dive into the terminal. The world of Linux commands awaits, offering you unmatched control over your system.

---

As you take your first steps in the tech domain with Linux, remember that every expert was once a beginner. This fest isn't just about installing an OS; it's about taking that first significant leap into the world of technology.

Welcome aboard the Linux train, and here's to many tech adventures ahead! 🐧🚀🎉