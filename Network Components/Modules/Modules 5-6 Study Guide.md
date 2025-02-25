**1. What additional information is contained in the 12-bit extended system ID of a BPDU?**

- MAC address
- **VLAN ID**
- IP address
- port ID

**2. During the implementation of Spanning Tree Protocol, all switches are rebooted by the network administrator. What is the first step of the spanning-tree election process?**

- Each switch with a lower root ID than its neighbor will not send BPDUs.
- **All the switches send out BPDUs advertising themselves as the root bridge.**
- Each switch determines the best path to forward traffic.
- Each switch determines what port to block to prevent a loop from occurring.

**3. Which STP port role is adopted by a switch port if there is no other port with a lower cost to the root bridge?**

- designated port
- **root port**
- alternate
- disabled port

**Explanation:** The root port is the port with the lowest cost to reach the root bridge.

**4. Which two concepts relate to a switch port that is intended to have only end devices attached and intended never to be used to connect to another switch? (Choose two.)**

- bridge ID
- **edge port**
- extended system ID
- **PortFast**
- PVST+

**5. Which three components are combined to form a bridge ID?**

- **extended system ID**
- cost
- IP address
- **bridge priority**
- **MAC address**
- port ID

**Explanation:** The three components that are combined to form a bridge ID are bridge priority, extended system ID, and MAC address.

**6. Match the STP protocol with the correct description. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-08_145807.jpg)  
![](https://itexamanswers.net/wp-content/uploads/2019/12/2020-04-04_153917.jpg)

**7. In which two port states does a switch learn MAC addresses and process BPDUs in a PVST network? (Choose two.)**

- disabled
- **forwarding**
- listening
- blocking
- **learning**

**Explanation:** Switches learn MAC addresses at the learning and forwarding port states. They receive and process BPDUs at the blocking, listening, learning, and forwarding port states.

**8. If no bridge priority is configured in PVST, which criteria is considered when electing the root bridge?**

- **lowest MAC address**
- lowest IP address
- highest IP address
- highest MAC address

**Explanation:** Only one switch can be the root bridge for a VLAN. The root bridge is the switch with the lowest BID. The BID is determined by priority and the MAC address. If no priority is configured then all switches use the default priority and the election of the root bridge will be based on the lowest MAC address.

**9. Match the spanning-tree feature with the protocol type. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-08_150524.jpg)  
**Place the options in the following order:**

|   |   |
|---|---|
|PVST|Cisco implementation of IEEE 802.1D|
|RSTP|Fast converging enhancement of IEEE 802.1D|
|MSTP|IEEE standard that reduces the number of STP instances|
|MST|Proprietary per VLAN implementation of IEEE 802.1w|
|Rapid PVST+|an evolution of STP that provides faster convergence|

**10. When the show spanning-tree vlan 33 command is issued on a switch, three ports are shown in the forwarding state. In which two port roles could these interfaces function while in the forwarding state? (Choose two.)**

- alternate
- **designated**
- disabled
- blocked
- **root**

**Explanation:** The role of each of the three ports will be either designated port or root port. Ports in the disabled state are administratively disabled. Ports in the blocking state are alternate ports.

**11. What is the function of STP in a scalable network?**

- It decreases the size of the failure domain to contain the impact of failures.
- It protects the edge of the enterprise network from malicious activity.
- It combines multiple switch trunk links to act as one logical link for increased bandwidth.
- **It disables redundant paths to eliminate Layer 2 loops.**

**Explanation:** STP is an important component in a scalable network because it allows redundant physical connections between Layer 2 devices to be implemented without creating Layer 2 loops. STP prevents Layer 2 loops from forming by disabling interfaces on Layer 2 devices when they would create a loop.

**12. What is a characteristic of spanning tree?**

- **It is enabled by default on Cisco switches.**
- It is used to discover information about an adjacent Cisco device.
- It has a TTL mechanism that works at Layer 2.
- It prevents propagation of Layer 2 broadcast frames.

**Explanation:** Spanning tree does work at Layer 2 on Ethernet-based networks and is enabled by default, but it does not have a TTL mechanism. Spanning tree exists because Layer 2 frames do not have a TTL mechanism. Layer 2 frames are still broadcast when spanning tree is enabled, but the frames can only be transmitted through a single path through the Layer 2 network that was created by spanning tree. Cisco Discovery Protocol (CDP) is used to discover information about an adjacent Cisco device.

**13. Which spanning tree standard supports only one root bridge so that traffic from all VLANs flows over the same path?**

- PVST+
- **802.1D**
- MST
- Rapid PVST

**Explanation:** MST is the Cisco implementation of MSTP, an IEEE standard protocol that provides up to 16 instances of RSTP. PVST+ provides a separate 802.1D spanning-tree instance for each VLAN that is configured in the network. 802.1D is the original STP standard defined by the IEEE and allows for only one root bridge for all VLANs. 802.1w, or RSTP, provides faster convergence but still uses only one STP instance for all VLANs.

**14. What is the purpose of the Spanning Tree Protocol (STP)?**

- creates smaller collision domains
- prevents routing loops on a router
- **prevents Layer 2 loops**
- allows Cisco devices to exchange routing table updates
- creates smaller broadcast domains

**Explanation:** The Spanning-Tree Protocol (STP) creates one path through a switch network in order to prevent Layer 2 loops.

**15. What is the value used to determine which port on a non-root bridge will become a root port in a STP network?**

- **the path cost**
- the highest MAC address of all the ports in the switch
- the lowest MAC address of all the ports in the switch
- the VTP revision number

**Explanation:** STP establishes one root port on each non-root bridge. The root port is the lowest-cost path from the non-root bridge to the root bridge, indicating the direction of the best path to the root bridge. This is primarily based on the path cost to the root bridge.

**16. Refer to the exhibit. Which switch will be the root bridge after the election process is complete?**

![CCNA-2-v7-Modules 5 - 6 Redundant Networks Exam 10](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA-2-v7-Modules-5-6-Redundant-Networks-Exam-10.png)

- S1
- **S2**
- S3
- S4

**Explanation:** The root bridge is determined by the lowest bridge ID, which consists of the priority value and the MAC address. Because the priority values of all of the switches are identical, the MAC address is used to determine the root bridge. Because S2 has the lowest MAC address, S2 becomes the root bridge.

**17. What are two drawbacks to turning spanning tree off and having multiple paths through the Layer 2 switch network? (Choose two.)**

- **The MAC address table becomes unstable.**
- The switch acts like a hub.
- Port security becomes unstable.
- **Broadcast frames are transmitted indefinitely.**
- Port security shuts down all of the ports that have attached devices.

**Explanation:** Spanning tree should never be disabled. Without it, the MAC address table becomes unstable, broadcast storms can render network clients and the switches unusable, and multiple copies of unicast frames can be delivered to the end devices.

**18. A small company network has six interconnected Layer 2 switches. Currently all switches are using the default bridge priority value. Which value can be used to configure the bridge priority of one of the switches to ensure that it becomes the root bridge in this design?**

- 1
- **28672**
- 32768
- 34816
- 61440

**Explanation:** The default bridge priority value for all Cisco switches is 32768. The range is 0 to 61440 in increments of 4096. Thus, the values 1 and 34816 are invalid. Configuring one switch with the lower value of 28672 (and leaving the bridge priority value of all other switches unchanged) will make the switch become the root bridge.

**19. Refer to the exhibit. The administrator tried to create an EtherChannel between S1 and the other two switches via the commands that are shown, but was unsuccessful. What is the problem?**

![CCNA-2-v7-Modules 5 - 6 Redundant Networks Exam 19](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA-2-v7-Modules-5-6-Redundant-Networks-Exam-19.png)

- **Traffic cannot be sent to two different switches through the same EtherChannel link.**
- Traffic cannot be sent to two different switches, but only to two different devices like an EtherChannel-enabled server and a switch.​
- Traffic can only be sent to two different switches if EtherChannel is implemented on Gigabit Ethernet interfaces.​
- Traffic can only be sent to two different switches if EtherChannel is implemented on Layer 3 switches.​

**Explanation:** An EtherChannel link can only be created between two switches or between an EtherChannel-enabled server and a switch. Traffic cannot be sent to two different switches through the same EtherChannel link.

**20. Which statement is true regarding the use of PAgP to create EtherChannels?**

- It requires full duplex.
- It increases the number of ports that are participating in spanning tree.
- It requires more physical links than LACP does.
- It mandates that an even number of ports (2, 4, 6, etc.) be used for aggregation.
- **It is Cisco proprietary.**

**Explanation:** PAgP is used to automatically aggregate multiple ports into an EtherChannel bundle, but it only works between Cisco devices. LACP can be used for the same purpose between Cisco and non-Cisco devices. PAgP must have the same duplex mode at both ends and can use two ports or more. The number of ports depends on the switch platform or module. An EtherChannel aggregated link is seen as one port by the spanning-tree algorithm.

**21. What are two requirements to be able to configure an EtherChannel between two switches? (Choose two.)**

- **All the interfaces need to work at the same speed.**
- All interfaces need to be assigned to different VLANs.
- Different allowed ranges of VLANs must exist on each end.
- **All the interfaces need to be working in the same duplex mode.**
- The interfaces that are involved need to be contiguous on the switch.

**Explanation:** All interfaces in the EtherChannel bundle must be assigned to the same VLAN or be configured as a trunk. If the allowed range of VLANs is not the same, the interfaces do not form an EtherChannel even when set to auto or desirable mode.

**22. Refer to the exhibit. On the basis of the output that is shown, what can be determined about the EtherChannel bundle?**

![CCNA-2-v7-Modules 5 - 6 Redundant Networks Exam 20](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA-2-v7-Modules-5-6-Redundant-Networks-Exam-20.png)

CCNA-2-v7-Modules 5 – 6 Redundant Networks Exam 22

- The EtherChannel bundle is down.
- Two Gigabit Ethernet ports are used to form the EtherChannel.
- **A Cisco proprietary protocol was used to negotiate the EtherChannel link.**
- The EtherChannel bundle is operating at both Layer 2 and Layer 3.

**Explanation:** Two protocols can be used to send negotiation frames that are used to try to establish an EtherChannel link: PAgP and LACP. PAgP is Cisco proprietary, and LACP adheres to the industry standard.

**23. Which two parameters must match on the ports of two switches to create a PAgP EtherChannel between the switches? (Choose two.)**

- port ID
- PAgP mode
- MAC address
- **speed**
- **VLAN information**

**Explanation:** For an EtherChannel to be created, the ports that are concerned on the two switches must match in terms of the speed, duplex, and VLAN information. The PAgP mode must be compatible but not necessarily equal. The port ID and the MAC addresses do not have to match.

**24. Refer to the exhibit. A network administrator is configuring an EtherChannel link between two switches, SW1 and SW2. Which statement describes the effect after the commands are issued on SW1 and SW2?**

![CCNA-2-v7-Modules 5 - 6 Redundant Networks Exam 21](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA-2-v7-Modules-5-6-Redundant-Networks-Exam-21.png)

CCNA-2-v7-Modules 5 – 6 Redundant Networks Exam 24

- The EtherChannel is established after SW2 initiates the link request.
- The EtherChannel is established after SW1 initiates the link request.
- The EtherChannel is established without negotiation.
- **The EtherChannel fails to establish.**

**Explanation:** The interfaces GigabitEthernet 0/1 and GigabitEthernet 0/2 are configured “on” for the EtherChannel link. This mode forces the interface to channel without PAgP or LACP. The EtherChannel will be established only if the other side is also set to “on”. However, the mode on SW2 side is set to PAgP desirable. Thus the EtherChannel link will not be established.

**25. Refer to the exhibit. A network administrator is configuring an EtherChannel link between two switches, SW1 and SW2. However, the EtherChannel link fails to establish. What change in configuration would correct the problem?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA-2-v7-Modules-5-6-Redundant-Networks-Exam-22.png)

CCNA-2-v7-Modules 5 – 6 Redundant Networks Exam 25

- **Configure SW2 EtherChannel mode to desirable.**
- Configure SW2 EtherChannel mode to on.
- Configure SW1 EtherChannel mode to on.
- Configure SW2 EtherChannel mode to auto.

**Explanation:** The EtherChannel mode must be compatible on each side for the link to work. The three modes from PAgP protocol are on, desirable, and auto. The three modes from LACP protocol are on, active, and passive. The compatible modes include on-on, auto-desirable, desirable-desirable, active-passive, and active-active. Any other combinations will not form an EtherChannel link.

**26. A network administrator configured an EtherChannel link with three interfaces between two switches. What is the result if one of the three interfaces is down?**

- **The remaining two interfaces continue to load balance traffic.**
- The remaining two interfaces become separate links between the two switches.
- One interface becomes an active link for data traffic and the other becomes a backup link.
- The EtherChannel fails.

**Explanation:** EtherChannel creates an aggregation that is seen as one logical link. It provides redundancy because the overall link is one logical connection. The loss of one physical link within the channel does not create a change in the topology; the EtherChannel remains functional.

**27. A network administrator is configuring an EtherChannel link between switches SW1 and SW2 by using the command SW1(config-if-range)# channel-group 1 mode auto. Which command must be used on SW2 to enable this EtherChannel?**

- SW2(config-if-range)# channel-group 1 mode passive
- **SW2(config-if-range)# channel-group 1 mode desirable**
- SW2(config-if-range)# channel-group 1 mode on
- SW2(config-if-range)# channel-group 1 mode active

**Explanation:** The possible combinations to establish an EtherChannel between SW1 and SW2 using LACP or PAgP are as follows:  
PAgP  
on on  
auto desirable  
desirable desirable

LACP  
on on  
active active  
passive active

The EtherChannel mode chosen on each side of the EtherChannel must be compatible in order to enable it.

**28. Which technology is an open protocol standard that allows switches to automatically bundle physical ports into a single logical link?**

- PAgP
- **LACP**
- Multilink PPP
- DTP

**Explanation:** LACP, or Link Aggregation Control Protocol, is defined by IEEE 802.3ad and is an open standard protocol. LACP allows switches to automatically bundle switch ports into a single logical link to increase bandwidth. PAgP, or Port Aggregation Protocol, performs a similar function, but it is a Cisco proprietary protocol. DTP is Dynamic Trunking Protocol and is used to automatically and dynamically build trunks between switches. Multilink PPP is used to load-balance PPP traffic across multiple serial interfaces.

**29. What is a requirement to configure a trunking EtherChannel between two switches?**

- **The allowed range of VLANs must be the same on both switches.**
- The participating interfaces must be assigned the same VLAN number on both switches.
- The participating interfaces must be physically contiguous on a switch.
- The participating interfaces must be on the same module on a switch.

**Explanation:** To enable a trunking EtherChannel successfully, the range of VLANs allowed on all the interfaces must match; otherwise, the EtherChannel cannot be formed. The interfaces involved in an EtherChannel do not have to be physically contiguous, or on the same module. Because the EtherChannel is a trunking one, participating interfaces are configured as trunk mode, not access mode.

**30. What are two advantages of using LACP? (Choose two.)**

- **It allows directly connected switches to negotiate an EtherChannel link.**
- It eliminates the need for configuring trunk interfaces when deploying VLANs on multiple switches.
- It decreases the amount of configuration that is needed on a switch.
- It provides a simulated environment for testing link aggregation.
- **It allows the use of multivendor devices.**
- LACP allows Fast Ethernet and Gigabit Ethernet interfaces to be mixed within a single EtherChannel.

**Explanation:** The Link Aggregation Control Protocol (LACP) allows directly connected multivendor switches to negotiate an EtherChannel link. LACP helps create the EtherChannel link by detecting the configuration of each side and making sure that they are compatible so that the EtherChannel link can be enabled when needed.

**31. A switch is configured to run STP. What term describes a non-root port that is permitted to forward traffic on the network?**

- root port
- **designated port**
- alternate port
- disabled

**32. What are two advantages of EtherChannel? (Choose two.)**

- **Spanning Tree Protocol views the physical links in an EtherChannel as one logical connection.**
- Load balancing occurs between links configured as different EtherChannels.
- **Configuring the EtherChannel interface provides consistency in the configuration of the physical links.**
- Spanning Tree Protocol ensures redundancy by transitioning failed interfaces in an EtherChannel to a forwarding state.
- EtherChannel uses upgraded physical links to provide increased bandwidth.

**Explanation:** EtherChannel configuration of one logical interface ensures configuration consistency across the physical links in the EtherChannel. The EtherChannel provides increased bandwidth using existing switch ports without requiring any upgrades to the physical interfaces. Load balancing methods are implemented between links that are part of the same Etherchannel. Because EtherChannel views the bundled physical links as one logical connection, spanning tree recalculation is not required if one of the bundled physical links fail. If a physical interface fails, STP cannot transition the failed interface into a forwarding state.

**33. Refer to the exhibit. What are the possible port roles for ports A, B, C, and D in this RSTP-enabled network?**

![Modules 5 - 6: Redundant Networks Exam](https://itexamanswers.net/wp-content/uploads/2020/01/CCNA-2-v7-Modules-5-6-Redundant-Networks-Exam.png)

Modules 5 – 6: Redundant Networks Exam 33

- **alternate, designated, root, root**
- designated, alternate, root, root
- alternate, root, designated, root
- designated, root, alternate, root

**Explanation:** Because S1 is the root bridge, B is a designated port, and C and D root ports. RSTP supports a new port type, alternate port in discarding state, that can be port A in this scenario.

**34. Refer to the exhibit. Which switching technology would allow each access layer switch link to be aggregated to provide more bandwidth between each Layer 2 switch and the Layer 3 switch?**

![CCNA-2-v7-Modules 5 - 6 Redundant Networks Exam 02](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA-2-v7-Modules-5-6-Redundant-Networks-Exam-02.png)

CCNA-2-v7-Modules 5 – 6 Redundant Networks Exam 02

- trunking
- HSRP
- PortFast
- **EtherChannel**

**Explanation:** PortFast is used to reduce the amount of time that a port spends going through the spanning-tree algorithm, so that devices can start sending data sooner. Trunking can be implemented in conjunction with EtherChannel, but trunking alone does not aggregate switch links. HSRP is used to load-balance traffic across two different connections to Layer 3 devices for default gateway redundancy. HSRP does not aggregate links at either Layer 2 or Layer 3 as EtherChannel does.

**35. Refer to the exhibit. An administrator wants to form an EtherChannel between the two switches by using the Port Aggregation Protocol. If switch S1 is configured to be in auto mode, which mode should be configured on S2 to form the EtherChannel?**

![CCNA-2-v7-Modules 5 - 6 Redundant Networks Exam 06](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA-2-v7-Modules-5-6-Redundant-Networks-Exam-06.png)

CCNA-2-v7-Modules 5 – 6 Redundant Networks Exam 06

- auto
- on
- off
- **desirable**

**Explanation:** An EtherChannel will be formed via PAgP when both switches are in on mode or when one of them is in auto or desirable mode and the other is in desirable mode.

**36. Open the PT Activity. Perform the tasks in the activity instructions and then answer the question.**  
**Which set of configuration commands issued on SW1 will successfully complete the EtherChannel link between SW1 and SW2?**

![Icon](https://itexamanswers.net/wp-content/plugins/download-manager/assets/file-type-icons/pka.svg)

###### [Modules 5 – 6 Redundant Networks](https://itexamanswers.net/download/modules-5-6-redundant-networks)

1 file(s) 283.11 KB

![CCNA-2-v7-Modules 5 - 6 Redundant Networks Exam 07](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA-2-v7-Modules-5-6-Redundant-Networks-Exam-07.png)

CCNA-2-v7-Modules 5 – 6 Redundant Networks Exam 36

- interface GigabitEthernet0/1  
    no shutdown
- interface Port-channel 1  
    no shutdown
- interface GigabitEthernet0/2  
    channel-group 2 mode desirable
- **interface GigabitEthernet0/1**  
    **channel-group 1 mode desirable**

**Explanation:** Issuing the show running-configuration command on SW1 shows that interface GigabitEthernet0/1 is missing the channel-group 1 mode desirable command which will compete the EtherChannel configuration for interface GigabitEthernet0/1 and interface GigabitEthernet0/2.

**37. A set of switches is being connected in a LAN topology. Which STP bridge priority value will make it least likely for the switch to be selected as the root?**

- 65535
- 4096
- 32768
- **61440**

**Explanation:** The STP bridge priority is a two byte number, but it can only be customized in increments of 4096. The smaller number is preferred, but the largest usable priority value is 61440.

**38. In which two PVST+ port states are MAC addresses learned? (Choose two.)**

- **learning**
- **forwarding**
- disabled
- listening
- blocking

**Explanation:** The two PVST+ port states during which MAC addresses are learned and populate the MAC address table are the learning and the forwarding states.

**39. Which port role is assigned to the switch port that has the lowest cost to reach the root bridge?**

- designated port
- disabled port
- **root port**
- non-designated port

**Explanation:** The root port on a switch is the port with the lowest cost to reach the root bridge.

**40. A switch is configured to run STP. What term describes the switch port closest, in terms of overall cost, to the root bridge?**

- **root port**
- designated port
- alternate port
- disabled

**42. A switch is configured to run STP. What term describes a field used to specify a VLAN ID?**

- **extended system ID**
- port ID
- bridge priority
- bridge ID

**43. A switch is configured to run STP. What term describes the reference point for all path calculations?**

- **root bridge**
- root port
- designated port
- alternate port

**44. A switch is configured to run STP. What term describes a field that has a default value of 32,768 and is the initial deciding factor when electing a root bridge?**

- **bridge priority**
- MAC Address
- extended system ID
- bridge ID

**45. Which statement describes an EtherChannel implementation?**

- EtherChannel operates only at Layer 2.
- PAgP cannot be used in conjunction with EtherChannel.
- **A trunked port can be part of an EtherChannel bundle.**
- EtherChannel can support up to a maximum of ten separate links.

**Explanation:** Up to 16 links can be grouped in an EtherChannel by using the the PAgP or LACP protocol. EtherChannel can be configured as a Layer 2 bundle or a Layer 3 bundle. Configuring a Layer 3 bundle is beyond the scope of this course. If a trunked port is a part of the EtherChannel bundle, all ports in the bundle need to be trunk ports and the native VLAN must be the same on all of these ports. A best practice is to apply the configuration to the port channel interface. The configuration is then automatically applied to the individual ports.

**46. Refer to the exhibit. A network administrator issued the show etherchannel summary command on the switch S1. What conclusion can be drawn?**

![CCNA2 v7 SRWE – Modules 5 – 6 Redundant Networks Exam Answers 46](https://itexamanswers.net/wp-content/uploads/2019/12/i247497v1n1_247497.png)

CCNA2 v7 SRWE – Modules 5 – 6 Redundant Networks Exam Answers

- The EtherChannel is suspended.
- **The EtherChannel is not functional.**
- The port aggregation protocol PAgP is misconfigured.
- FastEthernet ports Fa0/1, Fa0/2, and Fa0/3 do not join the EtherChannel.

**Explanation:** The EtherChannel status shows as (SD), which means it is a Layer 2 EtherChannel with a status of D or down. Because the EtherChannel is down, the status of the interfaces in the channel group is stand-alone. PAgP is configured on S1, but there is no indication whether it is configured correctly on S1. The problem might also be the adjacent switch EtherChannel configuration.

**47. Which statement describes a characteristic of EtherChannel?**

- It can combine up to a maximum of 4 physical links.
- It can bundle mixed types of 100 Mb/s and 1Gb/s Ethernet links.
- It consists of multiple parallel links between a switch and a router.
- **It is made by combining multiple physical links that are seen as one link between two switches.**

**Explanation:** An EtherChannel is formed by combining multiple (same type) Ethernet physical links so they are seen and configured as one logical link. It provides an aggregated link between two switches. Currently each EtherChannel can consist of up to eight compatibly configured Ethernet ports.

**48. Which two channel group modes would place an interface in a negotiating state using PAgP? (Choose two.)**

- on
- **desirable**
- active
- **auto**
- passive

**Explanation:** There are three modes available when configuring an interface for PAgP: on, desirable, and auto. Only desirable and auto place the interface in a negotiating state. The active and passive states are used to configure LACP and not PAgP.

**49. Which mode configuration setting would allow formation of an EtherChannel link between switches SW1 and SW2 without sending negotiation traffic?**

**SW1: on  
SW2: on**

SW1: desirable  
SW2: desirable

SW1: auto  
SW2: auto  
trunking enabled on both switches

SW1: auto  
SW2: auto  
PortFast enabled on both switches

SW1: passive  
SW2: active

**Explanation:** The auto channel-group keyword enables PAgP only if a PAgP device is detected on the opposite side of the link. If the auto keyword is used, the only way to form an EtherChannel link is if the opposite connected device is configured with the desirable keyword. PortFast and trunking technologies are irrelevant to forming an EtherChannel link. Even though an EtherChannel can be formed if both sides are configured in desirable mode, PAgP is active and PAgP messages are being sent constantly across the link, decreasing the amount of bandwidth available for user traffic.

**50. Refer to the exhibit. An EtherChannel was configured between switches S1 and S2, but the interfaces do not form an EtherChannel. What is the problem?**

![CCNA2 v7 SRWE – Modules 5 – 6 Redundant Networks Exam Answers 50](https://itexamanswers.net/wp-content/uploads/2019/12/i216436v1n4_Item-216436.png)

CCNA2 v7 SRWE – Modules 5 – 6 Redundant Networks Exam Answers 50

- The interface port-channel number has to be different on each switch.
- The switch ports were not configured with speed and duplex mode.
- The switch ports have to be configured as access ports with each port having a VLAN assigned.​
- **The EtherChannel was not configured with the same allowed range of VLANs on each interface.**

**51. When EtherChannel is configured, which mode will force an interface into a port channel without exchanging aggregation protocol packets?**

- active
- auto
- **on**
- desirable

**Explanation:** For both LACP and PAgP, the “on” mode will force an interface into an EtherChannel without exchanging protocol packets.

**52. What are two load-balancing methods in the EtherChannel technology? (Choose two.)**

- combination of source port and IP to destination port and IP
- **source IP to destination IP**
- source port to destination port
- combination of source MAC and IP to destination MAC and IP
- **source MAC to destination MAC**

**Explanation:** Depending on the hardware platform, one or more load-balancing methods can be implemented. These methods include source MAC to destination MAC load balancing or source IP to destination IP load balancing, across the physical links.

**53. Which protocol provides up to 16 instances of RSTP, combines many VLANs with the same physical and logical topology into a common RSTP instance, and provides support for PortFast, BPDU guard, BPDU filter, root guard, and loop guard?**

- STP
- Rapid PVST+
- PVST+
- **MST**

**Explanation:** MST is the Cisco implementation of MSTP, an IEEE standard protocol that provides up to 16 instances of RSTP and combines many VLANs with the same physical and logical topology into a common RSTP instance. Each instance supports PortFast, BPDU guard, BPDU filter, root guard, and loop guard. STP and RSTP assume only one spanning-tree instance for the entire bridged network, regardless of the number of VLANs. PVST+ provides a separate 802.1D spanning-tree instance for each VLAN that is configured in the network.

**54. What is the outcome of a Layer 2 broadcast storm?**

- Routers will take over the forwarding of frames as switches become congested.
- **New traffic is discarded by the switch because it is unable to be processed.**
- CSMA/CD will cause each host to continue transmitting frames.
- ARP broadcast requests are returned to the transmitting host.

**Explanation:** When the network is saturated with broadcast traffic that is looping between switches, new traffic is discarded by each switch because it is unable to be processed.

**55. Which two network design features require Spanning Tree Protocol (STP) to ensure correct network operation? (Choose two.)**

- static default routes
- implementing VLANs to contain broadcasts
- **redundant links between Layer 2 switches**
- link-state dynamic routing that provides redundant routes
- **removing single points of failure with multiple Layer 2 switches**

**Explanation:** Spanning Tree Protocol (STP) is required to ensure correct network operation when designing a network with multiple interconnected Layer 2 switches or using redundant links to eliminate single points of failure between Layer 2 switches. Routing is a Layer 3 function and does not relate to STP. VLANs do reduce the number of broadcast domains but relate to Layer 3 subnets, not STP.

**56. A network administrator has configured an EtherChannel between two switches that are connected via four trunk links. If the physical interface for one of the trunk links changes to a down state, what happens to the EtherChannel?**

- Spanning Tree Protocol will transition the failed physical interface into forwarding mode.
- Spanning Tree Protocol will recalculate the remaining trunk links.
- The EtherChannel will transition to a down state.
- **The EtherChannel will remain functional.**

**Explanation:** EtherChannel offers redundancy by bundling multiple trunk links into one logical connection. Failure of one physical link within the EtherChannel will not create a change in the topology and therefore a recalculation by Spanning Tree is unnecessary. Just one physical link must remain operational for the EtherChannel to continue to function.