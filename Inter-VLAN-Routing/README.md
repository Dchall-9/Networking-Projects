OVERVIEW

This project consists of Inter-VLAN routing with an ACL to deny 1 specified pc from the guests VLAN (30) from interacting with the Management VLAN (20)

There are 6 PCs, 3 Switches and 1 Router

There are 3 VLANS, 10 is Personal, 20 is Management and 30 is Guests each VLAN has 2 PCs and 1 Switch

On each switch there is an access port for the PCs and 1 trunk link for switch and another for the router

IPs were configured on PCs and default gateway was created on the router's subinterfaces

On the router there is a extended ACL to deny host 192.168.30.3 on guest VLAN from interacting with the Management VLAN

VERIFICATION

To test Inter-VLAN connectivity I used ping in the command prompt of each PC

show interfaces trunk command was used to verify each switch and the router trunk port was configured correctly

show vlan brief command was used to verify each PC has the right VLAN assignment

show ip route command was used to verify the router could reach each network

Extended ACL was confirmed by using ping command on blocked PC

CONCEPTS

Inter-VLAN Routing

VLANs

Extended ACLS

Router-on-a-stick

Trunking

TROUBLESHOOTING

When there was a issue I would use show-running config and show interfaces trunk to troubleshoot and the ping command on PCs
