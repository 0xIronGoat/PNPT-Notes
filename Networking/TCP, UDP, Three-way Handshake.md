# TCP vs UDP
### TCP - Transimission Control Protocol
- Connection-oriented
- Reliable
- Used for things like file transfers, web browsing, emails etc


### UDP - User Datagram Protocol
- Connectionless
- Speed over reliability
- Used for things like streaming services, VoIP calls etc

### Three-way Handshake
**SYN -> SYN-ACK -> ACK**  

There are three steps to establish a connection between hosts:  
1. First host requests connection with **SYN**
2. Second host responds with **SYNACK**
3. First host responds to that with **ACK**

Could use a packet capture tool such as `Wireshark` to see this happen in real-time.