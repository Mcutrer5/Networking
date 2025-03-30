![[Cisco.png]]

---
# *Table of Contents* 📚

[6.1. NAT Characteristics](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-1-nat-characteristics)

- 1. [6.1.1. IPv4 Private Address Space](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-1-1-ipv4-private-address-space)
        1. [Private Internet Addresses are Defined in RFC 1918](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-private-internet-addresses-are-defined-in-rfc-1918)
    2. [6.1.2. What is NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-1-2-what-is-nat)
    3. [6.1.3. How NAT Works](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-1-3-how-nat-works)
    4. [6.1.4. NAT Terminology](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-1-4-nat-terminology)

- [6.2. Types of NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-2-types-of-nat)
    1. [6.2.1. Static NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-2-1-static-nat)
    2. [6.2.2. Dynamic NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-2-2-dynamic-nat)
    3. [6.2.3. Port Address Translation](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-2-3-port-address-translation)
    4. [6.2.4. Next Available Port](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-2-4-next-available-port)
    5. [6.2.5. NAT and PAT Comparison](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-2-5-nat-and-pat-comparison)
    6. [6.2.6. Packets without a Layer 4 Segment](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-2-6-packets-without-a-layer-4-segment)
    7. [6.2.7. Packet Tracer – Investigate NAT Operations](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-2-7-packet-tracer-investigate-nat-operations)

- [6.3. NAT Advantages and Disadvantages](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-3-nat-advantages-and-disadvantages)
    1. [6.3.1. Advantages of NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-3-1-advantages-of-nat)
    2. [6.3.2. Disadvantages of NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-3-2-disadvantages-of-nat)

- [6.4. Static NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-4-static-nat)
    1. [6.4.1. Static NAT Scenario](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-4-1-static-nat-scenario)
    2. [6.4.2. Configure Static NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-4-2-configure-static-nat)
    3. [6.4.3. Analyze Static NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-4-3-analyze-static-nat)
    4. [6.4.4. Verify Static NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-4-4-verify-static-nat)
    5. [6.4.5. Packet Tracer – Configure Static NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-4-5-packet-tracer-configure-static-nat)

- [6.5. Dynamic NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-5-dynamic-nat)
    1. [6.5.1. Dynamic NAT Scenario](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-5-1-dynamic-nat-scenario)
    2. [6.5.2. Configure Dynamic NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-5-2-configure-dynamic-nat)
    3. [6.5.3. Analyze Dynamic NAT – Inside to Outside](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-5-3-analyze-dynamic-nat-inside-to-outside)
    4. [6.5.4. Analyze Dynamic NAT – Outside to Inside](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-5-4-analyze-dynamic-nat-outside-to-inside)
    5. [6.5.5. Verify Dynamic NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-5-5-verify-dynamic-nat)
    6. [6.5.6. Packet Tracer – Configure Dynamic NAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-5-6-packet-tracer-configure-dynamic-nat)

- [6.6. PAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-6-pat)
    1. [6.6.1. PAT Scenario](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-6-1-pat-scenario)
    2. [6.6.2. Configure PAT to Use a Single IPv4 Address](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-6-2-configure-pat-to-use-a-single-ipv4-address)
    3. [6.6.3. Configure PAT to Use an Address Pool](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-6-3-configure-pat-to-use-an-address-pool)
    4. [6.6.4. Analyze PAT – PC to Server](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-6-4-analyze-pat-pc-to-server)
    5. [6.6.5. Analyze PAT – Server to PC](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-6-5-analyze-pat-server-to-pc)
    6. [6.6.6. Verify PAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-6-6-verify-pat)
    7. [6.6.7. Packet Tracer – Configure PAT](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-6-7-packet-tracer-configure-pat)

- [6.7. NAT64](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-7-nat64)
    1. [6.7.1. NAT for IPv6?](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-7-1-nat-for-ipv6)
    2. [6.7.2. NAT64](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-7-2-nat64)

1. [6.8. Module Practice and Quiz](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-8-module-practice-and-quiz)
    1. [6.8.1. Packet Tracer – Configure NAT for IPv4](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-8-1-packet-tracer-configure-nat-for-ipv4)
    2. [6.8.2. Lab – Configure NAT for IPv4](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-8-2-lab-configure-nat-for-ipv4)
    3. [6.8.3. What did I learn in this module?](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-8-3-what-did-i-learn-in-this-module)
    4. [6.8.4 Module Quiz – NAT for IPv4](https://itexamanswers.net/ccna-3-v7-0-curriculum-module-6-nat-for-ipv4.html#section-6-8-4-module-quiz-nat-for-ipv4)

---

[[Module 5 ACLs for IPv4 Configuration|◀ Module 5]]         |         [[Network Implementation |Home 🏠]]         |         [[Module 7 ▶]] 