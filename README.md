# pfSense

Welcome to my pfSense exploration project! In this repository, I'll take you on a journey through the world of firewall security as I deploy pfSense in my homelab environment.

<h3>WHAT IS PFSENSE?</h3>

pfSense is a powerful, open-source firewall and routing platform based on FreeBSD. It offers a wide range of features and capabilities, making it an ideal choice for securing networks of all sizes, from small home networks to large enterprise environments. pfSense is renowned for its flexibility, performance, and robust security features.

<h3>WHY PFSENSE?</h3>

Firewalls are a critical component of network security, and pfSense is an excellent tool to explore and master firewall concepts. With pfSense, I can:

**1. Learn Firewall Fundamentals:** I'll dive into the core principles of firewalling, including packet filtering, NAT (Network Address Translation), VPN (Virtual Private Network) setup, and more.

**2. Expand Security Skills:** pfSense provides a platform for honing my skills in network security, intrusion detection, content filtering, and threat prevention.

**3. Customization:** I can tailor pfSense to meet my specific needs, whether it's for a home network, a lab environment, or even a production network.

<h3>HANDS ON, TIME TO INSTALL PFSENSE</h3>

**Prerequisites:**

Before you begin, ensure that you have the following:

1. A machine with at least two network interfaces (NICs).
2. A USB drive (minimum 4GB) to create a bootable pfSense installer.
3. A stable internet connection for downloading pfSense.

**Step 1: Download pfSense ISO**

1. Go to the pfSense download page: https://www.pfsense.org/download/.
2. Select the appropriate architecture for your hardware (usually "AMD64" for 64-bit systems).
3. Download the pfSense ISO image.

**Step 2: Create a Bootable USB Drive**

1. Download a tool like Rufus (for Windows) or Etcher (for Linux/macOS) to create a bootable USB drive.
2. Insert your USB drive into your computer.
3. Open Rufus or Etcher and select the pfSense ISO file you downloaded earlier.
4. Choose your USB drive as the target device.
5. Click "Start" or "Flash" to create the bootable USB drive. This process will erase any existing data on the USB drive.

**Step 3: Boot from the USB Drive**

1. Insert the bootable USB drive into your target machine.
2. Restart your machine and boot from the USB drive. You may need to access your BIOS or UEFI settings to set the boot order to prioritize the USB drive.

**Step 4: pfSense Installation**

1. When the pfSense installer menu appears, select "Install pfSense."
2. Choose your preferred keymap, and press "Enter."
3. Accept the pfSense software license agreement.
4. Select the installation mode. For most users, "Install" is the recommended option.
5. Choose the target drive where you want to install pfSense. Typically, this will be the primary hard drive of your machine.
6. Confirm the installation by typing "YES" (in uppercase) and press "Enter."
7. Wait for the installation process to complete.
8. Once the installation is finished, remove the USB drive and reboot your machine.

**Step 5: Initial pfSense Configuration**

1. After rebooting, you'll see pfSense booting up. It will assign IP addresses to your network interfaces. Note down the LAN interface's IP address, which is typically 192.168.1.1.
2. Open a web browser on another computer and enter the LAN interface's IP address in the address bar (e.g., http://192.168.1.1).
3. You'll be prompted to set up the initial configuration, including the administrator password and the WAN interface configuration.
4. Follow the on-screen prompts to complete the initial setup. You'll have the option to configure WAN and LAN settings, DHCP, and other network configurations.

Once the initial configuration is complete, you'll have access to the pfSense web interface.

**Step 6: pfSense Configuration**

Now that you have pfSense installed and configured, you can use the web interface to set up firewall rules, configure network services, and manage your firewall.

This is a basic overview of the installation process. Please refer to the official pfSense documentation for more detailed instructions and troubleshooting if needed.
</p>
<img src="https://i.imgur.com/EH4w56o.png" alt="pfSense access via CLI an example"/>
<i>pfSense access via CLI an example</i>
</p>
<img src="https://i.imgur.com/b7Es9Bl.png" alt="pfSense Web Interface"/>
<i>pfSense Web Interface</i>
</p>

**Contributions are more than Welcome**

I encourage contributions, feedback, and collaboration from the community. If you have suggestions, improvements, or questions, please feel free to open issues or submit pull requests.

Thank you,</br>
Lucas

