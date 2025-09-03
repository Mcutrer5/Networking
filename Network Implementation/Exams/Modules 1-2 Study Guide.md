#### Modules 1 – 2 of the CCNA3 – Enterprise Networking, Security, and Automation (ENSA) v7.0

**1. What is a function of OSPF hello packets?**

- to send specifically requested link-state records
- **to discover neighbors and build adjacencies between them**
- to ensure database synchronization between routers
- to request specific link-state records from neighbor routers

**2. Which OSPF packet contains the different types of link-state advertisements?**

- hello
- DBD
- LSR
- **LSU**
- LSAck

**3. Which three statements describe features of the OSPF topology table? (Choose three.)**

- **It is a link-state database that represents the network topology.**
- Its contents are the result of running the SPF algorithm.
- **When converged, all routers in an area have identical topology tables.**
- The topology table contains feasible successor routes.
- **The table can be viewed via the show ip ospf database command.**
- After convergence, the table only contains the lowest cost route entries for all known networks.

**Explanation:** The topology table on an OSPF router is a link-state database (LSDB) that lists information about all other routers in the network, and represents the network topology. All routers within an area have identical link-state databases, and the table can be viewed using the show ip ospf database command. The EIGRP topology table contains feasible successor routes. This concept is not used by OSPF. The SPF algorithm uses the LSDB to produce the unique routing table for each router which contains the lowest cost route entries for known networks.

**4. What does an OSPF area contain?**

- routers that share the same router ID
- routers whose SPF trees are identical
- **routers that have the same link-state information in their LSDBs**
- routers that share the same process ID

**Explanation:** An OSPF area contains one set of link-state information, although each router within the area will process that information individually to form its own SPF tree. OSPF process IDs are locally significant and are created by the administrator. Router IDs uniquely identify each router.

  
**5.** **What is used to facilitate hierarchical routing in OSPF?**

- **the use of multiple areas**
- frequent SPF calculations
- autosummarization
- the election of designated routers

**Explanation:** OSPF supports the concept of areas to prevent larger routing tables, excessive SPF calculations, and large LSDBs. Only routers within an area share link-state information. This allows OSPF to scale in a hierarchical fashion with all areas that connect to a backbone area.

**6. Which OSPF data structure is identical on all OSPF routers that share the same area?**

- forwarding database
- **link-state database**
- adjacency database
- routing table

**Explanation:** Regardless of which OSPF area a router resides in, the adjacency database, routing table, and forwarding database are unique for each router. The link-state database lists information about all other routers within an area and is identical across all OSPF routers participating in that area.

**7. Which step does an OSPF-enabled router take immediately after establishing an adjacency with another router?**

- builds the topology table
- **exchanges link-state advertisements**
- chooses the best path
- executes the SPF algorithm

**Explanation:** The OSPF operation steps are as follows:

1. Establish neighbor adjacencies
2. Exchange link-state advertisements
3. Build the topology table
4. Execute the SPF algorithm
5. Choose the best route
    

**8. A network engineer has manually configured the hello interval to 15 seconds on an interface of a router that is running OSPFv2. By default, how will the dead interval on the interface be affected?**

- The dead interval will not change from the default value.
- The dead interval will now be 30 seconds.
- **The dead interval will now be 60 seconds.**
- The dead interval will now be 15 seconds.

**Explanation:** Cisco IOS automatically modifies the dead interval to four times the hello interval.

**9. Refer to the exhibit. A network administrator has configured the OSPF timers to the values that are shown in the graphic. What is the result of having those manually configured timers?**

![](https://itexamanswers.net/wp-content/uploads/2020/05/i212851v1n1_212851.png)

- R1 automatically adjusts its own timers to match the R2 timers.
- **The R1 dead timer expires between hello packets from R2.**
- The hello timer on R2 expires every ten seconds.
- The neighbor adjacency has formed.

**Explanation:** The dead timer (20 seconds) on R1 expires before the next hello packet from R2 (25 seconds).

**10. To establish a neighbor adjacency two OSPF routers will exchange hello packets. Which two values in the hello packets must match on both routers? (Choose two.)**

- **dead interval**
- router priority
- list of neighbors
- router ID
- **hello interval**

**Explanation:** The hello and dead interval timers contained in a hello packet must be the same on neighboring routers in order to form an adjacency.

**11. What is the default router priority value for all Cisco OSPF routers?**

- 0
- **1**
- 10
- 255

**Explanation:** The router priority value is used in a DR/BDR election. The default priority for all OSPF routers is 1 but it can be manually altered to any value 0 to 255.

**12. Which type of OSPFv2 packet contains an abbreviated list of the LSDB of a sending router and is used by receiving routers to check against the local LSDB?**

- **database description**
- link-state update
- link-state request
- link-state acknowledgment

**Explanation:** The database description (DBD) packet contains an abbreviated list of the LSDB sent by a neighboring router and is used by receiving routers to check against the local LSDB.

**13. In an OSPF network when are DR and BDR elections required?**

- when the two adjacent neighbors are interconnected over a point-to-point link
- when all the routers in an OSPF area cannot form adjacencies
- **when the routers are interconnected over a common Ethernet network**
- when the two adjacent neighbors are in two different networks

**Explanation:** When the routers are interconnected over a common Ethernet network, then a designated router (DR) and a backup DR (BDR) must be elected.

**14. When an OSPF network is converged and no network topology change has been detected by a router, how often will LSU packets be sent to neighboring routers?**

- every 5 minutes
- every 10 minutes
- **every 30 minutes**
- every 60 minutes

**Explanation:** After all LSRs have been satisfied for a given router, the adjacent routers are considered synchronized and in a full state. Updates (LSUs) are sent to neighbors only under the following conditions:

- when a network topology change is detected (incremental updates)
- every 30 minutes
    

**15. What will an OSPF router prefer to use first as a router ID?**

- a loopback interface that is configured with the highest IP address on the router
- **any IP address that is configured using the router-id command**
- the highest active interface IP that is configured on the router
- the highest active interface that participates in the routing process because of a specifically configured network statement

**Explanation:** The first preference for an OSPF router ID is an explicitly configured 32-bit address. This address is not included in the routing table and is not defined by the **network** command. If a router ID that is configured through the **router-id** command is not available, OSPF routers next use the highest IP address available on a loopback interface, as loopbacks used as router IDs are also not routable addresses. Lacking either of these alternatives, an OSPF router will use the highest IP address from its active physical interfaces.

**16. What are the two purposes of an OSPF router ID? (Choose two.)**

- **to uniquely identify the router within the OSPF domain**
- **to facilitate router participation in the election of the designated router**
- to enable the SPF algorithm to determine the lowest cost path to remote networks
- to facilitate the establishment of network convergence
- to facilitate the transition of the OSPF neighbor state to Full

**Explanation:** OSPF router ID does not contribute to SPF algorithm calculations, nor does it facilitate the transition of the OSPF neighbor state to Full. Although the router ID is contained within OSPF messages when router adjacencies are being established, it has no bearing on the actual convergence process.

**17. Refer to the exhibit. If no router ID was manually configured, what would router Branch1 use as its OSPF router ID?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i254793v1n2_254793.gif)

- 10.0.0.1
- 10.1.0.1
- **192.168.1.100**
- 209.165.201.1

**Explanation:** In OSPFv2, a Cisco router uses a three-tier method to derive its router ID. The first choice is the manually configured router ID with the **router-id** command. If the router ID is not manually configured, the router will choose the highest IPv4 address of the configured loopback interfaces. Finally if no loopback interfaces are configured, the router chooses the highest active IPv4 address of its physical interfaces.

**18. A network technician issues the following commands when configuring a router:**

R1(config)# router ospf 11 
R1(config-router)# network 10.10.10.0 0.0.0.255 area 0

**What does the number 11 represent?**

- **the OSPF process ID on R1**
- the cost of the link to R1
- the autonomous system number to which R1 belongs
- the administrative distance that is manually assigned to R1
- the area number where R1 is located

**Explanation:** There is no autonomous system number to configure on OSPF. The area number is located at the end of the network statement. The cost of a link can be modified in the interface configuration mode. The process ID is local to the router.

**19. An OSPF router has three directly connected networks; 172.16.0.0/16, 172.16.1.0/16, and 172.16.2.0/16. Which OSPF network command would advertise only the 172.16.1.0 network to neighbors?**

- router(config-router)# network 172.16.1.0 0.0.255.255 area 0
- router(config-router)# network 172.16.0.0 0.0.15.255 area 0
- **router(config-router)# network 172.16.1.0 255.255.255.0 area 0**
- router(config-router)# network 172.16.1.0 0.0.0.0 area 0

**Explanation:** To advertise only the 172.16.1.0/16 network the wildcard mask used in the network command must match the first 16-bits exactly. To match bits exactly, a wildcard mask uses a binary zero. This means that the first 16-bits of the wildcard mask must be zero. The low order 16-bits can all be set to 1.

**20. Refer to the exhibit. Which three statements describe the results of the OSPF election process of the topology that is shown in the exhibit? (Choose three.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i212853v1n1_212853.png)

- **R3 will be elected BDR.**
- The R4 FastEthernet 0/0 priority is 128.
- **The R4 router ID is 172.16.1.1.**
- R1 will be elected BDR.
- The router ID on R2 is the loopback interface.
- **R2 will be elected DR.**

**Explanation:** R2 will be elected DR because it has the highest priority of 255, all of the others have a priority of 1. R3 will be elected BDR because it has the numerically highest router-ID of 192.168.1.4. The R4 router-ID is 172.16.1.1 because it is the IPv4 address attached to the loopback 0 interface.

**21. Refer to the exhibit. If the switch reboots and all routers have to re-establish OSPF adjacencies, which routers will become the new DR and BDR?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i255836v1n1_255836.gif)

- **Router R4 will become the DR and router R1 will become the BDR.**
- Router R2 will become the DR and router R3 will become the BDR.
- Router R1 will become the DR and router R2 will become the BDR.
- Router R4 will become the DR and router R3 will become the BDR.

**Explanation:** OSPF elections of a DR are based on the following in order of precedence:

- highest pritority from 1 -255 (0 = never a DR)
- highest router ID
- highest IP address of a loopback or active interface in the absence of a manually configured router ID. Loopback IP addresses take higher precedence than other interfaces.

In this case routers R4 and R1 have the highest router priority. Between the two, R3 has the higher router ID. Therefore, R4 will become the DR and R1 will become the BDR.

**22. By default, what is the OSPF cost for any link with a bandwidth of 100 Mb/s or greater?**

- 100000000
- 10000
- **1**
- 100

**Explanation:** OSPF uses the formula: Cost = 100,000,000 / bandwidth. Because OSPF will only use integers as cost, any bandwidth of 100 Mb/s or greater will all equal a cost of 1.

**23. Refer to the exhibit. What is the OSPF cost to reach the router A LAN 172.16.1.0/24 from B?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i258065v1n1_Item-isomorph-258065.png)

- 782
- 74
- 128
- **65**

**Explanation:** The formula used to calculate the OSPF cost is as follows:

Cost = reference bandwidth / interface bandwidth

The default reference bandwidth is 10^8 (100,000,000); therefore, the formula is

Cost = 100,000,000 bps / interface bandwidth in bps

Thus the cost to reach the A LAN 172.16.1.0/24 from B is as follows:  
Serial link (1544 Kbps) from B to A cost => 100,000,000 / 1,544,000 = 64  
Gigabit Ethernet link on A cost => 100,000,000 / 1,000,000,000 = 1  
Total cost to reach 172.16.1.0/24 = 64 + 1 = 65

**24. Refer to the exhibit. On which router or routers would a default route be statically configured in a corporate environment that uses single area OSPF as the routing protocol?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i269030v1n1_ScalNch5.png)

- **R0-A**
- ISP, R0-A, R0-B, and R0-C
- ISP
- R0-B and R0-C
- ISP and R0-A
- R0-A, R0-B, and R0-C

**Explanation:** The default route is applied to the router that connects to the Internet, or R0-A. R0-A then distributes that default route using the OSPF routing protocol.

**25. What command would be used to determine if a routing protocol-initiated relationship had been made with an adjacent router?**

- ping
- **show ip ospf neighbor**
- show ip interface brief
- show ip protocols

**Explanation:** While the **show ip interface brief** and **ping** commands can be used to determine if Layer 1, 2, and 3 connectivity exists, neither command can be used to determine if a particular OSPF or EIGRP-initiated relationship has been made. The **show ip protocols** command is useful in determining the routing parameters such as timers, router ID, and metric information associated with a specific routing protocol. The **show ip ospf neighbor** command shows if two adjacent routers have exchanged OSPF messages in order to form a neighbor relationship.

**26. Refer to the exhibit. Which command did an administrator issue to produce this output?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i278236v1n1_212843.jpg)

- **R1# show ip ospf interface serial0/0/1**
- R1# show ip route ospf
- R1# show ip ospf
- R1# show ip ospf neighbor

**27. Which command is used to verify that OSPF is enabled and also provides a list of the networks that are being advertised by the network?​**

- show ip interface brief
- show ip ospf interface
- **show ip protocols**
- show ip route ospf

**Explanation:** The command **show ip ospf interface** verifies the active OSPF interfaces. The command **show ip interface brief** is used to check that the interfaces are operational. The command **show ip route ospf** displays the entries that are learned via OSPF in the routing table. The command **show ip protocols** checks that OSPF is enabled and lists the networks that are advertised.

**28. Refer to the exhibit. A network administrator has configured OSPFv2 on the two Cisco routers but PC1 is unable to connect to PC2. What is the most likely problem?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i285134v1n1_285134.png)

- **Interface Fa0/0 has not been activated for OSPFv2 on router R2.**
- Interface Fa0/0 is configured as a passive-interface on router R2.
- Interface S0/0 is configured as a passive-interface on router R2.
- Interface s0/0 has not been activated for OSPFv2 on router R2.

**Explanation:** If a LAN network is not advertised using OSPFv2, a remote network will not be reachable. The output displays a successful neighbor adjacency between router R1 and R2 on the interface S0/0 of both routers.

**29. What is the recommended Cisco best practice for configuring an OSPF-enabled router so that each router can be easily identified when troubleshooting routing issues?**

- **Configure a value using the router-id command.**
- Use the highest active interface IP address that is configured on the router.
- Use a loopback interface configured with the highest IP address on the router.
- Use the highest IP address assigned to an active interface participating in the routing process.

**Explanation:** A Cisco router is assigned a router ID to uniquely identify it. It can be automatically assigned and take the value of the highest configured IP address on any interface, the value of a specifically-configured loopback address, or the value assigned (which is in the exact form of an IP address) using the **router-id** command. Cisco recommends using the **router-id** command.

**30. Which step in the link-state routing process is described by a router running an algorithm to determine the best path to each destination?**

- load balancing equal-cost paths
- declaring a neighbor to be inaccessible
- choosing the best route
- **executing the SPF algorithm**

**31. An administrator is configuring single-area OSPF on a router. One of the networks that must be advertised is 192.168.223.0 255.255.254.0. What wildcard mask would the administrator use in the OSPF network statement?**

- **0.0.1.255**
- 0.0.7.255
- 0.0.15.255
- 0.0.31.255

**32. What is the format of the router ID on an OSPF-enabled router?**

- a unique router host name that is configured on the router
- a unique phrase with no more than 16 characters
- **a 32-bit number formatted like an IPv4 address**
- an 8-bit number with a decimal value between 0 and 255
- a character string with no space

**Explanation:** A router ID is a 32-bit number formatted like an IPv4 address and assigned in order to uniquely identify a router among OSPF peers.

**33. Question as presented:**

DUAL is the algorithm used by EIGRP. In multiarea OSPF, OSPF is implemented using multiple areas, and all of them must be connected to the backbone area.

**34. After modifying the router ID on an OSPF router, what is the preferred method to make the new router ID effective?**

- HQ# copy running-config startup-config
- HQ# resume
- HQ# clear ip route *
- **HQ# clear ip ospf process**

**Explanation:** To modify a router-id on an OSPF-enabled router, it is necessary to reset the OSPF routing process by entering either the **clear ip ospf process** command or **the reload** command.

**35. In an OSPFv2 configuration, what is the effect of entering the command network 192.168.1.1 0.0.0.0 area 0 ?**

- It allows all 192.168.1.0 networks to be advertised.
- **It tells the router which interface to turn on for the OSPF routing process.**
- It changes the router ID of the router to 192.168.1.1.
- It enables OSPF on all interfaces on the router.

**Explanation:** Entering the command **network 192.168.1.1 0.0.0.0 area 0** will turn on only the interface with that IP address for OSPF routing. It does not change the router ID. Instead, OSPF will use the network that is configured on that interface.

**36. What is the reason for a network engineer to alter the default reference bandwidth parameter when configuring OSPF?**

- to force that specific link to be used in the destination route
- **to more accurately reflect the cost of links greater than 100 Mb/s**
- to enable the link for OSPF routing
- to increase the speed of the link

**Explanation:** By default, Fast Ethernet, Gigabit, and 10 Gigabit Ethernet interfaces all have a cost of 1. Altering the default reference bandwidth alters the cost calculation, allowing each speed to be more accurately reflected in the cost.

**37. Open the PT Activity. Perform the tasks in the activity instructions and then answer the question.**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/2020-06-19_085822.jpg)  
**Which task has to be performed on Router 1 for it to establish an OSPF adjacency with Router 2?**

- Issue the clear ip ospf process command.
- **Change the subnet mask of interface FastEthernet 0/0 to 255.255.255.0.**
- Remove the passive interface command from interface FastEthernet 0/0.
- Add the network 10.0.1.0 0.0.0.255 area 0 command to the OSPF process.

![Icon](data:image/svg+xml;base64,CiAgICAgICAgICAgIDxzdmcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB2aWV3Qm94PSIwIDAgNDAgNDAiPgogICAgICAgICAgICAgICAgPGRlZnM+CiAgICAgICAgICAgICAgICAgICAgPGxpbmVhckdyYWRpZW50IGlkPSJncmFkaWVudCIgeDE9IjAiIHkxPSIwIiB4Mj0iMCIgeTI9IjEiPgogICAgICAgICAgICAgICAgICAgICAgICA8c3RvcCBzdG9wLWNvbG9yPSIjMjY5ZGVmIiBvZmZzZXQ9IjAiLz4KICAgICAgICAgICAgICAgICAgICAgICAgPHN0b3Agc3RvcC1jb2xvcj0iIzI2YmRlZiIgb2Zmc2V0PSIxIi8+CiAgICAgICAgICAgICAgICAgICAgPC9saW5lYXJHcmFkaWVudD4KICAgICAgICAgICAgICAgIDwvZGVmcz4KICAgICAgICAgICAgICAgIDxnPgogICAgICAgICAgICAgICAgICAgIDxyZWN0IGZpbGw9InVybCgjZ3JhZGllbnQpIiB4PSIwIiB5PSIwIiB3aWR0aD0iNDAiIGhlaWdodD0iNDAiIHJ4PSIzIiByeT0iMyIvPgogICAgICAgICAgICAgICAgICAgIDx0ZXh0IHg9IjUiIHk9IjE5IiBmb250LWZhbWlseT0iQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZiIgZm9udC1zaXplPSIxM3B4IiBsZXR0ZXItc3BhY2luZz0iMSIgZmlsbD0iI0ZGRkZGRiI+CiAgICAgICAgICAgICAgICAgICAgICAgIDx0c3Bhbj5QS1Q8L3RzcGFuPgogICAgICAgICAgICAgICAgICAgICAgICA8dHNwYW4geD0iNiIgeT0iMjgiPl88L3RzcGFuPgogICAgICAgICAgICAgICAgICAgIDwvdGV4dD4KICAgICAgICAgICAgICAgIDwvZz4KICAgICAgICAgICAgPC9zdmc+CgoJCQk=)

### [Modules 1 – 2: OSPF Concepts and Configuration Packet Tracer](https://itexamanswers.net/download/modules-1-2-ospf-concepts-and-configuration-packet-tracer) 40.09 KB 10007 downloads

...

  

**Explanation:** Each interface on the link connecting the OSPF routers must be in the same subnet for an adjacency to be established. The IP address subnet mask on FastEthernet interface 0/0 must be changed to 255.255.255.0. The FastEthernet interface 0/0 is not passive. The 10.0.1.0/24 network is only connected to Router2 so should not be advertised by Router1. The **clear ip ospf process** command will start the OPSF process on Router1 but will not cause an adjacency to be established if the subnet mask mismatch on the connecting interfaces still exists.

**38. Match the description to the term. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-09_135501.jpg)

|   |   |
|---|---|
|This is the algorithm used by OSPF.|Shortest Path First|
|This is where the details of the neighboring routers can be found.|Adjacency database|
|All the routers are in the backbone area.|Single-area OSPF|
|This is where you can find the topology table.|Link-state database|

**Explanation:** DUAL is the algorithm used by EIGRP. In multiarea OSPF, OSPF is implemented using multiple areas, and all of them must be connected to the backbone area.

**39. What is a benefit of multiarea OSPF routing?**

- **Topology changes in one area do not cause SPF recalculations in other areas.**
- Routers in all areas share the same link-state database and have a complete picture of the entire network.
- A backbone area is not required.
- Automatic route summarization occurs by default between areas.

**Explanation:** With multiarea OSPF, only routers within an area share the same link-state database. Changes to the network topology in one area do not impact other areas, which reduces the number of SPF algorithm calculations and the of link-state databases.

**40. Match the OSPF state with the order in which it occurs. (Not all options are used.)**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/2025-02-12_111248.jpg)

**Explanation:** The active and passive states are used by EIGRP.  
Place the options in the following order:

|   |   |
|---|---|
|second state|Init state|
|seventh state|Full state|
|fifth state|Exchange state|
|first state|Down state|
|fourth state|Exstart state|
|third state|Two-way state|
|sixth state|Loading state|

**41. What indicates to a link-state router that a neighbor is unreachable?**

- **if the router no longer receives hello packets**
- if the router receives an update with a hop count of 16
- if the router receives an LSP with previously learned information
- if the router no longer receives routing updates

**Explanation:** OSPF routers send hello packets to monitor the state of a neighbor. When a router stops receiving hello packets from a neighbor, that neighbor is considered unreachable and the adjacency is broken.

**42. Which three OSPF states are involved when two routers are forming an adjacency? (Choose three.)**

- Exchange
- **Init**
- ExStart
- **Two-way**
- Loading
- **Down**

**Explanation:** OSPF operation progresses through 7 states for establishing neighboring router adjacency, exchanging routing information, calculating the best routes, and reaching convergence. The Down, Init, and Two-way states are involved in the phase of neighboring router adjacency establishment.

**43. Refer to the exhibit. Suppose that routers B, C, and D have a default priority, and router A has a priority 0. Which conclusion can be drawn from the DR/BDR election process?​**

![CCNA 3 v7 Modules 1 - 2: OSPF Concepts and Configuration Exam](https://itexamanswers.net/wp-content/uploads/2019/12/i247460v1n3_Item-247460.png)

CCNA 3 v7 Modules 1 – 2: OSPF Concepts and Configuration Exam

- If the priority of router C is changed to 255, then it will become the DR.
- Router A will become the DR and router D will become the BDR.​
- **If the DR fails, the new DR will be router B.**
- If a new router with a higher priority is added to this network, it will become the DR.

**Explanation:** If the priority is set to 0, the router is not capable of becoming the DR, so router A cannot be the DR. OSPF DR and BDR elections are not preemptive. If a new router with a higher priority or higher router ID is added to the network after the DR and BDR election, the newly added router does not take over the DR or the BDR role.​

**44. An administrator is configuring single-area OSPF on a router. One of the networks that must be advertised is 64.102.0.0 255.255.255.128. What wildcard mask would the administrator use in the OSPF network statement?**

- 0.0.31.255
- 0.0.0.63
- 0.0.63.255
- **0.0.0.127**

**45. Which command will a network engineer issue to verify the configured hello and dead timer intervals on a point-to-point WAN link between two routers that are running OSPFv2?**

- show ipv6 ospf interface serial 0/0/0
- show ip ospf neighbor
- show ip ospf interface fastethernet 0/1
- **show ip ospf interface serial 0/0/0**

The show ip ospf interface serial 0/0/0 command will display the configured hello and dead timer intervals on a point-to-point serial WAN link between two OSPFv2 routers. The show ipv6 ospf interface serial 0/0/0 command will display the configured hello and dead timer intervals on a point-to-point serial link between two OSPFv3 routers. The show ip ospf interface fastethernet 0/1 command will display the configured hello and dead timer intervals on a multiaccess link between two (or more) OSPFv2 routers. The show ip ospf neighbor command will display the dead interval elapsed time since the last hello message was received, but does not show the configured value of the timer.  

  
**46. An administrator is configuring single-area OSPF on a router. One of the networks that must be advertised is 128.107.0.0 255.255.255.192. What wildcard mask would the administrator use in the OSPF network statement?**

- 0.0.63.255
- **0.0.0.63**
- 0.0.0.3
- 0.0.0.7

**47. Match each OSPF packet type to how it is used by a router. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-09_134235.jpg)

|   |   |
|---|---|
|link-state request packet|query another router for additional information|
|hello packet|establish and maintain adjacencies|
|database description packet|compare local topology to that sent by another router|
|link-state update packet|advertise new information|

**48. An administrator is configuring single-area OSPF on a router. One of the networks that must be advertised is 192.168.181.0 255.255.254.0. What wildcard mask would the administrator use in the OSPF network statement?**

- .0.63.255
- 0.0.15.255
- **0.0.1.255**
- 0.0.31.255

**49. An administrator is configuring single-area OSPF on a router. One of the networks that must be advertised is 198.19.0.0 255.255.252.0. What wildcard mask would the administrator use in the OSPF network statement?**

- 0.0.63.255
- **0.0.3.255**
- 0.0.31.255
- 0.0.0.255

**50. An administrator is configuring single-area OSPF on a router. One of the networks that must be advertised is 128.107.0.0 255.255.252.0. What wildcard mask would the administrator use in the OSPF network statement?**

- **0.0.3.255**
- 0.0.0.7
- 0.0.0.3
- 0.0.63.255

**51. Which step in the link-state routing process is described by a router flooding link-state and cost information about each directly connected link?**

- building the topology table
- selecting the router ID
- **exchanging link-state advertisements**
- injecting the default route

**52. Which step in the link-state routing process is described by a router sending Hello packets out all of the OSPF-enabled interfaces?**

- electing the designated router
- **establishing neighbor adjacencies**
- injecting the default route
- exchanging link-state advertisements

**53. An administrator is configuring single-area OSPF on a router. One of the networks that must be advertised is 64.100.0.0 255.255.255.0. What wildcard mask would the administrator use in the OSPF network statement?**

- 0.0.0.31
- **0.0.0.255**
- 0.0.0.63
- 0.0.0.127

**54. Which step in the link-state routing process is described by a router inserting best paths into the routing table?**

- declaring a neighbor to be inaccessible
- executing the SPF algorithm
- load balancing equal-cost paths
- **choosing the best route**

**55. What type of address is 64.101.198.197?**

- **public**
- private

**56. An OSPF router has three directly connected networks; 172.16.0.0/24, 172.16.1.0/24, and 172.16.2.0/24. Which OSPF network command would advertise only the 172.16.1.0 network to neighbors?**

- router(config-router)# network 172.16.1.0 0.0.255.255 area 0
- router(config-router)# network 172.16.0.0 0.0.15.255 area 0
- **router(config-router)# network 172.16.1.0 0.0.0.255 area 0**
- router(config-router)# network 172.16.1.0 0.0.0.0 area 0

**Explanation:** To advertise only the 172.16.1.0/24 network the wildcard mask used in the network command must match the first 24-bits exactly. To match bits exactly, a wildcard mask uses a binary zero. This means that the first 24-bits of the wildcard mask must be zero. The low order 8-bits can all be set to 1.

**57. Which step in the link-state routing process is described by a router building a link-state database based on received LSAs?**

- selecting the router ID
- declaring a neighbor to be inaccessible
- executing the SPF algorithm
- **building the topology table**