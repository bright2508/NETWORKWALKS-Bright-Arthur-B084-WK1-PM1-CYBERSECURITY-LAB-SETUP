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
