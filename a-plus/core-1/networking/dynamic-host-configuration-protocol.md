# Dynamic Host Configuration Protocol

[DHCP (Dynamic Host Configuration Protocol)](https://www.techtarget.com/searchnetworking/definition/DHCP) is a network management protocol used to dynamically assign an IP address to any device, or [node](https://www.techtarget.com/searchnetworking/definition/node), on a network so it can communicate using IP. DHCP automates and centrally manages these configurations rather than requiring network administrators to manually assign IP addresses to all network devices.

## Static vs. dynamic DHCP leases

With dynamic DHCP, a client does not own the IP address assigned to it, but instead _leases_ it for a period of time. Each time a device with a dynamic IP address is powered up, it must communicate with the DHCP server to lease another IP address.

Static DHCP assignment means the DHCP server assigns the same IP to the defined MAC address every time the device is connected to the network. The DHCP server serves the reserved IP address when the device using the corresponding MAC address requests an IP address.

## DHCP lease process

Under a dynamic DHCP setup, a client might also have to perform certain activities that lead to terminating its IP address and then reconnecting to the network using a different IP address. DHCP lease times can vary depending on how long a user is likely to need an internet connection at a particular location. Devices release their IP addresses when their DHCP leases expire and then request a renewal from the DHCP server if they are staying online. The DHCP server may assign a new address rather than renewing an old one.

The typical dynamic DHCP lease cycle is as follows:

1. A client acquires an IP address lease through the allocation process of requesting one from the DHCP server.
2. If a client already has an IP address from an existing lease, it needs to refresh its IP address when it reboots after being shut down and contact the DHCP server to have an IP address reallocated.
3. Once a lease is active, the client is bound to the lease and to the address.
4. Once the lease has expired, a client contacts the server that initially granted the lease to renew it so it can keep using its IP address.
5. If a client is moving to a different network, its dynamic IP address is terminated, and it requests a new IP address from the DHCP server of the new network.

### DORA

DORA helps in providing an IP address to hosts or client machines.[ DORA is the process that follows some steps](https://www.geeksforgeeks.org/how-dora-works/) between the server and client. It gets the IP address from the centralized server. It consists of four-stage:

- **Discover**: client sends a discover message to server
- **Offer**: server responds with an available IP address and options
- **Request**: client requests the IP address from server
- **Acknowledge**: server acknowledges client request and completes

## DHCP Scope

A DHCP scope is a valid range of IP addresses that are available for assignment or
lease to client computers on a particular subnet. In a DHCP server, a scope is
configured to determine the address pool of IPs that the server can provide to
DHCP clients.

Scopes determine which IP addresses are provided to the clients. They should be
defined and activated before DHCP clients use the DHCP server for
its dynamic IP configuration. Users can configure as many scopes on a DHCP server
as required in the network environment.
