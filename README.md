# vagrantFlexSwitch
This repository contains vagrant related files for FlexSwitch

Instructions on how to get Vagrant box up with FlexSwitch package:

Download this file "snaproute.box" and "VagrantFile" from [Github OpenSnapRoute Vagrant] (https://github.com/OpenSnaproute/binaries/tree/master/vagrant "Vagrant").  

1. Make folder to store images:
   mkdir srBox; cd srBox
2. Copy files into srBox:
   cp snaproute.box VagrantFile srBox/
3. vagrant box add SnapRoute112 snaproute.box
4. vagrant up
5. vagrant ssh
   password is vagrant
      
This vagrant image is based on Ubuntu 14.04 and two ports are created within this image by default "Eth0" and "Eth1".
