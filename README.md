# vagrantFlexSwitch
This repository contains vagrant related files for FlexSwitch

Instructions on how to get Vagrant box up with FlexSwitch package:

Instructions on how to get Vagrant FlexSwitch resources:

1. Make Directory Vagrant (mkdir Vagrant)
2. Change Directory to Vagrant Directory (cd Vagrant)
3. Clone this repository using "git clone https://github.com/OpenSnaproute/vagrantFlexSwitch.git"
4. Change directory (cd vagrantFlexSwitch)
5. Execute this step if git lfs is not installed

> For Debian based Host Machines:

      curl -s https://packagecloud.io/install/repositories/github/git-lfs/script.deb.sh | sudo bash
      
      sudo apt-get install git-lfs
      
> For Mac OSX, please follow the steps on given link: [Git LFS OSX] (http://macappstore.org/git-lfs/ "Git LFS OSX").
      
      
7. git lfs install
8. git lfs fetch
9. git lfs checkout

Note:
Please verify the size of files in this repository, if sizes are not same there is some issue with git lfs. Please refer to [Git LFS Debian] (https://git-lfs.github.com/ "Git LFS Debian"). or [Git LFS OSX] (http://macappstore.org/git-lfs/ "Git LFS OSX").

>

      opensnaproute@snaproute-lab-r815-2:~/Vagrant/vagrantFlexSwitch$ ls -lart

      total 816236

      drwxrwxr-x 3 opensnaproute opensnaproute      4096 Jul 22 09:24 ..

      -rw-rw-r-- 1 opensnaproute opensnaproute      3601 Jul 22 09:24 Vagrantfile

      -rw-rw-r-- 1 opensnaproute opensnaproute       663 Jul 22 09:24 README.md

      drwxrwxr-x 3 opensnaproute opensnaproute      4096 Jul 22 09:24 .

      -rwxrwxr-x 1 opensnaproute opensnaproute 835800676 Jul 22 09:28 snaproute.box

      drwxrwxr-x 9 opensnaproute opensnaproute      4096 Jul 22 09:29 .git

In case you run into issues with github you can download the vagrant files from our  [Google Drive] (https://drive.google.com/open?id=0B2sb_hH-7YHycHYtSndVbU1GVzg "Google Drive Vagrant Flexswitch")

Instructions on how to run this vagrant (snaproute.box):

1. vagrant box add SnapRoute170 snaproute.box
2. vagrant up
3. vagrant ssh
4. password is "vagrant"
      
This vagrant image is based on Ubuntu 14.04 and two ports are created within this image by default "Eth0" and "Eth1".
"Eth1" will be your management interface ip address if you are using public network
