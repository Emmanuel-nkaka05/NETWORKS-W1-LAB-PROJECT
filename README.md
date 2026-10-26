# Week 1 - Project Module 1
## Lab Setup: VirtualBox and Kali Linux Installation

---

# Objective

The objective of this project was to create a virtual cybersecurity lab environment by installing Kali Linux inside Oracle VirtualBox and configuring networking to provide internet connectivity for future cybersecurity exercises.

---

# Tools Used

- Oracle VirtualBox
- Kali Linux ISO Image
- NAT Network Configuration
- Virtual Machine Snapshots

---

# Lab Environment

| Component | Configuration |
|------------|---------------|
| Hypervisor | Oracle VirtualBox |
| Operating System | Kali Linux |
| Network Type | NAT Network |
| IPv4 Network | 10.0.0.0/24 |
| DNS Server | 8.8.8.8 |
| Snapshot | Fresh Installation Snapshot |

---

# Lab Setup Procedure

## Step 1: Install Oracle VirtualBox

Oracle VirtualBox was installed on the host machine to create and manage virtual machines.

Purpose:

- Isolate the cybersecurity lab environment
- Run Kali Linux safely
- Create snapshots for recovery

---

## Step 2: Create NAT Network

A NAT Network was created before installing the operating system.

Configuration:

```text
Network Name: NatNetwork
Network Address: 10.0.0.0/24
DHCP: Enabled
```

This configuration allows internet connectivity while maintaining a private network for virtual machines.

### Evidence

Insert screenshot of NAT Network configuration below:

![NAT Network Configuration](NAT-NETWORK.png)

---

## Step 3: Create Kali Linux Virtual Machine

A new virtual machine was created with the following specifications:

```text
Operating System: Kali Linux (64-bit)
Memory: 2048 MB RAM
Storage: Virtual Hard Disk
Network Adapter: NAT Network
```

The Kali Linux ISO image was mounted as the bootable installation media.

---

## Step 4: Install Kali Linux from ISO

Unlike the sample environment that used a prebuilt virtual appliance, Kali Linux was installed manually using the official ISO disk image.

Installation tasks completed:

- Boot Kali Linux installer
- Configure system language
- Configure keyboard layout
- Configure hostname
- Create user account
- Configure password
- Partition virtual disk
- Install operating system
- Install GRUB bootloader
- Reboot into Kali Linux

Installation was completed successfully and the system booted into the Kali Linux desktop environment.

---

## Step 5: Configure Network Settings

After installation, networking was configured to ensure internet access.

Configuration:

```text
IPv4 Address: 10.0.0.2
Gateway: 10.0.0.1
DNS Server: 8.8.8.8
Subnet Prefix: /24
```

### Evidence

Insert screenshot showing network settings:

![Network Configuration](CONFIG-ADDRESSES-AND-DNS-SERVER.png)

---

## Step 6: Verify Internet Connectivity

Internet connectivity was tested after configuration.

Verification tasks:

- Access web browser
- Reach external websites
- Verify DNS resolution
- Confirm network communication

Successful web access confirmed that the Kali Linux virtual machine had internet connectivity.

### Evidence

Insert screenshot showing successful internet connection:

![Internet Connectivity](FULL-INTERNET-CONNECTIVITY.png)

---

## Step 7: Create System Snapshot

After completing installation and network verification, a VirtualBox snapshot was created.

Snapshot Name:

```text
my fresh snapshot
```

Purpose:

- Quickly restore the system if issues occur
- Maintain a clean baseline installation
- Preserve the working lab setup

---

# Challenges Encountered

### Network Configuration

Configuring the virtual machine networking required understanding how NAT Networks operate within VirtualBox and ensuring correct address assignment.

### Initial Connectivity Testing

Internet connectivity had to be verified after installation to confirm that DNS resolution and network routing were functioning correctly.

---

# Skills Gained

Through this project I learned how to:

- Install Oracle VirtualBox
- Create and configure NAT Networks
- Install Kali Linux from an ISO image
- Configure virtual machine networking
- Configure DNS settings
- Verify internet connectivity
- Create and manage VirtualBox snapshots
- Build a secure virtual lab environment

---

# Key Takeaways

This project provided practical experience in:

- Virtualisation technologies
- Operating system installation
- Network configuration
- Snapshot management
- Cybersecurity lab preparation

The completed environment provides a stable foundation for future cybersecurity exercises, penetration testing activities, and network security projects.

---

# Project Status

✅ VirtualBox Verified

✅ DNS Configuration Completed

✅ Initial Snapshot Created

✅ Cybersecurity Lab Ready

---