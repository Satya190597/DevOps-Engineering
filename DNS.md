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
## Types Of DNS Records.
DNS records are key-value pairs stored in DNS zones that map domain names to data like IP addresses or services, enabling resolution queries.
|DNS Record|Purpose|
|----------|-------|
| A        | Maps domain to IPv4 address               |
| AAAA     | Maps domain to IPv6 address               |
| CNAME    | Maps one domain to another                |
| MX       | Email server info                         |
| TXT      | Extra text for security (e.g., SPF, DKIM) |
| NS       | Nameserver for a domain                   |
| PTR      | Reverse DNS lookup (IP to domain)         |
