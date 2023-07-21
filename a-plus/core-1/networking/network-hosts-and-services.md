# Network Hosts and Services

## Directory services server

In computing, a **directory service or name service** maps the names of network resources to their respective network addresses. One of the most popular ones in an enterprise level environment is what is known as [Active Directory Directory Services](https://learn.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview). 

Active Directory Directory Services is a LDAP compliant directory service that allows us to create and store users. We can store computers, we can store all kinds of various objects and scalable to a very large enterprise networks.

## Mail server 

- **SMTP server**: used for outbound communication. 
- **POP3 server**: used for retrieving email, inbound email.
- **IMAP server**: one of the more common servers used.
 
## DNS server

The domain name system server holds records for the computers that are within your network. It provides us name resolution, taking those user friendly, fully qualified domain names and allowing us to map them to IP addresses. A very important service. 

## DHCP server

The dynamic host configuration protocol server or DHCP server allows us to dynamically push out configuration settings. It allows us to distribute, IP addresses to various clients within our network easing the burden of manually assigning IP addresses across large enterprises. Even small enterprises and makes it our lives as administrators a little bit easier when it comes to IP addressing.

## File server

A[ file server](https://www.techtarget.com/searchnetworking/definition/file-server) is a computer responsible for the storage and management of data files so that other computers on the same network can access the files. It enables users to share information over a network without having to physically transfer files. File servers are a common target for [hackers](https://www.techtarget.com/searchsecurity/definition/hacker) and [ransomware](https://www.techtarget.com/searchsecurity/definition/ransomware), so particular attention must be given to securing them against attacks.

## Print servers

A print server is a dedicated appliance or central point of software. They help clients/users/devices connect to shared printers and they process or pass through spool files from a client to the printer. 

A print server may be a networked computer with one or more shared printers. Alternatively, a print server may be a dedicated device on the network, with connections to the LAN and one or more printers. Dedicated server appliances tend to be fairly simple in both configuration and features. Print server functionality may be integrated with other devices such as a wireless router, a firewall, or both. A printer may have a built-in print server.  

## Syslog server

Syslog servers are typically something that we have inside of Nix based systems (UNIX and Linux). A [daemon](https://itsfoss.com/linux-daemons/) is a service process that runs in the background and supervises the system or provides functionality to other processes. A commonly found daemon in a Nix based system generates the system logs and stores them locally. We can set up a Syslog server and all your Nix based systems can report over to that Syslog server. 

## Web server

A [web server](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Web_mechanics/What_is_a_web_server) is a computer that stores web server software and a website's component files (for example, HTML documents, images, CSS stylesheets, and JavaScript files). A web server connects to the Internet and supports physical data interchange with other devices connected to the web.

## Internet Appliances

Internet appliances, generally in IT, is very expensive security based devices. It is a type of computing appliance that aids in the flow of information to other network-connected computing devices. Services that may be provided by a network appliance include firewall functions, caching, authentication, network address translation and IP address management. It takes multiple security functionalities and integrates it into a single component that you can manage in a centralized fashion. Thereby making it a lot easier for us to manage some of our security infrastructure.

Other ones that exist are load balancers;  a way to distribute resource requests from some of those servers in our networks. We can take a load balancer and when a client request we can spread that workload across multiple servers, and evenly distribute the workload. So that if one server is getting a little bit too overburdened, we can send those requests to multiple servers making the performance and the user experience a lot better on the back end.

Another one is a proxy server; a server that centrally manages what and who can gain access outbound to the internet. A proxy sits in between a client's browser and the web server and makes requests on behalf of the client.

## SCADA

SCADA is the acronym for Supervisory Control and Data Acquisition. SCADA is a computer-based system for gathering and analyzing real-time data to monitor and control equipment that deals with critical and time-sensitive materials or events. Think of industrial control systems, power plants, or any other large infrastructure that uses a variety of components in where remote telemetry units send wireless information and collect it in a centralized, isolated location.

## IOT

internet of things is a variety of devices that basically connect to the internet. A lot of times they are very low powered devices that form networks and communicate together.