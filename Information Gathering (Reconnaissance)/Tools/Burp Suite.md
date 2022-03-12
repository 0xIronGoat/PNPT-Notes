# Burp Suite
Web proxy tool - has the capability to intercept web traffic

### Setup
These setup instructions assume you are using Firefox

1. 
You need to direct your web browser traffic to the Burp proxy on **127.0.0.1:8080**. You can either do this manually in the preferences or, if you are using FireFox, using an extension called Foxy Proxy  

2. 
Navigate to https://burp  
It may ask you to store a certificate, if it does then click allow.  
In top right, click on "CA Certificate" and download the Burp certificate file.  
Back in the preferences menu click on "Privacy & Security" scroll to the bottom and click "View Certificates..."  
Click "Import" and select the downloaded "cacert.der" file  

**Alternatively**, you could also use the integrated web browser built in to Burp without needing to alter any of your browser settings!
