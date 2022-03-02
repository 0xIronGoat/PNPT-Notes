# Common Network Commands
`ifconfig` (or `ipconfig` in Windows) - show your local network/IP info, network interface card info etc  
`iwconfig` - show wireless network interface details  
`ping` - ping an address or domain name for a response, local or remote. Will run endlessly until cancelled or given a count parameter in Linux, or only 4 pings in Windows. Uses ICMP.  
`arp` - Address Resolution Protocol, check local ARP table for network, resolve IP addresses to MAC addresses (e.g. `arp -a`)  
`netstat` - show active network connections on your machine (e.g. `netstat -ano`)   
`route` - show your routing table (exit route, gateway, netmask etc). Could be useful to see if a device has 2 x NICs for example and it is talking to an entire other network you were unaware of  

`ip` - new and improved network info command to replace `ifconfig`, `arp` or `route`  
	`ip -a` - similar to `ifconfig`  
	`ip -n` - similar to `arp`  
	`ip -r` - similar to `route`  