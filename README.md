# Useful-Linux-Commands
This is just a simple showcase of my favourite linux commands, I will be updating this list periodically.

Favourite commands
___________________

**Manual pages and man page alternatives**

`man` The linux man pages.

`tldr` A simple alternative to the linux man pages.

**run command with superuser priviledges**

`sudo`  
**Regex filtering**

exclude pattern
`cat file.txt | awk "! /expression/"

search pattern
cat file.txt | grep "pattern"

**run last command as sudo**

`sudo !!` 

**run command as a background process**

`nohup` 

`&`

**check background jobs**

`bg`

**check linux permissions**
`id`

**print local ip addresses**

`ifconfig`

`ip a`

`ip addr`

`ip address`

**Connect over ssh**

`ssh user@hostname`

connect with key
`ssh -i key user@hostname`


**print public ip address**

`curl ifconfig.me`

**print $PATH**

`echo $PATH`

add executable to PATH variable

`PATH=$PATH:/path-to-program`


**print environments**

`env`

**print background processes** 

`ps aux`

`top`

`htop`

**print network ports and connections**

`netstat -a`

**download files from a URL**

`wget`

`curl -o`

**Reverse Engineering**
print strings from binary file
`strings file`

print objects from binary file
`objdump -d file`

print hexdump from binary file
`xxd file`

**Wifi Scanning & cracking tools**
Enable monitor mode for wifi card
`sudo airmon-ng start <interface>`

**check wifi cards and their status**

`iwconfig`

`iw dev`

**hcxdumptool & hcxpcaptool for hashcat WPA2 PMKID cracking and hash conversion**

`sudo hcxdumptool -i <interface> -w <outputfile> -F --rds=1 --beacontx=10 --gpsd`

`hashcat -m 22000 <file.hc22000> -a 3 ?d?d?d?d?d?d?d?d?d?d`

scan all wifi APs in range
`sudo airodump-ng <interface>` 

`sudo airodump-ng <interface> -c <channel> -w <pcap output file> -d <target bssid>`

`sudo aireplay-ng wlan0 -0 0 -a <bssid>`
deauth wifi AP for EAPOL capture

**start nessus**
`sudo systemctl start nessusd.service`
open browser at https://localhost:8834

**virus scanners and rootkithunter**

`clamtk`

`rkhunter --check`

**Binary Analysis & Executable Tools**

`objdump -M -d`
disassembly executable in intel syntax


`gdb ./program`
start gdb on executable binary

`gdb() starti`
start the program

`gdb() stepi`
step through the program

`gdb() x`
examine a memory register in hex

`gdb() x/d`
examine a memory register in decimal

`gdb() run`
run the executable






