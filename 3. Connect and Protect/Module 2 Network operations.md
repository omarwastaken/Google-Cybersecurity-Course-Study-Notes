## Network Protocols

**Introduction**

- Networks rely on rules called **network protocols** to ensure data is delivered correctly.
- Protocols define how devices on a network communicate by establishing the order and structure of data transmission.

**Network Protocols in Action - Example**

- You want to access a recipe website (www.yummyrecipesforme.org).
- Your device establishes communication with the web server using **Transmission Control Protocol (TCP)**.
    - TCP allows devices to connect and send data streams.
    - It performs a handshake to verify both devices before data exchange.
- Once connected, your device requests data from the server.
- The server responds by sending data packets back to your device.
- **Address Resolution Protocol (ARP)** helps determine the MAC address of the next device on the data path, ensuring it reaches the right destination.
- **Hypertext Transfer Protocol Secure (HTTPS)** provides a secure communication channel between your browser and the server.
    - HTTPS encrypts data using SSL/TLS for protection against malicious actors.
- To find the web server's address, **Domain Name System (DNS)** translates the domain name (yummyrecipesforme.org) into an IP address.

**Key Points**

- This example highlights four essential protocols: TCP, ARP, HTTPS, and DNS.
- Many other protocols exist in network communication.
- Security protocols like HTTPS play a crucial role in protecting data from unauthorized access.

## Common Network Protocols

**Network Protocols Overview**

- Network protocols are sets of rules that govern communication between devices on a network.
- They define how data is transmitted (order, structure) and act like instructions for receiving devices.
- Protocols are crucial for network communication and understanding them is essential for security analysts.
- Some protocols have security vulnerabilities that attackers can exploit (e.g., DNS).

**Network Protocol Categories**

There are three main categories of network protocols:

1. **Communication Protocols:** Manage information exchange during network transmission.
    
    - Examples: TCP, UDP, HTTP, DNS
2. **Management Protocols:** Used for monitoring and managing network activity.
    
    - Examples: SNMP, ICMP
3. **Security Protocols:** Ensure secure data transmission and reception.
    
    - Examples: HTTPS, SFTP

**Communication Protocols**

- **Transmission Control Protocol (TCP):** Reliable, connection-oriented protocol for data streaming. Uses a three-way handshake to establish a connection. (Transport layer)
- **User Datagram Protocol (UDP):** Connectionless protocol for quick data transmissions. Less reliable than TCP. (Transport layer)
- **Hypertext Transfer Protocol (HTTP):** Application layer protocol for communication between clients and web servers. Often insecure (HTTP) and replaced by secure version (HTTPS). (Application layer)
- **Domain Name System (DNS):** Translates domain names into IP addresses. Uses UDP on port 53 (default). (Application layer)

**Management Protocols**

- **Simple Network Management Protocol (SNMP):** Used for monitoring and managing network devices. Can reset passwords, change configurations, and report on bandwidth usage. (Application layer)
- **Internet Control Message Protocol (ICMP):** Used by devices to communicate about data transmission errors. Commonly used for network troubleshooting with "ping" command. (Internet layer)

**Security Protocols**

- **Hypertext Transfer Protocol Secure (HTTPS):** Secure version of HTTP that encrypts data transmissions using SSL/TLS for protection against eavesdropping. Uses port 443. (Application layer)
- **Secure File Transfer Protocol (SFTP):** Secure protocol for transferring files over a network. Uses SSH (typically on port 22) with encryption to ensure data confidentiality. (Application layer)

**Key Points**

- This reading covers essential network protocols for entry-level security analysts.
- Understanding protocol functionality is crucial for network security and vulnerability mitigation.
- Encryption protocols (like those used in HTTPS and SFTP) protect data content, but not source or destination IP addresses.

## Network Protocols: Additional Concepts

**Network Address Translation (NAT)**

- Enables devices with private IP addresses on a local network to access the public internet using a single public IP address assigned by the router.
- Router translates private source IP addresses to public IP for outgoing messages and vice versa for incoming responses.
- Typically configured on routers or firewalls.
- Operates at Layer 2 (Internet layer) and Layer 3 (Transport layer) of the TCP/IP model.

**Private vs Public IP Addresses**

- Private IP addresses:
    - Assigned by the router within a private network.
    - Not unique on the global internet.
    - Free to use.
    - Example ranges: 10.0.0.0 - 10.255.255.255, 172.16.0.0 - 172.31.255.255, 192.168.0.0 - 192.168.255.255
- Public IP addresses:
    - Assigned by ISP and IANA (Internet Assigned Numbers Authority).
    - Unique globally on the internet.
    - May incur costs for leasing.
    - Example ranges: 1.0.0.0 - 9.255.255.255, 11.0.0.0 - 126.255.255.255, etc.

**Dynamic Host Configuration Protocol (DHCP)**

- Management protocol used to automatically configure network devices.
- Assigns unique IP addresses to each device on a network.
- Provides DNS server and default gateway addresses to devices.
- Operates on UDP port 67 (servers) and UDP port 68 (clients).

**Address Resolution Protocol (ARP)**

- Network access layer protocol used to translate IP addresses into MAC addresses.
- Devices maintain an ARP cache to store IP-MAC address mappings.
- Doesn't have a specific port number as it operates at Layer 2 (no ports used).

**Telnet vs Secure Shell (SSH)**

- Telnet:
    - Application layer protocol for remote system connection.
    - Uses clear text for communication (not secure).
    - Uses command line prompts for control.
    - Uses TCP port 23.
- SSH:
    - Secure alternative to Telnet for remote connections.
    - Provides secure authentication and encrypted communication.
    - Uses TCP port 22.

**Mail Protocols**

- Post Office Protocol (POP):
    - Application layer protocol for managing and retrieving email from a mail server.
    - POP3 (most common version) downloads emails locally.
    - Uses TCP/UDP port 110 (unencrypted) or 995 (encrypted with SSL/TLS).
    - Emails need to be downloaded completely before reading.
    - Doesn't guarantee syncing across multiple devices.
- Internet Message Access Protocol (IMAP):
    - Used for accessing and managing incoming emails.
    - Downloads email headers and content, remaining on the server for multi-device access.
    - Uses TCP port 143 (unencrypted) or 993 (encrypted with TLS).
    - Allows partial reading before download completion and syncing across devices.

**Simple Mail Transfer Protocol (SMTP)**

- Used for transmitting and routing emails between sender and recipient.
    - Works with Message Transfer Agent (MTA) software for email delivery.
    - Uses TCP/UDP port 25 (unencrypted) or 587 (encrypted with TLS).
    - Port 25 commonly used for spam.
    - Helps regulate email volume by source.

**Key Takeaways**

- Cybersecurity analysts encounter various protocols daily (NAT, DHCP, ARP, Telnet, SSH, POP3, IMAP, SMTP).
- Understanding protocol location within the TCP/IP model and associated port numbers is crucial.

## Evolution of Wireless Security Protocols

**Early Wireless Communication**

The internet initially relied on physical cables for communication. In the mid-1980s, the US designated a radio wave frequency spectrum for unlicensed use, enabling wireless internet access.

**Introduction to Wireless Communication Protocols**

Wi-Fi refers to a set of standards for wireless LAN (Local Area Network) communication defined by the Wi-Fi Alliance (formerly WECA). These standards are based on the IEEE 802.11 family of internet communication protocols. Wi-Fi security is ensured by wireless networking protocols, which have evolved over time.

**The Evolution of Wireless Security Protocols**

This section explores the evolution of wireless security protocols, from Wired Equivalent Privacy (WEP) to WPA, WPA2, and WPA3. It also covers the Wireless Application Protocol (WAP) used for mobile internet communication.

- **Wired Equivalent Privacy (WEP)** (1999)
    
    - Aimed to provide similar privacy on wireless networks as wired networks.
    - Considered outdated and highly vulnerable due to weak encryption and protocol flaws.
    - May still be encountered in older devices or network routers.
- **Wi-Fi Protected Access (WPA)** (2003)
    
    - Developed to address WEP's security issues.
    - Introduced Temporal Key Integrity Protocol (TKIP) for stronger encryption.
    - Implemented message integrity checks for transmission verification.
    - Still vulnerable to KRACK attacks (key reinstallation attacks).
- **WPA2** (2004)
    
    - Improved security over WPA by using Advanced Encryption Standard (AES).
        
    - Employed Counter Mode Cipher Block Chaining Message Authentication Code Protocol (CCMP) for message authentication and integrity.
        
    - Considered the current security standard for Wi-Fi due to its strength.
        
    - Susceptible to KRACK attacks similar to WPA.
        
        - **WPA2 Personal:** Ideal for home networks due to its ease of setup. Requires a global passphrase for all devices.
        - **WPA2 Enterprise:** Designed for businesses, offering centralized control over Wi-Fi access and user management. Users lack access to encryption keys.
- **WPA3** (2018)
    
    - The most secure Wi-Fi protocol with growing adoption as compatible devices become available.
    - Addresses KRACK attack vulnerabilities present in WPA2.
    - Utilizes Simultaneous Authentication of Equals (SAE) to prevent attackers from capturing and decrypting network data.
    - Provides stronger password encryption with 128-bit encryption (optional 192-bit encryption in WPA3-Enterprise mode).


**Conclusion**

Understanding the evolution of wireless security protocols is crucial for security analysts. This knowledge helps them identify potential vulnerabilities in wireless networks and implement appropriate security measures. WPA3 offers the most robust security currently available, and its adoption is expected to increase as compatible devices become more widespread.

---
## Firewalls: Protecting Your Network

Firewalls are network security devices that monitor incoming and outgoing traffic, allowing or blocking it based on a set of security rules. They act as a barrier between your network and the wider internet, filtering out potentially harmful traffic.

### Types of Firewalls

Firewalls come in three main varieties:

- **Hardware Firewalls:** These are physical devices that sit between your network and the internet. They inspect each data packet before it enters the network, providing a strong layer of defence.
    
- **Software Firewalls:** These are programs installed on individual computers or servers. They offer similar functionality to hardware firewalls but can slow down the device they're installed on.
    
- **Cloud-based Firewalls (FWaaS):** Offered by cloud service providers, these firewalls are hosted in the cloud and protect your network traffic before it reaches your physical location. They're a good option for organizations that leverage cloud-based resources.
    

### Stateful vs. Stateless Firewalls

Firewalls can be classified into stateful or stateless based on how they handle traffic:

- **Stateful Firewalls:** These firewalls maintain a record of network connections and use this information to make informed decisions about allowing or blocking traffic. They can identify suspicious behaviour and proactively block potential threats.
    
- **Stateless Firewalls:** These firewalls rely solely on predefined rules to filter traffic. They don't track connection history and offer a less sophisticated level of security compared to stateful firewalls.
    

**Choosing Between Stateful and Stateless Firewalls:**

Stateful firewalls provide more comprehensive security due to their ability to analyse traffic patterns and identify suspicious activities. However, they can be more complex to configure and manage. Stateless firewalls are simpler to set up but offer a lower level of protection.

### Next-Generation Firewalls (NGFWs)

NGFWs are advanced firewalls that go beyond basic traffic filtering. They offer features like:

- **Deep Packet Inspection:** Examines the content of data packets for malware and other threats.
- **Intrusion Prevention:** Actively blocks suspicious attempts to access your network.
- **Threat Intelligence Updates:** Continuously update their defences against emerging cyber threats.

NGFWs provide the most robust security but come at a higher cost and require more technical expertise to manage.

## Virtual Private Networks (VPNs): Protecting Your Online Privacy

VPNs are network security services that enhance your online privacy and data security. Let's delve into how VPNs work to achieve this:

### The Problem: Exposed Data on Public Networks

When you use the internet, your internet service provider (ISP) routes your requests to their destination servers. This internet traffic contains your private information, making you vulnerable to eavesdropping. If someone intercepts this traffic, they could potentially:

- Link your online activity to your physical location.
- Access sensitive information like bank accounts or credit card numbers.

VPNs address these concerns by providing solutions for both privacy and security.

### How VPNs Work

VPNs create a secure tunnel between your device and a VPN server. This tunnel encrypts your data, making it unreadable to anyone who might intercept it. Here's a breakdown of the process:

1. **IP Address Masking:** A VPN hides your public IP address, the unique identifier assigned to your network by your ISP. Instead, websites and online services will see the IP address of the VPN server, masking your location and identity.
    
2. **Data Encryption:** VPNs encrypt your data packets using a secure encryption algorithm. This encryption scrambles the data, rendering it indecipherable without a special key. Even if someone intercepts the data, they cannot access the information it contains.
    
3. **Encapsulation:** VPNs encapsulate your encrypted data packets within another layer of data. This outer layer contains the destination address, allowing network routers to properly route the data packets while keeping your private information hidden within.
    

**The Analogy of a Secure Mailbox:**

Imagine a VPN as a secure mailbox. You place your message (data) inside a sealed envelope (encryption) and put it in a locked box (VPN tunnel). The locked box is then delivered to the recipient's address (destination server). The recipient unlocks the box (VPN server) to access your message (data), which remains confidential throughout the process.

### Benefits of Using a VPN

- **Enhanced Privacy:** VPNs shield your online activity and location from prying eyes, making it more difficult to be tracked by websites, advertisers, or even your ISP.
    
- **Data Security:** Encryption safeguards your data from unauthorized access, especially on untrusted public Wi-Fi networks.
    
- **Access Geo-Restricted Content:** Some websites or streaming services restrict content based on geographical location. A VPN can allow you to connect to a server in a different location, potentially bypassing these restrictions (**Note:** This may violate the terms of service of some websites).

## Network Security Zones: Segmentation for Enhanced Protection

Security zones are a network security strategy that segments a network into isolated sections. This approach, also known as network segmentation, improves overall network security by controlling access and preventing issues from spreading.

### Benefits of Security Zones

- **Improved Security:** Segmenting the network creates barriers between different sections, making it more difficult for unauthorized users or malware to infiltrate critical systems.
    
- **Privacy and Access Control:** Security zones allow organizations to define specific access permissions for each segment. This ensures that only authorized users can access sensitive data within the network.
    
- **Reduced Impact of Security Incidents:** If a security breach occurs within one zone, the damage can be contained, preventing it from spreading to the entire network.
    

### Network Segmentation with Security Zones

Here's how security zones are typically implemented:

1. **Uncontrolled Zone (External Network):** This refers to any network outside the organization's control, such as the internet. It represents the least secure zone.
    
2. **Controlled Zone (Internal Network):** This zone encompasses the organization's internal network and is further divided into subnets for departments or specific purposes.
    
    - **Demilitarized Zone (DMZ):** Located between the internal network and the uncontrolled zone, the DMZ houses public-facing services like web servers, email servers, and DNS servers. It acts as a buffer zone, protecting the internal network from external threats.
        
    - **Internal Network:** This zone contains an organization's private servers and sensitive data.
        
    - **Restricted Zone (Optional):** This highly secure zone safeguards critical data and is only accessible to authorized personnel with special privileges.
        

### Firewalls and Security Zones

Firewalls play a crucial role in securing network zones:

- **Double Firewall Protection for the DMZ:** Ideally, the DMZ is positioned between two firewalls. One firewall filters traffic entering the DMZ from the uncontrolled zone, while the other filters traffic leaving the DMZ towards the internal network. This provides a multi-layered defence.
    
- **Firewall Control of Access:** Security teams can configure firewalls to manage traffic flow within the network zones. This may involve restricting access based on IP addresses or ports. For instance, a firewall might be set to allow only secure HTTPS traffic to reach web servers in the DMZ.

## Subnetting and CIDR: Efficient Network Management

Subnetting and CIDR are fundamental concepts in network security that enable efficient network management and enhanced security.

### Subnetting: Dividing a Network

Subnetting is the process of dividing a large network into smaller, logical subnets. Imagine a large network as a big apartment complex. Subnetting creates smaller, self-contained units (subnets) within the complex, improving organization and manageability.

Here's how subnetting works:

- **Network Address Range:** A network address range is a block of IP addresses allocated to a network.
    
- **Subnet Mask:** A subnet mask is a 32-bit number that defines the network portion (subnet address) and the host portion (usable IP addresses) within an IP address.
    
- **Subnet Creation:** By applying a subnet mask to the network address range, we create subnets. Each subnet has its own network address and a pool of usable IP addresses for devices within that subnet.
    

**Benefits of Subnetting:**

- **Improved Network Efficiency:** Subnetting reduces network congestion by creating smaller broadcast domains. This means broadcasts are limited to specific subnets, improving overall network performance.
    
- **Enhanced Security:** Subnetting allows for the creation of security zones. By isolating sensitive data on separate subnets, we can implement stricter access controls and firewalls, minimizing the impact of security breaches.
    
- **Better Scalability:** Subnetting facilitates easier network expansion. As a network grows, new subnets can be created within the existing network address range to accommodate additional devices.
    

### CIDR Notation: Simplifying Subnetting

CIDR (Classless Inter-Domain Routing) notation is a shorthand method for representing subnets. It combines the IP address with a forward slash (/) followed by a number indicating the number of contiguous 1s in the subnet mask.

Here's an example:

- IP Address: 192.168.1.0
- Subnet Mask: 255.255.255.0 (written in binary as 11111111.11111111.11111111.00000000)

**CIDR Notation:** 192.168.1.0/24

The /24 in the CIDR notation signifies that the first 24 bits of the IP address (192.168.1) represent the network portion, and the remaining 8 bits (0) define the usable host addresses within the subnet.

**Benefits of CIDR Notation:**

- **Simplicity:** CIDR notation provides a concise way to represent subnets, making it easier to understand and manage network configurations.
    
- **Efficiency:** CIDR simplifies routing table entries, improving network performance.

## Securing Internal Networks with Proxy Servers

Proxy servers are a valuable tool for enhancing internal network security. They act as intermediaries between a client computer on the internal network and the internet.

### How Proxy Servers Work

- **Client-Server Interaction:** When a user on the internal network requests a website, the request is first sent to the proxy server.
    
- **Filtering and Security Checks:** The proxy server acts as a gatekeeper, analysing the request to determine if it's safe. It can block access to malicious websites or content.
    
- **Hiding Internal Network IP:** The proxy server has its own public IP address that interacts with the internet. This masks the private IP addresses of devices within the internal network, adding a layer of security.
    
- **Improved Efficiency:** Proxy servers can cache frequently accessed data, reducing the need to fetch it directly from internal servers every time. This lessens the load on internal servers and improves overall network performance.
    

### Benefits of Proxy Servers

- **Enhanced Security:** Proxy servers filter incoming and outgoing traffic, blocking access to malicious websites and protecting internal systems from external threats.
    
- **Privacy:** Proxy servers hide the internal network's IP addresses, making it more difficult for attackers to target specific devices.
    
- **Content Filtering:** Organizations can use proxy servers to restrict access to inappropriate or unproductive websites.
    
- **Improved Performance:** Caching frequently accessed data reduces traffic on internal servers, leading to faster network performance.
    

### Types of Proxy Servers

- **Forward Proxy Server:** This is the most common type. It sits between the client and the internet, filtering outgoing traffic and hiding internal IP addresses.
    
- **Reverse Proxy Server:** This type acts as a shield for internal servers. It receives incoming traffic from the internet, validates it, and then forwards it to the appropriate internal server while hiding the server's IP address.
    
- **Email Proxy Server:** This specialized proxy filters incoming emails to identify and block spam messages. It helps prevent phishing attacks by verifying sender addresses.
    

### Real-World Example

A large internet service provider (ISP) used a proxy server to implement multi-layered spam filtering for incoming emails. This approach effectively filtered out nearly 95% of spam messages before they reached user inboxes. The proxy server allowed for efficient filtering without impacting the core email platform.

## Network Security Refresher
### Network Security Goals

- **Confidentiality:** Ensuring only authorized users can access sensitive data.
    
- **Integrity:** Maintaining the accuracy and completeness of data.
    
- **Availability:** Guaranteeing authorized users have timely access to data and resources.
    

### Network Security Tools and Practices

- **Firewalls:** Hardware or software devices that filter incoming and outgoing network traffic based on predefined security rules.
    
    - **Stateless Firewalls:** These basic firewalls make filtering decisions based on individual data packets without considering connection history.
        
    - **Stateful Firewalls:** These more advanced firewalls maintain a state table to track connections, allowing for more dynamic filtering decisions.
        
    - **Next-Generation Firewalls (NGFWs):** The most sophisticated firewalls, NGFWs offer deep packet inspection, intrusion prevention features, and application-layer filtering capabilities.
        
- **Proxy Servers:** Intermediary servers that act as a barrier between internal network clients and external threats.
    
    - **Forward Proxy Servers:** Manage requests from internal clients accessing external resources.
        
    - **Reverse Proxy Servers:** Handle requests from external systems directed to internal network services.
        
    - **Filtering Proxy Servers:** Can be configured with rules to block malicious websites or content.
        
- **Virtual Private Networks (VPNs):** Create secure tunnels for encrypted data transmission across public networks.
    
    - **Encapsulation:** VPNs wrap unencrypted data within encrypted packets for secure transmission.
        
    - **IP Address Masking:** VPNs conceal your true IP address, enhancing privacy.
        
    - **Use Cases:** VPNs are used by businesses to secure communication between user devices and corporate resources, and by individuals for increased online privacy.
        
- **Network Protocols:** Defined rules governing communication between network devices.
    
    - **Communication Protocols:** Establish connections between servers (e.g., TCP, UDP, SMTP).
        
    - **Management Protocols:** Facilitate network troubleshooting (e.g., ICMP).
        
    - **Security Protocols:** Provide data encryption during transmission (e.g., IPSec, SSL/TLS).
        
    - **Application Layer Protocols:**
        
        - **HTTP:** Enables communication between web browsers and servers.
            
        - **DNS:** Translates domain names into corresponding IP addresses.
            
        - **ARP:** Maps IP addresses to physical devices on a local network.
            
- **Wireless Security Protocols:** Secure communication over Wi-Fi networks.
    
    - **WEP, WPA, WPA2, WPA3:** Encryption protocols offering varying levels of security (WPA3 is the most secure).
        
    - **Personal vs. Enterprise Modes:** Personal mode is suitable for home networks, while enterprise mode is better suited for businesses.

## Understanding VPN Protocols: WireGuard vs. IPSec

Virtual Private Networks (VPNs) secure your online activity by encrypting data and masking your IP address. Different VPN protocols dictate how this secure tunnel is established. This study guide explores two common protocols: WireGuard and IPSec.

### VPN Protocols: The Rulebook for Secure Connections

Imagine a VPN protocol as a rulebook for building a secure tunnel. It defines how data travels between endpoints (devices) within the tunnel. By choosing the right protocol, you can balance factors like speed, security, and ease of use.

### Remote Access vs. Site-to-Site VPNs

- **Remote Access VPNs:** Designed for individual users. They encrypt data traveling between a personal device (like a laptop) and a remote VPN server.
    
- **Site-to-Site VPNs:** Used by businesses to connect geographically separate networks. They create an encrypted tunnel between two networks, often using IPSec.
    

### WireGuard VPN: Speedy and Simple

- **Pros:**
    
    - **High Speeds:** Ideal for streaming or downloading large files due to its efficient code.
    - **Simple Setup:** Easy to configure and maintain.
    - **Open Source:** Open code allows for transparency and easy troubleshooting.
- **Cons:**
    
    - **Newer Technology:** Less established compared to IPSec.

### IPSec VPN: The Established Choice

- **Pros:**
    
    - **Widely Supported:** Compatible with most devices and operating systems.
    - **Extensive Testing:** Well-tested and proven secure.
    - **Mature Technology:** A reliable and longstanding protocol.
- **Cons:**
    
    - **Slower Speeds:** May be slower than WireGuard due to its more complex design.
    - **Complex Setup:** Configuration can be more challenging for non-technical users.

### Choosing the Right Protocol

The best protocol depends on your needs:

- **For speed and simplicity:** WireGuard is a strong choice, especially for streaming or downloading large files.
    
- **For established security and broad compatibility:** IPSec might be preferable, particularly for business use.
    

**Remember:** Both WireGuard and IPSec offer secure connections. Consider your priorities (speed, ease of use, or established security) when making your choice.

---
# Glossary terms from module 2

**Address Resolution Protocol (ARP):** A network protocol used to determine the MAC address of the next router or device on the path

**Cloud-based firewalls:** Software firewalls that are hosted by the cloud service provider

**Controlled zone:** A subnet that protects the internal network from the uncontrolled zone

**Domain Name System (DNS):** A networking protocol that translates internet domain names into IP addresses

**Encapsulation:** A process performed by a VPN service that protects your data by wrapping sensitive data in other data packets

**Firewall:** A network security device that monitors traffic to or from your network

**Forward proxy server:** A server that regulates and restricts a person’s access to the internet

**Hypertext Transfer Protocol (HTTP):** An application layer protocol that provides a method of communication between clients and website servers

**Hypertext Transfer Protocol Secure (HTTPS):** A network protocol that provides a secure method of communication between clients and servers

**IEEE 802.11 (Wi-Fi):** A set of standards that define communication for wireless LANs

**Network protocols:** A set of rules used by two or more devices on a network to describe the order of delivery of data and the structure of data

**Network segmentation:** A security technique that divides the network into segments

**Port filtering:** A firewall function that blocks or allows certain port numbers to limit unwanted communication

**Proxy server:** A server that fulfils the requests of its clients by forwarding them to other servers

**Reverse proxy server:** A server that regulates and restricts the internet's access to an internal server

**Secure File Transfer Protocol (SFTP):** A secure protocol used to transfer files from one device to another over a network

**Secure shell (SSH):** A security protocol used to create a shell with a remote system 

**Security zone:** A segment of a company’s network that protects the internal network from the internet

**Simple Network Management Protocol (SNMP):** A network protocol used for monitoring and managing devices on a network

**Stateful:** A class of firewall that keeps track of information passing through it and proactively filters out threats 

**Stateless:** A class of firewall that operates based on predefined rules and does not keep track of information from data packets

**Subnetting:** The subdivision of a network into logical groups called subnets

**Transmission Control Protocol (TCP):** An internet communication protocol that allows two devices to form a connection and stream data

**Uncontrolled zone:** The portion of the network outside the organization

**Virtual private network (VPN):** A network security service that changes your public IP address and masks your virtual location so that you can keep your data private when you are using a public network like the internet

**Wi-Fi Protected Access (WPA):** A wireless security protocol for devices to connect to the internet