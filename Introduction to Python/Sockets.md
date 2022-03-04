# Sockets
##### This small script will connect one node to another
In this case, we are trying to connect to ourselves (localhost, 127.0.0.1) on port 7777:
```
#!/bin/python

import socket

HOST = '127.0.0.1'
PORT = 7777

s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
s.connect((HOST,PORT))
```

Think of the socket parameters as follows:
`AF_INET` = IPv4 connection
`SOCK_STREAM` = port

In a separate terminal window, run netcat listening on port 7777:
`nc -lvnp 7777`

Then run the python script from above and you should see a connection come through in netcat:
![[python-sockets.png.png]]