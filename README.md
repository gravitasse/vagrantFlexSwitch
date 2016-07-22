# vagrantFlexSwitch
This repository contains vagrant related files for FlexSwitch

Instructions on how to get Vagrant box up with FlexSwitch package (Prefered host machine is debain based linux distro.):

Instructions on how to get Vagrant FlexSwitch resources:

1. Make Directory Vagrant (mkdir Vagrant)
2. Change Directory to Vagrant Directory (cd Vagrant)
3. Clone this repository using "git clone https://github.com/OpenSnaproute/vagrantFlexSwitch.git"
4. Change directory (cd vagrantFlexSwitch)
5. Execute this step if git lfs is not installed

> curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | sudo bash

> sudo apt-get install git-lfs
      
7. git lfs install
8. git lfs fetch
9. git lfs checkout

Note:
Please verify the size of files in this repository, if sizes are not same there is some issue with git lfs. Please refer to [Git Lfs] (https://git-lfs.github.com/ "Git lfs").

>

      opensnaproute@snaproute-lab-r815-2:~/Vagrant/vagrantFlexSwitch$ ls -lart

      total 816236

      drwxrwxr-x 3 opensnaproute opensnaproute      4096 Jul 22 09:24 ..

      -rw-rw-r-- 1 opensnaproute opensnaproute      3601 Jul 22 09:24 Vagrantfile

      -rw-rw-r-- 1 opensnaproute opensnaproute       663 Jul 22 09:24 README.md

      drwxrwxr-x 3 opensnaproute opensnaproute      4096 Jul 22 09:24 .

      -rwxrwxr-x 1 opensnaproute opensnaproute 835800676 Jul 22 09:28 snaproute.box

      drwxrwxr-x 9 opensnaproute opensnaproute      4096 Jul 22 09:29 .git


Instructions on how to run this vagrant (snaproute.box):

1. Make folder to store images:
   mkdir srBox; cd srBox
2. Copy files into srBox:
   cp snaproute.box VagrantFile srBox/
3. vagrant box add SnapRoute112 snaproute.box
4. vagrant up
5. vagrant ssh
   password is vagrant
      
This vagrant image is based on Ubuntu 14.04 and two ports are created within this image by default "Eth0" and "Eth1".
