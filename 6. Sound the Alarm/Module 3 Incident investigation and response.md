# Incident detection and verification

## The Detection and Analysis Phase of the Lifecycle

### Introduction

Incidents are inevitable, and as a security analyst, you'll be responsible for investigating and responding to them. This phase focuses on the Detection and Analysis phase of the incident response lifecycle, where incidents are verified and analysed.

### Detection

Detection enables the prompt discovery of security events.

- **Events vs. Incidents**:
    
    - Not all events are incidents, but all incidents are events.
    - **Events**: Regular occurrences in business operations (e.g., website visits, password reset requests).
    - **Incidents**: Security-related events that require investigation (e.g., unauthorized access).
- **Tools Used**:
    
    - **Intrusion Detection Systems (IDS)**: Monitor and analyse network traffic for signs of malicious activity.
    - **Security Information and Event Management (SIEM) tools**: Collect and analyse event data from various sources to identify potential unusual activity.
- **Alert Generation**:
    
    - If an incident is detected, an alert is sent out.
    - The security team then moves to the Analysis phase.

### Analysis

Analysis involves investigating and validating alerts.

- **Investigation and Validation**:
    
    - Analysts apply critical thinking and incident analysis skills.
    - They examine indicators of compromise (IoCs) to determine if an incident has occurred.
- **Challenges in Detection**:
    
    - **Detection Limitations**: It's impossible to detect everything.
        - Detection tools have limitations.
        - Automated tools may not be fully deployed due to limited resources.
    - **High Volume of Alerts**:
        - Analysts can receive thousands of alerts per shift.
        - High alert volumes are often caused by misconfigured alert settings.
        - Broad and untuned alert rules can create false positives.
        - Legitimate high alert volumes can occur when malicious actors exploit newly discovered vulnerabilities.

### Key Takeaways

- **Detection**: Critical for the prompt discovery of security events.
- **Analysis**: Essential for validating and investigating alerts to confirm incidents.
- **Challenges**: Analysts face limitations in detection tools and high volumes of alerts, requiring efficient incident response plans.

## Cybersecurity Incident Detection Methods

Security analysts use detection tools to help them discover threats, but there are additional methods of detection that can be used as well.

Previously, you learned about how detection tools can identify attacks like data exfiltration. In this reading, you’ll be introduced to different detection methods that organizations can employ to discover threats.

### Methods of Detection

During the **Detection and Analysis Phase** of the incident response lifecycle, security teams are notified of a possible incident and work to investigate and verify the incident by collecting and analyzing data. As a reminder, **detection** refers to the prompt discovery of security events and **analysis** involves the investigation and validation of alerts.

As you’ve learned, an intrusion detection system (IDS) can detect possible intrusions and send out alerts to security analysts to investigate the suspicious activity. Security analysts can also use security information and event management (SIEM) tools to detect, collect, and analyse security data.

You’ve also learned that there are challenges with detection. Even the best security teams can fail to detect real threats for a variety of reasons. For example, detection tools can only detect what security teams configure them to monitor. If they aren’t properly configured, they can fail to detect suspicious activity, leaving systems vulnerable to attack. It’s important for security teams to use additional methods of detection to increase their coverage and accuracy.

### Threat Hunting

Threats evolve and attackers advance their tactics and techniques. Automated, technology-driven detection can be limited in keeping up to date with the evolving threat landscape. Human-driven detection like threat hunting combines the power of technology with a human element to discover hidden threats left undetected by detection tools.

**Threat hunting** is the proactive search for threats on a network. Security professionals use threat hunting to uncover malicious activity that was not identified by detection tools and as a way to do further analysis on detections. Threat hunting is also used to detect threats before they cause damage. For example, fileless malware is difficult for detection tools to identify. It’s a form of malware that uses sophisticated evasion techniques such as hiding in memory instead of using files or applications, allowing it to bypass traditional methods of detection like signature analysis. With threat hunting, the combination of active human analysis and technology is used to identify threats like fileless malware.

**Note**: Threat hunting specialists are known as threat hunters. Threat hunters perform research on emerging threats and attacks and then determine the probability of an organization being vulnerable to a particular attack. Threat hunters use a combination of threat intelligence, indicators of compromise, indicators of attack, and machine learning to search for threats in an organization.

### Threat Intelligence

Organizations can improve their detection capabilities by staying updated on the evolving threat landscape and understanding the relationship between their environment and malicious actors. One way to understand threats is by using **threat intelligence**, which is evidence-based threat information that provides context about existing or emerging threats.

Threat intelligence can come from private or public sources like:

- **Industry reports**: These often include details about attackers' tactics, techniques, and procedures (TTP).
- **Government advisories**: Similar to industry reports, government advisories include details about attackers' TTP.
- **Threat data feeds**: Threat data feeds provide a stream of threat-related data that can be used to help protect against sophisticated attackers like **advanced persistent threats (APTs)**. APTs are instances when a threat actor maintains unauthorized access to a system for an extended period of time. The data is usually a list of indicators like IP addresses, domains, and file hashes.

It can be difficult for organizations to efficiently manage large volumes of threat intelligence. Organizations can leverage a _threat intelligence platform_ (TIP) which is an application that collects, centralizes, and analyses threat intelligence from different sources. TIPs provide a centralized platform for organizations to identify and prioritize relevant threats and improve their security posture.

**Note**: Threat intelligence data feeds are best used to add context to detections. They should not drive detections completely and should be assessed before applied to an organization.

### Cyber Deception

Cyber deception involves techniques that deliberately deceive malicious actors with the goal of increasing detection and improving defensive strategies.

**Honeypots** are an example of an active cyber defense mechanism that uses deception technology. Honeypots are systems or resources that are created as decoys vulnerable to attacks with the purpose of attracting potential intruders. For example, having a fake file labeled _Client Credit Card Information - 2022_ can be used to capture the activity of malicious actors by tricking them into accessing the file because it appears to be legitimate. Once a malicious actor tries to access this file, security teams are alerted.

### Key Takeaways

Various detection methods can be implemented to identify and locate security events in an environment. It’s essential for organizations to use a variety of detection methods, tools, and technologies to adapt to the ever-evolving threat landscape and better protect assets.

### Resources for More Information

If you would like to explore more on threat hunting and threat intelligence, here are some resources:

- An [informational repository about threat hunting](https://www.threathunting.net/) from The ThreatHunting Project.
- Research on [state-sponsored hackers](https://blog.google/threat-analysis-group/) from Threat Analysis Group (TAG).

## Indicators of Compromise

In this reading, you’ll be introduced to the concept of the Pyramid of Pain and explore examples of the different types of indicators of compromise. Understanding and applying this concept helps organizations improve their defense and reduce the damage an incident can cause.

### Indicators of Compromise

**Indicators of Compromise (IoCs)** are observable evidence that suggests signs of a potential security incident. IoCs chart specific pieces of evidence that are associated with an attack, like a file name associated with a type of malware. You can think of an IoC as evidence that points to something that's already happened, like noticing that a valuable has been stolen from inside of a car.

**Indicators of Attack (IoAs)** are the series of observed events that indicate a real-time incident. IoAs focus on identifying the behavioral evidence of an attacker, including their methods and intentions.

Essentially, IoCs help to identify the _who_ and _what_ of an attack after it's taken place, while IoAs focus on finding the _why_ and _how_ of an ongoing or unknown attack. For example, observing a process that makes a network connection is an example of an IoA. The filename of the process and the IP address that the process contacted are examples of the related IoCs.

**Note**: Indicators of compromise are not always a confirmation that a security incident has happened. IoCs may be the result of human error, system malfunctions, and other reasons not related to security.

### Pyramid of Pain

Not all indicators of compromise are equal in the value they provide to security teams. It’s important for security professionals to understand the different types of indicators of compromise so that they can quickly and effectively detect and respond to them. This is why security researcher David J. Bianco created the concept of the [Pyramid of Pain](http://detect-respond.blogspot.com/2013/03/the-pyramid-of-pain.html), with the goal of improving how indicators of compromise are used in incident detection.

![Pyramid of Pain](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/5wpDfG3dRQyt3j7I9Vem3Q_31d63be045bc492e9b94aaeeb809a2f1_b5ndsAVFpYfEQSnQvmCly3Ws1dMEo2js79jF_lmAHf6cke-2RsAJfd2JrQ4GoFZdLOIdxxGx-AyNc-cnn4dolkvJLj1dydB1g0JmArLZWeZy7VJLFagiJ0xcq1oz7oirJA4dN8qjz6CI87yrOt-QSvGE7J28YVbPtj59GiU35sLHgGU8RIqqEkRI-JAk5w?expiry=1716508800000&hmac=EfW425wPFtQW1_U58ndoOyLS_h3GBw8cXlgGyv1padg)

The Pyramid of Pain captures the relationship between indicators of compromise and the level of difficulty that malicious actors experience when indicators of compromise are blocked by security teams. It lists the different types of indicators of compromise that security professionals use to identify malicious activity.

Each type of indicator of compromise is separated into levels of difficulty. These levels represent the “pain” levels that an attacker faces when security teams block the activity associated with the indicator of compromise. For example, blocking an IP address associated with a malicious actor is labeled as easy because malicious actors can easily use different IP addresses to work around this and continue with their malicious efforts. If security teams are able to block the IoCs located at the top of the pyramid, the more difficult it becomes for attackers to continue their attacks. Here’s a breakdown of the different types of indicators of compromise found in the Pyramid of Pain.

1. **Hash Values**: Hashes that correspond to known malicious files. These are often used to provide unique references to specific samples of malware or to files involved in an intrusion.
2. **IP Addresses**: An internet protocol address like 192.168.1.1.
3. **Domain Names**: A web address such as [www.google.com](http://www.google.com/).
4. **Network Artifacts**: Observable evidence created by malicious actors on a network. For example, information found in network protocols such as User-Agent strings.
5. **Host Artifacts**: Observable evidence created by malicious actors on a host. A host is any device that’s connected on a network. For example, the name of a file created by malware.
6. **Tools**: Software that’s used by a malicious actor to achieve their goal. For example, attackers can use password-cracking tools like John the Ripper to perform password attacks to gain access to an account.
7. **Tactics, Techniques, and Procedures (TTPs)**: This is the behaviour of a malicious actor. Tactics refer to the high-level overview of the behaviour. Techniques provide detailed descriptions of the behaviour relating to the tactic. Procedures are highly detailed descriptions of the technique. TTPs are the hardest to detect.

### Key Takeaways

Indicators of compromise and indicators of attack are valuable sources of information for security professionals when it comes to detecting incidents. The Pyramid of Pain is a concept that can be used to understand the different types of indicators of compromise and the value they have in detecting and stopping malicious activity.

## analyse Indicators of Compromise with Investigative Tools

So far, you've learned about the different types of detection methods that can be used to detect security incidents. This reading explores how investigative tools can be used during investigations to analyse suspicious **indicators of compromise (IoCs)** and build context around alerts. Remember, an IoC is observable evidence that suggests signs of a potential security incident.

### Adding Context to Investigations

You've learned about the Pyramid of Pain which describes the relationship between indicators of compromise and the level of difficulty that malicious actors experience when indicators of compromise are blocked by security teams. You also learned about different types of IoCs, but as you know, not all IoCs are equal. Malicious actors can manage to evade detection and continue compromising systems despite having their IoC-related activity blocked or limited.

For example, identifying and blocking a single IP address associated with malicious activity does not provide a broader insight on an attack, nor does it stop a malicious actor from continuing their activity. Focusing on a single piece of evidence is like fixating on a single section of a painting: You miss out on the bigger picture.


Security analysts need a way to expand the use of IoCs so that they can add context to alerts. **Threat intelligence** is evidence-based threat information that provides context about existing or emerging threats. By accessing additional information related to IoCs, security analysts can expand their viewpoint to observe the bigger picture and construct a narrative that helps inform their response actions.

By adding context to an IoC—for instance, identifying other artifacts related to the suspicious IP address, such as suspicious network communications or unusual processes—security teams can start to develop a detailed picture of a security incident. This context can help security teams detect security incidents faster and take a more informed approach in their response.

### The Power of Crowdsourcing

**Crowdsourcing** is the practice of gathering information using public input and collaboration. Threat intelligence platforms use crowdsourcing to collect information from the global cybersecurity community. Traditionally, an organization's response to incidents was performed in isolation. A security team would receive and analyse an alert, and then work to remediate it without additional insights on how to approach it. Without crowdsourcing, attackers can perform the same attacks against multiple organizations.


With crowdsourcing, organizations harness the knowledge of millions of other cybersecurity professionals, including cybersecurity product vendors, government agencies, cloud providers, and more. Crowdsourcing allows people and organizations from the global cybersecurity community to openly share and access a collection of threat intelligence data, which helps to continuously improve detection technologies and methodologies.

Examples of information-sharing organizations include Information Sharing and Analysis Centers (ISACs), which focus on collecting and sharing sector-specific threat intelligence to companies within specific industries like energy, healthcare, and others. **Open-source intelligence (OSINT)** is the collection and analysis of information from publicly available sources to generate usable intelligence. OSINT can also be used as a method to gather information related to threat actors, threats, vulnerabilities, and more.

This threat intelligence data is used to improve the detection methods and techniques of security products, like detection tools or anti-virus software. For example, attackers often perform the same attacks on multiple targets with the hope that one of them will be successful. Once an organization detects an attack, they can immediately publish the attack details, such as malicious files, IP addresses, or URLs, to tools like VirusTotal. This threat intelligence can then help other organizations defend against the same attack.


### VirusTotal

[**VirusTotal**](https://www.virustotal.com/gui/home) is a service that allows anyone to analyse suspicious files, domains, URLs, and IP addresses for malicious content. VirusTotal also offers additional services and tools for enterprise use. This reading focuses on the VirusTotal website, which is available for free and non-commercial use.

It can be used to analyse suspicious files, IP addresses, domains, and URLs to detect cybersecurity threats such as malware. Users can submit and check artifacts, like file hashes or IP addresses, to get VirusTotal reports, which provide additional information on whether an IoC is considered malicious or not, how that IoC is connected or related to other IoCs in the dataset, and more.


1. **Detection**: The Detection tab provides a list of third-party security vendors and their detection verdicts on an IoC. For example, vendors can list their detection verdict as malicious, suspicious, unsafe, and more.
    
2. **Details**: The Details tab provides additional information extracted from a static analysis of the IoC. Information such as different hashes, file types, file sizes, headers, creation time, and first and last submission information can all be found in this tab.
    
3. **Relations**: The Relations tab provides related IoCs that are somehow connected to an artifact, such as contacted URLs, domains, IP addresses, and dropped files if the artifact is an executable.
    
4. **Behavior**: The Behavior tab contains information related to the observed activity and behaviors of an artifact after executing it in a controlled or sandboxed environment. This information includes tactics and techniques detected, network communications, registry and file systems actions, processes, and more.
    
5. **Community**: The Community tab is where members of the VirusTotal community, such as security professionals or researchers, can leave comments and insights about the IoC.
    
6. **Vendors’ ratio and community score**: The score displayed at the top of the report is the vendors’ ratio. The vendors’ ratio shows how many security vendors have flagged the IoC as malicious overall. Below this score, there is also the community score, based on the inputs of the VirusTotal community. The more detections a file has and the higher its community score is, the more likely that the file is malicious.
    

**Note**: Data uploaded to VirusTotal will be publicly shared with the entire VirusTotal community. Be careful of what you submit, and make sure you do not upload personal information.

### Other Tools

There are other investigative tools that can be used to analyse IoCs. These tools can also share the data that's uploaded to them with the security community.

#### **Jotti Malware Scan**

[Jotti's malware scan](https://virusscan.jotti.org/) is a free service that lets you scan suspicious files with several antivirus programs. There are some limitations to the number of files that you can submit.

#### **[Urlscan.io](http://urlscan.io/)**

[Urlscan.io](https://urlscan.io/) is a free service that scans and analyses URLs and provides a detailed report summarizing the URL information.

#### **MalwareBazaar**

[MalwareBazaar](https://bazaar.abuse.ch/browse/) is a free repository for malware samples. Malware samples are a great source of threat intelligence that can be used for research purposes.

### Key Takeaways

As a security analyst, you'll analyse IoCs. It's important to understand how adding context to investigations can help improve detection capabilities and make informed and effective decisions.


----

# Create and use documentation

## Document Evidence with Chain of Custody Forms

During incident response, it is crucial to document evidence possession and control throughout the entire incident lifecycle. This ensures transparency and accountability, particularly if the evidence is requested for legal proceedings. This process is managed through the use of chain of custody forms.

### Chain of Custody

**Chain of custody** is the process of documenting the possession and control of evidence during an incident's lifecycle. It ensures that evidence is tracked from the moment it is collected until it is presented in court, if necessary. Chain of custody forms are used to log every instance of evidence handling, providing a detailed record of who handled the evidence, and when, why, and where it was handled.

### Example of Chain of Custody in Digital Forensics

Consider a scenario in digital forensic analysis:

1. **Evidence Collection**: Aisha verifies that a compromised hard drive needs to be examined by the forensics team.
2. **Write Protection**: Aisha ensures the hard drive is write-protected to prevent data alteration or erasure.
3. **Hash Calculation**: She calculates and records a cryptographic hash of the hard drive image. This hash acts as a unique identifier to detect tampering.
4. **Evidence Transfer**: Aisha transfers the hard drive to Colin in the forensics department, who then sends it to Nav, another analyst.
5. **Chain of Custody Form**: Each transfer is logged in the chain of custody form, recording the handler's name, date and time of transfer, and the purpose of the transfer.
6. **Verification**: Any tampering with the hard drive can be detected by comparing the original hash calculated by Aisha.

### Elements of a Chain of Custody Form

A chain of custody form typically includes:

- **Evidence Description**: Detailed information identifying the evidence, such as location, hostname, MAC address, or IP address.
- **Custody Log**: Records the names of individuals who transferred and received the evidence, along with the date, time, and purpose of each transfer.

### Importance of Chain of Custody

The chain of custody is vital for establishing the integrity, reliability, and accuracy of evidence in legal proceedings. It ensures:

- **Transparency**: Provides a clear record of evidence handling.
- **Accountability**: Tracks who handled the evidence and when.
- **Integrity**: Helps to detect tampering through recorded hashes and logs.

### Consequences of a Broken Chain of Custody

A broken chain of custody occurs when there are inconsistencies or missing entries in the evidence log. This can undermine the trustworthiness of the evidence, potentially making it inadmissible in court. Therefore, maintaining an unbroken chain of custody is essential for the evidence to be considered reliable and accurate.

### Key Takeaways

Chain of custody forms are critical for maintaining the integrity of evidence throughout the incident lifecycle. They ensure that evidence can be trusted in legal proceedings and that malicious actors can be held accountable for their actions. Proper documentation and handling of evidence using chain of custody forms are fundamental to the incident response process.

## Best Practices for Effective Documentation

Documentation is any form of recorded content used for a specific purpose, and it is essential in the field of security. Security teams use documentation to support investigations, complete tasks, and communicate findings. This reading explores the benefits of documentation and provides common practices to help you create effective documentation in your security career.

### Documentation Benefits

You’ve already learned about many types of security documentation, including playbooks, final reports, and more. Effective documentation has three primary benefits:

1. **Transparency**
2. **Standardization**
3. **Clarity**

#### Transparency

In security, transparency is critical for demonstrating compliance with regulations and internal processes, meeting insurance requirements, and for legal proceedings. Chain of custody is the process of documenting evidence possession and control during an incident lifecycle. Chain of custody is an example of how documentation produces transparency and an audit trail.

#### Standardization

Standardization through repeatable processes and procedures supports continuous improvement efforts, helps with knowledge transfer, and facilitates the onboarding of new team members. Standards are references that inform how to set policies.

For example, NIST provides various security frameworks that are used to improve security measures. Likewise, organizations set up their own standards to meet their business needs. An incident response plan is a document that outlines the procedures to take in each step of incident response. Incident response plans standardize an organization’s response process by outlining procedures in advance of an incident. By documenting an organization’s incident response plan, you create a standard that people follow, maintaining consistency with repeatable processes and procedures.

#### Clarity

Ideally, all documentation provides clarity to its audience. Clear documentation helps people quickly access the information they need so they can take necessary action. Security analysts are required to document the reasoning behind any action they take so that it’s clear to their team why an alert was escalated or closed.

### Best Practices

As a security professional, you’ll need to apply documentation best practices in your career. Here are some general guidelines to remember:

#### Know Your Audience

Before you start creating documentation, consider your audience and their needs. For instance, an incident summary written for a security operations center (SOC) manager will be written differently than one that's drafted for a chief executive officer (CEO). The SOC manager can understand technical security language but a CEO might not. Tailor your document to meet your audience’s needs.

#### Be Concise

You might be tasked with creating long documentation, such as a report. But when documentation is too long, people can be discouraged from using it. To ensure that your documentation is useful, establish the purpose immediately. This helps people quickly identify the objective of the document. For example, executive summaries outline the major facts of an incident at the beginning of a final report. This summary should be brief so that it can be easily skimmed to identify the key findings.

#### Update Regularly

In security, new vulnerabilities are discovered and exploited constantly. Documentation must be regularly reviewed and updated to keep up with the evolving threat landscape. For example, after an incident has been resolved, a comprehensive review of the incident can identify gaps in processes and procedures that require changes and updates. By regularly updating documentation, security teams stay well informed and incident response plans stay updated.

### Key Takeaways

Effective documentation produces benefits for everyone in an organization. Knowing how to create documentation is an essential skill to have as a security analyst. As you continue in your journey to become a security professional, be sure to consider these practices for creating effective documentation.

## The Value of Cybersecurity Playbooks

### Introduction

Have you ever taken a trip to a place you've never visited before? You may have used a travel itinerary to plan your trip activities. Travel itineraries are essential documents to have, especially for travel to a new place. They help keep you organized and give you a clear picture of your travel plans. They detail the activities you'll do, the places you'll visit, and your travel time between destinations.

Playbooks are similar to travel itineraries. As you may remember from our previous discussions, a playbook is a manual that provides details about any operational action. They provide security analysts with instructions on exactly what to do when an incident occurs.

### Purpose of Playbooks

Playbooks provide security professionals with a clear picture of their tasks during the entire incident response lifecycle. Responding to an incident can be unpredictable and chaotic at times. Security teams are expected to act quickly and effectively. Playbooks offer structure and order during this time by clearly outlining the actions to take when responding to a specific incident. By following a playbook, security teams can reduce any guesswork and uncertainty during response times. This allows security teams to act quickly and without any hesitation. Without playbooks, an effective and swift response to an incident is nearly impossible.

### Components of Playbooks

Within playbooks, there may be checklists that can also help security teams perform effectively during stressful times by helping them remember to complete each step in the incident response lifecycle.

Playbooks outline the steps that are necessary in response to an attack like ransomware, data breach, malware, or DDoS. Here's an example of a playbook that uses a flowchart diagram with the steps to take during the detection of a DDoS attack. This depicts the process for detecting a DDoS and begins with determining the indicators of compromise, like unknown incoming traffic. Once the indicators of compromise are determined, the next step is to collect the logs and finally analyse the evidence.

### Types of Playbooks

There are three different types of playbooks: non-automated, automated, and semi-automated.

#### Non-automated Playbooks

- **Description**: Require step-by-step actions performed by an analyst.
- **Example**: The DDoS playbook we just explored is an example of a non-automated playbook.

#### Automated Playbooks

- **Description**: Automate tasks in incident response processes.
- **Benefits**: Can help lower the time to resolution during an incident.
- **Tools**: SOAR and SIEM tools can be configured to automate playbooks.
- **Example Tasks**: Categorizing the severity of the incident, gathering evidence.

#### Semi-automated Playbooks

- **Description**: Combine a person's action with automation.
- **Benefits**: Tedious, error-prone, or time-consuming tasks can be automated, allowing analysts to prioritize their time with other tasks.
- **Outcome**: Can help increase productivity and decrease time to resolution.

### Maintenance of Playbooks

As a security team responds to incidents, they may discover that a playbook needs updates or changes. Threats are constantly evolving and for playbooks to be effective, they must be maintained and updated regularly.

### Key Takeaways

- **Purpose**: Playbooks provide structured and ordered actions for security teams during incidents, reducing guesswork and enabling quick, effective responses.
- **Components**: Include steps, checklists, and detailed processes for handling specific incidents.
- **Types**: Non-automated, automated, and semi-automated playbooks, each with distinct advantages and use cases.
- **Maintenance**: Regular updates are essential to keep playbooks effective and relevant to evolving threats.


---

# Response and recovery

## The Role of Triage in Incident Response

### Introduction

Security analysts often deal with a large number of alerts daily. Managing these alerts efficiently is crucial for effective incident response. This process is known as triage, similar to how hospital emergency departments handle patients based on the urgency of their conditions.

### What is Triage?

In medicine, triage categorizes patients based on the urgency of their conditions. Patients with life-threatening conditions receive immediate care, while those with less severe conditions may wait. This helps manage limited resources effectively, ensuring that those in critical need get prompt attention.

### Triage in Security

In security, triage prioritizes incidents based on their level of importance or urgency. Security teams, like hospitals, have limited resources. Not all incidents are the same, and some require urgent responses. Incidents are triaged according to the threat they pose to the confidentiality, integrity, and availability of systems.

- **High Priority Example**: An incident involving ransomware, which can cause financial, reputational, and operational damage, requires immediate response.
- **Lower Priority Example**: An incident involving an employee receiving a phishing email, which might not be immediately urgent.

### When Does Triage Happen?

Triage begins once an incident is detected and an alert is sent out. Security analysts then identify the different types of alerts and prioritize them according to urgency.

### Triage Process

The triage process generally involves the following steps:

1. **Receive and Assess the Alert**: Determine if it's a false positive and whether it's related to an existing incident.
2. **Assign Priority**: Based on the organization's policy and guidelines, assign a priority level to the alert. This priority defines how the security team will respond to the incident.
3. **Investigate the Alert**: Collect and analyse any evidence associated with the alert, such as system logs.

### Adding Context to Alerts

As a security analyst, thorough analysis is crucial for making informed decisions about alerts. This involves adding context to the investigation by asking relevant questions:

- Is there anything out of the ordinary associated with this alert?
- Are there multiple failed login attempts?
- Did the login happen outside of normal working hours?
- Did the login happen outside of the network?

These questions help paint a complete picture of the incident, avoiding assumptions that can lead to incomplete or incorrect conclusions.

### Key Takeaways

- **Purpose of Triage**: Manage limited resources efficiently by prioritizing incidents based on urgency.
- **Triage Process**: Assess alerts, assign priority, and investigate thoroughly.
- **Adding Context**: Ask relevant questions to understand the full scope of an incident.


## The Triage Process

### Introduction

Triage is an essential process used by security analysts to assess alerts and assign priority to incidents. This process helps manage the large volume of alerts that analysts deal with daily, ensuring that critical incidents are addressed promptly and efficiently.

### Importance of Triage

Incidents can potentially cause significant damage to an organization. Quick and efficient response is necessary to prevent or limit the impact of an incident. Triage prioritizes incidents according to their level of importance or urgency, helping security teams evaluate and allocate resources effectively.

### Steps in the Triage Process

The triage process consists of three main steps:

1. **Receive and Assess**
2. **Assign Priority**
3. **Collect and analyse**

#### Step 1: Receive and Assess

- **Alert Reception**: A security analyst receives an alert from an alerting system, such as an intrusion detection system (IDS).
- **Verify Validity**: The analyst reviews the alert to verify its validity and gather as much information as possible.
- **Questions to Consider**:
    - Is the alert a false positive?
    - Has this alert been triggered in the past? How was it resolved?
    - Is the alert triggered by a known vulnerability?
    - What is the severity of the alert?

#### Step 2: Assign Priority

- **Assessment**: Once verified as a genuine security issue, the alert needs to be prioritized.
- **Factors to Consider**:
    - **Functional Impact**: How does the incident impact the service provided by the affected system?
    - **Information Impact**: What are the effects on the confidentiality, integrity, and availability of data?
    - **Recoverability**: Is recovery possible, and is it worth the time and cost?

#### Step 3: Collect and analyse

- **Comprehensive Analysis**: The analyst performs a detailed analysis of the incident.
- **Evidence Gathering**: Collect evidence from various sources and conduct external research.
- **Documentation**: Document the investigative process.
- **Escalation**: Depending on severity, escalate to a level two analyst or a manager for further investigation.

### Benefits of Triage

- **Resource Management**: Allows security teams to focus resources on urgent threats, reducing response time.
- **Standardized Approach**: Provides a standardized method for incident handling, ensuring that only valid alerts are escalated.

### Key Takeaways

- **Prioritization**: Triage helps prioritize incidents based on their potential impact.
- **Efficiency**: Ensures timely response to critical incidents, reducing the scope of impact.
- **Resource Allocation**: Helps manage resources effectively, avoiding time spent on lower priority tasks.
- **Documentation**: A standardized approach through documentation ensures consistency in handling incidents.

## The Containment, Eradication, and Recovery Phase of the Lifecycle

In this phase, security teams focus on containing the incident, eradicating it, and recovering affected systems. These steps are interconnected, with containment facilitating eradication, which in turn aids recovery. This phase aligns with the NIST Cybersecurity Framework's core functions: Respond and Recover.

### Containment

**Containment** is the process of limiting and preventing additional damage caused by an incident. Organizations outline their containment strategies in their incident response plans. Different incidents require different containment strategies.

- **Example**: For a malware incident on a single computer, a common containment strategy is to isolate the affected system by disconnecting it from the network. This prevents the malware from spreading to other systems.

**Goals of Containment**:

1. Limit the scope of the incident.
2. Prevent further damage.
3. Maintain integrity of unaffected systems.

### Eradication

Once an incident is contained, the next step is **eradication**. Eradication involves completely removing all traces of the incident from affected systems.

- **Example**: Performing vulnerability tests and applying patches to address vulnerabilities exploited by the threat.

**Eradication Actions**:

1. Remove malware or unauthorized access.
2. Clean affected systems.
3. Validate that the threat is no longer present.

### Recovery

The final step in this phase is **recovery**, which is the process of returning affected systems to normal operations. An incident can disrupt key business functions and services. During recovery, impacted services are restored to normal operation.

**Recovery Actions**:

1. Reimage affected systems to ensure they are clean.
2. Reset passwords to prevent unauthorized access.
3. Adjust network configurations, such as firewall rules, to prevent future incidents.

**Goals of Recovery**:

1. Restore normal business operations.
2. Ensure affected systems are secure.
3. Prevent recurrence of the incident.

### Key Points

- **Containment** helps to limit the incident's damage.
- **Eradication** removes the threat from all affected systems.
- **Recovery** restores systems to normal operations and prevents future incidents.
- The incident response lifecycle is cyclical; security teams may revisit previous phases to conduct further investigations as new incidents occur.

## Business Continuity Considerations

Security teams develop incident response plans to ensure a prepared and consistent process for quickly responding to security incidents. Additionally, business continuity planning plays a crucial role in recovering from incidents and maintaining operations.

### Business Continuity Planning

**Business continuity planning (BCP)** involves preparing for the potential impacts that security incidents can have on normal business operations. Significant disruptions can cause legal, financial, and reputational damages. A BCP ensures that critical business functions can continue or be quickly restored during and after a major disruption.

- **Incident Response Plan**: Focuses on the immediate actions to manage and mitigate a security incident.
- **Business Continuity Plan**: Ensures the organization can sustain operations during and after disruptions.

### Key Components of a Business Continuity Plan

1. **Risk Assessment**: Identifying potential risks and their impacts on business operations.
2. **Business Impact Analysis**: Determining the critical functions and processes essential to the organization's operations.
3. **Recovery Strategies**: Developing strategies to restore business operations quickly.
4. **Plan Development**: Documenting the procedures and resources needed for continuity.
5. **Testing and Exercises**: Regularly testing the plan to ensure its effectiveness.

### Differences Between BCP and Disaster Recovery Plan

- **Business Continuity Plan (BCP)**: Focuses on maintaining business operations during and after disruptions.
- **Disaster Recovery Plan (DRP)**: Focuses on recovering information systems and data after a major disaster, such as hardware failures or natural disasters.

### Consider the Impacts of Ransomware on Business Continuity

**Ransomware attacks** can significantly disrupt business operations, especially in critical infrastructure sectors like healthcare. These attacks can encrypt data, disabling access to essential medical records and preventing healthcare providers from delivering services.

- **Potential Impacts**:
    - Accessibility: Inability to access critical data.
    - Availability: Disruption of essential services.
    - Delivery: Delays in service provision.

BCPs help to minimize interruptions to operations, ensuring essential services remain accessible and functional.

### Recovery Strategies

When an outage occurs due to a security incident, organizations must have a recovery plan to resolve the issue and restore full operations. BCPs include various recovery strategies.

#### Site Resilience

**Resilience** is the ability to prepare for, respond to, and recover from disruptions. Site resilience ensures the availability of networks, data centers, or other infrastructure.

- **Types of Recovery Sites**:
    - **Hot Sites**: Fully operational facilities that duplicate the primary environment, ready for immediate activation.
    - **Warm Sites**: Partially operational facilities that can quickly become fully functional.
    - **Cold Sites**: Backup facilities with basic infrastructure, requiring additional setup to become operational.

### Key Takeaways

- **Security Incidents**: Can cause significant disruptions to business operations.
- **Business Continuity Plans**: Essential for ensuring organizations can continue to function during and after incidents.
- **Site Resilience**: Key strategy for maintaining operational continuity.
- **Recovery Strategies**: Vital for returning to normal operations efficiently.

## The Post-Incident Activity Phase of the Lifecycle

### Overview

After a security team has successfully contained, eradicated, and recovered from an incident, the work isn't completely done. The post-incident activity phase is essential for learning and improvement. This phase focuses on reviewing the incident to identify areas for improvement in incident handling.

### Key Activities

#### 1. Reviewing the Incident

The post-incident activity phase involves thoroughly reviewing the incident to understand what happened, how it was handled, and how the response process can be improved. This review is critical for continuous improvement and preparedness for future incidents.

#### 2. Creating and Updating Documentation

During this phase, various types of documentation are updated or created to ensure all information about the incident is accurately recorded. This documentation serves as a reference for future incidents and helps in training and preparation.

##### Final Report

One of the most important documents created during this phase is the final report. This comprehensive review includes:

- A timeline of events related to the incident.
- Details of all actions taken during the incident.
- Recommendations for preventing similar incidents in the future.

#### 3. Lessons Learned Meeting

A lessons learned meeting is held to discuss the incident in detail. This meeting typically includes all parties involved in the incident and is held within two weeks after the incident.

##### Objectives of the Lessons Learned Meeting

- **Review the Incident:** Understand what happened, the timeline, and the actions taken.
- **Evaluate Effectiveness:** Determine how well the response actions worked and identify any gaps.
- **Share Insights:** Share ideas and information about the incident to improve future response efforts.

##### Questions to Ask During the Lessons Learned Meeting

- What happened?
- What time did it happen?
- Who discovered it?
- How did it get contained?
- What were the actions taken for recovery?
- What could have been done differently?

### Importance of Avoiding Blame

Incident reviews can reveal human errors that occurred before detection and during the response. It's important to avoid blaming individuals for their actions or mistakes. Instead, the focus should be on learning from these errors to improve future incident response.

### Key Takeaways

- **Continuous Improvement:** The post-incident activity phase is crucial for learning and improving incident response processes.
- **Comprehensive Documentation:** Creating detailed documentation, including a final report, is essential for accurate record-keeping and future reference.
- **Collaborative Learning:** Holding a lessons learned meeting helps share insights and improve response strategies.
- **Constructive Feedback:** Avoiding blame and focusing on learning from mistakes fosters a positive and productive environment for continuous improvement.

## Post-Incident Review

### The Post-Incident Activity Phase

The Post-Incident Activity phase of the NIST Incident Response Lifecycle involves reviewing an incident to identify areas for improvement during incident handling. This phase is crucial for learning and improving responses to future incidents.

### Lessons Learned

After containing, eradicating, and recovering from an incident, the work isn't complete. Incidents provide an opportunity for organizations and security teams to learn and improve their incident handling processes. This is typically done through a lessons learned meeting, also known as a post-mortem.

#### Lessons Learned Meeting

- **Purpose**: Evaluate the incident, assess response actions, and identify areas for improvement.
- **Timing**: Held within two weeks after an incident has been successfully remediated.
- **Participants**: All involved parties.
- **Questions Addressed**:
    - What happened?
    - What time did it happen?
    - Who discovered it?
    - How did it get contained?
    - What were the actions taken for recovery?
    - What could have been done differently?

#### Additional Benefits

- **Information Sharing**: Provides a platform for team members across departments to share information and recommendations.
- **Preparation**: Attendees should come prepared with a meeting agenda, and roles such as a moderator and scribe should be assigned in advance.

### Recommendations

Lessons learned meetings should result in actionable recommendations to improve an organization’s incident handling processes and overall security posture. Examples include:

- Updating and improving playbook instructions.
- Implementing new security tools and technologies.

### Final Report

The final report is a comprehensive review of the incident, capturing details necessary for developing additional documents at the end of the lifecycle. The format can vary across organizations and can be tailored to different audiences.

#### Common Elements in a Final Report

- **Executive Summary**: High-level summary including key findings and essential facts.
- **Timeline**: Detailed chronological timeline of the incident with timestamps.
- **Investigation**: Compilation of actions taken during detection and analysis, such as network artifact analysis.
- **Recommendations**: List of suggested actions for future prevention.

### Writing the Final Report

When writing the final report, consider the audience. Business executives and other non-security professionals may read the report, so it's important to communicate the most important details effectively.

### Key Takeaways

- **Learning and Improvement**: Post-incident actions provide an opportunity to evaluate response actions and improve future responses.
- **Documentation**: Essential for capturing details and developing the final report.
- **Collaboration**: Lessons learned meetings facilitate information sharing and collaborative improvement.
- **Actionable Recommendations**: Ensure organizations implement the lessons learned to avoid future incidents.

---
# Glossary terms from module 3


**Analysis:** The investigation and validation of alerts 

**Broken chain of custody:** Inconsistencies in the collection and logging of evidence in the chain of custody

**Business continuity plan (BCP):** A document that outlines the procedures to sustain business operations during and after a significant disruption

**Chain of custody:** The process of documenting evidence possession and control during an incident lifecycle

**Containment:** The act of limiting and preventing additional damage caused by an incident

**Crowdsourcing:** The practice of gathering information using public input and collaboration

**Detection:** The prompt discovery of security events

**Documentation**: Any form of recorded content that is used for a specific purpose

**Eradication:** The complete removal of the incident elements from all affected systems

**Final report:** Documentation that provides a comprehensive review of an incident

**Honeypot:** A system or resource created as a decoy vulnerable to attacks with the purpose of attracting potential intruders

**Incident response plan:** A document that outlines the procedures to take in each step of incident response

**Indicators of attack (IoA):** The series of observed events that indicate a real-time incident

**Indicators of compromise (IoC):** Observable evidence that suggests signs of a potential security incident

**Intrusion detection system (IDS):** An application that monitors system activity and alerts on possible intrusions

**Lessons learned meeting:** A meeting that includes all involved parties after a major incident

**Open-source intelligence (OSINT):** The collection and analysis of information from publicly available sources to generate usable intelligence

**Playbook:** A manual that provides details about any operational action

**Post-incident activity:** The process of reviewing an incident to identify areas for improvement during incident handling

**Recovery:** The process of returning affected systems back to normal operations

**Resilience**: The ability to prepare for, respond to, and recover from disruptions

**Standards:** References that inform how to set policies

**Threat hunting:** The proactive search for threats on a network

**Threat intelligence:** Evidence-based threat information that provides context about existing or emerging threats

**Triage**: The prioritizing of incidents according to their level of importance or urgency

**VirusTotal:** A service that allows anyone to analyse suspicious files, domains, URLs, and IP addresses for malicious content