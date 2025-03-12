#### Modules 7 – 9 of the CCNA2 – Switching, Routing and Wireless Essentials v7.0 (SRWE)

**1. A DHCP-enabled client PC has just booted. During which two steps will the client PC use broadcast messages when communicating with a DHCP server? (Choose two.)**

- **DHCPDISCOVER**
- DHCPACK
- DHCPOFFER
- **DHCPREQUEST**
- DHCPNAK

**Explanation:** All DHCP messages between a DHCP-enabled client and a DHCP server are using broadcast messages until after the DHCPACK message. The DHCPDISCOVER and DHCPREQUEST messages are the only messages that are sent by a DHCP-enabled client. All DHCP messages between a DHCP-enabled client and a DHCP server use broadcast messages when the client is obtaining a lease for the first time.

**2. An administrator issues the commands:**

Router(config)# interface g0/1
Router(config-if)# ip address dhcp

**What is the administrator trying to achieve?**

- configuring the router to act as a DHCPv4 server
- **configuring the router to obtain IP parameters from a DHCPv4 server**
- configuring the router to act as a relay agent
- configuring the router to resolve IP address conflicts

**3. When a client is requesting an initial address lease from a DHCP server, why is the DHCPREQUEST message sent as a broadcast?**

- The client does not yet know the IP address of the DHCP server that sent the offer.
- The DHCP server may be on a different subnet, so the request must be sent as a broadcast.
- The client does not have a MAC address assigned yet, so it cannot send a unicast message at Layer 2.
- **The client may have received offers from multiple servers, and the broadcast serves to implicitly decline those other offers.**

**Explanation:** During the initial DHCP exchange between a client and server, the client broadcasts a DHCPDISCOVER message looking for DHCP servers. Multiple servers may be configured to respond to this request with DHCPOFFER messages. The client will choose the lease from one of the servers by sending a DHCPREQUEST message. It sends this message as a broadcast so that the other DHCP servers that sent offers will know that their offers were declined and the corresponding address can go back into the pool.

**4. Which DHCP IPv4 message contains the following information?**

Destination address: 255.255.255.255  
Client IPv4 address: 0.0.0.0  
Default gateway address: 0.0.0.0  
Subnet mask: 0.0.0.0

- DHCPACK
- **DHCPDISCOVER**
- DHCPOFFER
- DHCPREQUEST

**5. Place the options in the following order:**

- a client initiating a message to find a DHCP server – DHCPDISCOVER
- a DHCP server responding to the initial request by a client – DHCPOFFER
- the client accepting the IP address provided by the DHCP server – DHCPREQUEST
- the DHCP server confirming that the lease has been accepted – DHCPACK

**6. Which protocol automates assignment of IP addresses on a network, and which port number does it use? (Choose two.)**

- **DHCP**
- DNS
- SMB
- 53
- **67**
- 80

**Explanation:** DNS uses port 53 and translates URLs to IP addresses. SMB provides shared access to files and printers and uses port 445. Port 80 is used by HTTP. HTTP is a protocol used to communicate between a web browser and a server.

**7. Refer to the exhibit. PC1 is configured to obtain a dynamic IP address from the DHCP server. PC1 has been shut down for two weeks. When PC1 boots and tries to request an available IP address, which destination IP address will PC1 place in the IP header?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i207537v1n2_207537.png)

- 192.168.1.1
- 192.168.1.255
- **255.255.255.255**
- 192.168.1.8

**Explanation:** When a host boots and has been configured for dynamic IP addressing, the device tries to obtain a valid IP address. It sends a DHCPDISCOVER message. This is a broadcast message because the DHCP server address is unknown (by design). The destination IP address in the IP header is 255.255.255.255 and the destination MAC address is FF:FF:FF:FF:FF:FF.

**8. Which message does an IPv4 host use to reply when it receives a DHCPOFFER message from a DHCP server?**

- DHCPOFFER
- DHCPDISCOVER
- **DHCPREQUEST**
- DHCPACK

**Explanation:** When the client receives the DHCPOFFER from the server, it sends back a DHCPREQUEST broadcast message. On receiving the DHCPREQUEST message, the server replies with a unicast DHCPACK message.

**9. Which command, when issued in the interface configuration mode of a router, enables the interface to acquire an IPv4 address automatically from an ISP, when that link to the ISP is enabled?**

- service dhcp
- **ip address dhcp**
- ip helper-address
- ip dhcp pool

**Explanation:** The **ip address dhcp** interface configuration command configures an Ethernet interface as a DHCP client. The **service dhcp** global configuration command enables the DHCPv4 server process on the router. The **ip helper-address** command is issued to enable DHCP relay on the router. The **ip dhcp pool** command creates the name of a pool of addresses that the server can assign to hosts.

**10. Which kind of message is sent by a DHCP client when its IP address lease has expired?​**

- a DHCPDISCOVER unicast message​
- a DHCPREQUEST broadcast message​
- **a DHCPREQUEST unicast message​**
- a DHCPDISCOVER broadcast message

**Explanation:** When the IP address lease time of the DHCP client expires, it sends a DHCPREQUEST unicast message directly to the DHCPv4 server that originally offered the IPv4 address.

**11. A host PC is attempting to lease an address through DHCP. What message is sent by the server to let the client know it is able to use the provided IP information?**

- DHCPDISCOVER
- DHCPOFFER
- DHCPREQUEST
- **DHCPACK**
- DHCPNACK

**Explanation:** When a host uses DHCP to automatically configure an IP address, the typically sends two messages: the DHCPDISCOVER message and the DHCPREQUEST message. These two messages are usually sent as broadcasts to ensure that all DHCP servers receive them. The servers respond to these messages using DHCPOFFER, DHCPACK, and DHCPNACK messages, depending on the circumstance.

**12. What is one indication that a Windows computer did not receive an IPv4 address from a DHCP server?**

- The computer cannot ping 127.0.0.1.
- **The computer receives an IP address that starts with 169.254.**
- Windows displays a DHCP timeout message.
- The computer cannot ping other devices on the same network with IP addresses in the 169.254.0.0/16 range.

**Explanation:** When a Windows PC cannot communicate with an IPv4 DHCP server, the computer automatically assigns an IP address in the 169.254.0.0/16 range. Any other device on the same network that receives an address in the same range is reachable.​

**13. Which DHCPv4 message will a client send to accept an IPv4 address that is offered by a DHCP server?**

- broadcast DHCPACK
- **broadcast DHCPREQUEST**
- unicast DHCPACK
- unicast DHCPREQUEST

**Explanation:** When a DHCP client receives DHCPOFFER messages, it will send a broadcast DHCPREQUEST message for two purposes. First, it indicates to the offering DHCP server that it would like to accept the offer and bind the IP address. Second, it notifies any other responding DHCP servers that their offers are declined.

**14. A small coffee shop is offering free Wi-Fi to customers. The network includes a wireless router and a DSL modem that is connected to the local phone company. What method is typically used to configure the connection to the phone company?**

- **Set the WAN connection in the wireless router as a DHCP client.**
- Set the connection between the wireless router and the DSL modem as a private IP network.
- Set the DSL modem as a DHCP client to get a public IP address from the wireless router.
- Set the DSL modem as a DHCP client to the phone company and a DHCP server for the internal connection.

**Explanation:** In a SOHO environment, a wireless router connects to an ISP via a DSL or cable modem. The IP address between the wireless router and ISP site is typically assigned by the ISP through DHCP. The DSL modem does not manage IP address allocation.

**15. A company uses DHCP to manage IP address deployment for employee workstations. The IT department deploys multiple DHCP servers in the data center and uses DHCP relay agents to facilitate the DHCP requests from workstations. Which two UDP ports are used to forward DHCP traffic? (Choose two.)**

- 23
- 53
- **67**
- **68**
- 80

**Explanation:** The DHCP protocol operates with 2 UDP ports. UDP port 67 is the destination port for DHCP servers, and DHCP clients use UDP port 68.

**16. A client device on an Ethernet segment needs an IP address in order to communicate on the network. A DHCP server with IP address 192.168.1.1 has been configured and enabled on the network. How will a client device obtain a usable IP address for this network?**

- Send a DHCPACK packet to the default gateway address.
- Use a statically configured IP address from the pool of IP addresses that is offered by the DHCP server.
- **Send a DHCPDISCOVER message to physical address FF-FF-FF-FF-FF-FF.**
- Send a DHCPREQUEST packet to IP address 255.255.255.255.

**Explanation:** Like IP addressing, there is also a special MAC address for broadcast purposes: FF-FF-FF-FF-FF-FF. When a DHCP client needs to send a DHCP Discover message in order to seek DHCP servers, the client will use this MAC address as the destination MAC address in the Ethernet frame. It does this because it has no knowledge of the IP and MAC addresses of DHCP servers.

**17. What is an advantage of configuring a Cisco router as a relay agent?**

- **It can provide relay services for multiple UDP services.**
- It reduces the response time from a DHCP server.
- It can forward both broadcast and multicast messages on behalf of clients.
- It will allow DHCPDISCOVER messages to pass without alteration.

**Explanation:** By default, the **ip helper-address** command forwards the following eight UDP services:  
Port 37: Time  
Port 49: TACACS  
Port 53: DNS  
Port 67: DHCP/BOOTP client  
Port 68: DHCP/BOOTP server  
Port 69: TFTP  
Port 137: NetBIOS name service  
Port 138: NetBIOS datagram service

**18. Which statement is true about DHCP operation?​**

- **When a device that is configured to use DHCP boots, the client broadcasts a DHCPDISCOVER message to identify any available DHCP servers on the network.​**
- A client must wait for lease expiration before it sends another DHCPREQUEST message.​
- If the client receives several DHCPOFFER messages from different servers, it sends a unicast DHCPREQUEST message to the server from which it chooses to obtain the IP information.
- The DHCPDISCOVER message contains the IP address and subnet mask to be assigned, the IP address of the DNS server, and the IP address of the default gateway.​

**Explanation:** The client broadcasts a DHCPDISCOVER message to identify any available DHCP servers on the network. A DHCP server replies with a DHCPOFFER message. This message offers to the client a lease that contains such information as the IP address and subnet mask to be assigned, the IP address of the DNS server, and the IP address of the default gateway. After the client receives the lease, the received information must be renewed through another DHCPREQUEST message prior to the lease expiration.

**19. Order the DHCP message types as they would occur between a DHCP client and a DHCP server.**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/349.jpg)  

**Explanation:** The DHCPDISCOVER message is used to identify any DHCP servers on a network.  
The DHCPOFFER message is used by a server to offer a lease to a client. The DHCPREQUEST message is used to identify both the specific DHCP server and the lease that the client is accepting.  
The DHCPACK message is used by a server to finalize a successful lease with a client.  
The DHCPNAK message is used when an offered lease is no longer valid.

**20. A network administrator configures a router to send RA messages with M flag as 0 and O flag as 1. Which statement describes the effect of this configuration when a PC tries to configure its IPv6 address?**

- It should contact a DHCPv6 server for the prefix, the prefix-length information, and an interface ID that is both random and unique.
- **It should use the information that is contained in the RA message and contact a DHCPv6 server for additional information.**
- It should use the information that is contained in the RA message exclusively.
- It should contact a DHCPv6 server for all the information that it needs.

**Explanation:** ICMPv6 RA messages contain two flags to indicate whether a workstation should use SLAAC, a DHCPv6 server, or a combination to configure its IPv6 address. These two flags are M flag and O flag. When both flags are 0 (by default), a client must only use the information in the RA message. When M flag is 0 and O flag is 1, a client should use the information in the RA message and look for the other configuration parameters (such as DNS server addresses) on DHCPv6 servers.

**21. Refer to the exhibit. What should be done to allow PC-A to receive an IPv6 address from the DHCPv6 server?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i210917v1n1_Question-8.png)

- **Add the _ipv6 dhcp relay_ command to interface Fa0/0.**
- Change the _ipv6 nd managed-config-flag_ command to _ipv6 nd other-config-flag._
- Configure the _ipv6 nd managed-config-flag_ command on interface Fa0/1.
- Add the IPv6 address 2001:DB8:1234:5678::10/64 to the interface configuration of the DHCPv6 server.

**Explanation:** Client DHCPv6 messages are sent to a multicast address with link-local scope, which means that the messages will not be forwarded by routers. Because the client and server are on different subnets on different interfaces, the message will not reach the server. The router can be configured to relay the DHCPv6 messages from the client to the server by configuring the ipv6 dhcp relay command on the interface that is connected to the client.

**22. Refer to the exhibit. A network administrator is implementing the stateless DHCPv6 operation for the company. Clients are configuring IPv6 addresses as expected. However, the clients are not getting the DNS server address and the domain name information configured in the DHCP pool. What could be the cause of the problem?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i222841v1n1_210900.png)

- The DNS server address is not on the same network as the clients are on.
- **The router is configured for SLAAC operation.**
- The GigabitEthernet interface is not activated.
- The clients cannot communicate with the DHCPv6 server, evidenced by the number of active clients being 0.

**Explanation:** The router is configured for SLAAC operation because there is no configuration command to change the RA M and O flag value. By default, both M and O flags are set to 0. In order to permint stateless DHCPv6 operation, the interface command **ipv6 nd other-config-flag** should be issued. The GigabitEthernet interface is in working condition because clients can get RA messages and configure their IPv6 addresses as expected. Also, the fact that R1 is the DHCPv6 server and clients are getting RA messages indicates that clients can communicate with the DHCP server. The number of active clients is 0 because the DHCPv6 server does not maintain the state of clients IPv6 addresses (it is not configured for stateful DHCPv6 operation). The DNS server address issue is not relevant to the problem.

**23. Question as presented:**

A stateless DHCPv6 client would send a DHCPv6 INFORMATION-REQUEST message as step 3 in the process.

**24. A company uses the SLAAC method to configure IPv6 addresses for the employee workstations. Which address will a client use as its default gateway?​**

- the global unicast address of the router interface that is attached to the network
- the unique local address of the router interface that is attached to the network
- the all-routers multicast address
- **the link-local address of the router interface that is attached to the network**

**Explanation:** When a PC is configured to use the SLAAC method for configuring IPv6 addresses, it will use the prefix and prefix-length information that is contained in the RA message, combined with a 64-bit interface ID (obtained by using the EUI-64 process or by using a random number that is generated by the client operating system), to form an IPv6 address. It uses the link-local address of the router interface that is attached to the LAN segment as its IPv6 default gateway address.

**25. Refer to the exhibit. A network administrator is configuring a router for DHCPv6 operation. Which conclusion can be drawn based on the commands?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i210893v1n1_210893.png)

- The router is configured for stateful DHCPv6 operation, but the DHCP pool configuration is incomplete.
- The DHCPv6 server name is ACAD_CLASS.
- Clients would configure the interface IDs above 0010.
- **The router is configured for stateless DHCPv6 operation.**

**Explanation:** The DHCPv6 is for the stateless DHCPv6 operation that is indicated by changing the O flag to 1 and leaving the M flag as default, which is 0. Therefore, it is not configured for stateful DHCPv6 operation. Although the DNS server has the interface ID 0010, clients in stateless DHCPv6 operation will configure their interface IDs either by EUI-64 or a random number. The ACAD_CLASS is the name of the DHCP pool, not the DHCP server name.

**26. A network administrator is analyzing the features that are supported by different first-hop router redundancy protocols. Which statement describes a feature that is associated with HSRP?**

- **HSRP uses active and standby routers.**
- HSRP is nonproprietary.
- It allows load balancing between a group of redundant routers.
- It uses ICMP messages in order to assign the default gateway to hosts.

**Explanation:** The HSRP first-hop router redundancy protocol is Cisco proprietary and supports standby and active devices. VRRPv2 and VRRPv3 are nonproprietary. GLBP is Cisco proprietary and supports load balancing between a group of redundant routers.

**27. Refer to the exhibit. What protocol can be configured on gateway routers R1 and R2 that will allow traffic from the internal LAN to be load balanced across the two gateways to the Internet?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i216443v1n1_216443.png)

- **GLBP**
- PVST+
- PVST
- STP

**Explanation:** GLBP, or Group Load Balancing Protocol, allows multiple routers to act as a single default gateway for hosts. GLBP load balances the traffic across the individual routers on a per host basis.

**28. Refer to the exhibit. A network engineer is troubleshooting host connectivity on a LAN that uses a first hop redundancy protocol. Which IPv4 gateway address should be configured on the host?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i216427v1n1_216427v2.png)

- 192.168.2.0
- 192.168.2.1
- 192.168.2.2
- **192.168.2.100**

**Explanation:** The host default gateway address should be the FHRP (in this case GLBP) virtual IP address.

**29. Refer to the exhibit. Which destination MAC address is used when frames are sent from the workstation to the default gateway?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i223091v1n1_223091.png)

- **MAC address of the virtual router**
- MAC address of the standby router
- MAC addresses of both the forwarding and standby routers
- MAC address of the forwarding router

**Explanation:** The IP address of the virtual router acts as the default gateway for all the workstations. Therefore, the MAC address that is returned by the Address Resolution Protocol to the workstation will be the MAC address of the virtual router.

**30. Question as presented:**

Hot Standby Router Protocol (HSRP) is a Cisco-proprietary protocol that is designed to allow for transparent failover of a first-hop IPv4 device.

**31. Which FHRP implementation is a Cisco-proprietary protocol that suppports IPv4 load sharing?**

- IRDP
- **GLBP**
- VRRPv3
- GLBP for IPv6

**32. The address pool of a DHCP server is configured with 10.92.71.0/25. The network administrator reserves 8 IP addresses for servers. How many IP addresses are left in the pool to be assigned to other hosts?**

- 122
- **118**
- 119
- 108
- 116

**Explanation:** Calculate the maximum number of hosts available for the slash value and subtract the required static IP addresses required for the devices.  
/24 = 254 hosts  
/25 = 126 hosts  
/26 = 62 hosts  
/27 = 30 hosts  
/28 = 14 hosts

**33. Question as presented:**

The broadcast DHCPDISCOVER message finds DHCPv4 servers on the network. When the DHCPv4 server receives a DHCPDISCOVER message, it reserves an available IPv4 address to lease to the client and sends the unicast DHCPOFFER message to the requesting client. When the client receives the DHCPOFFER from the server, it sends back a DHCPREQUEST. On receiving the DHCPREQUEST message the server replies with a unicast DHCPACK message. DHCPREPLY and DHCPINFORMATION-REQUEST are DHCPv6 messages.

**34. After a host has generated an IPv6 address by using the DHCPv6 or SLAAC process, how does the host verify that the address is unique and therefore usable?**

- The host sends an ICMPv6 echo request message to the DHCPv6 or SLAAC-learned address and if no reply is returned, the address is considered unique.
- **The host sends an ICMPv6 neighbor solicitation message to the DHCP or SLAAC-learned address and if no neighbor advertisement is returned, the address is considered unique.**
- The host checks the local neighbor cache for the learned address and if the address is not cached, it it considered unique.
- The host sends an ARP broadcast to the local link and if no hosts send a reply, the address is considered unique.

**Explanation:** Before a host can actually configure and use an IPv6 address learned through SLAAC or DHCP, the host must verify that no other host is already using that address. To verify that the address is indeed unique, the host sends an ICMPv6 neighbor solicitation to the address. If no neighbor advertisement is returned, the host considers the address to be unique and configures it on the interface.

**35. Which statement describes HSRP?​**

- **It is used within a group of routers for selecting an active device and a standby device to provide gateway services to a LAN.**
- It uses ICMP to allow IPv4 hosts to locate routers that provide IPv4 connectivity to remote IP networks.​
- If the virtual router master fails, one router is elected as the virtual router master with the other routers acting as backups.
- It is an open standard protocol.

**Explanation:** It is VRRP that elects one router as the virtual router master, with the other routers acting as backups in case the virtual router master fails. HSRP is a Cisco-proprietary protocol. IRDP uses ICMP messages to allow IPv4 hosts to locate routers that provide IPv4 connectivity to other (nonlocal) IP networks. HSRP selects active and standby routers to provide gateway services to hosts on a LAN.

**36.Open the PT Activity. Perform the tasks in the activity instructions and then answer the question.**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/2020-03-31_170332.jpg)

![Icon](https://itexamanswers.net/wp-content/plugins/download-manager/assets/file-type-icons/pka.svg)

###### [Modules 7 - 9 Available and Reliable Networks](https://itexamanswers.net/download/modules-7-9-available-and-reliable-networks)

1 file(s) 159.43 KB

**What is the keyword that is displayed on www.netacad.com?**

- DHCP
- switch
- **Router**
- networking
- Cisco
- IPv6

**Explanation:** In order for the host to receive the address of the DNS server, the host must use stateless DHCPv6. The router is configured with the correct DHCPv6 pool, but is missing the command ipv6 nd other-config-flag that signals to the host that it should use DHCPv6 to get additional address information. This command should be added to the interface Gigabit0/0 configuration on the router.

**37. Match each DHCP message type with its description. (Not all options are used.)**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/2020-01-20_231506.jpg)  

**Explanation:** Place the options in the following order:

- a client initiating a message to find a DHCP server – DHCPDISCOVER
- a DHCP server responding to the initial request by a client – DHCPOFFER
- the client accepting the IP address provided by the DHCP server – DHCPREQUEST
- the DHCP server confirming that the lease has been accepted – DHCPACK

**38. Match the purpose with its DHCP message type. (Not all options are used.)**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/2020-01-20_232028.jpg)  

**Explanation:** The DHCPDISCOVER message is used to identify any DHCP servers on a network. The DHCPOFFER message is used by a server to offer a lease to a client. The DHCPREQUEST message is used to identify both the specific DHCP server and the lease that the client is accepting.  
The DHCPACK message is used by a server to finalize a successful lease with a client.  
The DHCPNAK message is used when an offered lease is no longer valid.

**39. Match the DHCP message types to the order of the stateful DHCPv6 process when a client first connects to an IPv6 network. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-08_154259.jpg)

|   |   |
|---|---|
|Step 1|DHCPv6 SOLICIT|
|Step 2|DHCPv6 ADVERTISE|
|Step 3|DHCPv6 REQUEST|
|Step 4|DHCPv6 REPLY|

**40. Match the step number to the sequence of stages that occur during the HSRP failover process. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-08_154407.jpg)

|   |   |
|---|---|
|Step 1|The forwarding router fails.|
|Step 2|The standby router stops seeing hello messages from the forwarding router.|
|Step 3|The standby router assumes the role of the forwarding router.|
|Step 4|The new forwarding router assumes both the IP and MAC addresses of the virtual router.|

**Explanation:** Hot Standby Router Protocol (HSRP) is a Cisco-proprietary protocol that is designed to allow for transparent failover of a first-hop IPv4 device.

**41. Match the FHRP protocols to the appropriate description. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-08_154524.jpg)

|   |   |
|---|---|
|HSRP|A Cisco proprietary FHRP that provides redundancy through use of an active device and standby device|
|VRRP|An open standard FHRP that provides redundancy through use of a virtual routers master and one or more backups|
|GLBP|A Cisco proprietary FHRP that provides load sharing in addition to redundancy|

**42. Match the DHCP message types to the order of the DHCPv4 process. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-08_153922.jpg)

|   |   |
|---|---|
|Step 1|DHCPDISCOVER|
|Step 2|DHCPOFFER|
|Step 3|DHCPREQUEST|
|Step 4|DHCPACK|

**Explanation:** The broadcast DHCPDISCOVER message finds DHCPv4 servers on the network. When the DHCPv4 server receives a DHCPDISCOVER message, it reserves an available IPv4 address to lease to the client and sends the unicast DHCPOFFER message to the requesting client. When the client receives the DHCPOFFER from the server, it sends back a DHCPREQUEST. On receiving the DHCPREQUEST message the server replies with a unicast DHCPACK message. DHCPREPLY and DHCPINFORMATION-REQUEST are DHCPv6 messages.

**43. The address pool of a DHCP server is configured with 192.168.234.0/27. The network administrator reserves 22 IP addresses for IP phones. How many IP addresses are left in the pool to be assigned to other hosts?**

- 10
- 0
- **8**
- 21
- 18

**Explanation:** Calculate the maximum number of hosts available for the slash value and subtract the required static IP addresses required for the devices.  
/24 = 254 hosts  
/25 = 126 hosts  
/26 = 62 hosts  
/27 = 30 hosts  
/28 = 14 hosts

**44. A company uses DHCP servers to dynamically assign IPv4 addresses to employee workstations. The address lease duration is set as 5 days. An employee returns to the office after an absence of one week. When the employee boots the workstation, it sends a message to obtain an IP address. Which Layer 2 and Layer 3 destination addresses will the message contain?**

- both MAC and IPv4 addresses of the DHCP server
- FF-FF-FF-FF-FF-FF and IPv4 address of the DHCP server
- **FF-FF-FF-FF-FF-FF and 255.255.255.255**
- MAC address of the DHCP server and 255.255.255.255

**Explanation:**When the lease of a dynamically assigned IPv4 address has expired, a workstation will send a DHCPDISCOVER message to start the process of obtaining a valid IP address. Because the workstation does not know the addresses of DHCP servers, it sends the message via broadcast, with destination addresses of FF-FF-FF-FF-FF-FF and 255.255.255.255.

**45. Which command will allow a network administrator to check the IP address that is assigned to a particular MAC address?**

- Router# show running-config I section_dhcp
- Router# show ip dhcp server statistics
- **Router# show ip dhcp binding**
- Router# show ip dhcp pool

**Explanation:** The `show ip dhcp binding` command will show the leases, including IP addresses, MAC addresses, lease expiration, type of lease, client ID, and user name.

**46. What is the reason that an ISP commonly assigns a DHCP address to a wireless router in a SOHO environment?**

- better network performance
- better connectivity
- **easy IP address management**
- easy configuration on ISP firewall

**Explanation:**In a SOHO environment, a wireless router connects to the ISP via a DSL or cable modem. The IP address between the wireless router and ISP site is typically assigned by the ISP through DHCP. This method facilitates the IP addressing management in that IP addresses for clients are dynamically assigned so that if a client is dropped, the assigned IP address can be easily reassigned to another client.

**47. What information can be verified through the show ip dhcp binding command?**

- **the IPv4 addresses that are assigned to hosts by the DHCP server**
- that DHCPv4 discover messages are still being received by the DHCP server
- the IPv4 addresses that have been excluded from the DHCPv4 pool
- the number of IP addresses remaining in the DHCP pool

**Explanation:**The `show ip dhcp binding` command shows a list of IPv4 addresses and the MAC addresses of the hosts to which they are assigned. Using this information an administrator can determine which host interfaces have been assigned to specific hosts.

**48. What is the result of a network technician issuing the command ip dhcp excluded-address 10.0.15.1 10.0.15.15 on a Cisco router?**

- The Cisco router will exclude only the 10.0.15.1 and 10.0.15.15 IP addresses from being leased to DHCP clients.
- **The Cisco router will exclude 15 IP addresses from being leased to DHCP clients.**
- The Cisco router will automatically create a DHCP pool using a /28 mask.
- The Cisco router will allow only the specified IP addresses to be leased to clients.

**Explanation:** The `ip dhcp excluded-address` command is followed by the first and the last addresses to be excluded from being leased to DHCP clients.

**49. Match the descriptions to the corresponding DHCPv6 server type. (Not all options are used.)**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/2020-01-22_235504.jpg)

**50. Refer to the exhibit. Based on the output that is shown, what kind of IPv6 addressing is being configured?**

![CCNA 2 v7 Modules 7 - 9: Available and Reliable Networks Exam Answers](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA-2-v7-Modules-7-9-Available-and-Reliable-Networks-Exam-Answers-50.png)

CCNA 2 v7 Modules 7 – 9: Available and Reliable Networks Exam Answers

- **stateless DHCPv6**
- SLAAC
- static link-local
- stateful DHCPv6

**Explanation:** Stateful DHCPv6 pools are configured with address prefixes for hosts via the `address` command, whereas stateless DHCPv6 pools typically only contain information such as DNS server addresses and the domain name. RA messages that are sent from routers that are configured as stateful DHCPv6 servers have the M flag set to 1 with the command `ipv6 nd managed-config-flag`, whereas stateless DHCPv6 servers are indicated by setting the O flag to 1 with the `ipv6 nd other-config-flag` command.

**51. Which FHRP implementation is a Cisco-proprietary protocol that suppports IPv6 load balancing?**

- GLBP
- **GLBP for IPv6**
- VRRPv3
- VRRPv2

**52. Which set of commands will configure a router as a DHCP server that will assign IPv4 addresses to the 192.168.100.0/23 LAN while reserving the first 10 and the last addresses for static assignment?**

ip dhcp excluded-address 192.168.100.1 192.168.100.9  
ip dhcp excluded-address 192.168.101.254  
ip dhcp pool LAN-POOL-100  
ip network 192.168.100.0 255.255.254.0  
ip default-gateway 192.168.100.1

dhcp pool LAN-POOL-100  
ip dhcp excluded-address 192.168.100.1 192.168.100.9  
ip dhcp excluded-address 192.168.100.254  
network 192.168.100.0 255.255.254.0  
default-router 192.168.101.1

ip dhcp excluded-address 192.168.100.1 192.168.100.10  
ip dhcp excluded-address 192.168.100.254  
ip dhcp pool LAN-POOL-100  
network 192.168.100.0 255.255.255.0  
ip default-gateway 192.168.100.1

**ip dhcp excluded-address 192.168.100.1 192.168.100.10  
ip dhcp excluded-address 192.168.101.254  
ip dhcp pool LAN-POOL-100  
network 192.168.100.0 255.255.254.0  
default-router 192.168.100.1**  

**Explanation:** The /23 prefix is equivalent to a network mask of 255.255.254.0. The network usable IPv4 address range is 192.168.100.1 to 192.168.101.254 inclusive. The commands dhcp pool, ip default-gateway, and ip network are not valid DHCP configuration commands.

**53. What is a result when the DHCP servers are not operational in a network?**

- Workstations are assigned with the IP address 127.0.0.1.
- Workstations are assigned with IP addresses in the 10.0.0.0/8 network.
- **Workstations are assigned with IP addresses in the 169.254.0.0/16 network.**
- Workstations are assigned with the IP address 0.0.0.0.

**Explanation:** When workstations are configured with obtaining IP address automatically but DHCP servers are not available to respond to the requests, a workstation can assign itself an IP addresses from the 169.254.0.0/16 network.

**54. A company uses the method SLAAC to configure IPv6 addresses for the workstations of the employees. A network administrator configured the IPv6 address on the LAN interface of the router. The interface status is UP. However, the workstations on the LAN segment did not obtain the correct prefix and prefix length. What else should be configured on the router that is attached to the LAN segment for the workstations to obtain the information?​**

R1(config)# ipv6 dhcp pool  
R1(config-if)# ipv6 enable  
**R1(config)# ipv6 unicast-routing**  
R1(config-if)# ipv6 nd other-config-flag  

**Explanation:** A PC that is configured to use the SLAAC method obtains the IPv6 prefix and prefix length from a router. When the PC boots, it sends an RS message to inform the routers that it needs the information. A router sends an RA message that includes the required information. For a router to be able to send RA messages, it must be enabled as an IPv6 router by the unicast ipv6-routing command in global configuration mode. The other options are not used to enable IPv6 routing on a router.

**55. Which FHRP implementation is a nonproprietary protocol which relies on ICMP to provide IPv4 redundancy?**

- VRRPv3
- GLBP for IPv6
- **IRDP**
- GLBP

**56. Refer to the exhibit. PC-A is unable to receive an IPv6 address from the stateful DHCPv6 server. What is the problem?**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/download.png)

- **The ipv6 dhcp relay command should be applied to interface Gig0/0.**
- The ipv6 nd managed-config-flag should be applied to interface Gig0/1.
- The ipv6 dhcp relay command should use the link-local address of the DHCP server.
- The ipv6 nd managed-config-flag command should be ipv6 nd other-config-flag .

**Explanation:** The **ipv6 dhcp relay** command must be applied to the interface where the clients are located. The **ipv6 dhcp relay** command can use either the link-local or global unicast address of the DHCPv6 server, or even a multicast address. The **ipv6 nd managed-config-flag** indicates to the clients that they should use stateful DHCPv6 and is also applied to the interface where the clients are located.

**57. Refer to the exhibit. A network administrator is configuring a router as a DHCPv6 server. The administrator issues a show ipv6 dhcp pool command to verify the configuration. Which statement explains the reason that the number of active clients is 0?**  
![](https://itexamanswers.net/wp-content/uploads/2016/02/i210895v1n1_210895.jpg)

- The default gateway address is not provided in the pool.
- No clients have communicated with the DHCPv6 server yet.
- The IPv6 DHCP pool configuration has no IPv6 address range specified.
- **The state is not maintained by the DHCPv6 server under stateless DHCPv6 operation.**

**Explain:**  
Under the stateless DHCPv6 configuration, indicated by the command ipv6 nd other-config-flag, the DHCPv6 server does not maintain the state information, because client IPv6 addresses are not managed by the DHCP server. Because the clients will configure their IPv6 addresses by combining the prefix/prefix-length and a self-generated interface ID, the ipv6 dhcp pool configuration does not need to specify the valid IPv6 address range. And because clients will use the link-local address of the router interface as the default gateway address, the default gateway address is not necessary.

**58. Which FHRP implementation is Cisco-proprietary and permits only one router in a group to forward IPv6 packets?**

- VRRPv3
- HSRP
- **HSRP for IPv6**
- VRRPv2

**59. Which FHRP implementation is a nonproprietary IPv4-only election protocol which has one master router per group?**

- HSRP for IPv6
- GLBP
- **VRRPv2**
- VRRPv3

**60. The address pool of a DHCP server is configured with 172.18.93.0/25. The network administrator reserves 10 IP addresses for web servers. How many IP addresses are left in the pool to be assigned to other hosts?**

- 106
- 117
- 114
- 120
- **116**

**Explain:**  
Calculate the maximum number of hosts available for the slash value and subtract the required static IP addresses required for the devices.  
/24 = 254 hosts  
/25 = 126 hosts  
/26 = 62 hosts  
/27 = 30 hosts  
/28 = 14 hosts

**61. The address pool of a DHCP server is configured with 10.3.2.0/24. The network administrator reserves 3 IP addresses for printers. How many IP addresses are left in the pool to be assigned to other hosts?**

- 252
- 241
- 255
- 249
- **251**

**Explain:** [**CIDR Subnet Calculator Online**](https://itexamanswers.net/ipv4-classless-inter-domain-routing-cidr-subnet-calculator-online.html)

**62. The address pool of a DHCP server is configured with 172.23.143.0/26. The network administrator reserves 14 IP addresses for file servers. How many IP addresses are left in the pool to be assigned to other hosts?**

- 58
- **48**
- 50
- 61
- 40

**63. The address pool of a DHCP server is configured with 10.7.30.0/24. The network administrator reserves 5 IP addresses for printers. How many IP addresses are left in the pool to be assigned to other hosts?**

- 253
- 239
- **249**
- 250
- 247

**Explain:** Calculate the maximum number of hosts available for the slash value and subtract the required static IP addresses required for the devices.  
/24 = 254 hosts  
/25 = 126 hosts  
/26 = 62 hosts  
/27 = 30 hosts  
/28 = 14 hosts

**64. Which FHRP implementation is a nonproprietary IPv4-only election protocol with limited scalability?**

- **VRRPv2**
- GLBP
- GLBP for IPv6
- IRDP

**65. The address pool of a DHCP server is configured with 192.168.184.0/26. The network administrator reserves 18 IP addresses for access points. How many IP addresses are left in the pool to be assigned to other hosts?**

- 57
- **44**
- 54
- 36
- 46

**66. The address pool of a DHCP server is configured with 10.19.44.0/24. The network administrator reserves 3 IP addresses for servers. How many IP addresses are left in the pool to be assigned to other hosts?**

- 255
- 252
- 241
- **251**
- 249

**67. The address pool of a DHCP server is configured with 10.19.44.0/24. The network administrator reserves 6 IP addresses for servers. How many IP addresses are left in the pool to be assigned to other hosts?**

- 246
- 252
- 249
- **248**
- 238

**68. The address pool of a DHCP server is configured with 172.21.121.0/25. The network administrator reserves 12 IP addresses for web servers. How many IP addresses are left in the pool to be assigned to other hosts?**

- 115
- **114**
- 118
- 104
- 112

**Explanation:** Calculate the maximum number of hosts available for the slash value and subtract the required static IP addresses required for the devices.  
/24 = 254 hosts  
/25 = 126 hosts  
/26 = 62 hosts  
/27 = 30 hosts  
/28 = 14 hosts

**69. Which kind of message is sent by a DHCP client when its IP address lease is about to expire?​**

- a DHCPREQUEST broadcast message​
- a DHCPDISCOVER unicast message​
- a DHCPDISCOVER broadcast message
- a DHCPREQUEST unicast message​