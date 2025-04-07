#### Modules 9 – 12 of the CCNA3 – Enterprise Networking, Security, and Automation (ENSA) v7.0

**1. What is the term used to indicate a variation of delay?**

- latency
- serialization delay
- speed mismatch
- **jitter**

**Explanation:** Jitter is a phenomenon caused by a variation in delay. Delay (or latency) is the time it takes for the packet to arrive at its destination. Jitter describes how the voice packets arrive at the destination at varying intervals (not in a steady, consistent stream).

**2. A network engineer performs a ping test and receives a value that shows the time it takes for a packet to travel from a source to a destination device and return. Which term describes the value?**

- jitter
- **latency**
- priority
- bandwidth

**3. What role do network devices play in the IntServ QoS model?**

- **Network devices ensure that resources are available before traffic is allowed to be sent by a host through the network.**
- Network devices provide a best-effort approach to forwarding traffic.
- Network devices are configured to service multiple classes of traffic and handle traffic as it may arrive.
- Network devices use QoS on a hop-by-hop basis to provide excellent scalability.

**4. Which device would be classified as a trusted endpoint?**

- switch
- router
- firewall
- **IP phone**

**Explanation:** Trusted endpoints are devices that have the capability to mark application traffic at Layer 2 or Layer 3. Trusted endpoints include the following:  
– IP phones  
– Wireless access points  
– Videoconferencing gateways and systems  
– IP conferencing stations and more

**5. What is the benefit of deploying Layer 3 QoS marking across an enterprise network?**

- **Layer 3 marking can carry the QoS information end-to-end.**
- Layer 3 marking can carry QoS information on switches that are not IP aware.
- Layer 3 marking can be carried in the 802.1Q fields.
- Layer 3 marking can be used to carry non-IP traffic.

**Explanation:** Marking traffic at Layer 2 or Layer 3 is very important and will affect how traffic is treated in a network using QoS.

- Layer 2 marking of frames can be performed for non-IP traffic.
- Layer 2 marking of frames is the only QoS option available for switches that are not “IP aware.”
- Layer 3 marking will carry the QoS information end-to-end.
    

**6. What is the function of a QoS trust boundary?**

- A trust boundary identifies the location where traffic cannot be remarked.
- A trust boundary only allows traffic to enter if it has previously been marked.
- **A trust boundary identifies which devices trust the marking on packets that enter a network.**
- A trust boundary only allows traffic from trusted endpoints to enter the network.

**Explanation:** Network traffic is classified and marked as close to the source device as possible. The trust boundary is the location where the QoS markings on a packet are trusted as they enter an enterprise network.

**7. What are two approaches to prevent packet loss due to congestion on an interface? (Choose two.)**

- Decrease buffer space.
- Disable queuing mechanisms.
- **Drop lower-priority packets.**
- Prevent bursts of traffic.
- **Increase link capacity.**

**Explanation:** There are three approaches to prevent sensitive traffic from being dropped:

- Increase link capacity to ease or prevent congestion.
- Guarantee enough bandwidth and increase buffer space to accommodate bursts of traffic from fragile flows.
- Prevent congestion by dropping lower-priority packets before congestion occurs.
    

**8. What configuration scenario would offer the most protection to SNMP get and set messages?**

- SNMPv2 for in-band management with read-write community strings
- SNMPv1 with out-of-band management in a private subnet
- **SNMPv3 configured with the auth security level**
- SNMP community strings

**Explanation:** SNMPv3 supports authentication and encryption with the auth and priv security levels. SNMPv1 and SNMPv2 do not support authentication or encryption. Using a default community string is not secure because the default string of “public” is well known and would allow anyone with SNMP systems to read device MIBs.

**9. Refer to the exhibit. The network administrator enters these commands into the R1 router:**

R1# copy running-config tftp
Address or name of remote host [ ]?

**When the router prompts for an address or remote host name, what IP address should the administrator enter at the prompt?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i283561v1n1_208760.jpg)

- 192.168.9.254
- 192.168.10.2
- **192.168.11.252**
- 192.168.11.254
- 192.168.10.1

**Explanation:** The requested address is the address of the TFTP server. A TFTP server is an application that can run on a multitude of network devices including a router, server, or even a networked PC.

**10. The command ntp server 10.1.1.1 is issued on a router. What impact does this command have?**

- determines which server to send system log files to
- **synchronizes the system clock with the time source with IP address 10.1.1.1**
- identifies the server on which to store backup configurations
- ensures that all logging will have a time stamp associated with it

**Explanation:** The **ntp server** _ip-address_ global configuration command configures the NTP server for IOS devices.

**11. As the network administrator you have been asked to implement EtherChannel on the corporate network. What does this configuration consist of?**

- providing redundant links that dynamically block or forward traffic
- grouping two devices to share a virtual IP address
- **grouping multiple physical ports to increase bandwidth between two switches**
- providing redundant devices to allow traffic to flow in the event of device failure

**Explanation:** EtherChannel is utilized on a network to increase speed capabilities by grouping multiple physical ports into one or more logical EtherChannel links between two switches. STP is used to provide redundant links that dynamically block or forward traffic between switches. FHRPs are used to group physical devices to provide traffic flow in the event of failure.

**12. What is a definition of a two-tier LAN network design?**

- access and core layers collapsed into one tier, and the distribution layer on a separate tier
- **distribution and core layers collapsed into one tier, and the access layer on a separate tier**
- access, distribution, and core layers collapsed into one tier, with a separate backbone layer
- access and distribution layers collapsed into one tier, and the core layer on a separate tier

**Explanation:** Maintaining three separate network tiers is not always required or cost-efficient. All network designs require an access layer, but a two-tier design can collapse the distribution and core layers into one layer to serve the needs of a small location with few users.

**13. What are two reasons to create a network baseline? (Choose two.)**

- to select a routing protocol
- to determine what kind of equipment to implement
- to design a network according to a proper model
- **to identify future abnormal network behavior**
- to evaluate security vulnerabilities in the network
- **to determine if the network can deliver the required policies**

**Explanation:** A network baseline is created to provide a comparison point, at the time that the network is performing optimally, to whatever changes are implemented in the infrastructure. A baseline helps to keep track of the performance, to track the traffic patterns, and to monitor network behavior.

**14. A computer can access devices on the same network but cannot access devices on other networks. What is the probable cause of this problem?**

- The computer has an incorrect subnet mask.
- **The computer has an invalid default gateway address.**
- The cable is not connected properly to the NIC.
- The computer has an invalid IP address.

**Explanation:** The default gateway is the address of the device a host uses to access the Internet or another network. If the default gateway is missing or incorrect, that host will not be able to communicate outside the local network. Because the host can access other hosts on the local network, the network cable and the other parts of the IP configuration are working.

**15. In which step of gathering symptoms does the network engineer determine if the problem is at the core, distribution, or access layer of the network?**

- Gather information.
- **Narrow the scope.**
- Document the symptoms.
- Determine ownership.
- Determine the symptoms.

**Explanation:** In the “narrow the scope” step of gathering symptoms, a network engineer will determine if the network problem is at the core, distribution, or access layer of the network. Once this step is complete and the layer is identified, the network engineer can determine which pieces of equipment are the most likely cause.

**16. A network administrator is deploying QoS with the ability to provide a special queue for voice traffic so that voice traffic is forwarded before network traffic in other queues. Which queuing method would be the best choice?**

- **LLQ**
- CBWFQ
- WFQ
- FIFO

**Explanation:** Low latency queuing (LLQ) allows delay-sensitive data, such as voice traffic, to be defined in a strict priority queue (PQ) and to always be sent first before any packets in any other queue are forwarded.

**17. What are two characteristics of voice traffic? (Choose two.)**

- **Voice traffic latency should not exceed 150 ms.**
- Voice traffic is unpredictable and inconsistent.
- Voice traffic requires at least 384 kbs of bandwidth.
- Voice traffic consumes lots of network resources.
- **Dropped voice packets are not retransmitted.**

**Explanation:** Voice traffic does not consume a lot of network resources, such as bandwidth. However, it is very sensitive to delay and dropped packets cannot be retransmitted. For good voice quality, the amount of latency should always be less than 150 milliseconds.

**18. Which type of network traffic cannot be managed using congestion avoidance tools?**

- TCP
- ICMP
- IP
- **UDP**

**Explanation:** Queuing and compression techniques can help to reduce and prevent UDP packet loss, but there is no congestion avoidance for User Datagram Protocol (UDP) based traffic.

**19. When QoS is implemented in a converged network, which two factors can be controlled to improve network performance for real-time traffic? (Choose two.)**

- **delay**
- packet addressing
- **jitter**
- packet routing
- link speed

**Explanation:** Delay is the latency between a sending and receiving device. Jitter is the variation in the delay of the received packets. Both delay and jitter need to be controlled in order to support real-time voice and video traffic.

**20. An administrator wants to replace the configuration file on a Cisco router by loading a new configuration file from a TFTP server. What two things does the administrator need to know before performing this task? (Choose two.)**

- name of the configuration file that is currently stored on the router
- configuration register value
- **name of the configuration file that is stored on the TFTP server**
- router IP address
- **TFTP server IP address**

**Explanation:** In order to identify the exact location of the desired configuration file, the IP address of the TFTP server and the name of the configuration file are essential information. Because the file is a new configuration, the name of the current configuration file is not necessary.

**21. Refer to the exhibit. Which of the three Cisco IOS images shown will load into RAM?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i217901v1n1_217901.png)

- **The router selects an image depending on the boot system command in the configuration.**
- The router selects an image depending on the value of the configuration register.
- The router selects the third Cisco IOS image because it is the most recent IOS image.
- The router selects the third Cisco IOS image because it contains the advipservicesk9 image.
- The router selects the second Cisco IOS image because it is the smallest IOS image.

**Explanation:** When performing an upgrade or testing different IOS versions, the **boot system** command is used to select which image is used to boot the Cisco device.

**22. Refer to the exhibit. What two types of devices are connected to R1? (Choose two.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i210931v1n1_210931.png)

- **switch**
- hub
- **router**
- repeater
- Source Route Bridge

**Explanation:** The capabilities of the devices displayed by the output show them to be a Cisco 2811 series router, Cisco 1941 series router, and a Cisco 2960 switch.

**23. What are three functions provided by the syslog service? (Choose three.)**

- **to select the type of logging information that is captured**
- to periodically poll agents for data
- to provide statistics on packets that are flowing through a Cisco device
- to provide traffic analysis
- **to gather logging information for monitoring and troubleshooting**
- **to specify the destinations of captured messages**

**Explanation:** There are three primary functions provided by the syslog service:

1. gathering logging information
2. selection of the type of information to be logged
3. selection of the destination of the logged information
    

**24. What is the function of the MIB element as part of a network management system?**

- to collect data from SNMP agents
- to send and retrieve network management information
- to change configurations on SNMP agents
- **to store data about a device**

**Explanation:** The Management Information Base (MIB) resides on a networking device and stores operational data about the device. The SNMP manager can collect information from SNMP agents. The SNMP agent provides access to the information.

**25. What network design would contain the scope of disruptions on a network should a failure occur?**

- the reduction in the number of redundant devices and connections in the network core
- the installation of only enterprise class equipment throughout the network
- **the deployment of distribution layer switches in pairs and the division of access layer switch connections between them**
- the configuration of all access layer devices to share a single gateway

**Explanation:** One way to contain the impact of a failure on the network is to implement redundancy. One way this is accomplished is by deploying redundant distribution layer switches and dividing the access layer switch connections between the redundant distribution layer switches. This creates what is called a switch block. Failures in a switch block are contained to that block and do not bring down the whole network.

**26. Which action should be taken when planning for redundancy on a hierarchical network design?**

- **add alternate physical paths for data to traverse the network**
- continually purchase backup equipment for the network
- implement STP portfast between the switches on the network
- immediately replace a non-functioning module, service or device on a network

**Explanation:** One method of implementing redundancy is path redundancy, installing alternate physical paths for data to traverse the network. Redundant links in a switched network supports high availability and can be used for load balancing, reducing congestion on the network.

**27. What are two benefits of extending access layer connectivity to users through a wireless medium? (Choose two.)**

- **increased flexibility**
- increased network management options
- decreased number of critical points of failure
- **reduced costs**
- increased bandwidth availability

**Explanation:** Wireless connectivity at the access layer provides increased flexibility, reduced costs, and the ability to grow and adapt to changing business requirements. Utilizing wireless routers and access points can provide an increase in the number of central points of failure. Wireless routers and access points will not provide an increase in bandwidth availability.

**28. What is a basic function of the Cisco Borderless Architecture access layer?**

- aggregates Layer 2 broadcast domains
- **provides access to the user**
- aggregates Layer 3 routing boundaries
- provides fault isolation

**Explanation:** A function of the Cisco Borderless Architecture access layer is providing network access to the users. Layer 2 broadcast domain aggregation, Layer 3 routing boundaries aggregation, and high availability are distribution layer functions. The core layer provides fault isolation and high-speed backbone connectivity.

**29. Which characteristic would most influence a network design engineer to select a multilayer switch over a Layer 2 switch?**

- ability to have multiple forwarding paths through the switched network based on VLAN number(s)
- **ability to build a routing table**
- ability to provide power to directly-attached devices and the switch itself
- ability to aggregate multiple ports for maximum data throughput

**Explanation:** Multilayer switches, also known as Layer 3 switches, can route and build a routing table. This capability is required in a multi-VLAN network and would influence the network designer to select a multilayer switch. The other options are features also available on Layer 2 switches, so they would not influence the decision to select a multilayer switch.

**30. Refer to the exhibit. Why are routers R1 and R2 not able to establish an OSPF adjacency?​**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i219570v7n1_219570.gif)

- **The serial interfaces are not in the same area.**
- The process numbers are not the same in both routers.
- A backbone router cannot establish an adjacency with an ABR router.
- The router ID values are not the same in both routers.

**Explanation:** On router R1, the network 192.168.10.0/30 is defined in the wrong area (area 1). It has to be defined in area 0 in order to establish adjacency with router R2, which has the network 192.168.10.0/30 defined in area 0.

**31. When is the most appropriate time to measure network operations to establish a network performance baseline?**

- whenever high network use is detected, so that how the network performs under stress can be monitored
- during quiet vacation periods, so that the level of non-data traffic can be determined
- **at the same time each day across a set period of average working days, so that typical traffic patterns can be established**
- at random times during a 10 week period, so that abnormal traffic levels can be detected

**Explanation:** The purpose of establishing a network performance baseline is to provide a reference of normal or average network use to enable data traffic anomalies to be detected and then investigated. Network operations that are not average, or are not normal, cannot be used to establish a network performance baseline.

**32. Refer to the exhibit. A user has configured a NIC on the PC as shown but finds that the PC is unable to access the Internet. What is the problem?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i208776v9n1_208776.png)

- The preferred DNS address is incorrect.
- **The default gateway address is incorrect.**
- The settings were not validated upon exit.
- There should not be an alternate DNS server.

**Explanation:** In order for a computer to communicate outside its network, it must have a valid default gateway configured.This address cannot be the same as the IP address of the computer.

**33. Refer to the exhibit. A network engineer configured an ACL preventing Telnet and HTTP access to the HQ web server from guest users in the Branch LAN. The address of the web server is 192.168.1.10 and all guest users are assigned addresses in the 192.168.10.0/24 network. After implementing the ACL, no one can access any of the HQ servers. What is the problem?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2020-01-18_225619.jpg)

- Inbound ACLs must be routed before they are processed.
- **The ACL is implicitly denying access to all the servers.**
- Named ACLs require the use of port numbers.
- The ACL is applied to the interface using the wrong direction.

**Explanation:** Both named and numbered ACLs have an implicit deny ACE at the end of the list. This implicit deny blocks all traffic.

**34. Refer to the exhibit. A network administrator has configured OSPFv2 on the two Cisco routers as shown. PC1 is unable to connect to PC2. What should the administrator do first when troubleshooting the OSPFv2 implementation?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i285128v1n1_NewItem.png)

- Disconnect the serial link between router R1 and R2.
- Turn off OSPFv2.
- Implement the network 192.168.255.0 0.0.0.3 area 0 command on router R1.
- **Test Layer 3 connectivity between the directly connected routers.**

**Explanation:** A prerequisite for OSPFv2 neighbor relationships to form between two routers is Layer 3 connectivity. A successful ping confirms that a router interface is active and may be able to form an OSPF neighbor adjacency.

**35. What type of traffic is described as requiring latency to be no more than 150 milliseconds (ms)?**

- **voice**
- video
- data

**36. A network manager wants to add a time to log messages so that there is record of when the message was generated. What command should the administrator use on a Cisco router?**

- show cdp interface
- ntp server 10.10.14.9
- **service timestamps log datetime**
- clock timezone PST -7

**37. Match the functions to the corresponding layers. (Not all options are used.)**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/2020-01-21_005631.jpg)  
Place the options in the following order:

|   |   |
|---|---|
|represents the network edge|access layer|
|provides network access to the user|access layer|
|implements network access policy|distribution layer|
|establishes Layer 3 routing boundaries|distribution layer|
|provides high-speed backbone connectivity|core layer|
|functions as an aggregator for all the campus blocks|core layer|

**38. Match the borderless switched network guideline description to the principle. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-10_084218.jpg)

|   |   |
|---|---|
|facilitates understanding the role of each device at every tier, simplifies deployment, operation, management, and reduces fault domains at every tier|hierarchical|
|satisfies user expectations for keeping the network always on|resiliency|
|allows seamless network expansion and integrated service enablement on an on-demand basis|modularity|
|allows intelligent traffic load sharing by using all network resources|flexibility|

**39. What are two characteristics of the best-effort QoS model? (Choose two.)**

- It allows end hosts to signal their QoS needs to the network.
- It uses a connection-oriented approach with QoS.
- It provides preferential treatment for voice packets.
- **It does not provide a delivery guarantee for packets.**
- **It treats all network packets in the same way.**

**Explanation:** The best-effort QoS model provides no guarantees and it is commonly used on the Internet. The best-effort QoS model treats all network packets in the same way.

**40. Why is QoS an important issue in a converged network that combines voice, video, and data communications?**

- Data communications are sensitive to jitter.
- Legacy equipment is unable to transmit voice and video without QoS.  
    Correct Response
- **Voice and video communications are more sensitive to latency.**
- Data communications must be given the first priority.

**Explanation:** Without any QoS mechanisms in place, time-sensitive packets, such as voice and video, will be dropped with the same frequency as email and web browsing traffic.

**41. A network administrator configures a router with the command sequence:**

R1(config)# boot system tftp://c1900-universalk9-mz.SPA.152-4.M3.bin
R1(config)# boot system rom

**What is the effect of the command sequence?**

- On next reboot, the router will load the IOS image from ROM.
- The router will search and load a valid IOS image in the sequence of flash, TFTP, and ROM.
- The router will copy the IOS image from the TFTP server and then reboot the system.
- **The router will load IOS from the TFTP server. If the image fails to load, it will load the IOS image from ROM.**

**Explanation:** The **boot system** command is a global configuration command that allows the user to specify the source for the Cisco IOS Software image to load. In this case, the router is configured to boot from the IOS image that is stored on the TFTP server and will use the ROMmon imagethat is located in the ROM if it fails to locate the TFTP server or fails to load a valid image from the TFTP server.

**42. Which statement describes SNMP operation?**

- An SNMP agent that resides on a managed device collects information about the device and stores that information remotely in the MIB that is located on the NMS.​
- **A set request is used by the NMS to change configuration variables in the agent device.**
- An NMS periodically polls the SNMP agents that are residing on managed devices by using traps to query the devices for data.​
- A get request is used by the SNMP agent to query the device for data.​

**Explanation:** An SNMP agent that resides on a managed device collects and stores information about the device and its operation. This information is stored by the agent locally in the MIB. An NMS periodically polls the SNMP agents that are residing on managed devices by using the get request to query the devices for data.

**43. Refer to the exhibit. A network administrator issues the show lldp neighbors command on a switch. What are two conclusions that can be drawn? (Choose two.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i278776v1n1_278776.png)

- **Dev1 is connected to interface Fa0/5 of S1.**
- Dev1 is a switch with mixed types of interfaces.
- **Dev2 is a switch.**
- Dev1 is connected to interface Fa0/4 of Dev2.
- S1 has only two interfaces.

**Explanation:** In the output from the **show lldp** command, under Capability, R indicates a router and B indicates a bridge (switch). Nothing indicates that Dev1 and Dev2 are connected to one another.

**44. What are the three layers of the switch hierarchical design model? (Choose three.)**

- **distribution**
- network access
- data link
- enterprise
- **access**
- **core**

**Explanation:** The access layer is the lowest layer and it provides network access to users. The distribution layer has many functions, but it aggregates data from the access layer, provides filtering, policy control, and sets Layer 3 routing boundaries. The core layer provides high speed connectivity.

**45. Refer to the exhibit. Which devices exist in the failure domain when switch S3 loses power?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i278658v1n1_222708.png)

- S4 and PC_2
- PC_3 and PC_2
- **PC_3 and AP_2**
- S1 and S4
- AP_2 and AP_1

**Explanation:** A failure domain is the area of a network that is impacted when a critical device such as switch S3 has a failure or experiences problems.

**46. A network designer is considering whether to implement a switch block on the company network. What is the primary advantage of deploying a switch block?**

- This is network application software that prevents the failure of a single network device.
- **The failure of a switch block will not impact all end users.**
- This is a security feature that is available on all new Catalyst switches.
- A single core router provides all the routing between VLANs.

**Explanation:** The configuration of a switch block provides redundancy so that the failure of a single network device generally has little or no effect on end users.

**47. Which troubleshooting tool would a network administrator use to check the Layer 2 header of frames that are leaving a particular host?**

- knowledge base
- **protocol analyzer**
- CiscoView
- baselining tool

**Explanation:** A protocol analyzer such as Wireshark is capable of displaying the headers of data at any OSI Layer.

**48. Refer to the exhibit. R1 and R3 are connected to each other via the local serial 0/0/0 interface. Why are they not forming an adjacency?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i212841v1n2_212841.jpg)

- They have different routing processes.
- They have different router IDs.
- **They are in different subnets.**
- The connecting interfaces are configured as passive.

**Explanation:** The routers need to be in the same subnet in order to form an adjacency. The routing processes can be different on each router. The router IDs must be different for routers that participate in the same routing domain. The interfaces are not passive.

**49. What type of traffic is described as not resilient to loss?**

- **video**
- data
- voice

**Explanation:** Video traffic tends to be unpredictable, inconsistent, and bursty compared to voice traffic. Compared to voice, video is less resilient to loss and has a higher volume of data per packet.

**50. A network manager wants lists the contents of flash. What command should the administrator use on a Cisco router?**

- show file systems
- **dir**
- lldp enable
- service timestamps log datetime

**51. Voice packets are being received in a continuous stream by an IP phone, but because of network congestion the delay between each packet varies and is causing broken conversations. What term describes the cause of this condition?**

- buffering
- latency
- queuing
- **jitter**

**Explanation:** Jitter is the variation in the latency or delay of received packets. When data is sent, packets are sent in a continuous stream and are spaced evenly apart. Because of network congestion, the delay between each packet can vary instead of remaining constant.

**52. A user is unable to reach the website when typing http://www.cisco.com in a web browser, but can reach the same site by typing http://72.163.4.161. What is the issue?**

- DHCP
- **DNS**
- Default Gateway
- TCP/IP Protocol stack

**Explanation:** Domain Name Service (DNS) is used to translate a web address to an IP address. The address of the DNS server is provided via DHCP to host computers.​

**53. What type of traffic is described as tending to be unpredictable, inconsistent, and bursty?**

- Audio
- **Video**
- Data
- Voice

**54. A network manager wants to determine the size of the Cisco IOS image file on the networking device. What command should the administrator use on a Cisco router?**

- **show flash:0**
- copy flash: tftp:
- config-register 0x2102
- confreg 0x2142

**55. What is the principle that is applied when a network technician is troubleshooting a network fault by using the divide-and-conquer method?**

- Testing is performed at Layer 7 and at Layer 1, then at Layers 6 and 2, and so on, working towards the middle of the stack until all layers are verified as operational.
- **Once it is verified that components in a particular layer are functioning properly, it can then be assumed that components in the layers below it are also functional.**
- Testing is performed at all layers of the OSI model until a non-functioning component is found.
- Once it is verified that a component in a particular layer is functioning properly, testing can then be performed on any other layer.

**Explanation:** The nature of the OSI and TCP/IP layered models is that upper layers are dependent on lower layers. So when troubleshooting, if a particular layer is found to be working correctly then it can be assumed that all layers below it are also functioning correctly.

**56. Which queuing algorithm has only a single queue and treats all packets equally?**

- CBWFQ
- **FIFO**
- LLQ
- WFQ

**57. What type of traffic is described as traffic that requires at least 30 Kbps of bandwidth?**

- **voice**
- data
- video

**58. What type of traffic is described as being able to tolerate a certain amount of latency, jitter, and loss without any noticeable effects?**

- **voice**
- video
- data

**59. A network manager wants to view the amount of available and free memory, the type of file system, and its permissions. What command should the administrator use on a Cisco router?**

- ntp server 10.10.14.9
- lldp enable
- clock timezone PST -7
- **show file systems**

**60. What type of traffic is described as requiring latency to be no more than 400 milliseconds (ms)?**

- voice
- data
- **video**

**61. What type of traffic is described as consisting of traffic that requires a higher priority if interactive?**

- **data**
- voice
- video

**62. A network manager wants to configure the router to load a new image from flash during bootup. What command should the administrator use on a Cisco router?**

- copy flash: tftp:
- **boot system**
- clock set 14:25:00 nov 13 2018
- copy tftp startup-config

**63. What type of traffic is described as predictable and smooth?**

- data
- video
- **voice**

**64. A network manager wants to ensure that the device will ignore the startup config file during startup and bypass the required passwords. What command should the administrator use on a Cisco router?**

- copy usbflash0:/R1-Config
- copy running-config tftp
- **confreg 0x2142**
- config-register 0x2102

**65. What type of traffic is described as having a high volume of data per packet?**

- **video**
- voice
- data

**66. A network manager wants to backup the running configuration to a file server. What command should the administrator use on a Cisco router?**

- cd usbflash0:
- show file systems
- **copy running-config tftp**
- dir

**67. What type of traffic is described as consisting of traffic that gets a lower priority if it is not mission-critical?**

- voice
- **data**
- video