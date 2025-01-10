# Installing-Kali-on-virtual-box
<h2>Step 1: Download Kali Linux ISO</h2>
<a href="https://www.kali.org/get-kali/#kali-virtual-machines">Click here</a> to Visit the Official Kali and download the latest version of Kali Linux ISO suitable for your system (32-bit or 64-bit). Generally, you'll want the 64-bit version if your system supports.

<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Download%20Kali.png">

Extract the file.

<img src="https://github.com/Corporate101/Setting-up-a-Virtual-home-Lab/blob/main/Folder/Extract%20file.jpg">
<h2>Step 2: Create a New Virtual Machine</h2>
At this stage, I believe you've already downloaded and installed virtual box, if not, I have create a <a href="https://github.com/Corporate101/Setting-up-a-Virtual-home-Lab/blob/main/Creating%20Windows%20Virtual%20machine.md">guide here</a> on how to go about it.
Open VirtualBox and click on "New".

<img src="https://github.com/Corporate101/Setting-up-a-Virtual-home-Lab/blob/main/Folder/New.jpg">

<h2>Name and Operating System</h2> Name your VM (e.g., "Kali Linux") and select "Linux" as the Type, "Ubuntu(64-bit)" as the Version if you're using the 64-bit ISO.

<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Name%20your%20OS.png">

<h2>Step 2: Memory Size:</h2> Allocate at least 4096 MB, but 8192 MB (8 GB) or more is recommended for smoother performance.
Processor: Allocate at least 4 CPUs if available.

<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Base%20mem%20and%20Proccessor.png">

<h2>Step 3: Create a Virtual Hard Disk</h2>
Set the size to at least 20 GB for Kali Linux, but you can increase this if you have space.

<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Create%20HDD.png">

<H2>Step 4: Configure VM Settings</H2>
Select your VM and click "Settings":
Storage: Click on the empty CD symbol under Controller: IDE, then choose "Choose a disk file..." and select the Kali Linux ISO you downloaded.

<img src="https://github.com/Corporate101/Setting-up-a-Virtual-home-Lab/blob/main/Folder/Attach-an-ISO.jpg">

<h2>Step 5: Configure the Network</h2>
Ensure that your network settings are configured appropriately. It's recommended to use Bridged Adapter network settings as your VM acts like any other device on your physical network. It gets its own IP address directly from your network's DHCP server or can be statically configured, allowing it to interact with other devices on your network as if it were a physical machine. 

<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Linux%20Network.png">

<h2>Step 6:Start the VM</h2>
Click on "Start" to boot the VM. After booting, you'll be prompted to log in. The default username and password for Linux is "kali"

<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Click%20on%20start.png">
<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Start%20your%20Linux%20VM.png">

<H2>Step 7: Update Kali</H2>
Open a terminal and run, "sudo apt update"

<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Open%20The%20terminal.png">

 After updating, run "sudo apt upgrade -y" to upgrade your Linux

<img src="https://github.com/Corporate101/Installing-Kali-on-virtual-box/blob/main/Folders/Upgrade%20your%20VM.png">

<h2>Additional Tips:</h2>
<ul>
<li>Keep your VM software and Kali Linux updated for security purposes.</li>
<li>Allocate resources to the VM based on your host machine's capabilities to ensure smooth performance.</li>
<li>Familiarize yourself with the Kali Linux interface and tools for effective usage.</li>
</ul>
That's it! You now have Kali Linux installed on your virtual machine.
