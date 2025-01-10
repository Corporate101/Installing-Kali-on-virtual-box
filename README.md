# Installing-Kali-on-virtual-box
<h2>Step 1: Download Kali Linux ISO</h2>
<a href="https://www.kali.org/get-kali/#kali-virtual-machines">Click here</a> to Visit the Official Kali and download the latest version of Kali Linux ISO suitable for your system (32-bit or 64-bit). Generally, you'll want the 64-bit version if your system supports it.

<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Download%20Kali.png">

<h2>Step 2: Create a New Virtual Machine</h2>
At this stage, I believe you've already downloaded and installed virtual box, if not, I have create a <a href="https://github.com/Corporate101/Setting-up-a-Virtual-home-Lab/blob/main/Creating%20Windows%20Virtual%20machine.md">guide here</a> on how to go about it.
Open VirtualBox and click on "New".

<img src="https://github.com/Corporate101/Setting-up-a-Virtual-home-Lab/blob/main/Folder/New.jpg">

Name and Operating System: Name your VM (e.g., "Kali Linux") and select "Linux" as the Type, "Ubuntu(64-bit)" as the Version if you're using the 64-bit ISO.

<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Name%20your%20OS.png">

Memory Size: Allocate at least 4096 MB, but 8192 MB (8 GB) or more is recommended for smoother performance.

<img src="">

Hard Disk: Choose "Create a virtual hard disk now".
Hard Disk Settings:
File Location and Size: Use VDI (VirtualBox Disk Image) for type. 
Storage on Physical Hard Drive: Dynamically allocated is better for saving space, but fixed size gives better performance.
File Location: Keep the default or choose another location for the VM's HDD file.
Size: A minimum of 20 GB is recommended, but more space is better for storing tools and data.
Processor: Allocate at least 2 CPUs if available.

<img src="">

<H2>Step 4: Configure VM Settings</H2>
Select your VM and click "Settings":
System > 
Display > Video: Max out the Video Memory if possible.
Storage: Click on the empty CD symbol under Controller: IDE, then choose "Choose a disk file..." and select the Kali Linux ISO you downloaded.

<img src="">

Step 5: Install Kali Linux
Start your VM. You should boot into the Kali Linux live environment.
Select "Graphical install" or "Install" from the list of options.

Installation Process:
Language, Location, Keyboard: Choose your preferences.
Network: You can configure now or skip for later.
Hostname: Name your machine (e.g., kali).
Domain name: Usually left blank unless part of a domain.
Root Password: Set a strong password.
User Account: Create a non-root user with a password.
Partitioning: Choose "Guided - use entire disk" for simplicity.
Partition Disks: Write changes to disk.
Mirror: Select your country for the software repository.
Package Manager: Update and install GRUB boot loader.
Device for boot loader installation: Usually, the default drive.

Step 6: Finalize Installation
After installation, reboot the VM when prompted. Ensure you remove the ISO from the virtual CD drive (eject in VirtualBox Storage settings) to boot from the HDD.

Step 7: Post-Installation
Login with your user or root credentials.
Update Kali: Open a terminal and run:
bash
sudo apt update && sudo apt upgrade -y
Install Guest Additions: This improves VM performance and usability. From VirtualBox menu, go to "Devices" > "Insert Guest Additions CD image", then run the script from the mounted drive in Kali.
