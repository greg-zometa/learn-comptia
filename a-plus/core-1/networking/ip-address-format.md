# IP Address Format

‘IP’ stands for [Internet Protocol](https://www.cloudflare.com/learning/network-layer/internet-protocol/), which is the set of rules that makes it possible for devices to communicate over the [Internet](https://www.cloudflare.com/learning/network-layer/how-does-the-internet-work/). With billions of people accessing the Internet every day, unique identifiers are necessary to keep track of who is doing what. The Internet Protocol solves this by assigning IP numbers to every device accessing the Internet.

A computer’s [IP address](https://www.cloudflare.com/learning/dns/glossary/what-is-my-ip-address/) is like the physical address of a house. If someone calls a pizzeria to order a delivery, they need to provide their physical address. Without that address, the pizza delivery person will have no idea which house to deliver the pizza to.

### Binary decimal conversion

[Converting from binary to decimal](https://www.techtarget.com/searchnetworking/tip/Binary-to-decimal-conversion) isn't difficult. The numbers 0 and 1 in binary convert to 0 and 1 in decimal. After that, it gets a little more complicated.

To convert binary into decimal:
- always start on the right-hand side of the binary number
- understand that each decimal digit in the binary conversion chart doubles in size as it goes left

To convert decimal into binary:
- always start on the left-hand side of the decimal space
- subtract the number by the decimal space as it goes right
	- if the number subtracted is less than zero set the binary to 0 
	- if the number subtracted is greater than or equal to zero set the binary to 1
	- continue doing this until the number subtracted reaches zero

<table style="width: 100%;"> 
  <tbody> 
   <tr> 
    <td width="97"> <p>Power of two</p> </td> 
    <td width="34"> <p>2<sup>7</sup></p> </td> 
    <td width="27"> <p>2<sup>6</sup></p> </td> 
    <td width="27"> <p>2<sup>5</sup></p> </td> 
    <td width="27"> <p>2<sup>4</sup></p> </td> 
    <td width="24"> <p>2<sup>3</sup></p> </td> 
    <td width="24"> <p>2<sup>2</sup></p> </td> 
    <td width="24"> <p>2<sup>1</sup></p> </td> 
    <td width="24"> <p>2<sup>0</sup></p> </td> 
   </tr> 
   <tr> 
    <td width="97"> <p>Decimal space</p> </td> 
    <td width="34"> <p>128</p> </td> 
    <td width="27"> <p>64</p> </td> 
    <td width="27"> <p>32</p> </td> 
    <td width="27"> <p>16</p> </td> 
    <td width="24"> <p>8</p> </td> 
    <td width="24"> <p>4</p> </td> 
    <td width="24"> <p>2</p> </td> 
    <td width="24"> <p>1</p> </td> 
   </tr> 
   <tr> 
    <td width="97"> <p>Binary bits</p> </td> 
    <td width="34"></td> 
    <td width="27"></td> 
    <td width="27"></td> 
    <td width="27"></td> 
    <td width="24"></td> 
    <td width="24"></td> 
    <td width="24"></td> 
    <td width="24"></td> 
   </tr> 
  </tbody> 
 </table>

## Subnet mask

[A subnet (also known as a subnetwork) is a small network within a large one](https://nordvpn.com/blog/what-is-a-subnet-mask/). Large networks are generally difficult to maintain. Furthermore, traffic must travel a longer distance and pass through unnecessary routers to reach its destination. Subnetting –– or dividing the network into smaller pieces –– is used to make the network easier to maintain. While it has many benefits, subnetting requires additional hardware (e.g., routers), potentially costing extra to implement.

Here are the ways in which subnetting can improve your networking experience:

- Easier maintenance
- Advanced [network security](https://nordvpn.com/cybersecurity/network-security/) so that one subnet can’t access the other one
- Reduced network traffic
- When you can subnet your network, you don’t need to acquire additional IP addresses from ISPs (internet service providers)

## IP address classes

With an IPv4 IP address, [there are five classes of available IP ranges](https://www.computerhope.com/jargon/i/ip.htm#classes): Class A, Class B, Class C, Class D and Class E, while only A, B, and C are commonly used. Each class allows for a range of valid IP addresses, shown in the following table (does not include [private range](https://www.ibm.com/docs/en/networkmanager/4.2.0?topic=translation-private-address-ranges)s).

|Class|Address range|Supports|
|--- |--- |--- |
|Class A|1.0.0.1 to 126.255.255.254|Supports 16 million hosts on each of 127 networks.|
|Class B|128.1.0.1 to 191.255.255.254|Supports 65,000 hosts on each of 16,000 networks.|
|Class C|192.0.1.1 to 223.255.254.254|Supports 254 hosts on each of 2 million networks.|
|Class D|224.0.0.0 to 239.255.255.255|Reserved for multicast groups.|
|Class E|240.0.0.0 to 254.255.255.254|Reserved for future use, or research and development purposes.|


## APIPA addresses

[Automatic Private IP Addressing](https://www.techtarget.com/whatis/definition/Automatic-Private-IP-Addressing-APIPA) (APIPA) is a feature of [Windows](https://www.techtarget.com/searchwindowsserver/definition/Windows)-based [OSes](https://www.techtarget.com/whatis/definition/operating-system-OS) -- included since Windows 98 and Windows ME -- that enables a [Dynamic Host Configuration Protocol](https://www.techtarget.com/searchnetworking/definition/DHCP) client to automatically assign an [IP address](https://www.techtarget.com/whatis/definition/IP-address-Internet-Protocol-Address) to itself when there's no DHCP server available to perform that function. APIPA serves as a DHCP server failover mechanism and makes it easier to configure and support small [LANs](https://www.techtarget.com/searchnetworking/definition/local-area-network-LAN).

## IPv6

[IPv6 is the next generation Internet Protocol](https://www.techtarget.com/iotagenda/definition/IPv6-address) (IP) standard intended to eventually replace IPv4, the protocol many Internet services still use today. Every computer, mobile phone, and any other device connected to the Internet needs a numerical IP address in order to communicate with other devices.

### Format of an IPv6 address

In precise terms, an IPv6 address is 128 bits long and is arranged in eight groups, each of which is 16 bits. Each group is expressed as four [hexadecimal](https://www.techtarget.com/whatis/definition/hexadecimal) digits and the groups are separated by colons.

An example of a full IPv6 address could be:

**FE80:CD00:0000:0CDE:1257:0000:211E:729C**

### Types of IPv6 addresses

There are different types and formats of IPv6 addresses, of which, it's notable to mention that there are no broadcast addresses in IPv6. Some examples of IPv6 formats include:

- **Global unicast**. These addresses are routable on the internet and start with "2001:" as the prefix group. Global unicast addresses are the equivalent of IPv4 public addresses.
- **Unicast address**. Used to identify the interface of an individual node.
- **Anycast address.** Used to identify a group of interfaces on different nodes.
- **Multicast address.** An address used to define [multicast](https://www.techtarget.com/searchnetworking/definition/multicast) Multicasts are used to send a single packet to multiple destinations at one time.
- **Link local addresses.** One of the two internal address types that are not routed on the internet. Link local addresses are used inside an internal network, are self-assigned and start with "fe80:" as the prefix group.
- **Unique local addresses.** This is the other type of internal address that is not routed on the internet. Unique local addresses are equivalent to the IPv4 addresses 10.0.0.0/8, 172.16.0.0/12 and 192.168.0.0/16.