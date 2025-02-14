**1. Which tasks can be accomplished by using the command history feature? (Choose two.)**

- View a list of commands entered in a previous session.
- Recall up to 15 command lines by default.
- **Set the command history buffer size.**
- **Recall previously entered commands.**
- Save command lines in a log file for future reference.

**Explanation:** The history command allows you to view and reuse previously entered commands stored in the buffer. It is also used to manage the of the buffer.

**2. What is the first action in the boot sequence when a switch is powered on?**

- load the default Cisco IOS software
- load boot loader software
- low-level CPU initialization
- **load a power-on self-test program**

**Explanation:** The first action to take place when a switch is powered on is the POST or power-on self-test. POST performs tests on the CPU, memory, and flash in preparation for loading the boot loader.

**3. What must an administrator have in order to reset a lost password on a router?**

- a TFTP server
- a crossover cable
- access to another router
- **physical access to the router**

**Explanation:** Console access to the device through a terminal or terminal emulator software on a PC is required for password recovery.

**4. When configuring a switch for SSH access, what other command that is associated with the login local command is required to be entered on the switch?**

- enable secret _password_
- password _password_
- **username _username_ secret _secret_**
- login block-for _seconds_ attempts _number_ within*seconds*

**Explanation:** The login local command designates that the local username database is used to authenticate interfaces such as console or vty.

**5. Which command displays information about the auto-MDIX setting for a specific interface?​**

- show interfaces
- **show controllers**
- show processes
- show running-config

**Explanation:** To examine the auto-MDIX setting for a specific interface, the **show controllers ethernet-controller** command with the **phy** keyword should be used.

**6. If one end of an Ethernet connection is configured for full duplex and the other end of the connection is configured for half duplex, where would late collisions be observed?**

- on both ends of the connection
- on the full-duplex end of the connection
- only on serial interfaces
- **on the half-duplex end of the connection**

**Explanation:** Full-duplex communications do not produce collisions. However, collisions often occur in half-duplex operations. When a connection has two different duplex configurations, the half-duplex end will experience late collisions. Collisions are found on Ethernet networks. Serial interfaces use technologies other than Ethernet.

**7. Which command is used to set the BOOT environment variable that defines where to find the IOS image file on a switch?**

- config-register
- **boot system**
- boot loader
- confreg

**Explanation:** The **boot system** command is used to set the BOOT environment variable. The **config-register** and **confreg** commands are used to set the configuration register. The **boot loader** command supports commands to format the flash file system, reinstall the operating system software, and recover from a lost or forgotten password.

**8. What does a switch use to locate and load the IOS image?**

- **BOOT environment variable**
- IOS image file
- POST
- startup-config
- NVRAM

**Explanation:** The BOOT environment variable contains the information about where to find the IOS image file.

**9. Which protocol adds security to remote connections?**

- FTP
- HTTP
- NetBEUI
- POP
- **SSH**

**Explanation:** SSH allows a technician to securely connect to a remote network device for monitoring and troubleshooting. HTTP establishes web page requests. FTP manages file transfer. NetBEUI is not routed on the Internet. POP downloads email messages from email servers.

**10. What is a characteristic of an IPv4 loopback interface on a Cisco IOS router?​**

- The no shutdown command is required to place this interface in an UP state.​
- **It is a logical interface internal to the router.**
- Only one loopback interface can be enabled on a router.​
- It is assigned to a physical port and can be connected to other devices.

**Explanation:** The loopback interface is a logical interface internal to the router and is automatically placed in an UP state, as long as the router is functioning. It is not assigned to a physical port and can therefore never be connected to any other device. Multiple loopback interfaces can be enabled on a router.

**11. What is the minimum Ethernet frame size that will not be discarded by the receiver as a runt frame?**

- **64 bytes**
- 512 bytes
- 1024 bytes
- 1500 bytes

**Explanation:** The minimum Ethernet frame size is 64 bytes. Frames smaller than 64 bytes are considered collision fragments or runt frames and are discarded.

**12. After which step of the switch bootup sequence is the boot loader executed?**

- after CPU initialization
- after IOS localization
- after flash file system initialization
- **after POST execution**

**Explanation:** The correct bootup sequence order is as follows:  
1.- The switch loads and executes the POST.  
2.- The switch loads the boot loader software.  
3.- The boot loader performs low-level CPU initialization.  
4.- The boot loader initializes the flash memory.  
5.- The boot loader locates and loads the default IOS image.

**13. Which impact does adding a Layer 2 switch have on a network?**

- an increase in the number of dropped frames
- **an increase in the size of the broadcast domain**
- an increase in the number of network collisions
- an increase in the size of the collision domain

**Explanation:** Adding a Layer 2 switch to a network increases the number of collision domains and increases the size of the broadcast domain. Layer 2 switches do not decrease the amount of broadcast traffic, do not increase the amount of network collisions and do not increase the number of dropped frames.

**14. Which characteristic describes cut-through switching?**

- Error-free fragments are forwarded, so switching occurs with lower latency.
- **Frames are forwarded without any error checking.**
- Only outgoing frames are checked for errors.
- Buffering is used to support different Ethernet speeds.

**Explanation:** Cut-through switching reduces latency by forwarding frames as soon as the destination MAC address and the corresponding switch port are read from the MAC address table. This switching method does not perform any error checking and does not use buffers to support different Ethernet speeds. Error checking and buffers are characteristics of store-and-forward switching.

**15. What is the significant difference between a hub and a Layer 2 LAN switch?**

- **A hub extends a collision domain, and a switch divides collision domains.**
- A hub divides collision domains, and a switch divides broadcast domains.
- Each port of a hub is a collision domain, and each port of a switch is a broadcast domain.
- A hub forwards frames, and a switch forwards only packets.

**Explanation:** Hubs operate only at the physical layer, forwarding bits as wire signals out all ports, and extend the collision domain of a network. Switches forward frames at the data link layer and each switch port is a separate collision domain which creates more, but smaller, collision domains. Switches do not manage broadcast domains because broadcast frames are always forwarded out all active ports.

  
**16. Which statement is correct about Ethernet switch frame forwarding decisions?**

- **Frame forwarding decisions are based on MAC address and port mappings in the CAM table.**
- Cut-through frame forwarding ensures that invalid frames are always dropped.
- Only frames with a broadcast destination address are forwarded out all active switch ports.
- Unicast frames are always forwarded regardless of the destination MAC address.

**Explanation:** Cut-through frame forwarding reads up to only the first 22 bytes of a frame, which excludes the frame check sequence and thus invalid frames may be forwarded. In addition to broadcast frames, frames with a destination MAC address that is not in the CAM are also flooded out all active ports. Unicast frames are not always forwarded. Received frames with a destination MAC address that is associated with the switch port on which it is received are not forwarded because the destination exists on the network segment connected to that port.

**17. How do switch buffers affect network performance?**

- They provide error checking on the data received.
- **They store frames received, thus preventing premature frame discarding when network congestion occurs.**
- They provide extra memory for a particular port if autonegotiation of speed or duplex fails.
- They hold data temporarily when a collision occurs until normal data transmission resumes.

**Explanation:** Switches have large frame buffers that allow data waiting to be transmitted to be stored so the data will not be dropped. This feature is beneficial especially if the incoming traffic is from a faster port than the egress port used for transmitting.

**18. Which switch characteristic helps keep traffic local and alleviates network congestion?**

- **high port density**
- fast port speed
- large frame buffers
- fast internal switching

**Explanation:** Switches that have a lot of ports (high port density) reduce the number of switches required and keep some of the traffic locally on the switch, thus removing the need to send it between switches.

**19. Which switch component reduces the amount of packet handling time inside the switch?**

- **ASIC**
- dual processors
- large buffer size
- store-and-forward RAM

**Explanation:** Application-specific integrated circuits (ASICs) are used in Cisco switches to speed up switch operations so that the switch can have an increased number of ports without degrading switch performance.

**20. Refer to the exhibit. A switch receives a Layer 2 frame that contains a source MAC address of 000b.a023.c501 and a destination MAC address of 0050.0fae.75aa. Place the switch steps in the order they occur. (Not all options are used.)**

![CCNA2 v7 SRWE – Modules 1 – 4: Switching Concepts, VLANs, and InterVLAN Routing Exam Answers](https://itexamanswers.net/wp-content/uploads/2019/12/Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam.png)

CCNA2 v7 SRWE – Modules 1 – 4: Switching Concepts, VLANs, and InterVLAN Routing Exam Answers

![CCNA 2 v7 Modules 1 – 4: Switching Concepts, VLANs, and InterVLAN Routing Exam Answers](https://itexamanswers.net/wp-content/uploads/2019/12/2020-01-20_230521.jpg)

CCNA 2 v7 Modules 1 – 4: Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 20

**Explanation:** The first step a switch does when processing a frame is to see if the source MAC address is in the MAC address table. If the address is not there, the switch adds it. The switch then examines the destination MAC address and compares it to the MAC address table. If the address is in the table, the switch forwards the frame out the corresponding port. If the address is missing from the table, the switch will forward the frame to all ports except the port through which the frame arrived.

  
**21. What information is added to the switch table from incoming frames?**

- **source MAC address and incoming port number**
- destination MAC address and incoming port number
- source IP address and incoming port number
- destination IP address and incoming port number

**Explanation:** A switch “learns” or builds the MAC address table based on the source MAC address as a frame comes into the switch. A switch forwards the frame onward based on the destination MAC address.

**22. Which switching method ensures that the incoming frame is error-free before forwarding?**

- cut-through
- FCS
- fragment free
- **store-and-forward**

**Explanation:** Two methods used by switches to transmit frames are store-and-forward and cut-through switching. The store-and-forward method performs error checking on the frame using the frame check sequence (FCS) value before sending the frame. In contrast, cut-through switching sends the frame as soon as the destination MAC address part of the header has been read and processed.

**23. Refer to the exhibit. How many broadcast domains are displayed?**

![CCNA2 v7 SRWE – Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 23](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-SRWE-–-Modules-1-–-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-23.png)

CCNA2 v7 SRWE – Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 23

- 1
- 4
- **8**
- 16
- 55

**Explanation:** A router defines a broadcast boundary, so every link between two routers is a broadcast domain. In the exhibit, 4 links between routers make 4 broadcast domains. Also, each LAN that is connected to a router is a broadcast domain. The 4 LANs in the exhibit result in 4 more broadcast domains, so there are 8 broadcast domains in all.

**24. Under which two occasions should an administrator disable DTP while managing a local area network? (Choose two.)**

- **when connecting a Cisco switch to a non-Cisco switch**
- when a neighbor switch uses a DTP mode of dynamic auto
- when a neighbor switch uses a DTP mode of dynamic desirable
- **on links that should not be trunking**
- on links that should dynamically attempt trunking

**Explanation:** Cisco best practice recommends disabling DTP on links where trunking is not intended and when a Cisco switch is connected to a non-Cisco switch. DTP is required for dynamic trunk negotiation.

**25. Which two characteristics describe the native VLAN? (Choose two.)**

- Designed to carry traffic that is generated by users, this type of VLAN is also known as the default VLAN.
- **The native VLAN traffic will be untagged across the trunk link.**
- This VLAN is necessary for remote management of a switch.
- High priority traffic, such as voice traffic, uses the native VLAN.
- **The native VLAN provides a common identifier to both ends of a trunk.**

**Explanation:** The native VLAN is assigned to 802.1Q trunks to provide a common identifier to both ends of the trunk link. Whatever VLAN native number is assigned to a port, or if the port is the default VLAN of 1, the port does not tag any frame in that VLAN as the traffic travels across the trunk. At the other end of the link, the receiving device that sees no tag knows the specific VLAN number because the receiving device must have the exact native VLAN number. The native VLAN should be an unused VLAN that is distinct from VLAN1, the default VLAN, as well as other VLANs. Data VLANs, also known as user VLANs, are configured to carry user-generated traffic, with the exception of high priority traffic, such as VoIP. Voice VLANs are configured for VoIP traffic. The management VLAN is configured to provide access to the management capabilities of a switch.

**26. On a switch that is configured with multiple VLANs, which command will remove only VLAN 100 from the switch?**

- Switch# delete flash:vlan.dat
- Switch(config-if)# no switchport access vlan 100
- Switch(config-if)# no switchport trunk allowed vlan 100
- **Switch(config)# no vlan 100**

**Explanation:** To remove all VLANs from a switch, the delete flash:vlan.dat command would be used. To change the assigned VLAN for an interface, the no switchport access vlan 100 interface configuration command would be used. To remove VLAN 100 as an allowed VLAN on a trunk, the no switchport trunk allowed vlan 100 would be used, but this would not remove the VLAN from the switch. To delete a single VLAN, such as VLAN 100, the no vlan 100 global configuration command would be used.

  
**27. Refer to the exhibit. A network administrator is reviewing port and VLAN assignments on switch S2 and notices that interfaces Gi0/1 and Gi0/2 are not included in the output. Why would the interfaces be missing from the output?**

![CCNA 2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam 27](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA-2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-27.jpg)

CCNA 2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam 27

- There is a native VLAN mismatch between the switches.
- There is no media connected to the interfaces.
- They are administratively shut down.
- **They are configured as trunk interfaces.**

**Explanation:** Interfaces that are configured as trunks do not belong to a VLAN and therefore will not show in the output of the **show vlan brief** commands.

**28. A network contains multiple VLANs spanning multiple switches. What happens when a device in VLAN 20 sends a broadcast Ethernet frame?**

- All devices in all VLANs see the frame.
- Devices in VLAN 20 and the management VLAN see the frame.
- **Only devices in VLAN 20 see the frame.**
- Only devices that are connected to the local switch see the frame.

**Explanation:** VLANs create logical broadcast domains that can span multiple VLAN segments. Ethernet frames that are sent by a device on a specific VLAN can only be seen by other devices in the same VLAN.

**29. Refer to the exhibit. All workstations are configured correctly in VLAN 20. Workstations that are connected to switch SW1 are not able to send traffic to workstations on SW2. What could be done to remedy the problem?**

![CCNA2 v7 SRWE – Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 29](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-SRWE-–-Modules-1-–-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-29.png)

CCNA2 v7 SRWE – Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 29

- **Allow VLAN 20 on the trunk link.**
- Enable DTP on both ends of the trunk.
- Configure all workstations on SW1 to be part of the default VLAN.
- Configure all workstations on SW2 to be part of the native VLAN.

**Explanation:** Enabling DTP on both switches simply allows negotiation of trunking. The “Negotiation of Trunking” line in the graphic shows that DTP is already enabled. The graphic also shows how the native VLAN is 1, and the default VLAN for any Cisco switch is 1. The graphic shows the PCs are to be in VLAN 20.

**30. What happens to switch ports after the VLAN to which they are assigned is deleted?**

- The ports are disabled.
- The ports are placed in trunk mode.
- The ports are assigned to VLAN1, the default VLAN.
- **The ports stop communicating with the attached devices.**

**Explanation:** Any ports that are not moved to an active VLAN cannot communicate with other hosts after the VLAN is deleted. They must be assigned to an active VLAN or their VLAN must be created.

**31. Match the IEEE 802.1Q standard VLAN tag field with the description. (Not all options are used.)**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 31](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-31.png)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 31

**Explanation:** The IEEE 802.1Q standard header includes a 4-byte VLAN tag:

- **Type** – A 2-byte value called the tag protocol ID (TPID) value.
- **User priority** – A 3-bit value that supports level or service implementation.
- **Canonical Format Identifier (CFI)** – A 1-bit identifier that enables Token Ring frames to be carried across Ethernet links.
- **VLAN ID (VID)** – A 12-bit VLAN identification number that supports up to 4096 VLAN IDs.

  
**32. Refer to the exhibit. In what switch mode should port G0/1 be assigned if Cisco best practices are being used?**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 32](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-32.png)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 32

- access
- **trunk**
- native
- auto

**Explanation:** The router is used to route between the two VLANs, thus switch port G0/1 needs to be configured in trunk mode.

**33. Match the DTP mode with its function. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-08_141221.jpg)

**Explanation:** The dynamic auto mode makes the interface become a trunk interface if the neighboring interface is set to trunk or desirable mode. The dynamic desirable mode makes the interface actively attempt to convert the link to a trunk link. The trunk mode puts the interface into permanent trunking mode and negotiates to convert the neighboring link into a trunk link. The nonegotiate mode prevents the interface from generating DTP frames.

**34. Port Fa0/11 on a switch is assigned to VLAN 30. If the command no switchport access vlan 30 is entered on the Fa0/11 interface, what will happen?**

- Port Fa0/11 will be shutdown.
- An error message would be displayed.
- **Port Fa0/11 will be returned to VLAN 1.**
- VLAN 30 will be deleted.

**Explanation:** When the **no switchport access vlan** command is entered, the port is returned to the default VLAN 1. The port will remain active as a member of VLAN 1, and VLAN 30 will still be intact, even if no other ports are associated with it.

**35. Which command displays the encapsulation type, the voice VLAN ID, and the access mode VLAN for the Fa0/1 interface?**

- show vlan brief
- **show interfaces Fa0/1 switchport**
- show mac address-table interface Fa0/1
- show interfaces trunk

**Explanation:** The **show interfaces switchport** command displays the following information for a given port:  
Switchport  
Administrative Mode  
Operational Mode  
Administrative Trunking Encapsulation  
Operational Trunking Encapsulation  
Negotiation of Trunking  
Access Mode VLAN  
Trunking Native Mode VLAN  
Administrative Native VLAN tagging  
Voice VLAN

  
**36. Refer to the exhibit. A technician is programming switch SW3 to manage voice and data traffic through port Fa0/20. What, if anything, is wrong with the configuration?**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/i297770v1n1_297770.png)

- There is nothing wrong with the configuration.
- Interface Fa0/20 can only have one VLAN assigned.
- The mls qos trust cos command should reference VLAN 35.
- **The command used to assign the voice VLAN to the switch port is incorrect.**

**Explanation:** The voice VLAN should be configured with the **switchport voice vlan 150** command. A switch interface can be configured to support one data VLAN and one voice VLAN. The **mls qos trust cos** associates with the interface. Voice traffic must be trusted so that fields within the voice packet can be used to classify it for QoS.

**37. Which four steps are needed to configure a voice VLAN on a switch port? (Choose four).**

- Configure the interface as an IEEE 802.1Q trunk.
- **Assign the voice VLAN to the switch port.**
- Activate spanning-tree PortFast on the interface.
- **Ensure that voice traffic is trusted and tagged with a CoS priority value.**
- **Add a voice VLAN.**
- Configure the switch port interface with subinterfaces.
- Assign a data VLAN to the switch port.
- **Configure the switch port in access mode.**

**Explanation:** To add an IP phone, the following commands should be added to the switch port:  
SW3(config-vlan)# **vlan 150**  
SW3(config-vlan)# **name voice**  
SW3(config-vlan)# **int fa0/20**  
SW3(config-if)# **switchport mode access**  
SW3(config-if)# **mls qos trust cos**  
SW3(config-if)# **switchport access vlan 150**

**38. Refer to the exhibit. PC1 is unable to communicate with server 1. The network administrator issues the show interfaces trunk command to begin troubleshooting. What conclusion can be made based on the output of this command?**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 38](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-38.jpg)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 38

- **Interface G0/2 is not configured as a trunk.**
- VLAN 20 has not been created.
- The encapsulation on interface G0/1 is incorrect.
- The DTP mode is incorrectly set to dynamic auto on interface G0/1.

**Explanation:** In the **show interfaces trunk** output, the G0/2 interface of DLS1 is not listed. This indicates the interface has probably not been configured as a trunk link. In the **show interfaces trunk** output, the G0/2 interface of DLS1 is not listed. This indicates the interface has probably not been configured as a trunk link.

**39. Refer to the exhibit. What is the cause of the error that is displayed in the configuration of inter-VLAN routing on router CiscoVille?**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 39](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-39.png)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 39

- The gig0/0 interface does not support inter-VLAN routing.
- The no shutdown command has not been configured.
- The IP address on CiscoVille is incorrect.
- **The encapsulation dot1Q 20 command has not been configured.​**  

**40. Refer to the exhibit. A network administrator has configured router CiscoVille with the above commands to provide inter-VLAN routing. What command will be required on a switch that is connected to the Gi0/0 interface on router CiscoVille to allow inter-VLAN routing?​**

![](https://itexamanswers.net/wp-content/uploads/2020/09/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-40-1.png)

- switchport mode access
- no switchport
- **switchport mode trunk**
- switchport mode dynamic desirable

**Explanation:** When they are configured for inter-VLAN routing, routers do not support the dynamic trunking protocol that is used by switches. For router-on-a-stick configurations to function, a connected switch must use the command **switchport mode trunk**.

**41. A high school uses VLAN15 for the laboratory network and VLAN30 for the faculty network. What is required to enable communication between these two VLANs while using the router-on-a-stick approach?**

- A multilayer switch is needed.
- A router with at least two LAN interfaces is needed.
- Two groups of switches are needed, each with ports that are configured for one VLAN.
- **A switch with a port that is configured as a trunk is needed when connecting to the router.**

**Explanation:** With router-on-a-stick, inter-VLAN routing is performed by a router with a single router interface that is connected to a switch port configured with trunk mode. Multiple subinterfaces, each configured for a VLAN, can be configured under the single physical router interface. Switches can have ports that are assigned to different VLANs, but communication between those VLANs requires routing function from the router. A multilayer switch is not used in a router-on-a-stick approach to inter-VLAN routing.

**42. When routing a large number of VLANs, what are two disadvantages of using the router-on-a-stick inter-VLAN routing method rather than the multilayer switch inter-VLAN routing method? (Choose two.)**

- Multiple SVIs are needed.
- **A dedicated router is required.**
- Router-on-a-stick requires subinterfaces to be configured on the same subnets.
- Router-on-a-stick requires multiple physical interfaces on a router.
- **Multiple subinterfaces may impact the traffic flow speed.**

**Explanation:** With the router-on-a-stick inter-VLAN routing method, a dedicated router is required. It only needs one physical interface on the router to route traffic among multiple VLANs, by using subinterfaces on one physical interface. On the other hand, since traffic of all VLANs will have to go through the same physical interfaces, the throughput will be impacted. Also, a multilayer switch can use multiple SVIs to perform inter-VLAN routing.

**43. Refer to the exhibit. A network administrator is verifying the configuration of inter-VLAN routing. Users complain that PCs on different VLANs cannot communicate. Based on the output, what are two configuration errors on switch interface Gi1/1? (Choose two.)**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 43](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-43.png)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 43

- **Gi1/1 is in the default VLAN.**
- Voice VLAN is not assigned to Gi1/1.
- **Gi1/1 is configured as trunk mode.**
- Negotiation of trunking is turned on on Gi1/1.
- The trunking encapsulation protocol is configured wrong.

**Explanation:** With legacy inter-VLAN routing methods, the switch ports that connect to the router should be configured as access mode and be assigned appropriate VLANs. In this scenario, the Gi1/1 interface should be in access mode with VLAN 10 assigned. The other options are default settings on the switch and have no effect on legacy inter-VLAN routing.

**44. Refer to the exhibit. A network administrator is verifying the configuration of inter-VLAN routing. Users complain that PC2 cannot communicate with PC1. Based on the output, what is the possible cause of the problem?**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 44](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-44.png)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 44

- Gi0/0 is not configured as a trunk port.
- The command interface GigabitEthernet0/0.5 was entered incorrectly.
- There is no IP address configured on the interface Gi0/0.
- The no shutdown command is not entered on subinterfaces.
- **The encapsulation dot1Q 5 command contains the wrong VLAN.**

**Explanation:** In router-on-a-stick, the subinterface configuration should match the VLAN number in the encapsulation command, in this case, the command **encapsulation dot1Q 10** should be used for VLAN 10. Since subinterfaces are used, there is no need to configure IP on the physical interface Gi0/0. The trunk mode is configured on the switch port that connects to the router. The subinterfaces are turned on when they are added.

**45. Refer to the exhibit. A network administrator has configured router CiscoVille with the above commands to provide inter-VLAN routing. What type of port will be required on a switch that is connected to Gi0/0 on router CiscoVille to allow inter-VLAN routing?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/Q45.jpg)

- routed port
- access port
- **trunk port**
- SVI

**Explanation:** To allow a router-on-a-stick configuration to function, a switch must be connected to the router via a trunk port to carry the VLANs to be routed. An SVI would be used on a multilayer switch where the switch is performing inter-VLAN routing.

**46. Refer to the exhibit. A network administrator is configuring RT1 for inter-VLAN routing. The switch is configured correctly and is functional. Host1, Host2, and Host3 cannot communicate with each other. Based on the router configuration, what is causing the problem?**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 46](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-46.png)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 46

- Interface Fa0/0 is missing IP address configuration information.
- **IP addresses on the subinterfaces are incorrectly matched to the VLANs.**
- Each subinterface of Fa0/0 needs separate no shutdown commands.
- Routers do not support 802.1Q encapsulation on subinterfaces.

**Explanation:** Since Host 1 (in VLAN 20) has the IP 172.18.1.10/27, the subinterface Fa0/0.1 should be configured with an IP address in the network 172.168.1.0/27. Similarly, Fa0/0.2 should be with an IP address in the network 172.168.1.64/27 and Fa0/0.3 should be with an IP address in the network 172.168.1.96/27.

**47. Refer to the exhibit. A router-on-a-stick configuration was implemented for VLANs 15, 30, and 45, according to the show running-config command output. PCs on VLAN 45 that are using the 172.16.45.0 /24 network are having trouble connecting to PCs on VLAN 30 in the 172.16.30.0 /24 network. Which error is most likely causing this problem?​**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 47](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-47.png)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 47

- The wrong VLAN has been configured on GigabitEthernet 0/0.45.
- The command no shutdown is missing on GigabitEthernet 0/0.30.
- The GigabitEthernet 0/0 interface is missing an IP address.
- **There is an incorrect IP address configured on GigabitEthernet 0/0.30.**

**Explanation:** he subinterface GigabitEthernet 0/0.30 has an IP address that does not correspond to the VLAN addressing scheme. The physical interface GigabitEthernet 0/0 does not need an IP address for the subinterfaces to function. Subinterfaces do not require the **no shutdown** command.

**48. What is a characteristic of a routed port on a Layer 3 switch?**

- It supports trunking.
- **It is not assigned to a VLAN.**
- It is commonly used as a WAN link.
- It cannot have an IP address assigned to it.

**Explanation:** A routed port on a Layer 3 switch is commonly used for connecting between distribution and core layer switches or between a Layer 3 switch and a router. This port does not get VLAN or trunking commands assigned to it. Instead, the port is programmed with an IP address. This is commonly used when static routing is configured on the switch or when a routing protocol is being run between the Layer 3 switch and the router or another Layer 3 switch.

**49. Refer to the exhibit. A network administrator needs to configure router-on-a-stick for the networks that are shown. How many subinterfaces will have to be created on the router if each VLAN that is shown is to be routed and each VLAN has its own subinterface?**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 49](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-49.png)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 49

- 1
- 2
- 3
- **4**
- 5

**Explanation:** Based on the IP addresses and masks given, the PC, printer, IP phone, and switch management VLAN are all on different VLANs. This situation will require four subinterfaces on the router.

**50. A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the BranchSw(config-if)# mdix auto command?**

- **It automatically adjusts the port to allow device connections to use either a straight-through or a crossover cable.**
- It applies an IPv4 address to the virtual interface.
- It applies an IPv6 address to the virtual interface.
- It permits an IPv6 address to be configured on a switch physical interface.
- It updates the MAC address table for the associated port.

**51. A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the BranchSw(config-if)# ip address 172.18.33.88 255.255.255.0 command?**

- **It applies an IPv4 address to the virtual interface.**
- It applies an IPv6 address to the virtual interface.
- It activates a virtual or physical switch interface.
- It permits an IPv6 address to be configured on a switch physical interface.
- It updates the MAC address table for the associated port.

**52. A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the BranchSw# configure terminal command?**

- **It enters the global configuration mode.**
- It enters configuration mode for a switch virtual interface.
- It applies an IPv4 address to the virtual interface.
- It updates the MAC address table for the associated port.
- It permits an IPv6 address to be configured on a switch physical interface.

**53. A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the BranchSw# configure terminal command?**

- **It enters the global configuration mode.**
- It saves the running configuration to NVRAM.
- It disables a virtual or physical switch interface.
- It updates the MAC address table for the associated port.
- It saves the startup configuration to the running configuration.

**54. A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the BranchSw(config-if)# shutdown command?**

- **It disables a virtual or physical switch interface.**
- It saves the running configuration to NVRAM.
- It activates a virtual or physical switch interface.
- It updates the MAC address table for the associated port.
- It saves the startup configuration to the running configuration.

**55. A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the BranchSw(config-if)# shutdown command?**

- **It disables a virtual or physical switch interface.**
- It applies an IPv6 address to the virtual interface.
- It applies an IPv4 address to the virtual interface.
- It permits an IPv6 address to be configured on a switch physical interface.
- It updates the MAC address table for the associated port.

**56. A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the BranchSw(config-if)# ipv6 address 2001:db8:a2b4:88::1/64 command?**

- **It applies an IPv6 address to the virtual interface.**
- It activates a virtual or physical switch interface.
- It applies an IPv4 address to the virtual interface.
- It permits an IPv6 address to be configured on a switch physical interface.
- It updates the MAC address table for the associated port.

**57. A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the BranchSw(config-if)# exit command?**

- **It returns to global configuration mode.**
- It returns to privileged mode.
- It configures the default gateway for the switch.
- It enters user mode.
- It saves the startup configuration to the running configuration.

**58. A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the BranchSw> enable command?**

- **It enters privileged mode.**
- It enters the global configuration mode.
- It enters configuration mode for a switch virtual interface.
- It updates the MAC address table for the associated port.
- It permits an IPv6 address to be configured on a switch physical interface.

**58. A technician is configuring a new Cisco 2960 switch. What is the effect of issuing the BranchSw(config-if)# duplex full command?**

- **It allows data to flow in both directions at the same time on the interface.**
- It allows data to flow in only one direction at a time on the interface
- It automatically adjusts the port to allow device connections to use either a straight-through or a crossover cable.
- It configures the switch as the default gateway.
- It encrypts user-mode passwords when users connect remotely.

**60. What type of VLAN should not carry voice and network management traffic?**

- **data VLAN**
- voice VLAN
- management VLAN
- security VLAN

**62. What type of VLAN is designed to reserve bandwidth to ensure IP Phone quality?**

- **voice VLAN**
- trunk VLAN
- security VLAN
- management VLAN

**63. What type of VLAN is initially the management VLAN?**

- **default VLAN**
- native VLAN
- data VLAN
- management VLAN

**64. What type of VLAN is designed to have a delay of less than 150 ms across the network?**

- **voice VLAN**
- desirable VLAN
- trunk VLAN
- security VLAN

**65. What type of VLAN is used to separate the network into groups of users or devices?**

- **data VLAN**
- management VLAN
- voice VLAN
- native VLAN

**66. What type of VLAN is configured specifically for network traffic such as SSH, Telnet, HTTPS, HTTP, and SNMP?**

- **management VLAN**
- security VLAN
- trunk VLAN
- voice VLAN

**68. What type of VLAN supports untagged traffic?**

- **native VLAN**
- voice VLAN
- security VLAN
- management VLAN

**69. What type of VLAN supports untagged traffic?**

- **native VLAN**
- desirable VLAN
- trunk VLAN
- security VLAN

**70. Refer to the exhibit. A network administrator has configured R1 as shown. When the administrator checks the status of the serial interface, the interface is shown as being administratively down. What additional command must be entered on the serial interface of R1 to bring the interface up?**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 70](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-70.jpg)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 70

- IPv6 enable
- clockrate 128000
- end
- **no shutdown**

**Explanation:** By default all router interfaces are shut down. To bring the interfaces up, an administrator must issue the **no shutdown** command in interface mode.

**71. Refer to the exhibit. The network administrator wants to configure Switch1 to allow SSH connections and prohibit Telnet connections. How should the network administrator change the displayed configuration to satisfy the requirement?**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 71](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-71.jpg)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 71

- Use SSH version 1.
- Reconfigure the RSA key.
- Configure SSH on a different line.
- **Modify the transport input command.**

**72. Which solution would help a college alleviate network congestion due to collisions?**

- a firewall that connects to two Internet providers
- **a high port density switch**
- a router with two Ethernet ports
- a router with three Ethernet ports

**Explanation:** Switches provide microsegmentation so that one device does not compete for the same Ethernet network bandwidth with another network device, thus practically eliminating collisions. A high port density switch provides very fast connectivity for many devices.

**73. Which two statements are correct with respect to SVI inter-VLAN routing? (Choose two.)**

- **Switching packets is faster with SVI.**
- **There is no need for a connection to a router.**
- Virtual interfaces support subinterfaces.
- SVIs can be bundled into EtherChannels.
- SVIs eliminate the need for a default gateway in the hosts.

**Explanation:** The SVI inter-VLAN routing method is faster than other methods. The switch can route the existing VLANs without the need for a router.

**74. Refer to the exhibit. A network administrator is configuring inter-VLAN routing on a network. For now, only one VLAN is being used, but more will be added soon. What is the missing parameter that is shown as the highlighted question mark in the graphic?**

![CCNA2 v7 Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 74](https://itexamanswers.net/wp-content/uploads/2019/12/CCNA2-v7-Modules-1-4-Switching-Concepts-VLANs-and-InterVLAN-Routing-Exam-Answers-74.png)

CCNA2 v7 Modules 1 – 4 Switching Concepts, VLANs, and InterVLAN Routing Exam Answers 74

- It identifies the subinterface.
- **It identifies the VLAN number.**
- It identifies the native VLAN number.
- It identifies the type of encapsulation that is used.
- It identifies the number of hosts that are allowed on the interface.

**Explanation:** The completed command would be **encapsulation dot1q 7**. The **encapsulation dot1q** part of the command enables trunking and identifies the type of trunking to use. The **7** identifies the VLAN number.

**75. Which type of VLAN is used to designate which traffic is untagged when crossing a trunk port?**

- data
- default
- **native**
- management

**Explanation:** A native VLAN is the VLAN that does not receive a VLAN tag in the IEEE 802.1Q frame header. Cisco best practices recommend the use of an unused VLAN (not a data VLAN, the default VLAN of VLAN 1, or the management VLAN) as the native VLAN whenever possible.

**76. A network administrator issues the show vlan brief command while troubleshooting a user support ticket. What output will be displayed?**

- the VLAN assignment and membership for device MAC addresses
- **the VLAN assignment and membership for all switch ports**
- the VLAN assignment and trunking encapsulation
- the VLAN assignment and native VLAN

**Explanation:** The **show vlan brief** command will provide information displaying the VLAN assignment and membership for all switch ports on a switch.

**77. Open the PT Activity. Perform the tasks in the activity instructions and then answer the question.**  
![](https://itexamanswers.net/wp-content/uploads/2019/12/2020-01-20_224244.jpg)

![Icon](https://itexamanswers.net/wp-content/plugins/download-manager/assets/file-type-icons/pka.svg)

###### [Modules 1 - 4 Switching Concepts, VLANs, and InterVLAN Routing](https://itexamanswers.net/download/modules-1-4-switching-concepts-vlans-and-intervlan-routing)

1 file(s) 287.41 KB

  
**Which message is displayed when 10.10.10.1 is entered into the PC1 Web Browser address bar?**

- Local Server
- Test Server
- **File Server**
- Cisco Server

**Explanation:** Examining the configuration of switch SW1 shows that interface Gi0/1 is not configured as a trunk. Issuing the interface configuration command **switchport mode trunk** on this interface will enable communications between PC1 and Server1.

**78. Match each DHCP message type with its description. (Not all options are used.)**

![CCNA 2 v7 Modules 1 – 4: Switching Concepts, VLANs, and InterVLAN Routing Exam Answers](https://itexamanswers.net/wp-content/uploads/2019/12/2020-01-20_225135.jpg)

CCNA 2 v7 Modules 1 – 4: Switching Concepts, VLANs, and InterVLAN Routing Exam Answers

**Explanation:**Place the options in the following order:

- a client initiating a message to find a DHCP server – DHCPDISCOVER
- a DHCP server responding to the initial request by a client – DHCPOFFER
- the client accepting the IP address provided by the DHCP server – DHCPREQUEST
- the DHCP server confirming that the lease has been accepted – DHCPACK

**79. What type of VLAN is configured specifically for network traffic such as SSH, Telnet, HTTPS, HHTP, and SNMP?**

- voice VLAN
- **management VLAN**
- native VLAN
- security VLAN