## What is a router?

A router is a device that connects two or more packet-switched networks or subnetworks. It serves two primary functions: managing traffic between these networks by following data packets to their intended IP addresses, and allowing multiple devices to use the same internet connection.

### Do we actually need routers?
what happens if we just connect are switches directly to each other. NO it wont work and here is why , we could connect the switches together and make a griant switch. But one switch is on one network and the other switch is on a different network. This is no becuase they are two different switchs its because of there IP addresses. When we talk about a network we're talking about a group of IP addresses. 

### What is the ARP?
The Address Resolution Protocol is a layer 2 protocal used to map MAC addresses to IP addresses. All hosts on a network are located by their IP address, but NIC's(Network Interface Card) do not have IP addresses, they have MAC addresses. ARP is the protocol used to associte the IP address to a MAC address.

Lets say i dont know the person im trying to message MAC address, when I try to ping the computers ip address 10.1.1.2 that i dont know the MAC to the layer2 does this ARP broad-cast that would look like this 25:85:26:95:35:75 >> FF:FF:FF:FF:FF:FF ( the 'F' is the broad-cast) basically saying who belongs to 10.1.1.2. Sending this though all the ports to see who matchs the ip address and when it finds it, it also gets the MAC address. 

### Life with out a router
Gateway in the networking world is also called the router. If I want to message someone I need them to be in my Network. In the range of for example (this is only if i connect two switches together in different networks together) 10.1.1.1 - 10.1.1.255 is are network range if the ip address is not in are network it wont try to find it. 

### Routers save the day
If we had a router we could access stuff out of are network,  trying to reach something out of are network the gateway/router would say im the gateway looking for whatever your destination the ip address your looking for. The router only cares about layer 3(packet) so it sends an ARP message to find the MAC of the destination of the ip address to tell the switch where to go.

So now we know where to send are message it starts off this my MAC >> router MAC then from the router MAC >> destination MAC
### Sneak peak ... DNS
Switches muct know the MAC address (layer2), Routers must know the IP address (layer3), But who deals with youtube.com or google.com, this is called DNS (domain name service). The name like google.com is tied to and ip address like 8.8.8.8 so when we type the in on the network the computer makes a request of information, and the DNS server send the IP and MAC back. cd ..

###
###