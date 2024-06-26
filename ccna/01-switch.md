## What is a switch?
A Network switch connects devices in a network to each other, enabling them to talk by exchanging data packets. Switches can be hardware devices that manage physical networks or software-based virtual devices.The switch use ethernet cables to connect two or more computers together, sending electrical signals though the ports.

### Why HUBS Suck
The hub is dumb, Lets say i have four devices on my hub network and I only want to talk to one device the hub is an idiot and will send that message to everyone on the hub network.

### Labbing switch traffic
Now the switch has the same goal as the hub, trying to connect the computers to connect and talk to each other. With a switch if I have four devices on a switch network and i wan to send a message to soneone unlike the hub the message is going to go to that one person vs sending it to everyone on the network. How can this be?

### How does a switch work?!?
The switch is really smart it can remember the users on each of its ports to direct traffic, the data is saved in a CAM-Table (content addressable memory). The switch remembers the layer 2(data link layer) address the MAC address. Why does the switch not know devices based of there IP addresses (internet protocol address / layer 3 )? The simple answer is that the switch cant even see the IP address , the switch is a layer 2 device. The switch only cares about layer 2.

### Your 1st Cisco cli command!!!
Switch#show mac-address-table 
```
                Mac Address Table
-----------------------------------------------------
vlan       Mac address           type         ports
----       -----------           -----        -----
  1     45:15:12:12:02:85       DYNAMIC       Fa0/3
  1     45:15:12:12:78:23       DYNAMIC       Fa0/1
```
The swicth learns where everything is that is connected to it, unlike the hub. All the messages that are going though a switch are called frames / layer2, but when the message going though and we talk about ip address / layer 3 we call them a packets. 

### Quiz time 
Which of the following addresses will a switch use to populate the CAM table?
answer : Source MAC addresses