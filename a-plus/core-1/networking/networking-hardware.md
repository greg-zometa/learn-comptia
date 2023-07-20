# Networking Hardware

Identify and explain the purpose of networking devices and what they are doing with networks.

## Network Interface Card

Network adapters or network interface controllers (NICS) as they're called starts locally, to generate and put out on the electrical medium to connect to other devices within the networks. This is the first point of communication a computer generates via the operating system and is called the **networking stack**; to generate data to send out over the network. 

## Hubs

Hubs provided plug and play capabilities and was an easy way to add multiple devices to your networks. They're more of a legacy device.

Plugging into a hub from the network adapter, when the communication comes out of the network adapter and went into the hub, repeats signals across all the other ports. The more devices you connected into one of the hubs, the more congestion you would get within this type of networking device because every time a signal goes in, broadcast out all other ports, another signal goes into another port, broadcast out all of other ports. 

### Switches

[Switches make decisions on where to send the traffic](https://www.techtarget.com/searchnetworking/answer/What-is-the-difference-between-a-managed-and-unmanaged-switch). MAC addresses, an example, can address protocols and the connectivity device can start to make decisions on where to send the traffic.

### Unmanaged switches

Unmanaged switches use auto negotiated ports to determine parameters, such as data rates. Unmanaged switches do maintain a media access control (MAC) address table, however. This table tracks dynamically learned MAC addresses and the corresponding switch port on which the [MAC address was learned](https://www.techtarget.com/searchnetworking/answer/What-is-the-difference-between-an-IP-address-and-a-physical-address). The inclusion of a MAC address table means unmanaged network switches offer a separate, per-port [collision](https://www.techtarget.com/searchnetworking/definition/collision) domain.

### Managed switches

A managed switch allows us to go in and configure if we choose to each and every individual ports to do something a little bit different as we want to. Most of the switches today even allow us to logically divide that switch up into smaller switches that we also call villains. That's gonna be very important for businesses that can afford to buy one switch but really need, let's say three physical switches. So that's not the only thing that they can do and there's plenty of different functions with them today and they can even take on of course, even routing capabilities today as well.

## Power over ethernet

Power over ethernet is a technology that can actually inject power into the ethernet cable and this is very good for devices that do not have access to an AC outlet to power them via an AC adapter. It brings power to things like IP cameras, voice over IP phones.

## Power over ethernet standards

- POE (Type One): 15.4 watts of power
- POE+ (Type Two): 30 watts of power
- POE++ (Type Three): 60 watt capability
- POE++ (Type Four): 100 watt capability

## Access points

Wireless access points or access points gives wireless devices access to your wired network.

## Routers

Local area network communications are handled by switches, but one of the things that switch is limited to is it's only aware of the devices that are directly connected to the ports that we essentially see across the switch interface. **Routers** get communications to other remote networks.

Routers work on things like IP addresses and allow us to communicate across networks that we are no longer or we're not directly connected to. The switch would connect into the router and the router connects to your ISP. It allows you to send communications off of your local area network.

## Firewalls

Firewalls, whether physical network or a hardware based, screens all of the traffic coming in and out of your network and comparing it against a set of rules, and it either allows or denies the traffic. It would sit outside of your router in between your ISP's connectivity device, and it's a way that we try to increase the security of our networks.

## Edge network

The edge network is a point between our internal networks and the networks that are typically like ISPS, the router sits right there allowing, acting like a gateway to remote networks.

## Modem

A [modem](https://www.verizon.com/about/blog/modem-vs-router), which stands for "modulator-demodulator," is a device connecting your home to your [internet service provider (ISP)](https://www.verizon.com/about/blog/isp-meaning) through a physical connection. The modem translates the data from your ISP into a format that your home network devices can use.

There are three common types of modem connections:

- **Dial-up** — A modem that uses a phone line to connect to an ISP. This is the oldest type of modem connection and has largely been replaced by broadband connections.
- **DSL** — A digital subscriber line modem uses a phone line to connect to an ISP but with much higher speeds than dial-up.
- **Cable** — A modem that uses a cable TV line to connect to an ISP. This is the most common type of modem connection. 

### Optical Network Terminal

An ONT is a fiber optic connection, a residential fiber optic connection to a fiber optic network provider. This is what's connects the network adapter all the way out to the ISPS device that allows communication to our networks.

### Patch Panel

A patch panel really is nothing more than a series of ports. It's purpose is to bring different wires that may be spread across an entire building and have one location to plug our networking equipment into. 

## SDN 

SDN or software defined networking are physical devices that require configuration on an individual device level. It uses software to programmatically control all of the network devices, and control them in a way to build the network again using code in order to configure it. 