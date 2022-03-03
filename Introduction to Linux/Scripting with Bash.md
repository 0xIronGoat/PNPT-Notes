# Scripting with Bash
### Commands
`grep` - search for a string in a file or some command output  
- e.g. `grep "string" filename.txt` or `cat filename.txt | grep "string"`  
`cut` - cut some text based on a delimeter  
- e.g. `cut -d " " -f 4`, give me the 4th field based on a space delimeter  
`tr` - translate  
- e.g. `tr -d ":"`, remove : from my output  

### Ping sweep script:
```
#!/bin/bash

# Loop through numbers 1 to 254
# For each number, ping IP starting with $1 parameter, ending with loop parameter
# e.g. ./pingsweep.sh 192.168.1 will loop through 192.168.1.1 to 192.168.1.254
# grep, cut and tr mean we will only print out successful pings
# & means threading is enables

if [ "$1" == "" ]; then
	echo "You need to provide the first 3 octets of an IP address"
	echo "Syntax: ./pingsweep.sh 192.168.1"
else
	for ip in `seq 1 254`; do
		ping -c 1 $1.$ip | grep "64 bytes" | cut -d " " -f 4 | tr -d ":" &
	done
fi
```

### nmap for loop one liner:
Ensure you have a file called `iplist.txt` containing a simple list of IP addresses (one per line), then run the below to use `nmap` to scan port 80 on each IP:  

`for ip in $(cat iplist.txt); do nmap -sS -p 80 -T4 $ip & done`