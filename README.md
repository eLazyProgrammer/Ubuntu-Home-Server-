# Ubuntu-Home-Server-
Documentation for my Ubuntu Home Server 

Specs: 
1. Motherboard: ASRock EP2C602 SSI EEB Server Motherboard Dual LGA 2011 Intel C602
2. CPU: Intel(R) Xeon(R) CPU E5-2670 v2 @ 2.50GHz x2
3. Case: Fractal Design Define XL R2 Black Silent EATX Full Tower Computer Case
4. RAM: Generic DDR3 8GB sticks x4
5. Cooling: CORSAIR Hydro Series H50 120mm Quiet Edition Liquid CPU Cooler - Intel Only x2
6. HDD: WD Red 1TB x 3
7. SSD (Boot): Samsung EVO 500GB

Introduction:
Main inspiration for the start of this project was due to a hard drive failure in my very first laptop. At the time, I did not know proper security hygiene and neglected to keep backups, for which I paid dearly. During my search for a reliable portable hard drive to store future backups, I came across the terms automated backups, RAID servers, and home server. From there, I learned I could host minecraft and maplestory, my own website, as well as create a file server accessible from anywhere for extra storage. With this knowledge, I used Tim Gasser's Article (https://medium.com/@timgasser/build-a-16-core-128gb-server-for-less-than-intels-new-10-core-cpu-c6de4d10a686) as a basis for my build. I'll add resources for whoever also wants to start their server. 

Post-Build Steps:
1. Download the latest Ubuntu Release (20.04) Image onto a bootable disk using Rufus (https://ubuntu.com/tutorials/create-a-usb-stick-on-windows#1-overview)
2. Go through Initial Ubuntu setup (https://ubuntu.com/tutorials/install-ubuntu-server#1-overview) 
3. Download OpenSSH (https://linuxize.com/post/how-to-enable-ssh-on-ubuntu-18-04/) (To find your server's public ip: https://linuxconfig.org/check-your-local-and-public-ip-address) (Static IP Setup: https://linuxize.com/post/how-to-configure-static-ip-address-on-ubuntu-20-04/) (Configuring your netplan yaml file: https://linuxize.com/post/how-to-set-dns-nameservers-on-ubuntu-18-04/)
5. Download Samba File Server (for the 3+ Window PC's we currently have) (Guide: https://ubuntu.com/tutorials/install-and-configure-samba#1-overview) (Due to Windows 10 disabling and actively discouraging the use of SMB1 because of stuff like wannacry ruining our fun, I used christgau's wsdd.py script to get around this. Here's a website that describes more or less what I did: https://devanswers.co/discover-ubuntu-machines-samba-shares-windows-10-network/) ( If you're able to see the server on the network but unable to enter it, try resolving the hostname: https://www.cyberciti.biz/faq/ubuntu-change-hostname-command/)
6. 
