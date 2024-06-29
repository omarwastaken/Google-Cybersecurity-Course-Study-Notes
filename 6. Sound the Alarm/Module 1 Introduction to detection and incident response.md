# Detection and Response
---
#### In this course, you will:

- Explain the lifecycle of an incident
- Use packet sniffing tools to capture and view network communications
- Perform artifact investigations to analyse and verify security incidents
- Identify the steps to contain, eradicate, and recover from an incident
- Interpret the basic syntax and components of signatures and logs in IDS and NIDS tools

#### Skill sets:

- Capturing, viewing, and analysing a packet
- Investigating a suspicious hash file
- Following a playbook
- Examining alerts, logs, and rules
- Performing queries with SIEM tools

---
# The incident response lifecycle

## Introduction to the Incident Response Lifecycle

Incident lifecycle frameworks provide a structure to support incident response operations. Frameworks help organizations develop a standardized approach to their incident response process, ensuring incidents are managed in an effective and consistent way. There are various frameworks that organizations can adopt and modify according to their needs.

### NIST CSF and Incident Response Lifecycle

## In this course, we will focus on the NIST Cybersecurity Framework (CSF). The five core functions of the NIST CSF are:

- Identify
- Protect
- Detect
- Respond
- Recover

This course will explore the last three steps of this framework: detect, respond, and recover. These stages are critical during incident response, and as an analyst, you'll detect and respond to incidents and implement actions for recovery.

The NIST incident response lifecycle is another NIST framework with additional substeps dedicated to incident response. It consists of:

1. Preparation
2. Detection and Analysis
3. Containment, Eradication, and Recovery
4. Post-Incident Activity

It's important to note that the incident lifecycle isn't a linear process. It's a cycle, meaning steps can overlap as new discoveries are made.

### Understanding an Incident

According to NIST, an incident is:

> "An occurrence that actually or imminently jeopardizes, without lawful authority, the confidentiality, integrity, or availability of information or an information system; or constitutes a violation or imminent threat of violation of law, security policies, security procedures, or acceptable use policies."

All security incidents are events, but not all events are security incidents.

**Event Definition**: An observable occurrence on a network, system, or device.

## **Example of an Event**:

- A user forgets their password, requests a reset, and successfully changes their password.
    - This is an observable event logged by systems and applications.

## **Example of a Security Incident**:

- A malicious actor initiates a password change request and gains unauthorized access to an account.
    - This is both an event and a security incident.

### Incident Investigation

## Security analysts, like detectives, carefully handle and document their evidence and findings during an incident investigation. An incident investigation reveals critical information about the five W's of an incident:

- Who triggered the incident
- What happened
- When the incident took place
- Where the incident took place
- Why the incident occurred

### Documentation

Documenting and referencing information is essential during an incident investigation and when writing the final report. An incident handler's journal is a useful tool for this purpose.

### Key Points to Remember

- Incident lifecycle frameworks provide structure for effective incident response.
- NIST CSF's core functions: Identify, Protect, Detect, Respond, and Recover.
- NIST incident response lifecycle steps: Preparation, Detection and Analysis, Containment, Eradication and Recovery, Post-Incident Activity.
- All security incidents are events, but not all events are security incidents.
- Proper documentation is crucial for effective incident management.

---
# Incident response operations

## Incident Response Teams

### Overview

Incident response teams are critical in managing and responding to security incidents. A successful response requires a diverse team working towards a common goal. This includes both security and non-security professionals with defined roles.

### CSIRT - Computer Security Incident Response Team

- **Definition**: A specialized group trained in incident management and response.
- **Goals**:
    - Effectively manage incidents.
    - Provide response and recovery services and resources.
    - Prevent future incidents.

### Collaboration

- **Shared Responsibility**: Security is a shared responsibility requiring cross-functional teamwork.
- **Example**: If sensitive data (like PII or financial documents) is breached, the legal team must be consulted for regulatory compliance and public disclosure. CSIRTs must collaborate with public relations to manage disclosures.

### CSIRT Functions

1. **Security Analyst**
    
    - **Role**: Investigates security alerts to determine if an incident has occurred.
    - **Criticality Rating**: Determines the criticality of the incident. Low criticality incidents can be resolved by the analyst; high criticality incidents are escalated.
2. **Technical Lead**
    
    - **Role**: Provides technical leadership and guides incidents through their lifecycle.
3. **Incident Coordinator**
    
    - **Role**: Tracks and manages the activities of the CSIRT and other involved teams.
    - **Responsibility**: Ensures incident response processes are followed and teams are updated on incident status.

### Variations in CSIRTs

- **Different Names**: CSIRTs can also be known as Incident Handling Teams (IHT) or Security Incident Response Teams (SIRT).
- **Organizational Structure**:
    - **Specialization**: Some teams may focus solely on crisis management or be integrated with a Security Operations Center (SOC).
    - **Role Titles**: Roles can vary in name (e.g., Technical Lead can be known as Ops Lead).

### Common Goal

Regardless of the name or structure, all incident response teams share the goal of effective incident management and response.

### Key Takeaways

- Incident response requires a coordinated team effort.
- CSIRTs manage incidents, provide recovery resources, and prevent future incidents.
- Cross-functional collaboration is essential for effective incident response.
- Understanding the roles within a CSIRT helps in coordinating and managing security incidents efficiently.

## Roles in Response

So far, you've been introduced to the **National Institute of Standards and Technology (NIST) Incident Response Lifecycle**, which is a framework for incident response consisting of four phases:

- Preparation
- Detection and Analysis
- Containment, Eradication, and Recovery
- Post-incident activity

As a security professional, you'll work on a team to monitor, detect, and respond to incidents. Previously, you learned about a **computer security incident response team (CSIRT)** and a **security operations center (SOC)**. This reading explains the different functions, roles, and responsibilities that make up CSIRTs and SOCs.

Understanding the composition of incident response teams will help you navigate an organization’s hierarchy, openly collaborate and communicate with others, and work cohesively to respond to incidents. You may even discover specific roles that you’re interested in pursuing as you begin your security career!

### Command, Control, and Communication

A **computer security incident response team (CSIRT)** is a specialized group of security professionals trained in incident management and response. During incident response, teams can encounter various challenges. For incident response to be effective and efficient, there must be clear command, control, and communication of the situation to achieve the desired goal.

- **Command**: Having the appropriate leadership and direction to oversee the response.
- **Control**: Managing technical aspects during incident response, such as coordinating resources and assigning tasks.
- **Communication**: Keeping stakeholders informed.

Establishing a CSIRT organizational structure with clear and distinctive roles aids in achieving an effective and efficient response.

### Roles in CSIRTs

CSIRTs can vary in structure and operation depending on the organization. They can exist as a separate, dedicated team or as a task force that meets when necessary. CSIRTs involve both non-security and security professionals. Non-security professionals are often consulted to offer their expertise on the incident. These professionals can be from external departments, such as human resources, public relations, management, IT, legal, and others. Security professionals involved in a CSIRT typically include three key security-related roles:

1. **Security Analyst**
2. **Technical Lead**
3. **Incident Coordinator**

#### Security Analyst

The job of the **security analyst** is to continuously monitor an environment for any security threats. This includes:

- Analyzing and triaging alerts
- Performing root-cause investigations
- Escalating or resolving alerts

If a critical threat is identified, analysts escalate it to the appropriate team lead, such as the technical lead.

#### Technical Lead

The job of the **technical lead** is to manage all of the technical aspects of the incident response process, such as applying software patches or updates. They do this by first determining the root cause of the incident. Then, they create and implement the strategies for containing, eradicating, and recovering from the incident. Technical leads often collaborate with other teams to ensure their incident response priorities align with business priorities, such as reducing disruptions for customers or returning to normal operations.

#### Incident Coordinator

Responding to an incident also requires cross-collaboration with non-security professionals. CSIRTs will often consult with and leverage the expertise of members from external departments. The job of the **incident coordinator** is to coordinate with the relevant departments during a security incident. By doing so, the lines of communication are open and clear, and all personnel are made aware of the incident status. Incident coordinators can also be found in other teams, like the SOC.

#### Other Roles

Depending on the organization, many other roles can be found in a CSIRT, including a dedicated communications lead, a legal lead, a planning lead, and more.

**Note**: Teams, roles, responsibilities, and organizational structures can differ for each company. For example, some different job titles for incident coordinator include incident commander and incident manager.

### Security Operations Center (SOC)

A **security operations center (SOC)** is an organizational unit dedicated to monitoring networks, systems, and devices for security threats or attacks. Structurally, a SOC (usually pronounced "sock") often exists as its own separate unit or within a CSIRT. You may be familiar with the term _blue team_, which refers to the security professionals who are responsible for defending against all security threats and attacks at an organization. A SOC is involved in various types of blue team activities, such as network monitoring, analysis, and response to incidents.

### SOC Organization

A SOC is composed of SOC analysts, SOC leads, and SOC managers. Each role has its own respective responsibilities. SOC analysts are grouped into three different tiers.

![A triangle with four labeled tiers. From bottom to top: SOC Analyst L1, SOC Analyst L2, SOC Lead L3, and Manager.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/CMDszNSgSryqbipKuGOU2Q_222b5865df5f4a72a785cd94279d99f1_CkqInM-0iDHKapM_2jS_68ZBhx11oR2GR_fCveMT5EI39E4h_dsAwBstgiRAXmj-mLFWXeOLNnSpBeMpDrEOiP9N8P9efbhWwLqNx-nDZFmoa6ue7SuqH0iUjmnMPWmpEcZPjKUY7ONnH6qkmt7wqF1XpuxPDe1zCbwGriZcyQRpSru_CG-tzvFvMDe5cg?expiry=1716422400000&hmac=qh8Fo7qwyl8n-bUbNHvtuwJ9aRbugDMALnHSRyMPn14)

#### Tier 1 SOC Analyst

The first tier is composed of the least experienced SOC analysts who are known as level 1s (L1s). They are responsible for:

- Monitoring, reviewing, and prioritizing alerts based on criticality or severity
- Creating and closing alerts using ticketing systems
- Escalating alert tickets to Tier 2 or Tier 3

#### Tier 2 SOC Analyst

The second tier comprises the more experienced SOC analysts, or level 2s (L2s). They are responsible for:

- Receiving escalated tickets from L1 and conducting deeper investigations
- Configuring and refining security tools
- Reporting to the SOC Lead

#### Tier 3 SOC Lead

The third tier of a SOC is composed of the SOC leads, or level 3s (L3s). These highly experienced professionals are responsible for:

- Managing the operations of their team
- Exploring methods of detection by performing advanced detection techniques, such as malware and forensics analysis
- Reporting to the SOC manager

#### SOC Manager

The SOC manager is at the top of the pyramid and is responsible for:

- Hiring, training, and evaluating the SOC team members
- Creating performance metrics and managing the performance of the SOC team
- Developing reports related to incidents, compliance, and auditing
- Communicating findings to stakeholders such as executive management

#### Other Roles

SOCs can also contain other specialized roles such as:

- **Forensic Investigators**: Forensic investigators are commonly L2s and L3s who collect, preserve, and analyse digital evidence related to security incidents to determine what happened.
- **Threat Hunters**: Threat hunters are typically L3s who work to detect, analyse, and defend against new and advanced cybersecurity threats using threat intelligence.

**Note**: Just like CSIRTs, the organizational structure of a SOC can differ depending on the organization.

### Key Takeaways

As a security analyst, you will collaborate with your team members and people outside of your immediate team. Recognizing the organizational structure of an incident response team, such as a CSIRT or SOC, will help you understand how incidents move through their lifecycle and the responsibilities of different security roles throughout the process. Knowing the role that you and other professionals have during an incident response event will help you respond to challenging security situations by leveraging different perspectives and thinking of creative solutions.


## Incident Response Plans

### Overview

Incident response plans are critical for ensuring that teams can respond to security incidents quickly, efficiently, and effectively. These plans are tailored to meet the unique requirements of an organization and outline the procedures to take during each step of incident response.

### Common Elements of Incident Response Plans

**Incident response plans** typically include the following elements:

1. **Incident Response Procedures**: Step-by-step instructions on how to respond to various types of incidents.
2. **System Information**: This includes network diagrams, data flow diagrams, logging information, and asset inventory details.
3. **Supporting Documents**: Contact lists, forms, and templates that may be required during an incident response.

### Importance of Incident Response Plans

- **Quick Response**: Having a plan ensures that teams can respond promptly to incidents, minimizing potential damage.
- **Regulatory Compliance**: Plans help organizations meet regulatory requirements, such as reporting incidents within specific timeframes.
- **Consistency**: A formal plan ensures a consistent response to incidents, reducing the risk of oversight or error.

### Incident Response Plan Components

#### Incident Response Procedures

**Incident response procedures** provide detailed, step-by-step instructions for handling incidents. These procedures are designed to guide the team through the response process efficiently.

|Term|Definition|
|---|---|
|Incident Response Procedures|Step-by-step instructions on how to respond to incidents|
|System Information|Includes network diagrams, data flow diagrams, logging information, and asset inventory details|
|Supporting Documents|Contact lists, forms, and templates required during an incident response|

#### System Information

**System information** is crucial for understanding the organization's infrastructure and potential impact areas. This includes:

- **Network Diagrams**: Visual representations of the network structure.
- **Data Flow Diagrams**: Illustrations of how data moves within the system.
- **Logging Information**: Records of system activities that can help in tracing the incident's origin.
- **Asset Inventory**: A catalog of all assets that need protection.

|Term|Definition|
|---|---|
|Network Diagrams|Visual representations of the network structure|
|Data Flow Diagrams|Illustrations of how data moves within the system|
|Logging Information|Records of system activities that can help in tracing the incident's origin|
|Asset Inventory|A catalog of all assets that need protection|

#### Supporting Documents

Supporting documents ensure that the team has all necessary resources readily available during an incident. This includes:

- **Contact Lists**: Lists of key personnel and their contact information.
- **Forms**: Templates for documenting incidents and responses.
- **Templates**: Pre-defined formats for reporting and communication.

|Term|Definition|
|---|---|
|Contact Lists|Lists of key personnel and their contact information|
|Forms|Templates for documenting incidents and responses|
|Templates|Pre-defined formats for reporting and communication|

### Testing and Reviewing Incident Response Plans

Incident response plans must be regularly reviewed and tested to ensure their effectiveness. This can be done through exercises such as:

- **Tabletop Exercises**: Discussion-based sessions where team members walk through the response plan.
- **Simulations**: Realistic drills that mimic actual incident scenarios.

These exercises help familiarize team members with the plan and identify any gaps or areas for improvement.

### Key Takeaways

- Incident response plans are essential for a quick, efficient, and effective response to security incidents.
- Plans should be tailored to the organization's unique needs and regularly reviewed and tested.
- Common elements of incident response plans include procedures, system information, and supporting documents.
- Regular exercises ensure that team members are familiar with the plan and help identify any gaps.

---
# Incident response tools

## Incident Response Tools

As a security analyst, your role in incident detection is critical. You'll be at the front lines, actively identifying and responding to threats. To effectively carry out your duties, you’ll need a variety of tools and technologies. This guide will introduce you to some essential incident response tools and how they support your investigations.

### Detection and Management Tools

Detection and management tools are essential for monitoring system activity and identifying events that require investigation. These tools help you keep track of what's happening within the network and spot any anomalies or potential threats.

|**Term**|**Definition**|
|---|---|
|**Intrusion Detection System (IDS)**|A tool that monitors network traffic for suspicious activity and issues alerts.|
|**Security Information and Event Management (SIEM)**|A system that collects, analyses, and correlates security event data from various sources.|

### Documentation Tools

Documentation tools are crucial for collecting and compiling evidence during an investigation. Keeping thorough records helps ensure that all relevant information is available and can be referenced later.

|**Term**|**Definition**|
|---|---|
|**Incident Handler’s Journal**|A form of documentation used by security analysts to record details of incidents.|

### Investigative Tools

Investigative tools allow you to analyse events and gather detailed information about security incidents. These tools help you delve deeper into the data to understand the nature and impact of the threat.

|**Term**|**Definition**|
|---|---|
|**Packet Sniffer**|A tool that captures and analyses network packets to monitor data flow and detect anomalies.|
|**Network analyser**|A tool used to examine and diagnose network issues, often used to identify malicious traffic.|

### Continuous Learning and Adaptation

New security technologies constantly emerge, threats evolve, and attackers become stealthier to avoid detection. To remain effective at detecting threats, you must continuously expand your security toolbox and stay updated on the latest advancements in the field.

### Practical Application: Incident Handler’s Journal

The incident handler’s journal will be your first security tool. Use this journal to document every detail of incidents you encounter, from initial detection to resolution. This practice will help you maintain a clear and organized record of your investigations, which is essential for effective incident response.

## The Value of Documentation

### Overview

In incident response, documentation is crucial for tracking and managing incidents. This guide will explore the different types of documentation, their importance, and the tools used for effective documentation.

### Types of Documentation

There are various forms of documentation used in incident response. Each type serves a specific purpose in guiding and instructing security professionals on how to manage incidents effectively.

|**Term**|**Definition**|
|---|---|
|**Playbooks**|Manuals that provide detailed steps for operational actions during an incident.|
|**Incident Handler’s Journal**|A form of documentation used to record the 5 W's of an incident: who, what, where, when, and why.|
|**Policies**|Guidelines that outline the principles and rules for security practices.|
|**Plans**|Detailed strategies for responding to various types of incidents.|
|**Final Reports**|Comprehensive documents that summarize the incident, response actions, and outcomes.|

### Importance of Effective Documentation

Effective documentation is essential during a security incident. It ensures that all team members are on the same page and can respond quickly and accurately. Here are some key points about the importance of effective documentation:

- **Reduces Uncertainty and Confusion**: Clear documentation helps in reducing confusion during high-pressure situations.
- **Provides Clear Instructions**: Ensures that team members know exactly what steps to take during an incident.
- **Maintains Consistency**: Standardized documentation practices ensure that all incidents are handled in a consistent manner.
- **Facilitates Communication**: Good documentation aids in communicating the status and details of an incident to all relevant stakeholders.

### Tools for Documentation

Various tools can be used to document incidents effectively. These tools range from word processors to ticketing systems and even handwritten notes. Here are some commonly used tools:

|**Tool**|**Description**|
|---|---|
|**Google Docs**|A web-based word processor that allows for real-time collaboration and document sharing.|
|**OneNote**|A digital note-taking application that organizes notes in notebooks, sections, and pages.|
|**Evernote**|A note-taking app designed for organizing and storing various types of information.|
|**Notepad++**|A free source code editor and Notepad replacement that supports several programming languages.|
|**Jira**|A ticketing system used to document, track, and manage incidents and issues.|
|**Google Sheets**|A web-based spreadsheet application used for organizing and analyzing data.|
|**Audio Recorders**|Devices or applications used to record verbal reports and discussions.|
|**Cameras**|Tools used to capture visual evidence of incidents or affected areas.|
|**Handwritten Notes**|Traditional method for quickly jotting down observations, thoughts, and instructions.|

### Key Takeaways

Effective documentation is a cornerstone of successful incident response. It ensures clarity, consistency, and accuracy, which are vital for swift and decisive actions during an incident. Using the right tools and maintaining good documentation practices can significantly improve the efficiency and effectiveness of your incident response efforts.

## Intrusion Detection Systems (IDS)

### Overview

Intrusion Detection Systems (IDS) and Intrusion Prevention Systems (IPS) are critical components of network security. These systems help monitor, detect, and respond to potential threats within an organization's network.

### Intrusion Detection Systems (IDS)

An Intrusion Detection System (IDS) is a security application designed to monitor network and system activities for malicious actions or policy violations. The main function of an IDS is to produce alerts when suspicious activity is detected.

|Term|Definition|
|---|---|
|Intrusion Detection System (IDS)|An application that monitors system and network activity, producing alerts on possible intrusions.|

#### How IDS Works

- **Monitoring**: IDS continuously monitors network traffic and system activities.
- **Detection**: It uses various detection methods to identify abnormal or malicious behavior.
- **Alerting**: When suspicious activity is detected, the IDS sends alerts to the appropriate channels or personnel.

### Intrusion Prevention Systems (IPS)

An Intrusion Prevention System (IPS) builds on the capabilities of an IDS by not only detecting potential threats but also taking action to prevent them.

|Term|Definition|
|---|---|
|Intrusion Prevention System (IPS)|A system that monitors network and system activities for intrusions and takes action to stop them.|

#### How IPS Works

- **Monitoring and Detection**: Like IDS, IPS monitors and detects suspicious activities.
- **Prevention**: IPS can automatically take actions, such as blocking traffic or dropping malicious packets, to prevent potential intrusions.

### IDS vs. IPS

|Feature|IDS|IPS|
|---|---|---|
|Monitoring|Yes|Yes|
|Detection|Yes|Yes|
|Prevention|No|Yes|
|Action Taken|Alerts only|Blocks or mitigates threats|

### Common IDS/IPS Tools

There are several tools available that combine IDS and IPS functionalities. Some popular tools include:

|Tool|Description|
|---|---|
|Snort|An open-source network intrusion detection and prevention system.|
|Zeek|Formerly known as Bro, a powerful network analysis framework.|
|Kismet|A wireless network detector, sniffer, and intrusion detection system.|
|Sagan|A multi-threaded, real-time log analysis and correlation engine.|
|Suricata|An open-source threat detection engine that performs intrusion detection, prevention, and network security monitoring.|

### Managing Alerts with SIEM

Security Information and Event Management (SIEM) tools are used to manage and analyse the alerts generated by IDS and IPS. These tools collect, correlate, and analyse security event data from various sources, providing a centralized view of an organization's security posture.

|Term|Definition|
|---|---|
|SIEM|Security Information and Event Management, a set of tools and services offering real-time analysis of security alerts generated by applications and network hardware.|

### Key Takeaways

- **Intrusion Detection Systems (IDS)**: Monitor and detect suspicious activities, generating alerts.
- **Intrusion Prevention Systems (IPS)**: Extend IDS capabilities by taking action to prevent detected threats.
- **Tools**: Popular tools like Snort, Zeek, Kismet, Sagan, and Suricata can perform both IDS and IPS functions.
- **SIEM**: Used to manage and analyse security alerts from IDS/IPS, providing a comprehensive view of security events.

## Overview of Detection Tools

### Why You Need Detection Tools

Detection tools are essential for cybersecurity, much like home security systems. They help organizations protect their networks and systems by monitoring for unauthorized access and other suspicious activities. When an anomaly is detected, these tools alert security professionals to investigate and potentially stop the intrusion.

### Detection Tools

As a security analyst, you will encounter various detection tools, including IDS, IPS, and EDR. Understanding their differences is crucial.

|**Capability**|**IDS**|**IPS**|**EDR**|
|---|---|---|---|
|Detects malicious activity|✓|✓|✓|
|Prevents intrusions|N/A|✓|✓|
|Logs activity|✓|✓|✓|
|Generates alerts|✓|✓|✓|
|Performs behavioral analysis|N/A|N/A|✓|

### Overview of IDS Tools

An **Intrusion Detection System (IDS)** monitors system activity and alerts on possible intrusions. It provides continuous monitoring but does not stop the activity. Security professionals must investigate and take action if necessary.

Examples: Zeek, Suricata, Snort®, Sagan.

#### Detection Categories

|Term|Definition|
|---|---|
|True Positive|An alert that correctly detects the presence of an attack.|
|True Negative|A state where there is no detection of malicious activity, and no alert is triggered.|
|False Positive|An alert that incorrectly detects the presence of a threat, resulting in a wasted investigation.|
|False Negative|A state where the presence of a threat is not detected, leaving the system vulnerable.|

### Overview of IPS Tools

An **Intrusion Prevention System (IPS)** monitors system activity for intrusions and takes action to stop them. It works similarly to an IDS but also prevents the activity.

Examples: Suricata, Snort, Sagan.

### Overview of EDR Tools

**Endpoint Detection and Response (EDR)** monitors endpoints (devices connected to a network) for malicious activity. EDR tools analyse endpoint system activity, perform behavioral analysis using machine learning and AI, and use automation to stop attacks without manual intervention.

Examples: Open EDR®, Bitdefender™ Endpoint Detection and Response, FortiEDR™.

### Key Takeaways

- **IDS**: Detects and alerts on suspicious activities but does not prevent them.
- **IPS**: Detects, alerts, and prevents suspicious activities.
- **EDR**: Monitors, records, analyses endpoint activities, and performs behavioral analysis to identify and stop threats.

## Alert and Event Management with SIEM and SOAR Tools

### Overview

In this section, we'll delve into how security information and event management (SIEM) and security orchestration, automation, and response (SOAR) tools function. These tools are critical in the detection, analysis, and response phases of incident management.

### Why You Need Detection Tools

Detection tools help organizations protect their networks and systems from unauthorized access and potential security threats by continuously monitoring activities and generating alerts for suspicious behaviors.

### Detection Tools

|**Capability**|**IDS**|**IPS**|**EDR**|
|---|---|---|---|
|Detects malicious activity|✓|✓|✓|
|Prevents intrusions|N/A|✓|✓|
|Logs activity|✓|✓|✓|
|Generates alerts|✓|✓|✓|
|Performs behavioral analysis|N/A|N/A|✓|

### SIEM Tools

#### What is SIEM?

SIEM is a tool that collects and analyses log data to monitor critical activities in an organization. It provides a high-level overview of network activities and helps security professionals identify potential threats.

#### How SIEM Works

- **Collection and Aggregation**: SIEM tools gather data from various sources such as IDS/IPS, databases, firewalls, and applications. This data is centralized in one location.
- **Normalization**: The collected data is cleaned and formatted to ensure consistency, which makes searching and analysis easier.
- **Analysis**: SIEM tools analyse the normalized data against predefined rules to detect potential security incidents, generating alerts for security analysts to review.

### SOAR Tools

#### What is SOAR?

SOAR stands for Security Orchestration, Automation, and Response. It is a collection of tools, applications, and workflows that automate the analysis and response to security incidents.

#### How SOAR Works

- **Automation**: SOAR tools automate the processes of analyzing and responding to security events, reducing the need for manual intervention.
- **Case Management**: SOAR tools help track and manage incidents, allowing security teams to view multiple incidents in one centralized platform.

### Key Functions of SIEM and SOAR

#### SIEM Functions

1. **Collection and Aggregation**: Collects log data from various sources and centralizes it.
2. **Normalization**: Cleans and standardizes the collected data.
3. **Analysis**: Uses rules to analyse data and generate alerts for potential security threats.

#### SOAR Functions

1. **Automation**: Automates the response to security incidents.
2. **Orchestration**: Integrates with other security tools to streamline incident response.
3. **Case Management**: Tracks and manages security incidents in a centralized platform.

### Conclusion

SIEM and SOAR tools are essential for effective incident management. SIEM tools provide the ability to collect, normalize, and analyse large volumes of data to detect potential threats. SOAR tools enhance this capability by automating the response to these threats, ensuring quicker and more efficient incident management. Understanding these tools and their functionalities is crucial for any security analyst.

## Overview of SIEM Technology

Previously, you learned about the SIEM process. In this reading, you'll explore more about this process and why SIEM tools are an important part of incident detection and response. As a refresher, a security information and event management (SIEM) tool is an application that collects and analyses log data to monitor critical activities in an organization. You might recall that SIEM tools help security analysts perform log analysis which is the process of examining logs to identify events of interest.

### SIEM Advantages

SIEM tools collect and manage security-relevant data that can be used during investigations. This is important because SIEM tools provide awareness about the activity that occurs between devices on a network. The information SIEM tools provide can help security teams quickly investigate and respond to security incidents. SIEM tools have many advantages that can help security teams effectively respond to and manage incidents. Some of the advantages are:

- **Access to Event Data**: SIEM tools provide access to the event and activity data that happens on a network, including real-time activity. Networks can be connected to hundreds of different systems and devices. SIEM tools have the ability to ingest all of this data so that it can be accessed.
- **Monitoring, Detecting, and Alerting**: SIEM tools continuously monitor systems and networks in real-time. They then analyse the collected data using detection rules to detect malicious activity. If an activity matches the rule, an alert is generated and sent out for security teams to assess.
- **Log Storage**: SIEM tools can act as a system for data retention, which can provide access to historical data. Data can be kept or deleted after a period depending on an organization's requirements.

### The SIEM Process

The SIEM process consists of three critical steps:

1. **Collect and Aggregate Data**
2. **Normalize Data**
3. **analyse Data**

By understanding these steps, organizations can utilize the power of SIEM tools to gather, organize, and analyse security event data from different sources. Organizations can later use this information to improve their ability to identify and mitigate potential threats.

### Collect and Aggregate Data

SIEM tools require data for them to be effectively used. During the first step, the SIEM collects event data from various sources like firewalls, servers, routers, and more. This data, also known as logs, contains event details like timestamps, IP addresses, and more. Logs are a record of events that occur within an organization’s systems. After all of this log data is collected, it gets aggregated in one location. Aggregation refers to the process of consolidating log data into a centralized place. Through collection and aggregation, SIEM tools eliminate the need for manually reviewing and analyzing event data by accessing individual data sources. Instead, all event data is accessible in one location—the SIEM.

Parsing can occur during the first step of the SIEM process when data is collected and aggregated. Parsing maps data according to their fields and their corresponding values. For example, the following log example contains fields with values. At first, it might be difficult to interpret information from this log based on its format:

`April 3 11:01:21 server sshd[1088]: Failed password for user nuhara from 218.124.14.105 port 5023`

In a parsed format, the fields and values are extracted and paired making them easier to read and interpret:

|Field|Value|
|---|---|
|host|server|
|process|sshd|
|source_user|nuhara|
|source_ip|218.124.14.105|
|source_port|5023|

### Normalize Data

SIEM tools collect data from many different sources. This data must be transformed into a single format so that it can be easily processed by the SIEM. However, each data source is different and data can be formatted in many different ways. For example, a firewall log can be formatted differently than a server log.

Collected event data should go through the process of normalization. Normalization converts data into a standard, structured format that is easily searchable.

### analyse Data

After log data has been collected, aggregated, and normalized, the SIEM must do something useful with all of the data to enable security teams to investigate threats. During this final step in the process, SIEM tools analyse the data. Analysis can be done with some type of detection logic such as a set of rules and conditions. SIEM tools then apply these rules to the data, and if any of the log activity matches a rule, alerts are sent out to cybersecurity teams.

**Note**: A part of the analysis process includes correlation. Correlation involves the comparison of multiple log events to identify common patterns that indicate potential security threats.

### SIEM Tools

There are many SIEM tools. The following are some SIEM tools commonly used in the cybersecurity industry:

- AlienVault® OSSIM™
- Chronicle
- Elastic
- Exabeam
- IBM QRadar® Security Intelligence Platform
- LogRhythm
- Splunk

### Key Takeaways

SIEM tools collect and organize enormous amounts of data to create meaningful insights for security teams. By understanding how SIEM tools work, what the process includes, and how organizations leverage them, you can contribute to efforts in detecting and responding to security incidents effectively. With this knowledge, you can assist in analyzing log data, identifying threats, and aiding incident response activities to help improve security posture and protect valuable assets from threats.

---
## Glossary terms from module 1

**Computer security incident response teams (CSIRT):** A specialized group of security professionals that are trained in incident management and response 

**Documentation:** Any form of recorded content that is used for a specific purpose 

**Endpoint detection and response (EDR):** An application that monitors an endpoint for malicious activity

**Event:** An observable occurrence on a network, system, or device

**False negative**: A state where the presence of a threat is not detected

**False positive:** An alert that incorrectly detects the presence of a threat

**Incident:** An occurrence that actually or imminently jeopardizes, without lawful authority, the confidentiality, integrity, or availability of information or an information system; or constitutes a violation or imminent threat of violation of law, security policies, security procedures, or acceptable use policies

**Incident handler’s journal:** A form of documentation used in incident response

**Incident response plan:** A document that outlines the procedures to take in each step of incident response

**Intrusion detection system (IDS):** An application that monitors system activity and alerts on possible intrusions

**Intrusion prevention system (IPS):** An application that monitors system activity for intrusive activity and takes action to stop the activity

**National Institute of Standards and Technology (NIST) Incident Response Lifecycle:** A framework for incident response consisting of four phases: Preparation; Detection and Analysis; Containment, Eradication, and Recovery; and Post-incident activity

**Playbook:** A manual that provides details about any operational action

**Security information and event management (SIEM):** An application that collects and analyses log data to monitor critical activities in an organization 

**Security operations center (SOC):** An organizational unit dedicated to monitoring networks, systems, and devices for security threats or attacks

**Security orchestration, automation, and response (SOAR):** A collection of applications, tools, and workflows that uses automation to respond to security events

**True negative:** A state where there is no detection of malicious activity

**True positive** An alert that correctly detects the presence of an attack