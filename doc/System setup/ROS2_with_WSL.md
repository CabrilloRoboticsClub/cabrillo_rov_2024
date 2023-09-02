### Install Ubuntu and WSL
1. Open `Windows PowerShell` as administrator
2. Install wsl by entering the following command
	```shell
	`wsl --install`
	```

3. Open the Microsoft store and download the latest version of [Ubuntu](https://apps.microsoft.com/store/detail/ubuntu-22042-lts/9PN20MSR04DW)

### Configure Ubuntu
1. You will be prompted to create a username and password for Ubuntu. This does not need to be the same as what you used for your windows system
2. Run the following commands
	```shell
	sudo apt update
	sudo apt upgrade
	sudo apt install xterm
	xterm
	```
3. Run the `locale` command to ensure you have UTF-8
   ```shell
   locale
	```

### SSH
1. Generate an ssh key to connect the Ubuntu VM to your GitHub account
   ```shell
   ssh-keygen
	```
2. Copy the generated ssh key
	```shell
	cat ~/.ssh/id_rsa.pub
	```
3. Add the SSH key to GitHub
	1. Log into Github and open your settings. 
	2. Scroll to `🔑 SSH and GPG keys`. 
	3. Click the `New SSH key` button located in the top right corner. 
	4. Choose a name for the key (something like ubuntu so you remember what it was for) 
	5. Paste the key from step 2 into the `Key` box
	6. Save the key by clicking `Add SSH key` 
4. Integrate VS code with the SSH key 
	1. Open [Visual Studio Code](https://code.visualstudio.com/)
	2. Click on `extensions` and search for `remote`
	3. Install [Remote Development](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.vscode-remote-extensionpack) and [Remote - SSH](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-ssh) from Microsoft
	4. A new icon will appear on the left in VS code. Click it to open `Remote Explore`
	5. At the top of `Remote Explore` there will be a dropdown menu. Click `WSL Targets`. Then the `+` button and whatever version of Ubuntu you installed

### Set up sources
*The following documentation was used for this part of the setup: [Setup Sources)](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html#setup-sources)*
1. First ensure that the Ubuntu Universe repository is enabled
	```shell
   sudo apt install software-properties-common
	sudo add-apt-repository universe
	```
2. Now add the ROS 2 GPG key with apt
   ```shell
   sudo apt update && sudo apt install curl -y
	sudo curl -sSL https://raw.githubusercontent.com/ros/rosdistro/master/ros.key -o /usr/share/keyrings/ros-archive-keyring.gpg
	```
3. Then add the repository to your sources list
	```shell
	echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] http://packages.ros.org/ros2/ubuntu $(. /etc/os-release && echo $UBUNTU_CODENAME) main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null
	```

### Install ROS2 
*The following documentation was useful for this part of the setup: [Ubuntu (Debian packages)](https://docs.ros.org/en/humble/Installation/Ubuntu-Install-Debians.html#id4)*
1. Open a terminal in VS code
2. Install desktop 
	```shell
	sudo apt install ros-humble-desktop
	```
3. Install development tools
	```shell
	sudo apt install ros-dev-tools
	```
4. FIXME
   ```shell
   git submodule init 
   git submodule update
	```
5. Source the following file
	```shell
	source /opt/ros/humble/setup.bash
	```

### Install package specific to our project
FIXME: Finish this 

Here are the commands I ran
ssh-keygen  
cat ~/.ssh/id_rsa.pub  
git clone git@github.com:CabrilloRoboticsClub/cabrillo_rov_2023.git  
xterm  
sudu apt install xterm  
sudo apt install xterm  
sudo apt update  
sudo apt install xterm  
xterm  
locale  
sudo apt install software-properties-common  
sudo add-apt-repository universe  
sudo apt update && sudo apt install curl -y  
sudo curl -sSL [https://raw.githubusercontent.com/ros/rosdistro/master/ros.key](https://raw.githubusercontent.com/ros/rosdistro/master/ros.key) -o /usr/share/keyrings/ros-archive-keyring.gpg  
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/ros-archive-keyring.gpg] [http://packages.ros.org/ros2/ubuntu](http://packages.ros.org/ros2/ubuntu) $(. /etc/os-release && echo $UBUNTU_CODENAME) main" | sudo tee /etc/apt/sources.list.d/ros2.list > /dev/null  
sudo apt update  
sudo apt upgrade  
sudo apt install ros-humble-desktop  
sudo apt install ros-dev-tools  
git submodule init  
git submodule update  
make  
source /opt/ros/humble/setup.bash  
make  
rosdep update  
sudo rosdep init  
rosdep update  
make  
sudo apt install libavdevice-dev libavformat-dev libavcodec-dev libavutil-dev libswscale-dev  
make  
sudo apt install ros-humble-v4l2-camera ros-humble-image-transport-plugins v4l2-utils  
sudo apt install ros-humble-v4l2-camera ros-humble-image-transport-plugins v4l-utils  
make  
sudo apt install ros-humble-camera-calibration  
make  
sudo apt install ros-humble-camera-calibration  
make  
make clean  
make  
LS  
ls  
cd  
ls  
ls -a  
cat .bash_history  
rov$ ros2 run image_transport h264_cam_node --ros-args -p input_fn:='/dev/video0' -p fps:=30 -p size:='640x480'  
ros2 run image_transport h264_cam_node --ros-args -p input_fn:='/dev/video0' -p fps:=30 -p size:='640x480'  
ls  
cd cabrillo_rov_2023/  
source ./install/local_setup.bash  
ros2 run image_transport h264_cam_node --ros-args -p input_fn:='/dev/video0' -p fps:=30 -p size:='640x480'  
source /opt/ros/humble/setup.bash  
ros2 run image_transport h264_cam_node --ros-args -p input_fn:='/dev/video0' -p fps:=30 -p size:='640x480'  
ros2 run h264_image_transport h264_cam_node --ros-args -p input_fn:='/dev/video0' -p fps:=30 -p size:='640x480'  
ros2 run h264_image_transport h264_cam_node  
ros2 run h264_image_transport h264_cam_node --ros-args -p input_fn:='/dev/video0' -p fps:=30 -p size:='640x480'  
ros2 topic list  