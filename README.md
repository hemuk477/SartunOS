HI i am sure you want the file  this img file is only for QEMU vms due to simpilicity and old drivers so if you want to RUN boot.img do the following:

in windows: 7-11

go to powershell type:

> WSL --install
 go to launcher and type Ubuntu or other linux distro

select the appwait 12 min after that follow to instructions by adding username and passord
 next in the shell type:

 $ sudo apt update #or other package manager ex-apt,pacman,dnf,etc

 next type:

 $ sudo apt-get install qemu-kvm #or in non-debian based shell just type qemu insted of qemu-kvm

 after that make sure you copied the file to WSL folder

 then run:

 sudo qemu-system-x86_64 boot.img --vga cirrus

 then in boot: prompt type:

 /bzImage rw root=/dev/sda

 then if you want gui then in vm type    cd nanox

 then type: ./<the file you want to run>

 note: only mw starting line files or nano-X will work 

 Linux:

 open the terminal

 and type:

$  sudo apt update #or other package manager ex-apt,pacman,dnf,etc

and type:

 $ sudo apt-get install qemu-kvm #or in non-debian based shell just type qemu insted of qemu-kvm

  then run:

 sudo qemu-system-x86_64 boot.img --vga cirrus

 then in boot: prompt type:

 /bzImage rw root=/dev/sda

 then if you want gui then in vm type    cd nanox

 then type: ./<the file you want to run>

 note: only mw starting line files or nano-X will work 

 macOS 13->16

 same as linux but brew is required in place of linux pkg manager

Done!!

 


 

 
