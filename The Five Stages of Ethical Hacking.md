# The Five Stages of Ethical Hacking

1. **Reconnaissance** - Passive vs Active. **Passive** - Things such as Google searches, looking at publically available info e.g. websites, employee social media accounts, photos etc.  
2. **Scanning & Enumeration** - Active recon. **Scanning** - Using tools such as Nmap, Nessus, Nikto etc to actively scan a target. **Enumeration** - Digging in to results from recon/scanning to see if there's anything valuable. E.g. a scan shows Apache v1.2 running on the target, is this something you can exploit?
3. **Gaining Acces** - Actively trying to run exploits against the target, vulnerable services etc based on your recon results to try and get access to a machine/network/environment. Once you have access, you will scan/enumerate again to find paths to pivot to other devices/envioronments or escalate your privileges.
4. **Maintaining Access** - Once you have access you will also look for ways to maintain your access in case you are to get kicked out or a target is restarted etc.
5. **Covering Tracks** - Delete any logs, malware, accounts etc you have left behind.