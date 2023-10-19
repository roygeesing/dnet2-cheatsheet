# Useful commands
```
no ip domain-lookup
show ip int br
show vlan
```

# VLANs
## Auf Switch
```
vlan <n>
name <name>
exit
interface range <range>
switchport mode access
switchport access vlan <n>
exit

interface <upstream>
switchport mode trunk
switchport trunk encapsulation dot1q
no shutdown
end
```

## Auf Router
```
interface <interface>
encapsulation dto1q <n>
exit
```

# ACLs
```
access-list <n> {deny|permit|remark} <sourceAddr> <sourceWC>
interface <interface>
ip access-group <n> {in|out}
exit

ip access-list {standard|extended} <name>
{deny|permit} ...
exit
interface <interface>
ip access-group <name> {in|out}
exit

ipv6 access-list <name>
{deny|permit} ...
exit
interface <interface>
ipv6 traffic-filter <name> {in|out}
eixt
```
