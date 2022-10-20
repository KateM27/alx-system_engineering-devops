# 0x07. Networking Basics #0

## About

This project is about:
* The OSI model
* Different types of network
* LAN and WAN network
* The Internet
* TCP/UDP protocols
* The ping command/ICMP
* And much more!

# Tasks

### OSI Model

**What is the OSI model?**
1. Set of Specifications that network hardware manufacturers must repsect
2. The OSI model is a conceptual model that characterizes the communication functions of a telecommunication system without regard to their underlying internal structure and technology
3. The OSI model is a conceptual model that characterizes the communication functions of a telecommunication system with a regard to their underlying internal structure and technology

**How is the OSI model organized?**
1. Alphabetically
2. From the lowest to the highest level
3. Randomly

### Types of network

**What type of network is a computer in local connected to?**
1. Internet
2. WAN
3. LAN

**What type of network could connect an office in one building to another office in a building a few streets away?**
1. Internet
2. WAN
3. LAN

**What network do you use when you browse www.google.com from your smartphone not connected to the WiFi?**
1. Internet
2. WAN
3. LAN

### MAC and IP address

**What is a MAC address?**
1. The name of a network interface
2. The unique identifier of a nework interface
3. A network interface

**What is an IP address?**
1. Is to devices connected to a network what postal addresses is to houses
2. The unique identifier of a network interface
3. Is a number that network devices use to connect to networks

### TCP and UDP

**Which statement is correct for the TCP box:**
1. It is a protocol that is transferring data in a slow way but surely
2. It is a protocol that is transferring data in a fast way and might lose data along in the process

**Which statement is correct for the UDP box:**
1. It is a protocol that is transferring data in a slow way but surely
2. It is a protocol that is transferring data in a fast way and might loss data along in the process

**Which statement is correct for the TCP worker:**
1. Have you received boxes x, y, z?
2. May I increase the rate at which I'm sending you boxes?

### TCP and UDP Ports

Once packets have been sent to the right network device using IP using either UDP or TCP as a mode of transportation, it needs to actually enter the network device.

If we continue the comparison of a network device to your house, where IP address is like your postal address, UDP and TCP ports are like the windows and doors of your place. A TCP/UDP network device has 65535 ports. Some of them are officially reserved for a specific usage, some of them are known to be used for a specific usage (but nothing is officially declared) and the rest are free of use.

While the full list of ports should not be memorized, it is important to know the most used ports, let’s start by remembering 3 of them:

* 22 for SSH
* 80 for HTTP
* 443 for HTTPS

Note that a specific IP + port = socket

### Is the host on the network

The Internet Control Message Protocol (ICMP) is a protocol in the Internet protocol suite. It is used by network devices, to check if other network devices are available on the network. The command ping uses ICMP to make sure that a network device remains online or to troubleshoot issues on the network.

Write a Bash script that pings an IP address passed as an argument.

Requirements:

* Accepts a string as an argument
* Displays Usage: 5-is_the_host_on_the_network {IP_ADDRESS} if no argument passed
* Ping the IP 5 times
