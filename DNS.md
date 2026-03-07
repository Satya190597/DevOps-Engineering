# DNS (Domain Name System
DNS uses a request-response protocol primarily over **UDP** port **53** for fast queries, falling back to TCP for larger responses or zone transfers.
## Why DNS?
- Difficult to remember IPs.
- A domain name is a text points to an **IP** or a collection of **IPs**.
- IP can change while the domain remain the same.
- We can server the closest IP to a client requesting the same domain.
- Load balancing.
## Local Machine To DNS.
- Domain name needs **IP** to identify the requested machine.
- An **IP** needs **MAC address** to locate the requested machine witin a **local network**.
  
| DNS         |
|-------------|
| Domain Name |
| IP          |
| MAC Address |
