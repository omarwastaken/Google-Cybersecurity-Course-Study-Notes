# Understand network traffic

## The Importance of Network Traffic Flows

### Network Traffic Flows Overview

Network communication in many organizations involves data traveling over multiple networks across different countries and devices. It's crucial for security professionals to ensure that data is securely transmitted and stored, especially since it can unintentionally end up in insecure places like personal email inboxes or cloud storage platforms.

### Key Concepts

#### Network Traffic

Network traffic refers to the amount of data that moves across a network. This data is transmitted between devices on the network.

#### Network Data

Network data is the actual information that is transmitted between devices. This can include emails, files, and other forms of digital communication.

### Network Traffic Analysis

#### Importance of Network Traffic Analysis

Network traffic analysis involves monitoring and analyzing the data that moves across a network to identify potential malicious activity. This is critical for maintaining the security and integrity of the network.

#### Normal vs. Abnormal Traffic

Understanding what constitutes normal network traffic is essential for spotting abnormalities that may indicate a security incident.

### Traffic Patterns

#### Expected Traffic Flows

Like daily traffic patterns on roads, network traffic has peak times and expected behaviours. For example, in a large multinational organization, there may be thousands of employees sending and receiving emails during business hours.

#### Abnormal Traffic Flows

Unexpected changes in traffic patterns can indicate issues such as data breaches or other security incidents. For example, abnormal traffic during off-peak times or large volumes of outbound traffic may signal potential data exfiltration.

### Indicators of Compromise (IoC)

#### Definition

Indicators of compromise (IoC) are observable signs that suggest a potential security incident. These can include unusual network traffic patterns, unexpected system behaviour, or unauthorized data transfers.

#### Example: Data Exfiltration

Data exfiltration is the unauthorized transmission of data from a system. Attackers may use this method to steal sensitive information. Indicators of data exfiltration can include large volumes of outbound traffic, which should be further investigated.

### Key Takeaways

1. **Monitor Network Traffic:** Regularly monitor network traffic to understand normal patterns and identify abnormalities.
2. **Identify Indicators of Compromise:** Look for signs of potential security incidents, such as unusual outbound traffic volumes.
3. **Secure Data Transmission:** Implement security controls like data classification and encryption to protect data in transit and at rest.

## Maintain Awareness with Network Monitoring

### Network Communication and Monitoring

Network communication can be noisy with events like sending an email, streaming a video, or visiting a website producing network traffic and network data.

- **Network traffic**: The amount of data that moves across a network. It can also include the type of data that is transferred, such as HTTP.
- **Network data**: The data that’s transmitted between devices on a network.

Network monitoring is essential in maintaining situational awareness of any activity on a network. By collecting and analysing network traffic, organizations can detect suspicious network activity.

### Know Your Network

Networks connect devices, and devices then communicate and exchange data using network protocols. Network communications provide information about connections such as source and destination IP addresses, the amount of data transferred, date and time, and more. This information is valuable for security professionals when developing a **baseline** of normal or expected behaviour.

A **baseline** is a reference point used for comparison to identify patterns or changes in network behaviour.

### Monitor Your Network

Once a baseline is determined, monitoring a network involves examining network components to detect unusual activities, such as large and unusual data transfers.

#### Flow Analysis

Flow refers to the movement of network communications and includes information related to packets, protocols, and ports.

- **Command and Control (C2)**: Techniques used by malicious actors to maintain communications with compromised systems.

#### Packet Payload Information

Network packets contain components related to the transmission of the packet. This includes details like source and destination IP addresses and the packet payload information (the actual data transmitted).

#### Temporal Patterns

Network packets contain time-related information useful in understanding time patterns. Abnormal traffic patterns, such as large volumes of traffic outside normal operating hours, can indicate potential security incidents.

### Protect Your Network

Organizations may deploy a **Security Operations Centre (SOC)** and a **Network Operations Centre (NOC)**.

- **SOC**: Focuses on maintaining the security of an organization through detection and response.
- **NOC**: Responsible for maintaining network performance, availability, and uptime.

Security analysts monitor networks to identify potential security incidents known as **Indicators of Compromise (IoC)**.

### Network Monitoring Tools

Network monitoring can be automated or performed manually.

- **Intrusion Detection Systems (IDS)**: Monitor system activity and alert on possible intrusions.
- **Network Protocol analysers**: Also known as packet sniffers, are tools designed to capture and analyse data traffic within a network. Examples include tcpdump and Wireshark.

### Key Takeaways

Monitoring and protecting networks from intrusions and attacks are key responsibilities of security professionals. Understanding the components of a network and the communications that happen on it is essential for better protection.

## Data Exfiltration Attacks

### Monitoring Network Traffic

Monitoring network traffic is crucial for detecting, preventing, and responding to attacks. By monitoring deviations from typical network traffic patterns, security professionals can yield significant results. Even if information is encrypted, monitoring network traffic remains vital for security purposes.

### The Attacker's Perspective

1. **Initial Access**
    
    - **Phishing Attacks**: Attackers gain initial access through social engineering tactics like phishing. They send phishing emails with malicious attachments or links that trick targets into entering their credentials.
2. **Lateral Movement**
    
    - After gaining access, attackers aim to maintain and expand their access by exploring the network. This tactic is known as lateral movement or pivoting. They search for valuable assets, such as sensitive data, proprietary code, PII (names, addresses), and financial records.
3. **Identifying and Collecting Data**
    
    - Attackers identify valuable assets in locations like network file shares, intranet sites, and code repositories. They then collect, package, and prepare the data for exfiltration, often by reducing the data size to avoid detection and bypass security controls.
4. **Data Exfiltration**
    
    - Attackers exfiltrate the data to their destination of choice. Methods include emailing the stolen data to themselves using the compromised email account.

### Defending Against Data Exfiltration

1. **Preventing Attacker Access**
    
    - Use methods like multi-factor authentication (MFA) to protect the network from phishing attempts.
2. **Monitoring Network Activity**
    
    - Security teams should monitor network activity to identify suspicious activities indicating a compromise, such as multiple user logins from IP addresses outside the network.
3. **Asset Protection**
    
    - Identify, classify, and protect assets using asset inventories and security controls. Catalog all assets in an asset inventory and apply appropriate security controls to protect them from unauthorized access.
4. **Detecting and Stopping Data Exfiltration**
    
    - Indicators of unusual data collection can be identified through network monitoring. Indicators include large internal file transfers, large external uploads, and unexpected file writes.
    - Use SIEM tools to detect and alert on these activities. Once an alert is sent, security teams investigate and stop the attack by methods such as blocking the attacker's IP addresses using firewall rules.

### Key Takeaways

- **Importance of Monitoring**: Monitoring network traffic helps in early detection and response to data exfiltration attacks.
- **Attackers' Tactics**: Understanding the attackers' tactics, from initial access to data exfiltration, helps in defending against such attacks.
- **Preventive Measures**: Implementing multi-factor authentication, continuous network monitoring, and robust asset protection measures are crucial.
- **Detection Tools**: Utilizing tools like SIEM for detecting and responding to suspicious activities ensures prompt action against potential threats.

### Resources

- [MITRE ATT&CK® - Data Exfiltration Techniques](https://attack.mitre.org/tactics/TA0010/)
- [Network Traffic - MITRE ATT&CK®](https://attack.mitre.org/datasources/DS0029/)

---
# Capture and view network traffic

## Packets and Packet Captures

### Understanding Network Traffic

- Network traffic involves all data that is transmitted across a network.
- Monitoring network traffic flows helps identify activities performed on the network, whether by legitimate users or malicious actors.

### What is a Packet?

- **Packets** are small units of data sent over a network.
- Each packet contains:
    - **Header**: Contains delivery information, including the sender and receiver's IP address, type of packet, network protocol, and port.
    - **Payload**: Contains the actual data being transmitted.
    - **Footer**: Indicates the end of the packet.

### Components of a Packet

|Component|Description|
|---|---|
|Header|Includes the type of network protocol, port being used, source and destination IP addresses. It's like the name and mailing address on an envelope.|
|Payload|The actual data being sent, similar to the content inside an envelope.|
|Footer|Signifies the end of the packet.|

### Network Protocols and Ports

- **Network protocols**: Rules that determine how data is transmitted between devices.
- **Ports**: Non-physical locations on a computer that manage data transmission.

### Packet Sniffers

- **Packet sniffers** (network protocol analysers) are tools used to capture and analyse data traffic within a network.
- They help security analysts inspect packets for indicators of compromise.

### Packet Captures

- A **packet capture** (P-cap) is a file containing data packets intercepted from a network.
- Packet captures provide a detailed snapshot of network communications, which is essential for incident investigation.

### Importance of Packet Captures

- Packet captures allow security professionals to:
    - Observe the communications between devices on a network.
    - Identify abnormal or malicious activities.
    - Build a detailed storyline of events during an incident investigation.

### Example of Packet Capture Use

1. **Identifying an Attack**: By capturing network traffic, analysts can detect unusual patterns, such as repeated login attempts or data exfiltration activities.
2. **Analyzing Data Flow**: Packet captures can help trace the source and destination of data, providing insights into how an attack was carried out.
3. **Building an Incident Timeline**: Packet data can be used to reconstruct the sequence of events during an attack, helping to understand the attack's impact and scope.

## Key Takeaways

- Packets are the fundamental units of data transmission over a network, containing headers, payloads, and footers.
- Packet sniffers are essential tools for capturing and analyzing network traffic.
- Packet captures provide critical insights into network activities, helping security professionals detect, prevent, and respond to security incidents effectively.

## Learn More About Packet Captures

### Introduction

As a security analyst, monitoring and analyzing network traffic flows is crucial for identifying unusual activity on a network. Generating and analyzing packet captures are fundamental tasks in this process.

### Packets

Packets are basic units of information that travel from one device to another within a network. Understanding packets is essential for detecting network intrusions because they form the basis of information exchange over a network.

#### Components of Packets

|Component|Description|
|---|---|
|**Header**|Contains essential routing information like source and destination IP addresses, packet length, protocol, and packet identification numbers.|
|**Payload**|Contains the actual data being delivered, such as an image being uploaded to a website.|
|**Footer**|Provides error-checking information to determine if data has been corrupted.|

### Network Protocol analysers

Network protocol analysers, also known as packet sniffers, capture and analyse data traffic within a network. Examples include tcpdump, Wireshark, and TShark.

#### Uses of Network Protocol analysers

- **Security**: Monitor networks and identify suspicious activity.
- **Network Statistics**: Collect data on bandwidth and speed.
- **Troubleshooting**: Diagnose and resolve network performance issues.
- **Malicious Purposes**: Capture packets containing sensitive data, such as login information.

#### How Network Protocol analysers Work

1. **Packet Collection**: Packets are collected from the network via the Network Interface Card (NIC), which must be switched to monitoring mode or promiscuous mode to access all visible network data packets.
2. **Data Capture**: The network protocol analyser captures the network traffic in raw binary format.
3. **Data Conversion**: The binary data is converted into a human-readable format for analysis.

### Capturing Packets

Packet sniffing involves capturing and inspecting data packets across a network. Packet captures (P-caps) are files containing data packets intercepted from an interface or network.

#### Libraries and Formats for Packet Captures

|Library/Format|Description|
|---|---|
|**Libpcap**|Designed for Unix-like systems, used by tools like tcpdump.|
|**WinPcap**|An older open-source packet capture library for Windows.|
|**Npcap**|A library designed by Nmap, commonly used in Windows.|
|**PCAPng**|A modern format that captures packets and stores data simultaneously.|

### Key Takeaways

- Network protocol analysers are essential tools for security analysts.
- Packets contain critical information for understanding network activity.
- Packet captures provide detailed snapshots of network communications, useful for identifying and responding to security incidents.

## Interpret Network Communications with Packets

### Introduction

Analyzing packets is essential for interpreting and understanding network communications. Just like reading a letter inside an intercepted envelope, packet analysis helps us decipher the data transmitted over a network.

### Network Noise

Networks are inherently noisy, with numerous communications happening simultaneously between devices. Packet captures can contain vast amounts of data, making analysis both challenging and time-consuming.

### Importance of Packet Analysis

As a security professional, timely packet analysis is crucial for protecting networks and computer systems from potential attacks. Analyzing packet captures helps identify indicators of compromise (IoCs) and other security incidents.

### Filtering Network Traffic

Using packet sniffers like tcpdump and Wireshark, security analysts can filter network traffic to gather relevant information efficiently. Filtering helps isolate specific events, such as data exfiltration, from the vast amount of network traffic.

### Examples of Network analyser Tools

- **tcpdump**: A command-line packet analyser tool.
- **Wireshark**: A graphical user interface (GUI) packet analyser tool.

### Detailed Packet Fields: IP Headers

#### IPv4 Header Fields

|Field|Description|
|---|---|
|**Version**|Indicates the IP version (e.g., IPv4).|
|**IHL (Internet Header Length)**|Specifies the header length.|
|**Type of Service (ToS)**|Specifies the quality of service.|
|**Total Length**|Length of the entire packet (header + data).|
|**Identification**|Identifies fragments of the original packet.|
|**Flags**|Control flags such as Don't Fragment (DF) and More Fragments (MF).|
|**Fragment Offset**|Indicates the position of the fragment in the original packet.|
|**Time to Live (TTL)**|Specifies the lifespan of the packet.|
|**Protocol**|Indicates the protocol used in the data portion (e.g., TCP, UDP).|
|**Header Checksum**|Error-checking for the header.|
|**Source Address**|IP address of the sender.|
|**Destination Address**|IP address of the recipient.|
|**Options**|Additional options (if any).|

### Packet Analysis Process

1. **Capture Packets**: Use tools like tcpdump or Wireshark to capture network packets.
2. **Filter Packets**: Apply filters to isolate relevant traffic (e.g., specific IP addresses, protocols).
3. **analyse Headers**: Examine packet headers to understand the flow and routing of packets.
4. **Inspect Payload**: analyse the payload for actual data being transmitted, if not encrypted.
5. **Identify Anomalies**: Look for unusual patterns or indicators of compromise.

### Key Takeaways

- Packet analysis is essential for interpreting network communications and identifying potential security incidents.
- Network analyser tools like tcpdump and Wireshark help filter and analyse large volumes of network traffic.
- Understanding packet fields, especially IP headers, is crucial for effective packet analysis.

## Re-examine the Fields of a Packet Header

As a security analyst, it's crucial to learn how to manually read and analyse packets. Here, we will delve into an important packet component: IP headers.

### TCP/IP Model Recap

The **TCP/IP model** is a framework used to visualize how data is organized and transmitted across a network. It consists of four layers:

1. Application Layer
2. Transport Layer
3. Internet Layer
4. Network Interface Layer

The **Internet Layer** is where the Internet Protocol (IP) operates. It's responsible for ensuring packets reach their destinations.

### The Role of the Internet Protocol

The Internet Protocol functions like a mail courier delivering an envelope, using information in the packet header to determine the best route for packets. This ensures data is sent and received between hosts.

### IPv4 and IPv6

There are two versions of the Internet Protocol:

- **IPv4**: The foundation of internet communications.
- **IPv6**: The most recent version with expanded address capacity.

Different protocols use different headers. We'll focus on the IPv4 header.

### IPv4 Header Fields

The IPv4 header contains several fields essential for data transfer. Here are the fields explained:

|**Field**|**Description**|
|---|---|
|**Version**|Specifies the IP version (IPv4 or IPv6). Similar to mail classes like priority or express.|
|**IHL**|Internet Header Length. Specifies the length of the IP header plus any options.|
|**ToS**|Type of Service. Indicates if certain packets should be treated with different care.|
|**Total Length**|Length of the entire packet, including headers and data. Comparable to the dimensions of an envelope.|
|**Identification**|Identifies fragments of the original packet.|
|**Flags**|Control flags (e.g., Don't Fragment (DF) and More Fragments (MF)).|
|**Fragment Offset**|Specifies the position of a fragment in the original packet.|
|**TTL**|Time to Live. Determines how long a packet can exist before being dropped. Similar to tracking info for delivery date.|
|**Protocol**|Specifies the protocol used (e.g., TCP is represented by 6).|
|**Header Checksum**|Error-checking value for the header.|
|**Source Address**|IP address of the sender.|
|**Destination Address**|IP address of the recipient.|
|**Options**|Optional field used for network troubleshooting. Increases header length if used.|
|**Data**|The actual payload of the packet, similar to the content inside an envelope.|

### Importance of Packet Analysis

- **Header Analysis**: Helps determine routing and protocol information.
- **Payload Inspection**: Provides the actual data being transmitted.
- **Error Checking**: The Header Checksum field helps identify corrupted packets.

### Practical Application

By understanding these fields, security analysts can:

- **Detect Anomalies**: Identify unusual or malicious activity by examining packet headers.
- **Troubleshoot Issues**: Use the Options field and other header information for network troubleshooting.
- **Ensure Security**: Monitor network traffic to ensure data integrity and confidentiality.

### Conclusion

Understanding and analyzing packet headers is fundamental for network security. It allows security professionals to interpret network communications, detect anomalies, and protect against potential threats.

## Investigate Packet Details

So far, you've learned about how network protocol analysers (packet sniffers) intercept network communications. You've also learned how you can analyse packet captures (p-caps) to gain insight into the activity happening on a network. As a security analyst, you'll use your packet analysis skills to inspect network packets and identify suspicious activity during investigations.

In this reading, you'll re-examine IPv4 and IPv6 headers. Then, you'll explore how you can use Wireshark to investigate the details of packet capture files.

## Internet Protocol (IP)

Packets form the foundation of data exchange over a network, which means that detection begins at the packet level. The **Internet Protocol (IP)** includes a set of standards used for routing and addressing data packets as they travel between devices on a network. IP operates as the foundation for all communications over the internet.

IP ensures that packets reach their destinations. There are two versions of IP that you will find in use today: IPv4 and IPv6. Both versions use different headers to structure packet information.

### IPv4

IPv4 is the most commonly used version of IP. There are thirteen fields in the header:

- **Version**: This field indicates the IP version. For an IPv4 header, IPv4 is used.
- **Internet Header Length (IHL)**: This field specifies the length of the IPv4 header including any Options.
- **Type of Service (ToS)**: This field provides information about packet priority for delivery.
- **Total Length**: This field specifies the total length of the entire IP packet including the header and the data.
- **Identification**: Packets that are too large to send are fragmented into smaller pieces. This field specifies a unique identifier for fragments of an original IP packet so that they can be reassembled once they reach their destination.
- **Flags**: This field provides information about packet fragmentation including whether the original packet has been fragmented and if there are more fragments in transit.
- **Fragment Offset**: This field is used to identify the correct sequence of fragments.
- **Time to Live (TTL)**: This field limits how long a packet can be circulated in a network, preventing packets from being forwarded by routers indefinitely.
- **Protocol**: This field specifies the protocol used for the data portion of the packet.
- **Header Checksum**: This field specifies a checksum value which is used for error-checking the header.
- **Source Address**: This field specifies the source address of the sender.
- **Destination Address**: This field specifies the destination address of the receiver.
- **Options**: This field is optional and can be used to apply security options to a packet.

![An IPv4 header with its 13 fields.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/jkb0TBrPQSq9YoCeruRfqA_e1ec815e1edd4447a9a51b7f8945ccf1_7Fe1r5PP-rO933_0njaasi_PLYxnCK70uwxT7ZVgtLukfU1L_3B4ppP4aiLOiZ1QNlZCuuLku28h-mpQ5lEnQKly8HIeoDkaEvqkdh4Xbb_U9ba52JscXUcrmQFcluGPBPqNqA1v_gYZwv_JqR4di7niNF2R5uy2JBR0r-QshhE6zOIghv4lUCWa96872A?expiry=1716508800000&hmac=y4NtOP5IB5R6IMRIlOLAwgVuvT_pB1oTkIswNQO0vc8)

### IPv6

IPv6 adoption has been increasing because of its large address space. There are eight fields in the header:

- **Version**: This field indicates the IP version. For an IPv6 header, IPv6 is used.
- **Traffic Class**: This field is similar to the IPv4 Type of Service field. The Traffic Class field provides information about the packet's priority or class to help with packet delivery.
- **Flow Label**: This field identifies the packets of a flow. A flow is the sequence of packets sent from a specific source.
- **Payload Length**: This field specifies the length of the data portion of the packet.
- **Next Header**: This field indicates the type of header that follows the IPv6 header such as TCP.
- **Hop Limit**: This field is similar to the IPv4 Time to Live field. The Hop Limit limits how long a packet can travel in a network before being discarded.
- **Source Address**: This field specifies the source address of the sender.
- **Destination Address**: This field specifies the destination address of the receiver.

![An IPv6 header with its eight fields.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/i8ZlXBWcQnKMc9AvaOlTrg_9ae604f634bc4ea3b0bced51911d32f1_XjvmdLkZuzfhKQ0zQ_4RnCZGNxP0FDCtB0i8iwWtu30GL05Ziixkcd3YNSK8ng5tiu3X3XVOypCPywtGP01diUAvVWEkjwGWk7E_4fpFZdntBgohToxkS5cNsyZtqKsRCmssQUmWlH8Xhn2oJKG55Kv0-CUjA8Kj3yhZXTWbjjV4pYcCH9EUwPWpyFnhCQ?expiry=1716508800000&hmac=y_7xQuDbDsJ3huWvQ-7yDtUXiSQdu_Z6k_ssW7FvGVI)

Header fields contain valuable information for investigations and tools like Wireshark help to display these fields in a human-readable format.

## Wireshark

**Wireshark** is an open-source network protocol analyser. It uses a graphical user interface (GUI), which makes it easier to visualize network communications for packet analysis purposes. Wireshark has many features to explore that are beyond the scope of this course. You'll focus on how to use basic filtering to isolate network packets so that you can find what you need.

![Wireshark's interface.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/SrU-DA-pR1eTtgJe4lBOjQ_c841a1d648aa40069fe7e47e84ea79f1_CS_R-125_Wireshark-homepage.png?expiry=1716508800000&hmac=C__zLJFtcn1oLM_TBfAzBEyuc5Asf9_1NcTThlk9LME)

### Display Filters

Wireshark's display filters let you apply filters to packet capture files. This is helpful when you are inspecting packet captures with large volumes of information. Display filters will help you find specific information that's most relevant to your investigation. You can filter packets based on information such as protocols, IP addresses, ports, and virtually any other property found in a packet. Here, you'll focus on display filtering syntax and filtering for protocols, IP addresses, and ports.

### Comparison Operators

You can use different comparison operators to locate specific header fields and values. Comparison operators can be expressed using either abbreviations or symbols. For example, this filter using the == equal symbol in this filter ip.src == 8.8.8.8 is identical to using the eq abbreviation in this filter ip.src eq 8.8.8.8.

This table summarizes the different types of comparison operators you can use for display filtering.

|**Operator type**|**Symbol**|**Abbreviation**|
|---|---|---|
|Equal|==|eq|
|Not equal|!=|ne|
|Greater than|>|gt|
|Less than|<|lt|
|Greater than or equal to|>=|ge|
|Less than or equal to|<=|le|

**Pro tip:** You can combine comparison operators with Boolean logical operators like and and or to create complex display filters. Parentheses can also be used to group expressions and to prioritize search terms.

### Contains Operator

The contains operator is used to filter packets that contain an exact match of a string of text. Here is an example of a filter that displays all HTTP streams that match the keyword "moved".

![A Wireshark packet capture using the contains operator to find HTTP streams with the string "moved."](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/U-VFvCZpR-C7DiBud3CJ6Q_3d58fbc8790a4163b1fbd8d6689cf0f1_CS_R-125_packet-capture.png?expiry=1716508800000&hmac=rJnrRWVtimkS4lNrw4urNSxPRnftg6BDG0YHeg8uRJo)

### Matches Operator

The matches operator is used to filter packets based on the regular expression (regex) that's specified. Regular expression is a sequence of characters that forms a pattern. You'll explore more about regular expressions later in this program.

## Filter Toolbar

You can apply filters to a packet capture using Wireshark's filter toolbar. In this example, dns is the applied filter, which means Wireshark will only display packets containing the DNS protocol.

![A Wireshark filter toolbar with a dns filter applied.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/S2HoKdS_TnS0idDiU9XbJw_cb303cb11f2f45db944a6b22cbf3b4f1_ADA_R-125_DNS.png?expiry=1716508800000&hmac=kswyU9BlJxCAhpwDs_BW9XETnKYWVRMW_VlnkDl4M14)

**Pro tip**: Wireshark uses different colors to represent protocols. You can customize colors and create your own filters.

### Filter for Protocols

Protocol filtering is one of the simplest ways you can use display filters. You can simply enter the name of the protocol to filter. For example, to filter for DNS packets simply type `dns` in the filter toolbar. Here is a list of some protocols you can filter for:

- dns
- http
- ftp
- ssh
- arp
- telnet
- icmp

### Filter for an IP Address

You can use display filters to locate packets with a specific IP address.

For example, if you would like to filter packets that contain a specific IP address use `ip.addr`, followed by a space, the equal `==` comparison operator, and the IP address. Here is an example of a display filter that filters for the IP address 172.21.224.2:

`ip.addr == 172.21.224.2`

To filter for packets originating from a specific source IP address, you can use the `ip.src` filter. Here is an example that looks for the 10.10.10.10 source IP address:

`ip.src == 10.10.10.10`

To filter for packets delivered to a specific destination IP address, you can use the `ip.dst` filter. Here is an example that searches for the 4.4.4.4 destination IP address:

`ip.dst == 4.4.4.4`

### Filter for a MAC Address

You can also filter packets according to the **Media Access Control (MAC) address**. As a refresher, a MAC address is a unique alphanumeric identifier that is assigned to each physical device on a network.

Here's an example:

`eth.addr == 00:70:f4:23:18:c4`

### Filter for Ports

Port filtering is used to filter packets based on port numbers. This is helpful when you want to isolate specific types of traffic. DNS traffic uses TCP or UDP port 53 so this will list traffic related to DNS queries and responses only.

For example, if you would like to filter for a UDP port:

`udp.port == 53`

Likewise, you can filter for TCP ports as well:

`tcp.port == 25`

## Follow Streams

Wireshark provides a feature that lets you filter for packets specific to a protocol and view streams. A stream or conversation is the exchange of data between devices using a protocol. Wireshark reassembles the data that was transferred in the stream in a way that's simple to read.

![A Wireshark follow stream dialog box displays stream content of an HTTP conversation.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/qGiuzTybTNyYJXCUSuSStA_2353ba616b0c404d9b3d6df3af1fdef1_CS_R-125_dialog-box.png?expiry=1716508800000&hmac=l8_FPqqvJz0XMNdrnQiQ8EnzrcHVNf4AvJnRMGW9f4E)

Following a protocol stream is useful when trying to understand the details of a conversation. For example, you can examine the details of an HTTP conversation to view the content of the exchanged request and response messages.

## Key Takeaways

In this reading, you explored basic display filters with Wireshark. Packet analysis is an essential skill that you will continue to develop over time in your cybersecurity journey. Put your skills to practice in the upcoming activity and explore investigating the details of a packet capture file using Wireshark!

---
# Packet inspection

## Packet captures with tcpdump

### Introduction to tcpdump

Tcpdump is a powerful and popular network analyser used for capturing and monitoring network traffic. It is pre-installed on many Linux distributions and can be installed on most Unix-like operating systems, including macOS. Tcpdump captures various types of network traffic, including TCP, IP, ICMP, and more.

### Command Line Tool

Tcpdump operates from the command line, which provides an efficient and versatile interface for network traffic analysis. By using various options and flags in tcpdump commands, you can filter network traffic to pinpoint specific data of interest, such as a particular IP address, protocol, or port number.

### Basic tcpdump Command

Let’s examine a basic tcpdump command used to capture packets:

`sudo tcpdump -i any -v -c 1`

- `sudo`: Used to run tcpdump with superuser privileges, necessary because the regular user account lacks permissions.
- `tcpdump`: Starts the tcpdump application.
- `-i any`: Specifies that tcpdump should listen on any available network interfaces.
- `-v`: Stands for verbose, which provides detailed packet information.
- `-c 1`: Sets the count to capture only one packet.

### Analysing tcpdump Output

Upon executing the command, tcpdump will capture one packet and display the output. Let’s break down the output line by line.

1. **Listening on Interfaces and Capture Size:** Tcpdump indicates it is listening on all available network interfaces and provides information about the capture size.
    
2. **Timestamp:** The first field in the output is the timestamp, which includes hours, minutes, seconds, and fractions of a second. This helps in correlating events and determining timelines during an investigation.
    
3. **IP Version:** `IP` indicates the packet is using IPv4. The verbose option provides additional details about the IP packet fields, including protocol type and packet length.
    
4. **Type of Service (ToS):** This field, displayed in hexadecimal, indicates the Type of Service, which tells us how certain packets should be treated.
    
5. **Time to Live (TTL):** This field indicates the maximum duration a packet can travel across the network before being dropped.
    
6. **Fragmentation Fields:**
    
    - **Identification:** Unique identifier for fragmented packets.
    - **Offset:** Indicates the position of the fragment.
    - **Flags:** Instructions on how to reassemble fragments (e.g., DF stands for Don't Fragment).
7. **Protocol (proto):** Indicates the protocol in use, represented by a corresponding number (e.g., `tcp` is represented by `6`).
    
8. **Total Length:** Specifies the entire packet length, including the IP header.
    
9. **IP Addresses and Ports:** Displays the source and destination IP addresses, along with the port numbers or names.
    
10. **Checksum (cksum):** The header checksum field used to detect errors in the header. It confirms if the header is error-free.
    
11. **TCP Fields:**
    
    - **Flags:** Indicate various TCP flags. For example, `P` stands for the push flag, and a period indicates the ACK flag, signifying the packet is pushing data.

### Example Output Analysis

`16:42:21.123456 IP 192.168.1.2.56789 > 192.168.1.1.80: Flags [P.], seq 1:2, ack 1, win 512, length 1`

- **Timestamp:** `16:42:21.123456`
- **Source IP and Port:** `192.168.1.2.56789`
- **Destination IP and Port:** `192.168.1.1.80`
- **Flags:** `[P.]` (push flag with ACK)
- **Sequence Number:** `seq 1:2`
- **Acknowledgment Number:** `ack 1`
- **Window Size:** `win 512`
- **Length:** `length 1`

### Conclusion

Tcpdump is a versatile tool that provides detailed insights into network traffic through packet captures. By using tcpdump, you can analyse network packets, identify anomalies, and investigate potential security incidents efficiently.

## Overview of tcpdump

As a security analyst, you’ll use network protocol analysers to help defend against any network intrusions. Previously, you learned the following terms related to network monitoring and analysis:

- A **network protocol analyser (packet sniffer)** is a tool designed to capture and analyse data traffic within a network.
- **Packet sniffing** is the practice of capturing and inspecting data packets across a network.

In this reading, you'll learn more about tcpdump, a network protocol analyser that can be used to capture and view network communications.

### What is tcpdump?

**Tcpdump** is a command-line network protocol analyser. Recall that a **command-line interface (CLI)** is a text-based user interface that uses commands to interact with the computer.

Tcpdump is used to capture network traffic. This traffic can be saved to a **packet capture (p-cap)**, which is a file containing data packets intercepted from an interface or network. The p-cap file can be accessed, analysed, or shared at a later time. Analysts use tcpdump for a variety of reasons, from troubleshooting network issues to identifying malicious activity. Tcpdump comes pre-installed in many Linux distributions and can also be installed on other Unix-based operating systems such as macOS.

**Note**: It's common for network traffic to be encrypted, which means data is encoded and unreadable. Inspecting the network packets might require decrypting the data using the appropriate private keys.

### Capturing packets with tcpdump

Previously in this program, you learned that a Linux **root user (or superuser)** has elevated privileges to modify the system. You also learned that the **sudo** command temporarily grants elevated permissions to specific users in Linux. Like many other packet sniffing tools, you’ll need to have administrator-level privileges to capture network traffic using tcpdump. This means you will need to either be logged in as the root user or have the ability to use the sudo command. Here is a breakdown of the tcpdump syntax for capturing packets:

`sudo tcpdump [-i interface] [option(s)] [expression(s)]`

- The `sudo tcpdump` command begins running tcpdump using elevated permissions as sudo.
- The `-i` parameter specifies the network interface to capture network traffic. You must specify a network interface to capture from to begin capturing packets. For example, if you specify `-i any` you’ll sniff traffic from all network interfaces on the system.
- The option(s) are optional and provide you with the ability to alter the execution of the command. The expression(s) are a way to further filter network traffic packets so that you can isolate network traffic.

**Note**: Before you can begin capturing network traffic, you must identify which network interface you'll want to use to capture packets from. You can use the `-D` flag to list the network interfaces available on a system.

### Options

With tcpdump, you can apply options, also known as flags, to the end of commands to filter network traffic. Short options are abbreviated and represented by a hyphen and a single character like `-i`. Long options are spelled out using a double hyphen like `--interface`. Tcpdump has over fifty options that you can explore using [the manual page](https://www.tcpdump.org/manpages/tcpdump.1.html). Here, you’ll examine a couple of essential tcpdump options including how to write and read packet capture files.

**Note**: Options are case sensitive. For example, a lowercase `-w` is a separate option with a different use than the option with an uppercase `-W`.

**Note**: tcpdump options that are written using short options can be written with or without a space between the option and its value. For example, `sudo tcpdump -i any -c 3` and `sudo tcpdump -iany -c3` are equivalent commands.

#### **-w**

Using the `-w` flag, you can write or save the sniffed network packets to a packet capture file instead of just printing it out in the terminal. This is very useful because you can refer to this saved file for later analysis. In this command, tcpdump is capturing network traffic from all network interfaces and saving it to a packet capture file named `packetcapture.pcap`:

`sudo tcpdump -i any -w packetcapture.pcap`

#### **-r**

Using the `-r` flag, you can read a packet capture file by specifying the file name as a parameter. Here is an example of a tcpdump command that reads a file called `packetcapture.pcap`:

`sudo tcpdump -r packetcapture.pcap`

#### **-v**

As you’ve learned, packets contain a lot of information. By default, tcpdump will not print out all of a packet's information. This option, which stands for verbose, lets you control how much packet information you want tcpdump to print out.

There are three levels of verbosity you can use depending on how much packet information you want tcpdump to print out. The levels are `-v`, `-vv`, and `-vvv`. The level of verbosity increases with each added v. The verbose option can be helpful if you’re looking for packet information like the details of a packet’s IP header fields. Here’s an example of a tcpdump command that reads the `packetcapture.pcap` file with verbosity:

`sudo tcpdump -r packetcapture.pcap -v`

#### **-c**

The `-c` option stands for count. This option lets you control how many packets tcpdump will capture. For example, specifying `-c 1` will only print out one single packet, whereas `-c 10` prints out 10 packets. This example is telling tcpdump to only capture the first three packets it sniffs from any network interface:

`sudo tcpdump -i any -c 3`

#### **-n**

By default, tcpdump will perform name resolution. This means that tcpdump automatically converts IP addresses to names. It will also resolve ports to commonly associated services that use these ports. This can be problematic because tcpdump isn’t always accurate in name resolution. For example, tcpdump can capture traffic from port 80 and automatically translates port 80 to HTTP in the output. However, this is misleading because port 80 isn’t always going to be using HTTP; it could be using a different protocol.

Additionally, name resolution uses what’s known as a reverse DNS lookup. A reverse DNS lookup is a query that looks for the domain name associated with an IP address. If you perform a reverse DNS lookup on an attacker’s system, they might be alerted that you are investigating them through their DNS records.

Using the `-n` flag disables this automatic mapping of numbers to names and is considered to be best practice when sniffing or analysing traffic. Using `-n` will not resolve hostnames, whereas `-nn` will not resolve _both_ hostnames or ports. Here’s an example of a tcpdump command that reads the `packetcapture.pcap` file with verbosity and disables name resolution:

`sudo tcpdump -r packetcapture.pcap -v -n`

**Pro tip:** You can combine options together. For example, `-v` and `-n` can be combined as `-vn`. But, if an option accepts a parameter right after it like `-c 1` or `-r capture.pcap` then you can’t combine other options to it.

### Expressions

Using filter expressions in tcpdump commands is also optional, but knowing how and when to use filter expressions can be helpful during packet analysis. There are many ways to use filter expressions.

If you want to specifically search for network traffic by protocol, you can use filter expressions to isolate network packets. For example, you can filter to find only IPv6 traffic using the filter expression `ip6`.

You can also use boolean operators like `and`, `or`, or `not` to further filter network traffic for specific IP addresses, ports, and more. The example below reads the `packetcapture.pcap` file and combines two expressions `ip` and `port 80` using the `and` boolean operator:

`sudo tcpdump -r packetcapture.pcap -n 'ip and port 80'`

**Pro tip:** You can use single or double quotes to ensure that tcpdump executes all of the expressions. You can also use parentheses to group and prioritize different expressions. Grouping expressions is helpful for complex or lengthy commands. For example, the command `ip and (port 80 or port 443)` tells tcpdump to prioritize executing the filters enclosed in the parentheses before filtering for IPv4.

### Interpreting output

Once you run a command to capture packets, tcpdump will print the output of the command as the sniffed packets. In the output, tcpdump prints one line of text for each packet with each line beginning with a timestamp. Here’s an example of a command and output for a single TCP packet:

`sudo tcpdump -i any -v -c 1`

This command tells tcpdump to capture packets on `-i any` network interface. The option `-v` prints out the packet with detailed information and the option `-c 1` prints out only one packet. Here is the output of this command:

![Output of a tcpdump command with labels for the timestamp, source IP, source port, destination IP, and destination port.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/3LnHDkkeQ2-a-KjHKXkBCQ_940eb009d1674c7595f8361adf48c1f1_89by7cw_y0GWsyGI4iK19PqNyVHpVO4reyeIO0v-xYeZDBID0JG0PzpqRSA7fWjmD88HKjaZ8PhlONjdsKMLrUlx0lM9lPGBVSNqO87rZPPHt00BahLIQmfBNpRTyBAgjUklW2nn3hCB5Z-x_0HC56AKW7g2hk4tXgWyjInXVJYMosY9D4pyuX2VzerrhA?expiry=1716508800000&hmac=NDOrJdho5N1jskxojS1rrAX0pQPooob2zmpwEXO-v0w)

1. **Timestamp**: The output begins with the timestamp, which starts with hours, minutes, seconds, and fractions of a second.
2. **Source IP:** The packet’s origin is provided by its source IP address.
3. **Source port:** This port number is where the packet originated.
4. **Destination IP:** The destination IP address is where the packet is being transmitted to.
5. **Destination port:** This port number is where the packet is being transmitted to.

The remaining output contains details of the TCP connection including flags and sequence number. The options information is additional packet information that the `-v` option has provided.

### Key takeaways

In security, you’ll likely encounter using network protocol analyser tools like tcpdump. It’s important to be equipped with the knowledge of capturing, filtering, and interpreting network packets on the command line.



---
## Glossary terms from module 2


**Command and control (C2):** The techniques used by malicious actors to maintain communications with compromised systems

**Command-line interface (CLI):** A text-based user interface that uses commands to interact with the computer

**Data exfiltration:** Unauthorized transmission of data from a system

**Data packet:** A basic unit of information that travels from one device to another within a network

**Indicators of compromise (IoC):** Observable evidence that suggests signs of a potential security incident

**Internet Protocol (IP):** A set of standards used for routing and addressing data packets as they travel between devices on a network

**Intrusion detection systems (IDS):** An application that monitors system activity and alerts on possible intrusions

**Media Access Control (MAC) Address:** A unique alphanumeric identifier that is assigned to each physical device on a network

**National Institute of Standards and Technology (NIST) Incident Response Lifecycle:** A framework for incident response consisting of four phases: Preparation; Detection and Analysis; Containment, Eradication and Recovery; and Post-incident activity

**Network data:** The data that’s transmitted between devices on a network 

**Network protocol analyser (packet sniffer):** A tool designed to capture and analyse data traffic within a network

**Network traffic:** The amount of data that moves across a network 

**Network Interface Card (NIC):** Hardware that connects computers to a network

**Packet capture (p-cap):** A file containing data packets intercepted from an interface or network

**Packet sniffing:** The practice of capturing and inspecting data packets across a network

**Playbook:** A manual that provides details about any operational action

**Root user (or superuser)**: A user with elevated privileges to modify the system

**Sudo:** A command that temporarily grants elevated permissions to specific users

**tcpdump:** A command-line network protocol analyser

**Wireshark:** An open-source network protocol analyser