---
id: yxthiukg77rlnoqljpkzna5
title: IPv6
desc: ''
updated: 1667985436098
created: 1667510756183
---
# IPv6

IPv6 attacks the address exhaustion issues with IPv4 head-on.

IPv6 uses 128 bits (represented in hexadecimal)

## IPv6 header   
| Field| Field | Field | Field|
|------|-------|-------|-------|
| Version| Class | Flow Label | Flow Label|
| Payload Length |  Payload Length | Next Header | Hop Limit| 
| Source Address | Source Address |Source Address |Source Address |
| Destination Address | Destination Address | Destination Address | Destination Address |

<br>

IPv6 address format is 8 sets of 4 hex digits 
<br>
e.g. 2001:1111:A231:0001:2341:9AB3:1001:19C3

<br>

## Rules for shortening IPv6 addresses

Two rules for shortening IPv6 addresses 

* once in the address, you can represent
>  💡 consecutive sections of 0000's with a :: 
* as many times as you can in the address
>  💡 you can eliminate leading 0's 

<br>
🛑
e.g. 2001:0000:0011:0001:0000:0000:0001:1AB1/64

<br>
e.g. 2001:0:11:1::1:1AB1/64
first 64 bits above represent the network

Global unicast address is like the public IPv4 address.

<br>
The management of IPv6 address space is done by IANA (Internet Assigned Numbers Authority). IANA assigns blocks of address ranges to regional registries, who then affiliate address range/space to network service providers. Your organisation requests address space from a service provider.

<br>
To simplify subnetting in IPv6, companies often use a /64 mask.

## Configure, verify and troubleshoot IPv6
Dual stack is the term used for running IPv4 and IPv6 on the same network interface.

<br>

> **ipv6 address 2001:aaaa:bbbb::1/64**

<br>
Modified EUI-64 is the method which uses the interface hardware address as part of IPv6 layer 3 host address.

> **show ipv6 interface brief**
<br>
shows the status of the IPv6 interface

<br>
A global configuration command you will often use is 

> **ipv6 unicast-routing**
<br>
This permits your router to run IPv6-related routing protocols such as EIGRP for IPv6 or OSPF version 3.

## IPv6 address Verifications

> R1# **show ipv6 interface brief**

> R1# **show ipv6 interface fa 0/0**

<br>
Many engineers will not want the extra work to manually assigning host addresses to their systems, however, IPv6 offers a feature called modified EUI-64. This process takes the MAC address from the device and uses it to automatically generate a host portion.

<br>

> R1(config)# **interface fastEthernet 0/0**

> R1(config)# **ipv6 address 2001:AAAA:BBBB::/64 eui-64**

> R1(config)# **no shutdown**

## Configure and verify IPv6 Stateless Address Auto Config (SLAAC

<br>

<font color="red">**Stateful address assignment**</font> refers to a device "tracking" the automatic assignment of addressing information (e.g. DHCP for IPv4).


<font color="red">**Stateless address assignment**</font> refers to a lack of tracking information.

The <font color="red">ipv6 address autoconfig</font> command on Cisco routers is used to assign an IPv6 address using SLAAC.

<br>
SLAAC - having one network device assist another in the assignment of the entire address.


<br>
DHCP server used in a stateful manner.
DHCP server tracks the info in a database.


<br>
In IPv6 you can use SLAAC and stateless DHCP to provide a host with all of the information it might need (includes IPv6 address, prefix length, the default gateway and DNS server).


<br>
With SLAAC, the IPv6 address for the device is learnt by having the prefix information automatically sent over the local link from another device (such as the router), then the device can randomly assign its own host portion of the address, or use the modified EUI method.


<br>
Because SLAAC cannot provide additional information such as DNS server address, we often combine SLAAC with the use of stateless DHCP for IPv6.


<br>
How does the SLAAC host communicate with its neighbour if it does not yet possess the IPv6 address information it needs? This is the job of the 

**link-local addresss**. 

> R1(config)# **interface fa 0/0**

> R1(config-if)# **ipv6 address autoconfig**

## Compare and contrast IPv6 address types
1. What type of IPv6 address is similar to an RFC1918 in IPv6? 
<br>
<font color="red">A unique local address</font>
2. What type of IPv6 address allows a variety of IPv6 services to function between 2 devices on the same network? 
<br>
<font color="red">A link local address</font>
3. What type of IPv6 address has you configure identical addresses on different devices? 
<br>
<font color="red">An anycast address</font>


## IPv6 Address Types
| Type| Defition |
|------|-------|
| Global Unicast| Unique IPv6 (used on the public Internet) |
| Unique Local| similar to RFC1918 (in IPv4) |
| | private use only |
| | these addresses begin with FD |
| | e.g. FDE4:8DBA:82E1::/64 |
|Link Local | only function on the local link |
| | IPv6 devices automatically generate them to perform automated functions |
| | prefix used FE80::/10 |
| Multicast | a packet is sent to a group of devices interested in receiving the packet information |
| | in IPv6 multicast replaces completely the IPv5 broadcasting |
| | if your device wants to reach all devices, it sends traffic to the IPv6 multicast address of FF02::1 (all nodes IPv6 multicast) |
| Modified EUI64 | device uses it to assign itself its host portion of the address |
| IPv6 autoconfiguration | IPv6 address through SLAAC |
| IPv6 anycast | allows you to configure identical IPv6 addresses on your devices. When clients attempt to reach this address, IPv6 routers can send the traffic to the nearest anycast device (keyword anycast) |
| ipv6 enable | not required to enable IPv6 on an interface |
| | used to configure a link local address |
| | used to prepare the interface for processing IPv6 information |
| | the ipv6 enable command ensures a link local address exists |













