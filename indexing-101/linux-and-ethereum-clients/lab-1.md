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
    installimage -n slimdexor -r no -i images/Ubuntu-2204-jammy-amd64-base.tar.gz -d sda -p /boot:ext3:1024M,lvm:vg0:all -v vg0:root:/:ext4:all
    ```








## Configure the blockchain client

