# TCP
- Stands for Transmission Control Protocol.
- It's a layer 4 Protocol (Layer 4 protocols operate at the **transport layer** of the OSI model).
- Ability to address processes in a host using **ports**.
- **Controls** the transmission unlike **UDP** which is a firehose.
- Requires handshake.
- **20** bytes headers segment (can go to 60).
- Stateful.

## TCP Use Cases.
- 🏹 Reliable communication.
- 🏹 Remote shell.
- 🏹 Database connections.
- 🏹 Web communications.
- 🏹 Any bidirectional communication.

## What Is TCP Connection?
A TCP connection refers to a reliable, connection-oriented communication channel established between two endpoints using the **Transmission Control Protocol** at the transport layer. 
It ensures data is delivered in order, without errors or loss, through mechanisms like **handshakes** and **acknowledgments**. 
A connection is identified by 4 properties.
- SourceIP-SourcePort.
- DestinationIP-DestinationPort.

## How TCP Connection Work?
 - App 1 (10.0.0.1) on port **5555** want to send data to App X (10.0.0.2) on port **22**.
 - App 1 sends SYN to App X to synchronous sequence number.
 - App X sends SYN/ACK to synchronous it's sequence number.
 - App 1 ACKs App X SYN.
 - Three way handshake.

![TCP Three Way Handshake](./assets/images/tcp-connection-flow-three-way-handshake.png)

### Sending Data.
- App 1 sends data to App X.
- App 1 encapsulate the data in a segment and send it.
- App X acknowledge the segment.

![TCP Sending Data](./assets/images/tcp-sending-data.png)

## Flow Control
Flow control refers to the mechanism that ensures a sender does not **overwhelm** a receiver by sending more data than the receiver can process or store in its buffer. It is essential for maintaining reliable communication and preventing packet loss due to buffer overflow.

### How TCP Implements Flow Control.
- **Sliding Window Protocol:** TCP uses a dynamic sliding window mechanism. The receiver advertises a window size (called the receive window) to the sender, indicating how much data it can accept without acknowledgment.
- **Advertised Window:** This value is sent in the TCP header and updated as the receiver processes data. The sender must respect this limit.
- **Dynamic Adjustment:** As the receiver consumes data and frees buffer space, it updates the window size, allowing the sender to transmit more data.

### Flow Control Example - Scenario 1 (Sender Sends Each Segment Synchronously And Wait For Acknowledgment).
- A wants to send 10 segment to B.
- A sends segment 1 to B.
- B acknowledges segment 1.
- A sends segment 2 to B.
- B  acknowledges segment 2.
- The entire process is extremely slow.

![TCP Flow Control Scenario One](./assets/images/tcp-slow-flow-control.png)




## ✅ TCP Pros
- **Guarantee** Delivery.
- Much more secure than UDP - (No one can send data without prior knowledge).
- Flow Control and Congestion Control.
- **Ordered Packets** no corruption.
- Secure and can't be easily spoofed.
- Inherently supports **retransmission** by default.

## ❌ TCP Cons
- Large header overhead compared to UDP.
- More bandwidth.
- Stateful: consumes memory on server and client.
- Considered high latency for certain workloads.
- Does too much at a low level.
  - Single connection to send multiple streams of data (HTTP requests).
  - Stream 1 has nothing to do with Stream 2.
  - Both Stream 1 and Stream 2 packets must arrive.
- TCP Meltdown
  - Not a good candidate for **VPN**.



Note:
How TCP is Different from WebSockets.
