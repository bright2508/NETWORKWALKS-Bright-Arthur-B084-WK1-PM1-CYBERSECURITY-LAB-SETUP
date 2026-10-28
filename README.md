# NETWORKWALKS-Bright-Arthur-B084-WK1-PM1-CYBERSECURITY-LAB-SETUP
## My Cybersecurity Lab Environment Setup

## 1. Project Overview
For this project, I set up a basic cybersecurity lab using VirtualBox and Kali Linux. The main goal was to create a safe and controlled environment where I can grow my cybersecurity skills, practice penetration testing, and explore different security tools. I also configured a private virtual network for Kali Linux, which allows me to add other virtual machines and use them as targets for authorized security testing and practical learning.


## 2. Project Objectives

The **main objectives** of this project are:

• Install 7-Zip and VirtualBox.

• Download and import Kali Linux.

• Create a private NAT Network.

• Connect Kali Linux to the virtual network.

• Configure and check the IP address.

• Test network and Internet connectivity.

• Create a clean virtual machine snapshot.

• Document the setup for future projects.

## 3. Tools Needed for the Setup
   
Before starting, the following tools were needed for my setup:

## Tool	
7-Zip	- Extract compressed Kali Linux files

VirtualBox	- Run virtual machines

Kali Linux	- Operating system for cybersecurity activities and testing

## Step 1: Download and Install 7-Zip

I started by downloading 7-Zip from its official website and installed it on my computer.
7-Zip is a file extraction tool that allows me to open and extract compressed files.
It is particularly useful when working with Kali Linux files downloaded in a `.7z` archive format. After installation, I was ready to extract Kali Linux files whenever needed.


<img width="1337" height="732" alt="Image" src="https://github.com/user-attachments/assets/35422e55-65b6-433a-8ce7-6f22902a7580" />


 ## Step 2: Download and Install VirtualBox

The next step was to download and install VirtualBox on my computer. VirtualBox is a virtualization tool that allows me to run another operating system within my existing computer without replacing the main operating system.

For this project, I used VirtualBox to create and run a Kali Linux virtual machine. Once the installation was complete, I opened VirtualBox and got ready to set up the virtual machine and configure its network settings for the cybersecurity lab.
<img width="965" height="1022" alt="Image" src="https://github.com/user-attachments/assets/b89f8d18-eb24-4fad-abad-f9f9e33e4cf4" />

Here is a more natural, professional version you can copy directly into your GitHub `README.md` file.

## Step 3: Create a Private NAT Network

I created a dedicated NAT Network in VirtualBox for my cybersecurity lab. This network allows virtual machines connected to it to communicate with one another and access external networks through Network Address Translation (NAT).

Setting up a separate network helps me create a controlled environment for learning cybersecurity and carrying out authorized security testing.

### Network Configuration

| Setting      | Value       |
| ------------ | ----------- |
| Network Name | NATNetwork  |
| IPv4 Prefix  | 10.0.0.0/24 |
| DHCP         | Enabled     |
| IPv6         | Disabled    |

### Configuration Steps

1. Open VirtualBox on my computer.
2. Navigate to the Network settings or Network Manager.
3. Locate the **NAT Networks** section.
4. Create a new NAT Network.
5. Set the network name to `NATNetwork`.
6. Configure the IPv4 prefix as `10.0.0.0/24`.
7. Enable DHCP to allow connected virtual machines to receive IP addresses automatically.
8. Disable IPv6 because it is not required for this lab configuration.
9. Save the settings to complete the network setup.

After completing these steps, I had a dedicated NAT Network ready to be assigned to my Kali Linux virtual machine and other lab machines.

Note: **A NAT Network allows connected virtual machines to communicate with one another and access external networks. If you intend to isolate your lab completely from external networks, you would need a different network configuration.**

<img width="952" height="927" alt="Image" src="https://github.com/user-attachments/assets/f15c45f8-55e5-4752-945e-5d32aa972c11" />

<img width="1258" height="1051" alt="Image" src="https://github.com/user-attachments/assets/4afd0c81-993d-4e80-8c0d-48ed9011169c" />


## Step 4: Download and Import Kali Linux

I downloaded the Kali Linux virtual machine from the official Kali Linux website. After the download was complete, I prepared the virtual machine files for use in VirtualBox.

If the downloaded file was a compressed archive, I used 7-Zip to extract its contents. I then opened VirtualBox and imported the virtual machine using the provided VM file, following the appropriate import process for the file format.

Once the process was complete, Kali Linux was ready to be configured for my cybersecurity lab.

<img width="943" height="923" alt="Image" src="https://github.com/user-attachments/assets/96712431-c80c-49e6-9bdc-d01594209473" />


## Step 5: Configure the Virtual Machine

After importing Kali Linux into VirtualBox, I reviewed the virtual machine settings and configured its network adapter to connect to the NAT Network I created earlier.

### Network Adapter Configuration

| Setting | Value |
|---|---|
| Network Adapter | Adapter 1 |
| Attached To | NAT Network |
| Network Name | NATNetwork |
| Adapter Type | Intel PRO/1000 MT Desktop |

I saved the changes to apply the network configuration. This setup allows my Kali Linux virtual machine to connect to the designated NAT Network, making it possible to communicate with other virtual machines connected to the same network.

<img width="957" height="787" alt="Image" src="https://github.com/user-attachments/assets/bfa181fb-853e-46a8-b5db-bb591b8ac389" />

Here is a polished, natural version you can copy directly into your GitHub `README.md` file.

## Step 6: Start Kali Linux and Configure a Consistent IP Address

After configuring the virtual machine's network adapter, I started Kali Linux and prepared to configure a consistent IP address for the lab.

Using a consistent IP address makes it easier to identify the Kali Linux machine and manage network communication during future cybersecurity exercises.

### Network Configuration

| Setting         | Value                 |
| --------------- | --------------------- |
| IP Address      | `10.0.0.2`            |
| Subnet Mask     | `255.255.255.0 (/24)` |
| Default Gateway | `10.0.0.1`            |
| DNS Server      | `10.0.0.1`            |

This configuration was intended to make the Kali Linux virtual machine easier to identify and access within the lab network.

**Important**: Before applying these settings, confirm that `10.0.0.1` is the actual gateway address assigned to your VirtualBox NAT Network and that `10.0.0.2` is available. If DHCP is enabled, reserve the address or configure a suitable static IP to avoid address conflicts.

<img width="1917" height="1073" alt="Image" src="https://github.com/user-attachments/assets/5d603f93-e005-45de-b7a3-42ce040af16f" />

<img width="797" height="605" alt="Image" src="https://github.com/user-attachments/assets/acc6c310-cafd-4ab6-aa8c-215d1e5f7339" />


## Step 7: Test Network Connectivity

After configuring the network settings, I carried out a few connectivity tests to check whether my Kali Linux virtual machine could communicate with the network and access the internet.

These tests helped me to verify the network configuration and identify any connectivity issues that needed to be resolved before continuing with the cybersecurity lab exercises.


<img width="1901" height="942" alt="Image" src="https://github.com/user-attachments/assets/ee48d1a6-e36e-4bb8-a1c4-b5b7e37c926d" />


## Step 8: Create a Clean Virtual Machine Snapshot

After completing the initial setup and testing the network connection, I created a snapshot of my Kali Linux virtual machine.

A snapshot saves the virtual machine's state at a specific point in time. It provides a convenient way to return to a previous state if a future experiment or configuration change causes problems.

### Steps to Create the Snapshot

1. Shut down Kali Linux or prepare the virtual machine for snapshot creation.
2. Open VirtualBox and select the Kali Linux virtual machine.
3. Navigate to the **Snapshots** view.
4. Select the option to create a new snapshot.
5. Give the snapshot a clear and descriptive name, such as `Clean Kali Linux Setup`.
6. Add a short description if needed, then save the snapshot.

Creating this snapshot provides a clean recovery point that I can return to before performing further cybersecurity experiments in my lab.


<img width="917" height="892" alt="Image" src="https://github.com/user-attachments/assets/674306ce-0990-443b-9dcd-3a6689b1ef14" />
