`ifconfig` or `ip a` in Linux to find your private IP address  
`ipconfig` for WIndows  

Layer 3 concept (OSI model)

### IPv4 - decimal notation  
32 bit addressing
With 32 bits, there are just over 4 billion possible IP addresses (2^32)  
Made up of 4 octets, each octet made up of 8 bits  
This is why max number of each octet is 255

### IPv6 - hexadecimal notation  
128 bit addressing
2^128 addresses, ridiculous number, don't even bother



### NAT - Network Address Translation  
Devices on your local network are assigned a *private* IP address - these are not routable over the internet. In order for these devices to access the internet NAT is required to pass traffic through your *public* IP address provided by your ISP.

Certain IP address ranges are reserved for private and public addresses (including some reserved for special services, providers etc).

More info can be found at the following links:  
https://en.wikipedia.org/wiki/Reserved_IP_addresses  
https://datatracker.ietf.org/doc/html/rfc1918