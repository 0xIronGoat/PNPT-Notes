# Subnetting




### Subnet Mask vs CIDR Notation
A subnet mask will normally be presented as a decimal format IP address, e.g. `255.255.255.0`. However, this can also be represented in something called CIDR notation, which in this case would be `/24`. This notation indicates how many bits are switched on (i.e. set to `1`). This can be easier to see if we convert the decimal subnet mask in to binary:  

```
| 255      . 255      . 255      . 0        |
| 11111111 . 11111111 . 11111111 . 00000000 |
```

You can see above that there are 24 bits set to `1`.

**Note:** The bits set to `1` in the subnet mask *must be contiguous* - that is to say they must be continuous and uninterrupted. As soon as a `0` is encountered, that marks the end of the mask.


```
| Subnet Mask     | CIDR        |
| --------------- | ----------- |
| 255.0.0.0       | /8          |
| 255.255.0.0     | /16         |
| 255.255.255.0   | /24         |
```

[Sunny Subnetting - YouTube](https://www.youtube.com/watch?v=ecCuyq-Wprc)
