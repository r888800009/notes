# Iptables

``` bash
echo 1 > /proc/sys/net/ipv4/ip_forward
iptables -t nat -A POSTROUTING -j MASQUERADE
iptables -t nat -A PREROUTING -p tcp --dport [port] -j DNAT --to-destination [LAN ip]:[port]
```
