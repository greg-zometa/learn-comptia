# Ports and protocols

Identify the most common ports and protocols for network communications.

## Protocol

[Protocols are a specific type of communication between to end points](https://www.cloudflare.com/learning/network-layer/what-is-a-computer-port/). A structured set of rules for the type of communication in order to provide and get access to a service.

### Connection oriented

**[Transmission Control Protocol (TCP)](https://www.cloudflare.com/learning/ddos/glossary/tcp-ip/)**. Provide reliable delivery and error checking. When packets are not sent in the correct order, the protocol will make another request to resend the information. Considered "reliable delivery", transmissions get marked that the packets are being received in a orderly fashion. 

### Connectionless oriented

**[User Datagram Protocol (UDP)](https://www.cloudflare.com/learning/ddos/glossary/user-datagram-protocol-udp/)**. Provide faster delivery without error checking.  Considered "best effort delivery".

### Email protocols

Be aware of the type of protocols and port numbers.

Forwarding?
- [SMTP](https://www.cloudflare.com/learning/email-security/what-is-smtp/): Simple Mail Transfer Protocol
	- receives email at port `25`
- POP: Post Office Protocol
	- version 3 for receiving email at port number `110`
	- when we download email it is wiped from server
- [IMAP](https://www.cloudflare.com/learning/email-security/what-is-imap/): Internet Message Access Protocol
	- ability to look and view email like they were in locally, but can be accessed in the server
	- port `143`

### File protocols

File transfer protocol (FTP) has been around for a very long time. Port `20` is the control and command port for it; data comes in at port `21`. Trivial file transfer protocol (TFTP), uses UDP to transfer small files in a relative quick time at port `69`.

### Remote Connection Protocols

A way to connect to mainframes from a terminal or emulation software. [Telnet](https://www.extrahop.com/resources/protocols/telnet/), as an example, uses port `23` to connect for tele networking and has security vulnerabilities because there is no security built around it.

[SSH or Secure Shell](https://www.cloudflare.com/learning/access-management/what-is-ssh/) is a protocol for remote encrypted connections between computers that uses port `22`. Popular with macOS/Linux. [Windows has remote desktop protocol](https://www.cloudflare.com/learning/access-management/what-is-the-remote-desktop-protocol/) at port `3389`.

### Web protocols

Using port `80`, [a common port for web servers](https://www.ibm.com/docs/en/i/7.2?topic=tasks-managing-addresses-ports#taskd102022e43), is considered a security vulnerability because it is so commonly used. Unlike port `80`, that is the default port for [http,](https://www.cloudflare.com/learning/ddos/glossary/hypertext-transfer-protocol-http/) port `443` or [https provides security](https://www.cloudflare.com/learning/ssl/what-is-https/) with a [transport layer security](https://www.cloudflare.com/learning/ssl/transport-layer-security-tls/). 

## Port

An identifier for a logical end point of a connection i.e. severs listen to protocols for a connection from a certain port. [Internet Assigned Numbers Authority](https://www.iana.org/) are the association body that have set up the network protocols in the early history.

### Well known ports

Common services and protocols that most computing systems recognize. The range is typically from 0-1023.

The number of protocols available are 65,535 (including 0).

### Registered port ranges

Organizations set aside and register a port range intended for a specific piece of software.

Ex.) Microsoft has something called RDP that is set to port `3389`.

These port ranges start at 1024 and go all the way up to 49,151.

### Dynamic ports

A computer requests a service with a dynamic, temporary port that are between 49,152 and 65,535. Once a communication is established on request, the response will generate another dynamic port.

### Network Services

### Domain Controller

A[ domain controller](https://www.techtarget.com/searchwindowsserver/definition/domain-controller) is a directory services server within an active directory domain. It's not the only directory services out there, but it's one of the most popular in the world in the enterprise level market and it's using something known as LDAP.

### LDAP

[LDAP is the lightweight directory access protocol](https://www.okta.com/identity-101/what-is-ldap/), now it uses other protocols but it also uses LDAP. The lightweight directory access protocol, when connecting to a directory services database and communicating with it, send queries against it to retrieve information. It is at port `389`. 

Do not confuse LDAP and RDP because LDAP lightweight directory access protocol is port `389`, RDP is port `3389`.

### DNS

One of the networking services that we use so much today is what's known as [domain name system (DNS)](https://www.cloudflare.com/learning/dns/what-is-dns/). The DNS protocol, communicates over port 53.

### DHCP

Dynamic Host Configuration Protocol (DHCP) dynamically assigns IP addresses that over port `68` and port `67`. 

### NetBIOS

NetBIOS goes over ports `3`, `137`, and `139`. This is an earlier non-scalable, non reputable legacy type naming resolution service in a Windows environment.

### SNMP
SNMP is a protocol that tracks the health of connectivity devices, variety of networking devices on your network that they can send information back over the network to a management station. There are two ports: port `161` and port `162`.