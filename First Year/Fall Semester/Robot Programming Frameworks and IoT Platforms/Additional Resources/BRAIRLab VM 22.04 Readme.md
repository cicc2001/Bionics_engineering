# BRAIR Lab Ubuntu YARP/ROS VirtualBox Image


## How to run the Virtual Machine (VM) on a x86 PC
1. Install [VirtualBox](https://www.virtualbox.org/wiki/Downloads) ( >= v7.1) 

2. Download the image file **BRAIR VM 22.04** 

3. Launch VirtualBox

4. Import `.ova` image:
    - select `File menu -> Import Appliance`
    - NOTE: This file is too large even for git's Large File System transfers, so you will need to get the image from Teams, or from a classmate who has access to Teams (i.e., using Google Drive, or a physical thumb drive).

5. Start the VM
    - `user: brairlab`
    - `password: roscourse`

**Note** for Windows 11 Users:
If required during installation installation, install the [Microsoft Visual C++ Redistributable Framework](https://aka.ms/vs/17/release/vc_redist.x64.exe).

##  Alternatively, if you want to use your local Ubuntu 22.04

1. Install **Visual Studio Code** from Ubuntu Software 
    - From **Extensions**, install:
        - [*Python*](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
        - [*ROS*](https://marketplace.visualstudio.com/items?itemName=ms-iot.vscode-ros)

2. Install **ROS2 Humble**
 following the official installation guide [here](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debs.html#setup-sources).


3. Install **YARP** following the official installation guide [here](https://www.yarp.it/latest/install_yarp_linux.html).
    - Install the **ICub's software**: 
        ```bash
        $ sudo apt install icub

        $ echo "export LD_LIBRARY_PATH=/usr/lib/yarp:$LD_LIBRARY_PATH" >> ~/.bashrc 
        ```
