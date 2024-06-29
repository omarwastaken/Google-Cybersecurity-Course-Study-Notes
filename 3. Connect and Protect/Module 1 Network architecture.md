# Networks and Network Security
---
#### In this course, you will:

- Define types of networks
- Explain how data is sent and received over a network
- Recognize common network protocols
- Compare and contrast local networks to cloud computing
- Explain how to secure a network against intrusion tactics

#### Skill sets:

- Configuring a firewall
- Recognizing components of computer networks and cloud computing
- Analysing threats

---
## Network Components, Devices, and Diagrams

Network devices play a crucial role in maintaining information and services for users across wired and wireless connections. Here’s a breakdown of key components and devices:

### Network Devices

Network devices include routers, switches, computers, smartphones, and more. They facilitate data transmission and manage traffic within a network. Data packets are sent and received between devices, conveying information about the source and destination.

### Firewalls

Firewalls act as a primary security defence, monitoring and regulating network traffic. They enforce security rules, controlling incoming and outgoing traffic, especially between secure internal networks and external resources like the internet.

### Servers

Servers provide services and information to client devices. Examples include DNS servers for domain lookups, file servers for data storage, and mail servers for managing corporate emails.

### Hubs and Switches

Hubs provide a central point of connection for devices but are less secure due to repeating information to all ports. Switches, on the other hand, direct data packets more efficiently to intended devices, enhancing security and performance.

### Routers

Routers connect networks and direct traffic based on IP addresses. They facilitate communication between devices on different networks and often include firewall features for added security.

### Modems and Wireless Access Points

Modems link home or office networks to ISPs, translating internet signals for transmission. Wireless access points create wireless networks using Wi-Fi protocols, allowing devices to connect wirelessly.

## Cloud Computing and Software-Defined Networks Study Notes

### Cloud Computing Overview

- **Traditional vs. Cloud Networks**: On-premise networks are kept physically within a company's location, while cloud computing utilizes remote servers and services hosted on the internet.
- **Cloud Service Providers (CSPs)**: Companies offering cloud computing services with large data centres and various service categories:
    - **Software as a Service (SaaS)**: Operated software suites accessible remotely.
    - **Infrastructure as a Service (IaaS)**: Virtual computer components and storage.
    - **Platform as a Service (PaaS)**: Tools for designing custom cloud-based applications.

### Hybrid Cloud Environments

- **Hybrid Cloud**: Combines CSP services with on-premise resources, offering cost-efficiency and resource control.
- **Multi-Cloud**: Involves using multiple CSPs, commonly adopted to reduce reliance on a single provider.

### Software-Defined Networks (SDNs)

- **Virtual Network Devices**: SDNs comprise virtual switches, routers, firewalls, etc., hosted by CSPs.
- **Network Virtualization**: Physical devices use software for packet routing, enhancing flexibility and scalability.

### Benefits of Cloud Computing and SDNs

1. **Reliability**: Consistent access to resources with minimal downtime or interruptions.
2. **Cost Reduction**: Lower upfront costs compared to traditional infrastructure due to shared resources and economies of scale.
3. **Scalability**: Elastic utility model allows companies to scale resources up or down as needed, paying only for what they use.

### Key Takeaways

- **CSPs**: Offer diverse cloud services through remote data centers, enhancing reliability, cost-effectiveness, and scalability.
- **SDNs**: Provide virtualized network components, improving network management and performance.
- **Benefits**: Include reliability, cost reduction, and scalability, making cloud computing and SDNs attractive options for modern businesses.

---
## Introduction to Network Communication

- **Networks and Communication**: Networks facilitate communication and connectivity for organizations, but they also increase the risk of network attacks due to potential vulnerabilities.
- **Data Packets**: Data transfer in networks involves data packets, which are fundamental units of information traveling from one device to another within the network.
- **Composition of Data Packets**: Each data packet contains:
    - Header: Includes the destination's IP address, MAC address, and protocol number indicating how to handle the data.
    - Body: Contains the actual message or data to be transmitted.
    - Footer: Similar to a signature, signals the end of the packet to the receiving device.
- **Analogy to Physical Mail**: Data packets can be likened to physical mail, where the envelope (header), content (body), and signature (footer) mirror the structure of a data packet.
- **Network Performance**: The movement of data packets across a network is indicative of network performance, which can be measured in terms of bandwidth and speed.
- **Bandwidth and Speed**: Bandwidth refers to the amount of data received per second, calculated by dividing data quantity by time. Speed refers to the rate of data packet reception or download.
- **Importance of Network Communication**: Effective network communication is crucial for resource and data sharing within organizations, contributing to operational efficiency.
- **Packet Sniffing**: Security personnel monitor network bandwidth and speed for irregularities, as they can be signs of potential attacks, such as packet sniffing for data inspection.
- **Upcoming Topics**: Further exploration of protocols supporting network communication will be covered to enhance understanding of network functionality.

## Communication Protocols and TCP/IP Model

### Introduction to TCP/IP Model

- **TCP/IP Model**:
    - **Definition**: Transmission Control Protocol and Internet Protocol (TCP/IP) is the standard model for network communication.
    - **Purpose**: Facilitates communication and data streaming between devices across the internet.

### Transmission Control Protocol (TCP)

- **TCP Definition**:
    - Internet communication protocol enabling connection establishment and data streaming.
    - Organizes data into packets for network transmission.
    - Ensures packets reach their intended destination and establishes device connections.

### Internet Protocol (IP)

- **IP in TCP/IP**:
    - **Role**: Routing and addressing data packets across networks.
    - **Function**: Assigns IP addresses to devices, functioning as network identifiers.

### Ports in Network Communication

- **Port Definition**:
    - **Software-based**: Organizes data exchange within network devices.
    - **Segmentation**: Divides network traffic into service-specific segments based on port numbers.
    - **Example Ports**: Port 25 for email, port 443 for secure communication, and port 20 for file transfers.

### TCP/IP Model Layers

1. **Network Access Layer**:
    
    - Creates and transmits data packets across networks.
    - Includes hardware devices and switches managing data flow.
2. **Internet Layer**:
    
    - Attaches IP addresses to data packets for sender-receiver identification.
    - Manages network connections and routing between LANs and remote networks.
3. **Transport Layer**:
    
    - Controls traffic flow and communication permissions.
    - Ensures smooth data transmission and error control across networks.
4. **Application Layer**:
    
    - Determines interaction protocols for receiving devices.
    - Manages functions like file transfers and email services.

### Importance for Security Professionals

- **TCP/IP Model Significance**:
    - Framework for visualizing and understanding data organization and transmission across networks.
    - Enables security professionals to monitor, analyse, and secure network activities effectively.

### Conclusion

- Understanding TCP/IP model layers aids in identifying and resolving network communication issues.
- Proficiency in TCP/IP model structure enhances security monitoring and risk mitigation strategies for network professionals.

## TCP/IP Model

### Introduction to TCP/IP Model

- **Purpose**:
    - Build on understanding TCP/IP model.
    - Compare with OSI model.
    - Learn protocols in each layer.

![The four layers of the TCP/IP model labeled application layer, transport layer, internet layer, and network access layer](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/H9jj1YSsSDKlU8c8qzOgsQ_89f77799b50040b08911a8de1012e2f1_CS_R-210_S33G011-edited.png?expiry=1713744000000&hmac=FGR36CHpNnwFvxbAEstMdF3LaIK0EuWeNVOCIdO4fRM)

### TCP/IP Model Overview

- **Framework**:
    - Visualizes data organization and transmission across networks.
    - Assists in troubleshooting and security analysis.

### Layers of TCP/IP Model

1. **Network Access Layer**:
    
    - **Function**: Creation and transmission of data packets.
    - **Components**: Includes hardware like hubs, modems, and cables.
    - **Protocol**: Address Resolution Protocol (ARP) maps IP to MAC addresses.
2. **Internet Layer**:
    
    - **Responsibility**: Ensures delivery across different networks.
    - **Protocols**: IP for routing, ICMP for error reporting.
3. **Transport Layer**:
    
    - **Role**: Delivers data between systems or networks.
    - **Protocols**: TCP for reliable connection, UDP for connectionless data transfer.
4. **Application Layer**:
    
    - **Purpose**: Manages network requests and applications.
    - **Common Protocols**: HTTP, SMTP, SSH, FTP, DNS.

### TCP/IP Model vs OSI Model
  
![The TCP/IP model next to the OSI model](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/RbNt47PDRTGJZ6q_QtaNMg_9b9098ac04e84c2d8ad04b220c5456f1_CS_R-210_TCP-vs-OSI.png?expiry=1713744000000&hmac=x9ihetEGMBe7rFQtIBjm0D1K5swRHf173CUADALZ0iI)

- **TCP/IP Model**:
    - Simplified version.
    - Combines OSI layers for practical application.
- **OSI Model**:
    - Seven layers, more detailed.
    - Used for communication and troubleshooting.

### Key Takeaways

- TCP/IP and OSI models assist in visualizing network processes.
- TCP/IP model has four layers, OSI model has seven layers.
- Understanding these models aids in networking and security analysis.

## OSI Model

### Introduction to OSI Model

- **Purpose**:
  - Understand network communication processes.
  - Compare TCP/IP and OSI models.

### TCP/IP Model vs OSI Model
  
![The seven layers of the OSI model labeled application, presentation, session, transport, network, data link, and physical](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/b5ghKGCVSp6e-fAUC8oo4w_4efb617fe17648559c4a8a0bc0b1abf1_CS_R-043_OSI-Model.png?expiry=1713744000000&hmac=2Nk1t5t679GrzyLiPqKowUvG0JvJg92zNGJGhzmNfXQ)

- **TCP/IP Model**:
  - Framework for data transmission visualization.
  - Four layers: network access, internet, transport, application.

- **OSI Model**:
  - Standardized concept with seven layers.
  - Used for communication about network issues and security threats.

### OSI Model Layers Overview

1. **Layer 7: Application Layer**:
   - Involves direct user interaction with network.
   - Protocols like HTTP, SMTP, SSH, FTP operate here.

2. **Layer 6: Presentation Layer**:
   - Data translation and encryption for network.
   - SSL encryption for HTTPS websites.

3. **Layer 5: Session Layer**:
   - Establishes and maintains connections between devices.
   - Manages sessions for data transfer.

4. **Layer 4: Transport Layer**:
   - Delivers data between devices.
   - Handles data segmentation and speed of transfer.
   - TCP and UDP are transport layer protocols.

5. **Layer 3: Network Layer**:
   - Routes data packets to intended destinations.
   - Uses IP addresses for routing between networks.

6. **Layer 2: Data Link Layer**:
   - Organizes data packets within a single network.
   - Manages switches and network interface cards (NICs).
   - Uses protocols like NCP, HDLC, and SDLC.

7. **Layer 1: Physical Layer**:
   - Corresponds to physical hardware in network transmission.
   - Includes hubs, modems, cables, and wiring.

### Key Takeaways

- OSI model has seven layers, TCP/IP model has four layers.
- Both models assist in visualizing network processes and protocols.
- Used by network and security professionals for communication and troubleshooting.

---
### Study Notes: Components of Network Layer Communication

#### OSI Model Overview
  - Seven layers conceptualize data transmission across the internet.
  - Focus of this reading is on layer 3: the network layer.

#### Operations at the Network Layer
- **Function**:
  - Organizes addressing and delivery of data packets across the network.
  - Directs packets through routers until reaching the destination IP address.
- **Packet Components**:
  - Header contains source/destination IP, packet size, protocol info.
  - Data section carries the actual message being transmitted.
  
![IPv4 Packet Diagram](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/NHNCeVwQQCCcfSTfEUTolg_afd9af6faf854e3db824471a7f2e56f1_CS_R-044_Edited_IP-packet-header-and-data-final.png?expiry=1713744000000&hmac=XyKSAwNJW6z59uhjVcKJiUbYD6tekCMDHtgqBO9-YN0)

#### IPv4 Packet Format
- **Header Details**:
  - Contains version, header length, type of service, total length, identification, flags, and more.
  - Source and destination IP addresses crucial for routing.
  
![IPv4 Packet Header Diagram](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/ZlTJLULmT_-iQusFt5gHLA_34841ae20ac344f4a0248aebe8f0d6f1_CS_R-044_Edited_Pv4-packet-header-14-field.png?expiry=1713744000000&hmac=Az7BMircE-Vx4a78Rc9LVgKvRRoBj0BDx3bUpZvYSnM)

#### IPv6 Comparison
- **Differences**:
  - IPv4 addresses in decimal, IPv6 in hexadecimal.
  - IPv4: 4.3 billion addresses, IPv6: 340 undecillion addresses.
  - IPv6 simplifies packet header format compared to IPv4.

![IPv4 vs IPv6 Packet Diagram](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/PNld6YkmQNWyhZjFFHvC-Q_eb474e5ee3b3416fbc06a639503342f1_CS_R-044_IPv4-and-IPv6.png?expiry=1713744000000&hmac=pJtMdyRvo9wnsyBiKTbHAf16sEWGDWBxyHa5zX9O8AI)

#### Key Security Considerations
- **Packet Analysis**:
  - IP packet data reveals source, destination, protocol, and more.
  - Helps make critical security decisions during inspection.

---
## Glossary terms from module 1


**Bandwidth:** The maximum data transmission capacity over a network, measured by bits per second

**Cloud computing:** The practice of using remote servers, application, and network services that are hosted on the internet instead of on local physical devices

**Cloud network:** A collection of servers or computers that stores resources and data in remote data centres that can be accessed via the internet

**Data packet:** A basic unit of information that travels from one device to another within a network

**Hub:** A network device that broadcasts information to every device on the network

**Internet Protocol (IP):** A set of standards used for routing and addressing data packets as they travel between devices on a network

**Internet Protocol (IP) address:** A unique string of characters that identifies the location of a device on the internet

**Local Area Network (LAN):** A network that spans small areas like an office building, a school, or a home

**Media Access Control (MAC) address:** A unique alphanumeric identifier that is assigned to each physical device on a network

**Modem:** A device that connects your router to the internet and brings internet access to the LAN

**Network:** A group of connected devices

**Open systems interconnection (OSI) model:** A standardized concept that describes the seven layers computers use to communicate and send data over the network

**Packet sniffing:** The practice of capturing and inspecting data packets across a network

**Port:** A software-based location that organizes the sending and receiving of data between devices on a network

**Router:** A network device that connects multiple networks together

**Speed:** The rate at which a device sends and receives data, measured by bits per second

**Switch:** A device that makes connections between specific devices on a network by sending and receiving data between them

**TCP/IP model:** A framework used to visualize how data is organized and transmitted across a network

**Transmission Control Protocol (TCP):** An internet communication protocol that allows two devices to form a connection and stream data

**User Datagram Protocol (UDP):** A connectionless protocol that does not establish a connection between devices before transmissions

**Wide Area Network (WAN):** A network that spans a large geographic area like a city, state, or country