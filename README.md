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
