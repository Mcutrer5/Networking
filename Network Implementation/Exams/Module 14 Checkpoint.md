#### Modules 13 – 14 of the CCNA3 – Enterprise Networking, Security, and Automation (ENSA) v7.0

**1. A company uses a cloud-based payroll system. Which cloud computing technology is this company using?**

- browser as a service (BaaS)
- infrastructure as a service (IaaS)
- **software as a service (SaaS)**
- wireless as a service (WaaS)

**Explanation:** Curriculum Reference: Module 7.2  
This item is based on information contained in the presentation.  
There is no such thing as BaaS. Infrastructure as a service (IaaS) is when key network devices such as routers and firewalls are leased from a provider. Wireless as a service (WaaS) is when a provider provides wireless connectivity at a fixed monthly cost.

**2. For a data center, what is the difference in the server virtualization data traffic compared with the traditional client-server model?**

- Data traffic from clients will be routed to multiple virtual servers.
- **There are significant data exchanges between virtual servers.**
- There is more data traffic flowing from virtual servers to clients.
- More network control traffic is generated between virtual servers and clients.

**3. Which component in a traditional infrastructure device provides Layer 2 and Layer 3 functions to create data paths within a network?**

- data plane
- **control plane**
- adjacency table
- forwarding information base

**4. Which network traffic management technology is a basic element in SDN implementations?**

- **OpenFlow**
- OpenStack
- IEEE 802.1aq
- Interface to the Routing System

**Explanation:** OpenFlow was developed at Stanford University to manage traffic between routers, switches, and wireless access points and a controller. It is the original and widely implemented southbound API for SDN.​ OpenStack is a virtualization and orchestration platform available to build scalable cloud environments and provide an infrastructure as a service (IaaS) solution. It is often used with Cisco ACI. IEEE 802.1aq is a replacement to the Spanning Tree Protocol (STP) that allows all paths to be active with multiple equal cost paths.​ Interface to the Routing System uses a fast path protocol to populate the network device routing table.​

**5. Which type of hypervisor would most likely be used in a data center?**

- Type 2
- **Type 1**
- Nexus
- Hadoop

**Explanation:** The two type of hypervisors are Type 1 and Type 2. Type 1 hypervisors are usually used on enterprise servers. Enterprise servers rather than virtualized PCs are more likely to be in a data center.

**6. Which is a characteristic of a Type 1 hypervisor?​**

- **installed directly on a server​**
- best suited for consumers and not for an enterprise environment
- does not require management console software
- installed on an existing operating system​

**Explanation:** Type 1 hypervisors are installed directly on a server and are known as “bare metal” solutions giving direct access to hardware resources. They also require a management console and are best suited for enterprise environments.​

**7. Which two layers of the OSI model are associated with SDN network control plane functions that make forwarding decisions? (Choose two.)​**

- Layer 1
- **Layer 2**
- **Layer 3**
- Layer 4
- Layer 5

**Explanation:** The SDN control plane uses the Layer 2 ARP table and the Layer 3 routing table to make decisions about forwarding traffic.

**8. What pre-populates the FIB on Cisco devices that use CEF to process packets?**

- **the routing table**
- the adjacency table
- the ARP table
- the DSP

**Explanation:** CEF uses the FIB and adjacency table to make fast forwarding decisions without control plane processing. The adjacency table is pre-populated by the ARP table and the FIB is pre-populated by the routing table.​

**9. What is a function of the data plane of a network device?**

- sending information to the CPU for processing
- building the routing table
- resolving MAC addresses
- **forwarding traffic flows**

**Explanation:** Networking devices operate in two planes; the data plane and the control plane. The control plane maintains Layer 2 and Layer 3 forwarding mechanisms using the CPU. The data plane forwards traffic flows.

**10. Which statement describes the concept of cloud computing?**

- **separation of application from hardware**
- separation of management plane from control plane
- separation of operating system from hardware
- separation of control plane from data plane

**Explanation:** Cloud computing is used to separate the application or service from hardware. Virtualization separates the operating system from the hardware.

**11. Which cloud model provides services for a specific organization or entity?**

- a public cloud
- a hybrid cloud
- **a private cloud**
- a community cloud

**Explanation:** Private clouds are used to provide services and applications to a specific organization and may be set up within the private network of the organization or managed by an outside organization.

**12. What two benefits are gained when an organization adopts cloud computing and virtualization? (Choose two.)**

- **provides a “pay-as-you-go” model, allowing organizations to treat computing and storage expenses as a utility**
- **enables rapid responses to increasing data volume requirements**
- distributed processing of large data sets in the size of terabytes
- elimination of vulnerabilities to cyber attacks
- increases the dependance on onsite IT resources

**Explanation:** Organizations can use virtualization to consolidate the number of required servers by running many virtual servers on a single physical server. Cloud computing allows organizations to scale their solutions as required and to pay only for the resources they require.

**13. Which type of Hypervisor is implemented when a user with a laptop running the Mac OS installs a Windows virtual OS instance?**

- **type 2**
- virtual machine
- type 1
- bare metal

**Explanation:** Type 2 hypervisors, also know as hosted hypervisors, are installed on top of an existing operating system, such as Mac OS, Windows, or Linux.

**14. A small company is considering moving many of its data center functions to the cloud. What are three advantages of this plan? (Choose three.)**

- **The company only needs to pay for the amount of processing and storage capacity that it uses.**
- Cloud services are billed at a fixed fee no matter how much processing and storage are used by the company.
- **The company does not need to be concerned about how to handle increasing data storage and processing demands with in-house data center equipment.**
- **The company can increase processing and storage capacity as needed and then decrease capacity when it is no longer needed.**
- Single-tenant data centers can easily grow to accommodate increasing data storage requirements.
- Cloud services enable the company to own and administer its own servers and storage devices.

**Explanation:** Cloud computing offers many advantages to the company. Since the cloud data storage and processing facilities are owned by third-parties, the company does not need to be concerned about how it will handle increasing data storage and processing demands with its own data center equipment. The company can easily increase or decrease processing power and storage capacity based on need. Also, cloud services are billed by usage, so the company does not have the costs of supporting its own expensive data center that is not always used to maximum capacity.

**15. How does virtualization help with disaster recovery within a data center?**

- **support of live migration**
- guarantee of power
- improvement of business practices
- supply of consistent air flow

**Explanation:** Live migration allows moving of one virtual server to another virtual server that could be in a different location that is some distance from the original data center.

**16. What technology allows users to access data anywhere and at any time?**

- **Cloud computing**
- virtualization
- micromarketing
- data analytics

**Explanation:** Cloud computing allows organizations to eliminate the need for on-site IT equipment, maintenance, and management. Cloud computing allows organizations to expand their services or capabilities while avoiding the increased costs of energy and space.

**17. Which action takes place in the assurance element of the IBN model?**

- **verification and corrective action**
- configuring systems
- translation of policies
- integrity checks

**Explanation:** The assurance element of the IBN model is concerned with end-to-end verification of network-wide behavior.

**18. Refer to the exhibit. Which data format is used to represent the data for network automation applications?**

![](https://itexamanswers.net/wp-content/uploads/2019/12/i349058v2n1_347058.png)

- XML
- YAML
- HTML
- **JSON**

**Explanation:** The common data formats that are used in many applications including network automation and programmability are as follows:

- **JavaScript Object Notation (JSON)** – In JSON, the data known as an object is one or more key/value pairs enclosed in braces { }. Keys must be strings within double quotation marks ” “. Keys and values are separated by a colon.
- **eXtensible Markup Language (XML)** – In XML, the data is enclosed within a related set of tags <tag>data</tag>.
- **YAML Ain’t Markup Language (YAML)** – In YAML, the data known as an object is one or more key value pairs. Key value pairs are separated by a colon without the use of quotation marks. YAML uses indentation to define its structure, without the use of brackets or commas.
    

**19. What is the function of the key contained in most RESTful APIs?**

- It is the top-level object of the API query.
- **It is used to authenticate the requesting source.**
- It represents the main query components in the API request.
- It is used in the encryption of the message by an API request.

**Explanation:** Many RESTful APIs, including public APIs, require a key. The key is used to identify the source of the request through authentication.

**20. Which two configuration management tools are developed using Ruby? (Choose two.)**

- **Puppet**
- Ansible
- SaltStack
- **Chef**
- RESTCONF

**Explanation:** Chef and Puppet are configuration management tools developed using Ruby. Ansible and SaltStack are configuration management tools developed using Python. Ruby is typically considered a more difficult language to learn than Python. RESTCONF is a network management protocol.

**21. Which term is used to describe a set of instructions for execution by the configuration management tool Puppet?**

- Playbook
- Cookbook
- **Manifest**
- Pillar

**Explanation:** The configuration management tool Puppet uses the name Manifest to describe the set of instructions to be executed.

**22. Which term is used to describe a set of instructions for execution by the configuration management tool SaltStack?**

- Cookbook
- Manifest
- **Pillar**
- Playbook

**Explanation:** The configuration management tool SaltStack uses the name Pillar to describe the set of instructions to be executed.

**23. Which scenario describes the use of a public API?**

- It requires a license.
- **It can be used with no restrictions.**
- It is used between a company and its business partners.
- It is used only within an organization.

**Explanation:** Public, or open, APIs have no restrictions and are available to the public. Some API providers do require a user to obtain a free key or token prior to using the API in order to control the volume of API requests received and processed.

**24. What is YAML?**

- It is a scripting language.
- **It is a data format and superset of JSON.**
- It is a compiled programming language.
- It is a web application.

**Explanation:** Like JSON, YAML Ain’t Markup Language (YAML) is a data format used by applications to store and transport data. YAML is considered a superset of JSON.

**25. Which RESTFul operation corresponds to the HTTP GET method?**

- post
- patch
- update
- **read**

**Explanation:** RESTful operations correspond to the following HTTP methods (shown to the left with the RESTful operation on the right):

- POST > Create
- GET > Read
- PUT/PATCH > Update
- DELETE > Delete
    

**26. Which technology virtualizes the network control plane and moves it to a centralized controller?​**

- **SDN**
- fog computing
- cloud computing
- IaaS

**Explanation:** Networking devices operate in two planes: the data plane and the control plane. The control plane maintains Layer 2 and Layer 3 forwarding mechanisms using the CPU. The data plane forwards traffic flows. SDN virtualizes the control plane and moves it to a centralized network controller.​

**27. What are two functions of hypervisors? (Choose two.)**

- to partition the hard drive to run virtual machines
- **to manage virtual machines**
- to protect the host from malware infection from the virtual machines
- to share the antivirus software across the virtual machines
- **to allocate physical system resources to virtual machines**

**Explanation:** The hypervisor does not protect the hosting OS from malware. Neither does it allow sharing software across virtual machines. The hard drive of the supporting computer does not need to be partitioned to run virtual machines. The hypervisor creates and manages virtual machines on a host computer and allocates physical system resources to them.

**28. What is a difference between the functions of Cloud computing and virtualization?**

- Cloud computing requires hypervisor technology whereas virtualization is a fault tolerance technology.
- **Cloud computing separates the application from the hardware whereas virtualization separates the OS from the underlying hardware.**
- Cloud computing provides services on web-based access whereas virtualization provides services on data access through virtualized Internet connections.
- Cloud computing utilizes data center technology whereas virtualization is not used in data centers.

**Explanation:** Cloud computing separates the application from the hardware. Virtualization separates the OS from the underlying hardware. Virtualization is a typical component within cloud computing. Virtualization is also widely used in data centers. Although the implementation of virtualization facilitates an easy server fault tolerance setup, it is not a fault tolerance technology by design. The Internet connection from a data center or service provider needs redundant physical WAN connections to ISPs.​​

**29. How is the YAML data format structure different from JSON?**

- **It uses indentations.**
- It uses end tags.
- It uses hierarchical levels of nesting.
- It uses brackets and commas.

**Explanation:** The structure in YAML is defined by indentations rather than brackets and commas.

**30. What is the most widely used API for web services?**

- XML-RPC
- SOAP
- JSON-RPC
- **REST**

**Explanation:** REST accounts for more than 80% of all API types used for web services, making it the most widely used web service API.

**31. What is REST?**

- It is a way to store and interchange data in a structured format.
- **It is an architecture style for designing web service applications.**
- It is a human readable data structure that is used by applications for storing, transforming, and reading data.
- It is a protocol that allows administrators to manage nodes on an IP network.

**Explanation:** REST is not a protocol or service, but rather a style of software architecture for designing web service applications.

**32. What is a difference between the XML and HTML data formats?**

- **XML does not use predefined tags whereas HTML does use predefined tags.**
- XML encloses data within a pair of tags whereas HTML uses a pair of quotation makes to enclose data.
- XML formats data in binary whereas HTML formats data in plain text.
- XML does not require indentation for each key/value pair but HTML does require indentation.

**Explanation:** XML is a human readable data structure used to store, transfer, and read data by applications. Like HTML, XML uses a related set of tags to enclose data. However, unlike HTML, XML uses no predefined tags or document structure.

**33. To avoid purchasing new hardware, a company wants to take advantage of idle system resources and consolidate the number of servers while allowing for multiple operating systems on a single hardware platform. What service or technology would support this requirement?**

- dedicated servers
- Cisco ACI
- **virtualization**
- software defined networking

**34. Match the term to the RESTful API request http://www.mapquestapi.com/directions/v2/route?outFormat=json&key=KEY&from=San+Jose,Ca&to=Monterey,Ca component. (Not all options are used.)**

![](https://itexamanswers.net/wp-content/uploads/2019/12/2024-10-10_090149.jpg)

|   |   |
|---|---|
|resources|directions/v2/route|
|parameters|from=San+Jose,Ca&to=Monterey,Ca|
|query|outFormat=json&key=KEY&from=San+Jose,Ca&to=Monterey,Ca|
|API server|http://www.mapquestapi.com|
|format|outFormat=json|
|key|key=KEY|

**35. Which cloud computing opportunity would provide the use of network hardware such as routers and switches for a particular company?**

- software as a service (SaaS)
- wireless as a service (WaaS)
- **infrastructure as a service (IaaS)**
- browser as a service (BaaS)

**Explanation:** This item is based on information contained in the presentation.  
Routers, switches, and firewalls are infrastructure devices that can be provided in the cloud.

**36. What component is considered the brains of the ACI architecture and translates application policies​?**

- the Application Network Profile endpoints
- the Nexus 9000 switch
- the hypervisor​
- **the Application Policy Infrastructure Controller**

**Explanation:** The ACI architecture consists of three core components: the Application Network Profile, the Application Policy Infrastructure Controller, which serves as the brains of the ACI architecture, and the Cisco Nexus 9000 switch.

**37. Which statement describes the concept of cloud computing?**

- separation of management plane from control plane
- separation of control plane from data plane
- **separation of application from hardware**
- separation of operating system from hardware

**Explanation:** Cloud computing is used to separate the application or service from hardware. Virtualization separates the operating system from the hardware.

**38. In which situation would a partner API be appropriate?**

- an internet search engine allowing developers to integrate the search engine into their own software applications
- company sales staff accessing internal sales data from their mobile devices
- someone creating an account on an external app or website by using his or her social media credentials
- **a vacation service site interacting with hotel databases to display information from all the hotels on its web site**

**Explanation:** Partner API programs incorporate collaboration with other business. They facilitate communication and integration of software between a company and its business partners.

**39. Because of enormous growth in web traffic, a company has planned to purchase additional servers to help handle the web traffic. What service or technology would support this requirement?**

- virtualization
- data center
- cloud services
- **dedicated servers**

**40. ABCTech is investigating the use of automation for some of its products. In order to control and test these products, the programmers require Windows, Linux, and MAC OS on their computers. What service or technology would support this requirement?**

- dedicated servers
- software defined networking
- **virtualization**
- Cisco ACI

**41. What are three components used in the query portion of a typical RESTful API request? (Choose three.)**

- API server
- **format**
- **parameters**
- **key**
- protocol
- resources

**Explanation:** The query portion in a RESTful API request specifies the data format and information the client is requesting from the API service. Queries can include the following:

- **Format** – JSON, YAML, XML, and other supported data format
- **Key** – for authentication of the requesting source
- **Parameters** – used to send information pertaining to the query request

**42. A company has recently become multinational. Employees are working remotely, in different time zones, and they need access to company services from any place at any time. What service or technology would support this requirement?**

- dedicated servers
- **cloud services**
- Cisco ACI
- virtualization

**43. Following a multicontinent advertising campaign for a new product, a company finds its client database and volume of orders are overloading its on-site computer systems but the company does not have any room to expand. What service or technology would support this requirement?**

- **cloud services**
- dedicated servers
- data center
- virtualization

**44. A network administrator has been tasked with creating a disaster recovery plan. As part of this plan, the administrator is looking for a backup site for all of the data on the company servers. What service or technology would support this requirement?**

- virtualization
- software defined networking
- **data center**
- dedicated servers

**45. Which is a requirement of a site-to-site VPN?**

- It requires hosts to use VPN client software to encapsulate traffic.
- **It requires a VPN gateway at each end of the tunnel to encrypt and decrypt traffic.**
- It requires the placement of a VPN server at the edge of the company network.
- It requires a client/server architecture.

**Explanation:** Site-to-site VPNs are static and are used to connect entire networks. Hosts have no knowledge of the VPN and send TCP/IP traffic to VPN gateways. The VPN gateway is responsible for encapsulating the traffic and forwarding it through the VPN tunnel to a peer gateway at the other end which decapsulates the traffic.

**46. Which statement describes an important characteristic of a site-to-site VPN?**

- **It must be statically set up.**
- After the initial connection is established, it can dynamically change connection information.
- It requires using a VPN client on the host PC.
- It is commonly implemented over dialup and cable modem networks.
- It is ideally suited for use by mobile workers.

**Explanation:** A site-to-site VPN is created between the network devices of two separate networks. The VPN is static and stays established. The internal hosts of the two networks have no knowledge of the VPN.

**47. Which protocol is attacked when a cybercriminal provides an invalid gateway in order to create a man-in-the-middle attack?**

- **DHCP**
- ICMP
- DNS
- HTTP or HTTPS

**Explanation:** A cybercriminal could set up a rogue DHCP server that provides one or more of the following:

- Wrong default gateway that is used to create a man-in-the-middle attack and allow the attacker to intercept data
- Wrong DNS server that results in the user being sent to a malicious website
- Invalid default gateway IP address that results in a denial of service attack on the DHCP client

**48. In which TCP attack is the cybercriminal attempting to overwhelm a target host with half-open TCP connections?**

- reset attack
- session hijacking attack
- **SYN flood attack**
- port scan attack

**Explanation:** In a TCP SYN flood attack, the attacker sends to the target host a continuous flood of TCP SYN session requests with a spoofed source IP address. The target host responds with a TCP-SYN-ACK to each of the SYN session requests and waits for a TCP ACK that will never arrive. Eventually the target is overwhelmed with half-open TCP connections.

**49. Which statement describes a VPN?**

- VPNs use logical connections to create public networks through the Internet.
- VPNs use open source virtualization software to create the tunnel through the Internet.
- VPNs use dedicated physical connections to transfer data between remote users.
- **VPNs use virtual connections to create a private network through a public network.**

**Explanation:** A VPN is a private network that is created over a public network. Instead of using dedicated physical connections, a VPN uses virtual connections routed through a public network between two network devices.