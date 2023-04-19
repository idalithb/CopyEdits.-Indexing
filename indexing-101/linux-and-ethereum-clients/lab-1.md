# Lab 1: Sync a Gnosis blockchain node
This lab exercise assumes you are configuring a [Hetzner AX102 dedicated root server](https://www.hetzner.com/dedicated-rootserver/ax102) for your Gnosis blockchain node.

## Configure the server
### Put your Hetzner AX102 server into RescueMode
1. Log in to your Hetzner account and go to the "Server" tab.
1. Select the server you want to put into RescueMode.
1. Click on the "Rescue" tab in the server details.
1. Choose the Rescue system you want to use and click on "Activate".
1. Wait for the system to activate, which may take a few minutes.
1. Once the Rescue system is active, you can log in using the provided login credentials.

### Install the [Ubuntu 22.04](https://releases.ubuntu.com/22.04/) Linux distribution with the [`installimage`](https://docs.hetzner.com/robot/dedicated-server/operating-systems/installimage/) script
1. Use the password displayed on Hetzner Robot to log into the Rescue System as "root".
2. Run the `installimage` script by typing the following command
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

### Install Linux packages
1. Update packages
    ``` bash
    apt update && apt upgrade 
    ```

1. Install build-essential
    ``` bash
    apt install build-essential 
    ```

1. Install `git`
    ``` bash
    apt install git
    ```

1. Install `unzip`
    ``` bash
    apt install unzip
    ```

1. Install `ufw` firewall
    ``` bash
    apt install ufw 
    ```



### User management
1.  Add a new user account named `dev` to a Linux system
    ``` bash
    adduser dev 
    ```

1. Adds the `dev` user to the `sudo` group, giving them the ability to execute commands with administrative privileges. Note that after running this command, the user will need to log out and log back in for the changes to take effect. This type of user account is typically used for system services or applications that need to run with a specific set of permissions, but do not require direct access to the system.
    ``` bash
    usermod -aG sudo dev
    ```
    1. `usermod` - This is the command to modify user account properties.
    2. `-aG sudo` - The `-a` option appends the specified group to the user's list of groups, while the `-G` option specifies the groups to which the user should be added. In this case, the sudo group is added to the user's list of groups.
    3. `dev` - This is the username of the user account that will be modified.

1. Add a new user account named `nethermind` to a Linux system
    ``` bash
    sudo useradd --no-create-home --shell /bin/false nethermind
    ```
    1. `sudo` - This command is used to run the useradd command with elevated privileges. This is necessary because creating a new user account requires administrative privileges.
    2. `useradd` - This is the command to create a new user account.
    3. `--no-create-home` - This option specifies that a home directory should not be created for the new user account.
    4. `--shell /bin/false` - This option sets the login shell for the new user account to `/bin/false`, which means that the user will not be able to log in to the system.
    5. `nethermind` - This is the username of the new user account that will be created.


### SSH
Coming soon


### Firewall
1. Allow incoming SSH traffic on port 22 through the system's firewall. This is necessary in order to establish SSH connections to the system from remote clients, such as other computers or mobile devices.
    ``` bash
    sudo ufw allow 22
    ```
    1. `sudo` - This command is used to run the `ufw` command with elevated privileges. This is necessary because modifying firewall rules requires administrative privileges.
    2. `ufw` - This is the command to manage the system's firewall rules using the `ufw` utility.
    3. `allow` - This option is used to add a new rule to allow incoming traffic through the firewall.
    4. `22` - This specifies the port number for the incoming traffic that should be allowed. In this case, port 22 is used, which is the default port for SSH traffic.

1. Allow incoming traffic on port 40403 through the system's firewall. This is useful when running a service or application that requires incoming traffic on that particular port, such as a web server or a database server.
    ``` bash
    sudo ufw allow 40403
    ```

1. Enable the `ufw` (Uncomplicated Firewall) utility on your system, with administrative privileges. All incoming and outgoing traffic is blocked by default, except for ports with an `allow` rule. This is a good security measure, as it prevents unauthorized access to the system.  
    ``` bash
    sudo ufw enable
    ```

## Configure the blockchain client

### Nethermind
Coming soon
