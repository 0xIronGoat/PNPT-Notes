# Subnetting

An IP address is made up of two parts - a **Network ID** and a **Host ID**  
To identify these, we need to use a mask.  

**Example:**  
IP address - `192.168.30.41`
Subnet mask - `255.255.255.0`

Break it down a bit further by converting to binary  

IP Address:
```
| 192      . 168      . 30       . 41        |
| 11111111 . 10101000 . 00011110 . 00101001  |
```

Subnet mask:
```
| 255      . 255      . 255      . 0        |
| 11111111 . 11111111 . 11111111 . 00000000 |
```


A `1` in this subnet mask means that the corresponding bit in the IP address is part of the network ID. Therefore our network ID is `192.168.30.0`. The rest of the address is then available to assign to individual hosts on that network.

For example, `192.168.30.29`, `192.168.30.127`, `192.168.30.250` are all hosts on that network, however `192.168.31.29` is on a different subnet, and you would need routing rather than just switching to communicate with it.

**Note:** The bits set to `1` in the subnet mask *must be contiguous* - that is to say they must be continuous and uninterrupted. As soon as a `0` is encountered, that marks the end of the mask.

#### Broadcast Address
It's important to note that the highest available IP address in a subnet is designated as the **broadcast address** - i.e. it is reserved and used to send traffic to the entire network. In the above example, with a subnet mask of `255.255.255.0` and a network address of `192.168.30.0`, the broadcast address is `192.168.30.255` - i.e. the highest available IP address on that subnet before you cross over in to another subnet.

### Subnet Mask vs CIDR Notation
A subnet mask will normally be presented as a decimal format IP address, e.g. `255.255.240.0`. However, this can also be represented in something called CIDR notation, which in this case would be `/20`. This notation indicates how many bits are switched on (i.e. set to `1`). This can be easier to see if we convert the decimal subnet mask in to binary:  

```
| 255      . 255      . 240      . 0        |
| 11111111 . 11111111 . 11110000 . 00000000 |
```

You can see above that there are 20 bits set to `1`, meaning the CIDR notation of this mask is `/20`


```
| Subnet Mask     | CIDR        |
| --------------- | ----------- |
| 255.0.0.0       | /8          |
| 255.255.0.0     | /16         |
| 255.255.255.0   | /24         |
```


A great resource on subnetting is Sunny Classroom on YouTube, please see his channel and his specific subnetting playlist below:  
[Sunny Classroom - YouTube](https://www.youtube.com/channel/UCr0Ze4SR3MHXAgz1TvRYL7Q)
[Subnetting Playlist](https://www.youtube.com/playlist?list=PLSNNzog5eydueOR_p6dezKr2tosjGvdNH)


### Subnetting Table

The below table can help you work out number of hosts on a subnet