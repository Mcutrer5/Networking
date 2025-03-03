### TCP (Transmission Control Protocol) and UDP (User Datagram Protocol)

#### a. Overview

- **TCP (Transmission Control Protocol)** and **UDP (User Datagram Protocol)** are transport layer protocols in the TCP/IP model.

#### b. TCP (Transmission Control Protocol)

##### i. Characteristics

- Connection-oriented protocol.
- Provides reliable, ordered, and error-checked delivery of data.
- Uses a three-way handshake for connection establishment.

##### ii. Use Cases

- Ideal for applications requiring reliable and accurate data delivery.
- Examples include file transfer (FTP), email (SMTP), and web browsing (HTTP).

#### c. UDP (User Datagram Protocol)

##### i. Characteristics

- Connectionless protocol.
- Provides fast, low-overhead data transmission.
- Lacks error-checking and retransmission of lost packets.

##### ii. Use Cases

- Suitable for real-time applications where low latency is crucial.
- Examples include streaming media (UDP-based RTP), online gaming, and DNS.

#### d. Key Differences

1. **Connection Orientation:**
    
    - TCP is connection-oriented, ensuring data delivery in the correct order.
    - UDP is connectionless, allowing for faster transmission but with no guarantee of order.
2. **Reliability:**
    
    - TCP ensures reliable data delivery through acknowledgment and retransmission.
    - UDP sacrifices reliability for speed and simplicity.

#### e. [[Common Network Ports]]

- Both TCP and UDP use port numbers to identify specific services on a device.
- Well-known ports range from 0 to 1023, registered ports from 1024 to 49151, and dynamic or private ports from 49152 to 65535.