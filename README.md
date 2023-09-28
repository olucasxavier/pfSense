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

In my case, as I'm using Proxmox, I'm going to deploy pfSense using a VM (virtual Machine).
Below is a guide to help you set up pfSense in a Proxmox VM. This setup assumes you already have Proxmox installed and running on your hardware.

**Step 1: Download pfSense ISO**

1. Go to the pfSense download page: https://www.pfsense.org/download/.
2. Select the appropriate architecture for your hardware (usually "AMD64" for 64-bit systems).
3. Download the pfSense ISO image.

**Step 2: Upload pfSense ISO to Proxmox**

1. Open the Proxmox web interface using a web browser.
2. Navigate to the Proxmox node where you want to create the pfSense VM.
3. Click on "Datacenter" in the left sidebar, then select the storage where you want to upload the pfSense ISO (usually "local").
4. Click the "Upload" button and select the pfSense ISO file you downloaded. Upload it to the storage.

**Step 3: Create a New VM in Proxmox**

1. In the Proxmox web interface, select the node where you want to create the VM.
2. Click on "Create VM" to start the VM creation wizard.
3. Follow these settings in the wizard:

**- General:**

VM ID: Choose a unique ID for your VM (e.g., 100).
Name: Give your VM a descriptive name (e.g., pfSense).
Guest OS: Select "Linux 4.x/5.x Kernel."

**- CD/DVD:**

Select the pfSense ISO image you uploaded earlier.

**- System:**

BIOS: Choose "SeaBIOS" as the BIOS/UEFI.
**- Hard Disk:**

Add a hard disk if you plan to store VM data. For pfSense, you can use the default settings.
**- CPU:**

Allocate CPU cores as needed for your environment. Two cores are typically sufficient for a basic pfSense setup.
**- Memory:**

Allocate RAM based on your needs. A minimum of 2GB is recommended for pfSense.
**- Network:**

Select your network interfaces. Assign at least two network interfaces to your pfSense VM (one for WAN and one for LAN). Use the "virtio" driver for better performance.

**- Confirm:**

Review your settings and click "Finish" to create the VM.

**Step 4: Install pfSense**

1. Select the newly created VM (pfSense) in the Proxmox web interface.
2. Click "Start" to boot the VM.
3. In the console window, you will see the pfSense installation process. Follow the on-screen instructions to install pfSense. Configure the WAN and LAN interfaces as needed.
4. Once the installation is complete, the VM will reboot.

**Step 5: pfSense Configuration**

1. After the VM reboots, you can access the pfSense web interface using a web browser. To do this, find the IP address assigned to the LAN interface of your pfSense VM (usually 192.168.1.1) and enter it in your browser.
2. Complete the initial pfSense configuration by following the on-screen prompts. This includes setting up the WAN and LAN interfaces, DHCP, and other network settings.
3. Once the initial configuration is complete, you'll have full access to the pfSense web interface for further configuration, firewall rule setup, and network management.

That's it! You've successfully installed pfSense as a virtual machine within a Proxmox container. You can now use the pfSense web interface to configure your firewall and secure your network as needed.

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

