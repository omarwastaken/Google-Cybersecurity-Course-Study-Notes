## How Network Intrusions Compromise Your System

This course section explores how network intrusions exploit vulnerabilities and compromise systems.

**Motivations Behind Attacks**

- **Financial Gain:** Stealing money or valuable data for financial gain is a common attacker motive.
    
- **Personal or Political Reasons:** Attacks may be driven by personal vendettas or attempts to disrupt an organization's operations due to ideological differences.
    
- **Disgruntled Employees:** Employees upset with their employer may launch attacks as a form of revenge.
    

**Network Interception Attacks**

These attacks involve capturing and manipulating network traffic.

- **Packet Sniffing:** Attackers use software or hardware tools to capture data packets traveling across a network. This allows them to steal sensitive information like usernames, passwords, and credit card details.
    
- **Traffic Alteration:** Malicious actors can modify captured data packets, potentially leading to:
    
    - **Malicious Code Injection:** Inserting harmful code into network traffic to compromise systems.
        
    - **Message Tampering:** Altering messages to disrupt communication or steal information.
        

**Backdoor Attacks**

Backdoors are unauthorized access points created by programmers or network administrators to bypass security measures for legitimate purposes (e.g., troubleshooting). However, attackers can exploit these backdoors to gain unauthorized access to a system.

**Potential Impacts of Network Intrusions**

- **Financial Losses:** Network attacks can disrupt operations, leading to revenue loss. Additionally, repairing damage and dealing with legal ramifications of data breaches can be expensive.
    
- **Reputation Damage:** Public knowledge of a cyberattack can erode trust in an organization, potentially driving customers away.
    
- **Public Safety Risks:** Attacks on critical infrastructure like power grids or communication systems can pose safety threats to citizens.
    

**Security Analyst Role**

Security analysts play a vital role in protecting networks by:

- **Staying informed about emerging threats and vulnerabilities.**
    
- **Implementing robust security measures to mitigate risks.**
    
- **Monitoring network activity for suspicious behaviour.**
    

**Conclusion**

Network intrusions are a constant threat. Understanding attacker motivations, common attack methods, and potential consequences is crucial for organizations to implement effective security measures.

---
## Understanding Denial-of-Service (DoS) Attacks

This video lecture explores Denial-of-Service (DoS) attacks, a malicious attempt to disrupt normal network operations.

### DoS Attacks: An Overview

- A DoS attack floods a network or server with unwanted traffic, overwhelming its resources and preventing legitimate users from accessing services.
    
- The attack aims to crash the target system or render it unresponsive.
    
- DoS attacks can cause significant financial losses and leave the network vulnerable to further attacks.
    

### Distributed Denial-of-Service (DDoS) Attacks

- A DDoS attack is a variant of DoS that utilizes multiple compromised devices (bots) scattered across the internet to bombard the target with traffic.
    
- The distributed nature of the attack makes it harder to identify and mitigate the source.
    
- DDoS attacks can generate a much larger volume of traffic compared to traditional DoS attacks.
    

### Network Level DoS Attacks

These attacks target network bandwidth to slow down traffic flow. Here are three common examples:

- **SYN Flood Attack:** Exploits the TCP handshake process by overwhelming the server with SYN (synchronize) packets during connection initiation. The server runs out of ports to manage connections, rendering it dysfunctional.
    
- **ICMP Flood Attack:** Spams the target with ICMP (Internet Control Message Protocol) packets, consuming bandwidth and preventing legitimate traffic from reaching the server.
    
- **Ping of Death Attack:** Sends a malformed ICMP packet exceeding the standard size limit. This oversized packet can crash vulnerable systems due to resource overload.
    

### Conclusion

DoS and DDoS attacks pose a significant threat to network security. Understanding these attacks and their mechanisms is crucial for implementing effective defence strategies.

## Understanding Tcpdump: A Tool for Network Traffic Analysis

This study guide explores tcpdump, a command-line network protocol analyser used for network traffic monitoring and analysis.

### Network Protocol analysers

Network protocol analysers (packet sniffers/analysers) are tools designed to capture and inspect data flowing across a network. They are valuable for:

- **Network Monitoring:** Identifying suspicious activity and troubleshooting network issues.
    
- **Security Analysis:** Detecting and investigating potential security threats.
    

**Common Network Protocol analysers:**

- SolarWinds NetFlow Traffic analyser
- ManageEngine OpManager
- Azure Network Watcher
- Wireshark
- tcpdump (covered in this guide)

### Tcpdump: A Lightweight and Versatile Tool

tcpdump is a popular command-line network protocol analyser known for:

- **Efficiency:** Low memory usage and minimal CPU footprint.
    
- **Open-Source:** Freely available and built on the open-source libpcap library.
    
- **Cross-Platform Compatibility:** Primarily for Linux/Unix but also compatible with macOS.
    

**Functionality:**

- Captures network traffic data packets.
- analyses captured data and presents key information in a human-readable format.
- Displays details like source/destination IP addresses and port numbers.

### Interpreting Tcpdump Output
  
![types of information presented in a tcpdump packet capture.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/B-PaECh0ToSFgBWpFczYZg_4896abe8c06443f08eec4dc003dcf8f1_image.png?expiry=1713744000000&hmac=vfPuYU63u-CE3FjHq2GndeySPxtMzsl8mtOG3B62-Ec)

- Tcpdump displays captured packet information in the terminal window.
    
- The output includes:
    
    - **Timestamps:** Packet capture time (hours, minutes, seconds, milliseconds).
        
    - **Source IP Address:** Origin of the network packet.
        
    - **Source Port Number:** Port where the packet originated.
        
    - **Destination IP Address:** Target of the network packet.
        
    - **Destination Port Number:** Port where the packet is being sent.
        
- **Note:** tcpdump can resolve IP addresses to hostnames and ports to service names (e.g., HTTP for port 80).
    

### Common Uses of Tcpdump

Tcpdump, along with other network protocol analysers, is used for various network monitoring and security tasks:

- **Network Traffic Analysis:** Establishing baselines for network traffic patterns and resource utilization.
    
- **Security Threat Detection:** Identifying malicious traffic patterns indicative of potential attacks.
    
- **Alert Generation:** Creating custom alerts to notify administrators of network issues or security threats.
    
- **Troubleshooting Network Issues:** Investigating network performance problems for troubleshooting purposes.
    
- **Finding Unauthorized Activity:** Locating unauthorized instant messaging traffic or unauthorized wireless access points.
    

**Security Concerns:**

While a valuable tool for network analysis, attackers can misuse network protocol analysers to capture sensitive information like usernames and passwords. Cybersecurity professionals should be aware of both the benefits and potential risks associated with these tools.

### Key Takeaways

- Tcpdump is a powerful command-line network protocol analyser for Linux/Unix and macOS.
    
- It captures and analyses network traffic, providing valuable insights into network activity.
    
- Tcpdump output includes timestamps, IP addresses, and port numbers for analysis.
    
- While beneficial for network monitoring and security, tcpdump can also be misused for malicious purposes.

---
## Packet Sniffing: How Hackers Spy on Your Network

This study guide explores packet sniffing, a technique used for both legitimate network analysis and malicious purposes.

### What is Packet Sniffing?

Packet sniffing is the practice of capturing and examining data packets travelling across a network. It's like eavesdropping on a conversation between two devices.

- **Tools:** Software applications or hardware devices can be used for packet sniffing.

### Malicious Use of Packet Sniffing

Threat actors (hackers) can exploit packet sniffing to steal sensitive information:

- **Data Interception:** Hackers can insert themselves between two communicating devices and capture data packets containing valuable information like usernames, passwords, credit card numbers, etc.
    
- **Data Tampering:** Malicious actors can modify captured data packets to manipulate information.
    

### Passive vs. Active Sniffing

- **Passive Sniffing:** This is a more subtle attack where hackers simply read data packets flowing through the network. It's like passively reading someone else's mail without tampering with it.
    
- **Active Sniffing:** This is a more intrusive attack where hackers actively modify data packets. It's like altering the contents of someone's mail before delivery.
    

### Protecting Against Packet Sniffing

Here are some measures to safeguard against packet sniffing attacks:

- **Using a VPN:** A Virtual Private Network encrypts data travelling across the network, making it unreadable even if intercepted.
    
- **HTTPS Websites:** Look for websites that use HTTPS (Hypertext Transfer Protocol Secure) in the URL. HTTPS encrypts communication between your browser and the website.
    
- **Avoiding Unprotected Wi-Fi:** Public Wi-Fi networks are often unencrypted, making them vulnerable to packet sniffing. Avoid using them for sensitive activities unless you have a VPN.
    

### Conclusion

Packet sniffing can be a serious security threat. By understanding how it works and implementing the preventive measures mentioned above, you can significantly reduce the risk of falling victim to such attacks.

## Understanding IP Spoofing Attacks

This study guide explores IP spoofing, a network attack technique where attackers impersonate authorized devices to gain access to a network.

### IP Spoofing Explained

IP spoofing involves modifying the source IP address in a data packet to appear as a legitimate user. This allows attackers to bypass security measures like firewalls and infiltrate a network.

- **Attacker's Goal:** Gain unauthorized access to a network by masquerading as a trusted device.
    
- **Common Applications:** On-path attacks, replay attacks, and smurf attacks (discussed below).
    

### Types of IP Spoofing Attacks

- **On-Path Attack:**
    
    - The attacker positions themselves between two communicating devices (e.g., web browser and server) on the network.
        
    - The attacker intercepts data packets and steals information like IP and MAC addresses.
        
    - Using the stolen information, the attacker impersonates one of the legitimate devices to gain access to the network.
        
- **Replay Attack:**
    
    - The attacker captures a valid data packet travelling across the network.
        
    - The attacker delays or retransmits the captured packet to impersonate the authorized user and potentially manipulate data.
        
- **Smurf Attack (DDoS Attack Variant):**
    
    - The attacker spoofs the source IP address of a legitimate user to flood a target device or network with packets.
        
    - This overwhelms the target with traffic, causing denial-of-service (DoS).
        

### Mitigating IP Spoofing Attacks

Here are some methods to defend against IP spoofing attacks:

- **Encryption:** Encrypting network traffic safeguards data confidentiality, rendering it useless even if intercepted by attackers.
    
- **Firewall Configuration:** Firewalls can be configured to identify and block incoming traffic with spoofed IP addresses from the local network range.
    
- **Regular Security Audits:** Regularly assess and update network security configurations to identify and address vulnerabilities.
    

By understanding IP spoofing and implementing these preventive measures, you can significantly reduce the risk of falling victim to such attacks.

## Interception Tactics: Packet Sniffing and IP Spoofing

This study guide explores interception tactics, a category of network attacks that involve capturing data packets travelling across a network.

### Interception Attacks: An Overview

Interception attacks exploit packet sniffing and IP spoofing techniques to steal sensitive information or disrupt network operations.

- **Packet Sniffing:** Capturing network traffic to steal data like usernames, passwords, or credit card numbers.
    
- **IP Spoofing:** Impersonating authorized devices by forging IP addresses to gain access to a network or launch denial-of-service (DoS) attacks.
    

### Packet Sniffing in Detail

- **Standard Network Operation:**
    
    - Network Interface Card (NIC): Hardware that connects a device to a network.
        
    - NIC receives data packets addressed to the device's MAC address and processes the information.
        
- **Malicious Packet Sniffing:**
    
    - Promiscuous Mode: A NIC setting that captures all network traffic, even packets not addressed to the device.
        
    - Attackers use software like Wireshark to capture and analyse packets on a private network.
        
    - Stolen information can be used for identity theft or IP spoofing attacks.
        

### IP Spoofing in Detail

- **IP Spoofing Process:**
    
    - Attackers sniff packets to obtain IP and MAC addresses of authorized devices.
        
    - They then forge these addresses to impersonate legitimate devices on the network.
        
    - Firewalls can be configured to block spoofed IP addresses.
        

### Common IP Spoofing Attacks

- **On-Path Attack (Man-in-the-Middle Attack):**
    
    - Attackers intercept communication between two trusted devices to steal data or redirect traffic.
        
    - Encryption (e.g., TLS) protects against on-path attacks by making intercepted data unreadable.
        
- **Smurf Attack (DoS Attack Variant):**
    
    - Attackers spoof a legitimate user's IP address to flood a target network with packets.
        
    - This overwhelms the target with traffic, causing a DoS attack.
        
    - Advanced firewalls can detect and block smurf attacks by monitoring for unusual network traffic patterns.
        
- **DoS Attack:**
    
    - Attackers impersonate authorized users to overwhelm a network with legitimate requests, preventing legitimate users from accessing resources.
        
    - Layered defences, including encryption and firewalls, can help mitigate DoS attacks.
        
---
## Glossary terms from module 3

**Active packet sniffing:** A type of attack where data packets are manipulated in transit

**Botnet:** A collection of computers infected by malware that are under the control of a single threat actor, known as the “bot-herder"

**Denial of service (DoS) attack:** An attack that targets a network or server and floods it with network traffic

**Distributed denial of service (DDoS) attack:** A type of denial of service attack that uses multiple devices or servers located in different locations to flood the target network with unwanted traffic

**Internet Control Message Protocol (ICMP):** An internet protocol used by devices to tell each other about data transmission errors across the network

**Internet Control Message Protocol (ICMP) flood:** A type of DoS attack performed by an attacker repeatedly sending ICMP request packets to a network server

**IP spoofing:** A network attack performed when an attacker changes the source IP of a data packet to impersonate an authorized system and gain access to a network

**On-path attack:** An attack where a malicious actor places themselves in the middle of an authorized connection and intercepts or alters the data in transit

**Packet sniffing:** The practice of capturing and inspecting data packets across a network 

**Passive packet sniffing:** A type of attack where a malicious actor connects to a network hub and looks at all traffic on the network

**Ping of death:** A type of DoS attack caused when a hacker pings a system by sending it an oversized ICMP packet that is bigger than 64 KB

**Replay attack:** A network attack performed when a malicious actor intercepts a data packet in transit and delays it or repeats it at another time

**Smurf attack:** A network attack performed when an attacker sniffs an authorized user’s IP address and floods it with ICMP packets

**Synchronize (SYN) flood attack:** A type of DoS attack that simulates a TCP/IP connection and floods a server with SYN packets