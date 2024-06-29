## Security Hardening: Protecting Systems from Attack

This study guide explores security hardening, a process for strengthening systems and reducing their vulnerability to cyberattacks.

### What is Security Hardening?

Security hardening is the proactive practice of minimizing a system's attack surface, which refers to all potential entry points that attackers could exploit.

- **Analogy:** Imagine a network as a house. Security hardening is like adding locks to doors and windows to deter burglars.

### Why is Security Hardening Important?

By hardening systems, security analysts can:

- Reduce the likelihood of successful cyberattacks.
- Minimize the potential damage caused by an attack.

### Security Hardening Techniques

- **Regular Maintenance:**
    
    - Keeping network devices and systems updated with the latest security patches.
        
    - Performing security checks to identify and address vulnerabilities.
        
    - Maintaining physical security measures (cameras, guards) for critical systems.
        
- **Configuration Changes:**
    
    - Enforcing strong password policies (longer passwords, frequent changes).
        
    - Updating encryption standards for data storage (databases).
        
    - Disabling unused applications, services, and ports.
        
    - Reducing access permissions across devices and the network.
        
- **Penetration Testing:**
    
    - Simulating cyberattacks to identify weaknesses in systems, networks, applications, and processes.
        
    - Addressing vulnerabilities discovered during penetration testing.
        

### Key Takeaways

Security hardening is a fundamental security practice that organizations can leverage to significantly reduce their cyberattack risk. By employing a combination of the techniques mentioned above, security analysts can create a more secure and resilient IT infrastructure.

---
## Operating System Hardening: Securing the Core

This study guide explores operating system (OS) hardening, a critical security practice for protecting systems and networks.

### Why Harden the OS?

The operating system acts as the foundation for all software applications on a computer. A single compromised OS can expose the entire network to security risks.

- **OS Hardening:** The process of strengthening an operating system to minimize vulnerabilities and enhance its overall security posture.

### Common OS Hardening Techniques

- **Regular Tasks:**
    
    - **Patch Updates:** Installing updates (patches) released by software vendors to fix security vulnerabilities in the OS.
        
        - Patch updates should be applied promptly to address newly discovered vulnerabilities.
    - **Maintaining an Up-to-Date System Inventory:** Keeping a record of all devices and authorized users on the network.
        
    - **System Backups:** Regularly backing up systems to facilitate recovery in case of security incidents.
        
- **Baseline Configuration:**
    
    - Establishing a documented baseline configuration that defines the desired security state for the OS.
        
    - This baseline serves as a reference point for future system configurations and helps detect unauthorized changes.
        
    - The baseline configuration may include settings like firewall rules and access permissions.
        
- **Hardware and Software Disposal:**
    
    - Securely wiping and disposing of old hardware to prevent unauthorized access to potentially sensitive data.
        
    - Removing unused software applications to eliminate vulnerabilities associated with outdated or unneeded software.
        
- **Strong Password Policies:**
    
    - Enforcing password policies that mandate complex passwords (e.g., minimum length, character types).
        
    - Limiting login attempts to prevent brute-force attacks.
        
    - Implementing multi-factor authentication (MFA) for an additional layer of security. MFA requires users to verify their identity through two or more factors (e.g., password, fingerprint).
        

### Conclusion

OS hardening is an essential security practice that helps organizations significantly reduce their cyberattack risk. By following these hardening techniques, security professionals can create a more secure and stable IT environment.

## Brute Force Attacks and OS Hardening Strategies

This study guide explores brute force attacks, vulnerability assessment techniques, and preventive measures to enhance login security.

### Brute Force Attacks Explained

Brute force attacks involve systematically guessing login credentials (usernames and passwords) to gain unauthorized access to a system.

- **Types of Brute Force Attacks:**
    
    - **Simple Brute Force Attack:** Trying random combinations of usernames and passwords.
        
    - **Dictionary Attack:** Using lists of common words, phrases, and leaked credentials to guess passwords.
        
- **Attack Automation:** Attackers often use automated tools to accelerate the guessing process.
    

### Assessing System Vulnerabilities

- **Virtual Machines (VMs):** Isolated software environments that allow analysts to safely test suspicious files, applications, or potential security vulnerabilities without affecting the main system.
    
    - **Benefits:**
        
        - Secure testing of malware and threats.
            
        - Ability to revert to a clean VM state after testing.
            
        - Efficient testing of different configurations.
            
    - **Limitations:**
        
        - Risk of malicious code escaping the VM in rare cases.
- **Sandboxes:** Secure testing environments that isolate software execution from the main network.
    
    - **Applications:**
        
        - Testing software patches.
            
        - Identifying and addressing software vulnerabilities.
            
        - Analysing suspicious files and code.
            
        - Simulating cyberattacks.
            
    - **Considerations:**
        
        - Sandbox environments can be physical machines or cloud-based VMs.
            
        - Some malware can detect and bypass sandboxes.
            

### Preventing Brute Force Attacks

- **Salting and Hashing:**
    
    - **Hashing:** Converting passwords into unique, unreadable values (hashes) for secure storage.
        
    - **Salting:** Adding random characters to password hashes before hashing, making them more complex and resistant to brute-force cracking.
        
- **Multi-Factor Authentication (MFA/2FA):** Requiring two or more verification factors (e.g., password, fingerprint, one-time code) to access a system.
    
- **CAPTCHA and reCAPTCHA:** Challenge-response tests to distinguish human users from automated bots attempting brute-force attacks.
    
- **Strong Password Policies:** Enforcing password complexity requirements (length, character types), regular password updates, and limitations on login attempts.
    

### Conclusion

By understanding brute force attacks and implementing these preventive measures, organizations can significantly strengthen their login security posture. Combining OS hardening practices with robust authentication methods is crucial for mitigating cyberattacks.

---
## Network Hardening

**Network hardening** focuses on strengthening the security of your network by limiting access points and vulnerabilities. There are two main categories of tasks:

- **Regularly Performed Tasks:**
    
    - **Firewall Rules Maintenance:** Regularly review and update firewall rules to ensure only authorized traffic can enter or leave the network.
    - **Network Log Analysis:** analyse network logs using a SIEM (Security Information and Event Management) tool to identify suspicious activity. SIEM tools collect data from various network devices and present it in a centralized dashboard for easier analysis.
    - **Patch Updates:** Regularly install security patches on network devices to address vulnerabilities exploited by attackers.
    - **Server Backups:** Regularly back up your servers to ensure you can recover data in case of a security incident.
- **Tasks Performed Once and Updated as Needed:**
    
    - **Port Filtering:** Configure firewalls to block unused ports and only allow necessary communication through specific ports. This reduces the attack surface by minimizing potential entry points.
    - **Network Access Privileges:** Implement granular access controls to restrict network access only to authorized users and devices. Grant access based on the principle of least privilege, where users only have the access level required for their job function.
    - **Encryption:** Encrypt all network traffic using strong encryption standards to protect sensitive data even if it's intercepted. Implement stronger encryption standards for data in restricted zones containing highly confidential information.
    - **Network Segmentation:** Divide the network into isolated subnets for different departments or security zones. This prevents security issues in one subnet from impacting the entire network.

**Additional Points:**

- Use the latest available wireless protocols and disable older, less secure protocols.
- Network hardening is an essential security practice for security analysts and plays a vital role in protecting your organization's data.

## Network Security Applications

This section covers network hardening and monitoring. Security professionals use various devices and tools to secure a network. These layers of security build upon each other, creating a strong defense strategy known as **defense in depth**.

**Learning Objectives:**

- Understand the role of firewalls, intrusion detection systems (IDS), intrusion prevention systems (IPS), and security information and event management (SIEM) tools.
- Recognize the benefits of layered security.
- Identify the placement of these tools within a network architecture.

### Layered Security

This course material introduces four essential security tools:

- Firewalls
- Intrusion Detection Systems (IDS)
- Intrusion Prevention Systems (IPS)
- Security Information and Event Management (SIEM) tools

Network security professionals can choose to implement any or all of these tools depending on their desired security level. Each tool adds another layer of defense, progressively hardening the network. Firewalls provide the base level of security, while a combination of all these tools offers the most robust protection.

![An image showing the differences between a firewall, IPS, and IDS.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/4ENRXSswQSOsOrKt9KyG6A_06fe04a8d10846ba811fe89a969642f1_CS_R-055_Firewall-IDS-and-IPS.png?expiry=1714003200000&hmac=t86Jhjz4u3pn27CR0SrdLZmugMzleKfZdibO4CrRS-8)

It's crucial to understand where each tool resides within the network architecture. Security analysts need to be familiar with network topologies to make informed decisions about security tool placement.

### Firewalls

You've previously learned about different firewall types (stateless, stateful, next-generation) and their security advantages.

Most firewalls share similar functionalities. They analyse data packet headers and allow or deny traffic based on predefined rules. Firewalls inspect port numbers, and NGFWs can even examine packet payloads. Every system on a network should have its own firewall, regardless of the presence of a network-wide firewall.

  
![A firewall circled by dashes, protecting the internal network from internet traffic that comes in through the mode.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/dSLcIcXBSw-kw-9kzEwhAw_284c8540dab14a9e911296471c71d2f1_CS_R-055_Firewall.png?expiry=1714003200000&hmac=iE0vQ9KX-Ju5Nju-UuU16aIcOh02871z-8Kc-Sji7fk)
### Intrusion Detection System (IDS)

An IDS is an application that monitors network activity and raises alerts for potential intrusions. It identifies suspicious traffic based on signatures of malicious activity.

IDS systems typically monitor data packets traversing the network, searching for characteristics of known attacks. Some advanced systems can also detect anomalies that might indicate malicious intent. When an anomaly is detected, the IDS sends an alert to the network administrator for further investigation.

Here are some limitations of IDS:

- Limited to identifying known attacks or evident anomalies. New or sophisticated attacks might go unnoticed.
- Doesn't actively stop suspicious traffic. Network administrators need to intervene upon receiving alerts.

  
![An IDS circled above an image of a switch, which rests between a firewall and the network.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/5hPelJ74TwaKusUY4ZEkkQ_bcd56306ce904397a352cfe37e28b6f1_CS_R-055_IDS.png?expiry=1714003200000&hmac=vCNH6NzyeEzH2HjD__BB7ACmDqZ0DONS4SJrksA7TsA)

When paired with a firewall, an IDS strengthens the defense. The IDS is positioned behind the firewall, allowing analysis of data streams that haven't been filtered out by the firewall. This reduces the number of false positives (incorrect alerts) generated by the IDS.

### Intrusion Prevention System (IPS)

An IPS actively monitors network activity for intrusions and takes steps to stop them. It offers superior protection compared to an IDS because it can automatically block suspicious activity.

IPS systems search for known attack signatures and data irregularities. Upon detecting an anomaly, an IPS can report it to security personnel and block a specific sender or drop network packets that appear suspicious.

An IPS, similar to an IDS, is situated behind the firewall within the network architecture. This placement provides a high level of security by disrupting potentially risky data streams before they reach sensitive areas of the network. However, there are downsides to consider:

- **Inline nature:** If an IPS malfunctions, the connection between the private network and the internet might be disrupted.
- **False positives:** Like IDS, IPS systems are susceptible to generating false positives, potentially causing legitimate traffic to be dropped.

![An IPS is situated between a firewall and the internal network.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/sp1NiS2HR3KoLCBP36lq3g_f612a9b5e6cc47b2a9341208200b3ff1_CS_R-055_IPS.png?expiry=1714003200000&hmac=bDgfhodBDHXZrnbrywD-prKrVFI500Wk6iovCZlRCuQ)

### Full Packet Capture Devices

These devices can be incredibly valuable for network administrators and security professionals. They allow you to record and analyse all network traffic data, aiding in investigations triggered by IDS alerts.

### Security Information and Event Management (SIEM)

A SIEM system is an application designed to collect and analyse log data from various network devices in order to monitor critical activities within an organization. SIEM tools function in real-time to report suspicious activity on a centralized dashboard. Additionally, they analyse network log data collected from IDSs, IPSs, firewalls, VPNs, proxies, and DNS logs. SIEM tools serve as a way to aggregate security event data into a single location for analysis by security professionals. This centralized view is often referred to as a **single pane of glass**.

  
![Image of the Chronicle dashboard](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/sTtz1jL8QzCTVyhfvICu1A_ee623d56206843d6823598a8f0e70ef1_eyi2ksdTfw4mJcwZ6NvBKQBg-7CVFr-2tq8qNBLlVbloMUlJsvGdPwkSGEk-5VnBU3eXxe9dF7mGPjvyN2T3nWNKtXtu19K2Ycnbt_rEE5FAE4rbNvixbF_oeU82PyiZWpEVVoTqMf6eQJWl7uRMQyvIWA94vNp88ew46W52Kh7QkFeihWUfB8cQkB5dI5c?expiry=1714003200000&hmac=xj2fanoRUvRYlJNAOjE8auW7pgNWeOfY0vYip8IbGb4)

### Advantages and Disadvantages

|Device/Tool|Advantages|Disadvantages|
|---|---|---|
|Firewall|- Filters traffic based on rules|- Limited to packet header inspection|
|Intrusion Detection System|- Alerts on possible intrusions and attacks|- May miss new and sophisticated attacks|
|Intrusion Prevention System|- Actively stops intrusive activity|- Inline appliance, potential for false positives|
|SIEM|- Centralizes security event monitoring|- Reports on security issues, no direct action|

### Considerations

- Cost: Devices/tools require purchasing, installation, and maintenance costs.
- Personnel: Organizations may need additional staff for monitoring security tools, especially SIEMs.
- Risk Management: Decision-makers choose security levels based on cost and risk assessment.

---
## Cloud Network Hardening

Along with securing traditional on-premise networks, security analysts must also secure cloud-based networks used by many organizations today.

**What is a cloud network?**

A cloud network is a collection of servers or virtual machines that store data and resources in a remote data center. These resources are accessible via the internet and can be used to host company data and applications. Cloud computing offers on-demand storage, processing power, and data analytics capabilities.

**Why secure cloud servers?**

Just like physical web servers, cloud servers require proper maintenance and security hardening procedures. While cloud service providers are responsible for the overall infrastructure security, they cannot prevent all intrusions, especially those by malicious actors (internal or external).

**Cloud network hardening vs traditional network hardening**

One key difference between hardening traditional and cloud networks is the use of server baseline images. These baseline images are used as a reference point to compare cloud server data. Any deviations from the baseline image could indicate unauthorized changes or potential intrusions.

**Data and application separation**

Similar to OS hardening, data and applications on a cloud network should be segregated based on their service category. Here are some examples of separation best practices:

- Isolate older applications from newer ones.
- Separate software used for internal functions from user-facing front-end applications.

**Shared security responsibility**

Cloud service providers share security responsibility with the organizations using their services. However, organizations must still implement their own security measures to ensure the safety of their cloud network. These security measures are similar to those used in traditional networks and focus on securing cloud-based operations.

## Cloud Security Considerations

This reading focuses on security considerations specific to cloud computing environments and the shared responsibility model used for cloud security.

**Why is cloud security important?**

Many organizations migrate to the cloud for its benefits like ease of deployment, scalability, and cost savings. However, cloud environments introduce unique security challenges that require attention.

**Key Security Considerations**

- **Identity and Access Management (IAM):** A critical aspect of cloud security is IAM, which controls user access to cloud resources. Loose configuration of user roles can lead to unauthorized access and security risks.
    
- **Configuration Management:** The abundance of cloud services creates complexity. Each service needs careful configuration to meet security and compliance requirements. Improper configuration during migration or ongoing use can leave the network vulnerable.
    
- **Attack Surface:** Cloud service providers (CSPs) offer numerous applications and services, each with its own set of vulnerabilities. This expands the overall attack surface for organizations. While more services might seem to introduce more entry points, a well-designed cloud network can mitigate this risk.
    
- **Zero-Day Attacks:** These are previously unknown exploits. CSPs are more likely to be aware of zero-day attacks and have patching procedures in place to protect customer workloads. Organizations can also use patching tools at the operating system level.
    
- **Visibility and Tracking:** Unlike traditional networks where administrators can monitor all data packets, cloud visibility relies on flow logs and tools like packet mirroring offered by the CSP. While CSPs implement strong security measures, reduced visibility might be a concern for some organizations accustomed to full network control. CSPs undergo third-party audits to verify security posture and identify vulnerabilities.
    
- **Keeping Up with Change:** CSPs constantly update their services, which can impact security considerations for their customers. Organizations may need to adjust configurations or update IT processes to adapt to these changes.
    
- **Shared Responsibility Model:** This model defines the division of security responsibility between the CSP and the customer. The CSP is responsible for the underlying cloud infrastructure, while the customer is responsible for the security of their assets and processes stored or operated in the cloud. A clear understanding of these shared responsibilities is critical for effective cloud security.
    

**Key Takeaways**

- Cloud security requires understanding unique cloud security considerations and the shared responsibility model.
- Organizations must properly configure and maintain security best practices for their cloud services.
- The shared responsibility model clarifies security ownership between the CSP and the customer.

## Cloud Security Hardening with Cryptography

This reading covers cloud security hardening techniques and cryptography fundamentals essential for securing cloud storage and processing.

**Cloud Security Hardening Techniques**

- **Identity and Access Management (IAM):** Similar to on-premise networks, IAM controls user access to cloud resources, preventing unauthorized actions.
    
- **Hypervisors:** These tools virtualize hardware, allowing for multiple operating systems to run on a single machine. CSPs are responsible for managing hypervisors and patching vulnerabilities to prevent virtual machine escapes (unauthorized access to the primary hypervisor).
    
- **Baselining:** This establishes a reference point for cloud environment configuration. Regularly comparing the configuration to the baseline helps identify unauthorized changes and maintain a secure posture. Examples of baseline practices include restricting admin portal access, enabling password management, and file/database encryption.
    

**Cryptography in the Cloud**

- **Cryptography** protects data confidentiality and integrity through encryption and secure key management.
    
- **Encryption** scrambles data into an unreadable format (ciphertext) using an encryption key. Only those with the decryption key can access the original data (plaintext).
    
- **Cryptographic Erasure (Crypto-Shredding):** This method destroys encryption keys, rendering encrypted data permanently inaccessible. Traditional data destruction methods are ineffective in the cloud.
    

**Key Management**

- **Trusted Platform Module (TPM):** This secure chip stores passwords, certificates, and encryption keys on user devices.
    
- **Cloud Hardware Security Module (CloudHSM):** This secure device stores and processes cryptographic keys within the cloud provider's infrastructure.
    

**Shared Responsibility Model**

- Customers can request security audits from their CSPs but typically don't have access to the specific encryption keys used.
    
- Customers can bring their own encryption keys (BYOK) for certain services. They are then responsible for managing the confidentiality of these keys.
    
- The CSP is responsible for maintaining the underlying cryptographic infrastructure. Customers can assess this risk by reviewing the CSP's security controls and audits.
    

**Key Takeaways**

Cloud security hardening requires a combination of IAM, baselining, hypervisor security, cryptography, and cryptographic erasure. Understanding the shared responsibility model for encryption key management is crucial for effective cloud security.

---
## Glossary terms from module 4

**Baseline configuration (baseline image):** A documented set of specifications within a system that is used as a basis for future builds, releases, and updates

**Hardware:** The physical components of a computer

**Multi-factor authentication (MFA):** A security measure which requires a user to verify their identity in two or more ways to access a system or network

**Network log analysis:** The process of examining network logs to identify events of interest 

**Operating system (OS):** The interface between computer hardware and the user

**Patch update:** A software and operating system update that addresses security vulnerabilities within a program or product

**Penetration testing (pen test):** A simulated attack that helps identify vulnerabilities in systems, networks, websites, applications, and processes 

**Security hardening:** The process of strengthening a system to reduce its vulnerabilities and attack surface

**Security information and event management (SIEM):** An application that collects and analyses log data to monitor critical activities for an organization

**World-writable file:** A file that can be altered by anyone in the world