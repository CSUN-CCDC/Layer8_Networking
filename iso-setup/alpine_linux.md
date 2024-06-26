clear## Alpine linux 

>link to get alpine linux :https://www.alpinelinux.org/downloads/
>Once you get the iso file you need for your machine load up your virtual box and run though the normal steps of setting up a VM

### Setting up Alpine Linux
1. Open VM box 
1. Click Machine and click new
1. Virtual machine name and operating system
    - Name: < machine name >
    - ISO Image : < load alpine ISO >, click next
1. Hardware
    - Base Memory : < whatever you would like >
    - Processors: < always half of what you have for processors I have 6 i use 3 for my vm >
1. Virtual hard disk
    - Disk Size: < For linux i try and use about 15 to 20 GB >
1. Summary 
    - Click finish

### Booting up apline
1. Click the new Apline machin you just made 
1. Click the start arrow at the top right.
    - your system should start
        - This is the first error I have run into:
            ```
                alpine [Running]-Oracle VM VirtualBox
                ISOLINUX 6.04 6.04-pre1 ETCD Copyright (C) 1994-2015 H. Peter Anvin et al 
                boot:
                This kernel requires an x86-64 CPU, but only detected an i686 CPU.
                Unable to boot - please use a kernel appropriate for your CPU 
            ```
            * To fix this
                - Shutdown Alpine linux 
                - Open setting for the Alpine machine you made
                - Open **General**
                - Click Basic
                > Change version to Other /Unknown (64-bit)
                - Start up your Alpine vm again
                <above texted worked 6/2/2024>
1. localhost login : root
1. loalhost:~# setup-alpine
1. select keyboard layouts: us
1. Enter system hostname [localhost] alpine-vmbox
1. Available interfaces are :< Some interface >
    - Which do you want to initialize ? [select interface]
1. Ip address for eth0? [dhcp]
    - Do you want to do any manual nework configuration?(y/n) [n]
1. Chnaging passwork for root
    - New password: <enter your password>
1. Which time zone are you in ? [UTC] < America/Chicago>
1. HTTP/FTP proxy URl? [none]
1. Enter a mirror number [1]
1. Setup a user? < enter a name >
1. Enter a passwork for user
1. Enter ssh key or url for < user > [none]
1. Which ssh server? [openssh]
1. Which disk(s) would you ike to use ? [vda]
1. How would you like to use it? [?] sys
1. **WARNING** Earse the above disk(s) and continue? [n] y
1. **Installation is commplete** 
> you can reboot by typing poweroff and then restarting the vm box machine


