To install Ubuntu Desktop on VirtualBox, follow these steps:

### 1. **Download VirtualBox**

- If you don’t have VirtualBox installed already, download it from [VirtualBox's official site](https://www.virtualbox.org/) and install it.

### 2. **Download the Ubuntu Desktop ISO**

- Go to the official [Ubuntu download page](https://ubuntu.com/download/desktop) and choose the version you want to install (LTS is the most stable version). Here, the version downloaded is **Ubuntu 24.04.2 LTS**

### 3. **Ubuntu Install**

* Watch [How to install Ubuntu 24.4 LTS on Virtual Box in Windows 11? || Updated 2025](https://www.youtube.com/watch?v=zQQITfFrg4U)

### 4. **Guest Addons**

* For full screen and other cool features, extra step is required (included in the YouTube video).
  Steps:
	* Open Terminal
	* Type the commands: 
		* sudo apt update
		* sudo apt install build-essential dkms linux-headers-$(uname -r)
		* From  menu -> Devices -> Insert Guest Additions CD image. The CD icon appears showing that it is mounted. 
		* Back to terminal. cd /media -> cd username  -> cd VBox_GAs_7.1.4 (or disk name saved, find with ls command)
		* ls disk to see contents -> The disk contents must contain the ==autorun.sh==  to install addons.
		* Type command ./autorun.sh. After installation finishes, press enter(return) as instructed to get terminal handle back to main command line
		* From Menu -> Machine -> ACPI shutdown
		* Reboot -> the Ubuntu VM is now adjustable when scaling or clicking the maximize button

That’s it! You now have Ubuntu Desktop running on VirtualBox. 