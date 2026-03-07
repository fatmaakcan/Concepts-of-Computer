# NETWORKING BASICS

# 1.Basic Concepts

## IP (Internet Protocol)
### A digital identity card for every device on a network. It provides devices to locate and communicate with each other.
### IPv4: 32-bit addresses such as 192.168.1.1.
### IPv6: 128-bit addresses;a wide range of addressing structure developed for increasing number of devices.

## Port
### Acting as the doors to the computer's outer world. It determines which application (web,e-post,game etc.) the incoming data should be directed to.
### Example: Port 80 for HTTP, Port 443 for HTTPS.

## DNS(Domain Name System)
### It is the phonebook of the internet. It translates the field names like google.com to the IP addresses that understandable by computers.

# 2.Communication Protocols: TCP and UDP

### Two essential rule set that specifies how data will transport.
### TCP (Transmission Control System): It controls if data reaches to the destination. The speed is lower and it has approval mechanism. It is used for web sites,email and file transport.

### UDP(User Datagram Protocol): It does not control if data reaches to the destination. The speed is very high and it is used for live streams,online games and VoIP.

# 3.Packet Structure and Operation
### Data is divided into small units before sending on network called packets. Every packet has a Header and Payload part.

### Header: It includes IP of sender/receiver, port numbers and the sequence number of the packet.
### Payload: The actual data being transported.

### When this packets arrive at the destination,they are combined in the correct order by  protocols (especially TCP).

# 4.Network Analyze Devices

### To determine network problems or collect information, these following commands are used:

### Ping: It sends a small data packet to a target device to measure response time (latency). It checks if the device is alive.

### Traceroute: Shows the path a packet takes, listing each server (router) it passes through and where delays occur step-by-step.

### Nslookup: It provides users to examine a domain name to find its associated IP address.
