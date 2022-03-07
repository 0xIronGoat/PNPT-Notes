# Passive Recon
### Location Information
- Satellite images
- Drone recon
- Building layout (badge readers, break areas, security, fencing)

Get a feel for the building layout, look for entry/exit points, fire exits, physical security presence etc

e.g. Find good places to approach people, strike up conversations, glean info from them and maybe tailgate them in to the building.

### Job Information
- Employees (names, job titles, phone numbers, managers etc)
- Pictures (badge photos, desk photos, computer photos etc)

Use things like LinkedIn, Facebook, Twitter, make a fake badge for going on site, learn staff and manager names to be more convincing etc

e.g. someone once took a photo of themselves at work watching a basketball game, but in the background you could see many of the software tools the company used, a desk in the background that might have had sensetive information on it etc.

### Web/Host
- **Target Validation**
	- *WHOIS*, *nslookup*, *dnsrecon*
	- Client may give you an IP address or website, but could have made a mistake and given you the wrong info, you could end up attacking someone else's website.
- **Finding Subdomains**
	- *Google Fu*, *dig*, *Nmap*, *Sublist3r*, *Bluto*, *crt.sh*
- **Fingerprinting**
	- *Nmap*, *Wappalyzer*, *WhatWeb*, *BuiltWith*, *Netcat*
	- Find what is running on a website or host, what versions of services etc. Can be both active and passive depending on whether or not you are actually carrying out scans on the target.
- **Data Breaches**
	- *HaveIBeenPwned*, *Breach-Parse*, *WeLeakInfo* 
	- Most common way of getting in to networks. Breach incidents from the past that have leaked credentials, we can utilize usernames or re-used passwords to get access.