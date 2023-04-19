# Lab 1: Sync a Gnosis blockchain node
This lab exercise assumes you are configuring a [Hetzner AX102 dedicated root server](https://www.hetzner.com/dedicated-rootserver/ax102) for your Gnosis blockchain node.

## Configure the server
Put your Hetzner AX102 server into RescueMode
1. Log in to your Hetzner account and go to the "Server" tab.
1. Select the server you want to put into RescueMode.
1. Click on the "Rescue" tab in the server details.
1. Choose the Rescue system you want to use and click on "Activate".
1. Wait for the system to activate, which may take a few minutes.
1. Once the Rescue system is active, you can log in using the provided login credentials.

Install the [Ubuntu 22.04](https://releases.ubuntu.com/22.04/) Linux distribution with the [`installimage`](https://docs.hetzner.com/robot/dedicated-server/operating-systems/installimage/) script
1. Use the password displayed on Hetzner Robot to log into the Rescue System as "root".
2. Run the installimage script by typing the following command
    ``` bash
    installimage -n GnosisNode -r yes -i images/Ubuntu-2204-jammy-amd64-base.tar.gz -d sda -p /boot:ext3:1024M,lvm:vg0:all -v vg0:root:/:ext4:all
    ```
    
    Overall, this command will perform an installation of Ubuntu 22.04 on the "sda" device using the specified partition and logical volume layout, with the hostname set to "GnosisNode" and the server rebooting automatically after the installation is complete.

    1. `installimage` - This is the command to execute the installimage script.
    2. `-n GnosisNode` - This sets the hostname for the server to "GnosisNode".
    3. `-r yes` - This specifies that the server should automatically reboot after the installation process is complete.
    4. `-i images/Ubuntu-2204-jammy-amd64-base.tar.gz` - This specifies the path to the base installation image for Ubuntu 22.04. In this case, the file is located in the "images" directory and is named "Ubuntu-2204-jammy-amd64-base.tar.gz".
    5. `-d sda` - This specifies the device that will be used for the installation. In this case, the installation will be performed on the "sda" device.
    6. `-p /boot:ext3:1024M,lvm:vg0:all` - This specifies the partition layout for the installation. In this case, there will be two partitions created: one for the "/boot" directory, which will be formatted with the ext3 file system and will have a size of 1024MB, and one for LVM, which will contain all remaining space on the disk and will be used for logical volume management.
    7. `-v vg0:root:/:ext4:all` - This specifies the logical volume layout for the installation. In this case, one logical volume named "root" will be created in the volume group "vg0", which will be mounted at the root directory ("/") and formatted with the ext4 file system.





















## Configure the blockchain client

