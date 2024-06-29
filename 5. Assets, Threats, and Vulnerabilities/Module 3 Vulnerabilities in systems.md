# Flaws in the system

## Vulnerability Management

Vulnerability management is a crucial part of protecting assets from potential threats. This process involves identifying, assessing, and addressing weaknesses that could be exploited by threats. By continuously managing vulnerabilities, organizations can prevent potential security incidents and protect their valuable assets.

### Understanding Vulnerabilities

A **vulnerability** is a weakness that can be exploited by a threat. The word "can" is important because it highlights the potential for exploitation, rather than a guaranteed occurrence. Identifying vulnerabilities is the first step in protecting assets.

#### Example Scenario
Imagine you have an important document that you need to keep safe. You might:
- Lock it in a secure place, considering that documents can be easily moved and are vulnerable to theft.
- Protect it from fire and water damage, since paper is easily damaged by these elements.

### The Concept of Exploits

An **exploit** is a method used to take advantage of a vulnerability. Security teams focus on identifying vulnerabilities and potential exploits to plan effective defenses.

#### Example Scenario
Consider the vulnerability of glass windows in a home. Burglars can exploit this vulnerability by breaking the glass with a rock. By anticipating this exploit, you can plan defenses, such as installing an alarm system to deter the burglar and alert the police.

### The Vulnerability Management Process

Vulnerability management is a continuous cycle that involves four key steps:

1. **Identify Vulnerabilities**: Discover potential weaknesses in systems and processes.
2. **Assess Potential Exploits**: Evaluate how these vulnerabilities can be exploited.
3. **Prepare Defenses**: Implement measures to protect against potential threats.
4. **Evaluate Defenses**: Assess the effectiveness of the defenses and make necessary adjustments.

Once the cycle is complete, it starts over to ensure ongoing protection as new vulnerabilities and exploits emerge.

### The Importance of Diverse Perspectives

A diverse set of perspectives is invaluable in vulnerability management. Different backgrounds and experiences help security teams identify a broader range of potential exploits. However, even the most diverse and large teams can't anticipate every possible vulnerability.

### Zero-Day Exploits

A **zero-day exploit** is a previously unknown vulnerability that is exploited before it can be addressed. The term "zero-day" refers to the fact that there are zero days to fix the vulnerability before it is exploited.

#### Example Scenario
Consider a burglar breaking into a home. You can anticipate this threat and install locks. However, a zero-day exploit might be something unexpected, like the lock falling off due to intense heat. Similarly, a new form of spyware infecting a popular website represents a zero-day exploit, making assets more vulnerable to threats.

### Key Takeaways

- **Vulnerability Management**: A continuous process of identifying and addressing vulnerabilities to protect assets.
- **Vulnerabilities and Exploits**: Recognizing potential weaknesses and how they can be exploited is crucial for effective security planning.
- **Diverse Perspectives**: A broad range of experiences strengthens the ability to identify potential exploits.
- **Zero-Day Exploits**: Unanticipated vulnerabilities that are exploited before they can be addressed are particularly dangerous.

## Defense in Depth Strategy

### Introduction

Defense in depth is a security model that employs a layered approach to vulnerability management, reducing risk by using multiple layers of defense. Often referred to as the castle approach, this strategy is designed to protect assets by implementing various security controls at different layers, ensuring that if one barrier fails, another is in place to stop the attack.

### Concept and Historical Analogy

The defense in depth model is akin to the layered defenses of a medieval castle. In the Middle Ages, castles were built with multiple layers of defense, each posing unique challenges to attackers. For example:
- **Moat**: A water-filled barrier preventing large groups of attackers from reaching the castle walls.
- **Stone Walls**: Tall and difficult to climb, providing a robust physical barrier.
- **Watch Towers**: Filled with defenders ready to repel attackers with arrows, further complicating any attempt to breach the walls.

Similarly, defense in depth in cybersecurity employs multiple layers of defense to minimize the risk of attacks by addressing vulnerabilities with various security controls.

### Layers of Defense in Depth

The defense in depth strategy in cybersecurity consists of five layers, each featuring specific security controls to protect information as it travels in and out of the system.

#### 1. Perimeter Layer
- **Function**: User authentication layer that filters external access.
- **Technologies**: Usernames, passwords, and other authentication mechanisms.
- **Purpose**: Ensures only trusted partners can proceed to the next layer of defense.

#### 2. Network Layer
- **Function**: Focuses on authorization and network security.
- **Technologies**: Network firewalls, intrusion detection systems (IDS), and virtual private networks (VPNs).
- **Purpose**: Controls access to the network and monitors traffic for suspicious activities.

#### 3. Endpoint Layer
- **Function**: Protects devices connected to the network.
- **Technologies**: Anti-virus software, endpoint detection and response (EDR), and device management solutions.
- **Purpose**: Secures laptops, desktops, servers, and other endpoints against malware and unauthorized access.

#### 4. Application Layer
- **Function**: Secures the interfaces used to interact with technology.
- **Technologies**: Multi-factor authentication (MFA), application firewalls, and secure coding practices.
- **Purpose**: Ensures that applications are protected from threats and that user interactions are secure.

#### 5. Data Layer
- **Function**: Protects critical data, such as personally identifiable information (PII).
- **Technologies**: Data encryption, asset classification, and data loss prevention (DLP) solutions.
- **Purpose**: Safeguards sensitive data from unauthorized access and breaches.

### Flow of Information Through Layers

Information passes in and out of each of these five layers whenever it is exchanged over a network. Each layer has specific security controls designed to address potential vulnerabilities and threats, ensuring comprehensive protection of the organization's assets.

### Key Takeaways

- **Multi-layered Defense**: Defense in depth employs multiple layers of security to protect assets, ensuring that if one layer fails, others are in place to mitigate the risk.
- **Variety of Controls**: Each layer features different security controls tailored to address specific vulnerabilities and threats.
- **Comprehensive Protection**: By implementing a defense in depth strategy, organizations can create a robust security framework that protects information at various levels.

## Common Vulnerabilities and Exposures

### Introduction

Security is a global effort that extends well beyond a single security team. Protecting information involves sharing and documenting common vulnerabilities and exposures. Understanding these vulnerabilities and exposures is crucial for maintaining security.

### Vulnerabilities vs. Exposures

- **Vulnerability**: A weakness in a system that can be exploited by a threat.
- **Exposure**: A mistake that can be exploited by a threat.

#### Example
Imagine you're asked to protect an important document. 
- **Vulnerability**: The document is susceptible to being misplaced.
- **Exposure**: If you lay the document near an open window, it could be blown away.

### Common Vulnerabilities and Exposures (CVE) List

One of the most popular libraries of vulnerabilities and exposures is the CVE list. This list is an openly accessible dictionary of known vulnerabilities and exposures, created by MITRE corporation in 1999. 

#### Purpose
The main purpose of the CVE list is to offer a standard way of identifying and categorizing known vulnerabilities and exposures.

#### Contributors
Most CVEs in the list are reported by:
- Independent researchers
- Technology vendors
- Ethical hackers

Anyone can report a CVE. Each report goes through a strict review process by a CVE Numbering Authority (CNA).

### CVE Numbering Authority (CNA)

A CNA is an organization that volunteers to analyse and distribute information on eligible CVEs. They have a record of researching vulnerabilities and demonstrating security advisory capabilities. The CNA conducts a rigorous testing process before assigning a CVE ID.

#### Four Criteria for CVE Inclusion
1. **Independence**: The vulnerability must be independent of other issues.
2. **Recognition**: The vulnerability must be recognized as a potential security risk.
3. **Evidence**: The vulnerability must be submitted with supporting evidence.
4. **Codebase**: The vulnerability must affect only one codebase.

### National Vulnerabilities Database (NVD) and CVSS

Vulnerabilities added to the CVE list are often reviewed by other databases like the NIST National Vulnerabilities Database (NVD).

#### Common Vulnerability Scoring System (CVSS)
The CVSS is a measurement system that scores the severity of a vulnerability. It helps security teams calculate the impact a vulnerability could have on a system and prioritize security fixes.

#### CVSS Base Scores
- **Scale**: 0-10
- **Low Risk**: Scores below 4.0
- **Critical Risk**: Scores above 9.0

### Vulnerability Management Strategy

Security teams use the CVE list and CVSS scores as part of their vulnerability management strategy to determine:
- Is a vulnerability dangerous to the business?
- How soon should it be addressed?

#### Four-Step Vulnerability Management Process
1. **Identify Vulnerabilities**: Finding vulnerabilities in the system.
2. **Consider Exploits**: Understanding how vulnerabilities can be exploited.
3. **Prepare Defenses**: Implementing security controls to protect against exploits.
4. **Evaluate Defenses**: Regularly assessing the effectiveness of security controls.

### Zero-Day Exploits

Zero-day exploits are vulnerabilities that were previously unknown and are exploited in real-time with no days to fix them. These exploits are particularly dangerous because they represent unanticipated threats.

### Key Takeaways

- **CVE List**: A crucial resource for identifying and categorizing known vulnerabilities and exposures.
- **CVSS Scores**: Provide a standardized way to assess and prioritize vulnerabilities.
- **Vulnerability Management**: A continuous process of identifying, understanding, and mitigating vulnerabilities.
- **Global Effort**: Protecting information requires collaboration and diverse perspectives from around the world.

## The OWASP Top 10

### Introduction

To prepare for future risks, security professionals need to stay informed. One essential resource is the Open Web Application Security Project (OWASP). This nonprofit foundation aims to improve the security of software and provides valuable resources for security professionals.

### What is OWASP?

OWASP is a nonprofit foundation that works to improve the security of software. It serves as an open platform for security professionals worldwide to share information, tools, and events focused on securing web applications.

### The OWASP Top 10

One of OWASP’s most valuable resources is the OWASP Top 10. Since 2003, this list has highlighted the web’s most targeted vulnerabilities. It is primarily applicable to new or custom-made software and helps organizations address common security mistakes during application development.

#### Key Points
- The OWASP Top 10 is updated every few years as technologies evolve.
- Rankings are based on the frequency of discovered vulnerabilities and the level of risk they present.
- Auditors use the OWASP Top 10 as a reference for regulatory compliance checks.

### Common Vulnerabilities

Businesses often base critical security decisions on the OWASP Top 10, which influences how they design new software. Here are the most regularly listed vulnerabilities:

#### 1. Broken Access Control

Access controls limit user actions in a web application. Failures in these mechanisms can lead to unauthorized information disclosure, modification, or destruction, and can grant unauthorized access to other business applications.

#### 2. Cryptographic Failures

Vulnerabilities occur when sensitive data is not properly encrypted. Weak encryption methods, like MD5, increase the risk of data breaches.

#### 3. Injection

Injection attacks occur when malicious code is inserted into a vulnerable application, often via login forms. This can provide threat actors with unauthorized access to modify or steal user credentials.

#### 4. Insecure Design

Insecure design refers to missing or poorly implemented security controls that should have been included during application development, making the application more vulnerable to attacks.

#### 5. Security Misconfiguration

Misconfigurations happen when security settings are not properly set or maintained. Default settings on network servers, for example, can fail to meet an organization’s security objectives.

#### 6. Vulnerable and Outdated Components

Applications using outdated or vulnerable open-source libraries are at greater risk of exploitation. These components are often maintained by volunteer communities and can lag in updates and security patches.

#### 7. Identification and Authentication Failures

Failures in identification and authentication can lead to unauthorized access. For example, if a home Wi-Fi router’s login form fails, an attacker can invade the homeowner’s privacy.

#### 8. Software and Data Integrity Failures

These failures occur when updates or patches are inadequately reviewed before implementation. Such weaknesses can be exploited to deliver malicious software, potentially leading to supply chain attacks.

#### 9. Security Logging and Monitoring Failures

Effective logging and monitoring are crucial for tracing back events and responding to incidents. Insufficient logging and monitoring can delay the detection and response to security breaches.

#### 10. Server-Side Request Forgery (SSRF)

SSRFs occur when attackers manipulate server operations to access unauthorized data. Vulnerable applications on the server can carry malicious code to the host server, leading to unauthorized data access.

### Key Takeaways

Staying informed about the latest cybersecurity trends and vulnerabilities is crucial for defending against attacks and preparing for future risks. The OWASP Top 10 is a valuable resource for understanding and mitigating common vulnerabilities in web applications.

### Resources

- [OWASP’s Top 10](https://owasp.org/www-project-top-ten/)

## Open Source Intelligence

Cyber attacks can sometimes be prevented with the right information, which starts with knowing where your systems are vulnerable. Previously, you learned that the CVE® list and scanning tools are two useful ways of finding weaknesses. But, there are other ways to identify vulnerabilities and threats.

In this reading, you’ll learn about open-source intelligence, commonly known as OSINT. OSINT is the collection and analysis of information from publicly available sources to generate usable intelligence. It's commonly used to support cybersecurity activities, like identifying potential threats and vulnerabilities. You'll learn why open-source intelligence is gathered and how it can improve cybersecurity. You’ll also learn about commonly used resources and tools for gathering information and intelligence.

### Information vs Intelligence

The terms intelligence and information are often used interchangeably, making it easy to mix them up. Both are important aspects of cybersecurity that differ in their focus and objectives.

_Information_ refers to the collection of raw data or facts about a specific subject. _Intelligence_, on the other hand, refers to the analysis of information to produce knowledge or insights that can be used to support decision-making.

For example, new information might be released about an update to the operating system (OS) that's installed on your organization's workstations. Later, you might find that new cyber threats have been linked to this new update by researching multiple cybersecurity news resources. The analysis of this information can be used as intelligence to guide your organization's decision about installing the OS updates on employee workstations.

In other words, intelligence is derived from information through the process of analysis, interpretation, and integration. Gathering information and intelligence are both important aspects of cybersecurity.

### Intelligence Improves Decision-Making

Businesses often use information to gain insights into the behavior of their customers. Insights, or intelligence, can then be used to improve their decision making. In security, open-source information is used in a similar way to gain insights into threats and vulnerabilities that can pose risks to an organization.

OSINT plays a significant role in **information security (InfoSec)**, which is the practice of keeping data in all states away from unauthorized users.

For example, a company's InfoSec team is responsible for protecting their network from potential threats. They might utilize OSINT to monitor online forums and hacker communities for discussions about emerging vulnerabilities. If they come across a forum post discussing a newly discovered weakness in a popular software that the company uses, the team can quickly assess the risk, prioritize patching efforts, and implement necessary safeguards to prevent an attack.

Here are some of the ways OSINT can be used to generate intelligence:

- To provide insights into cyber attacks
- To detect potential data exposures
- To evaluate existing defenses
- To identify unknown vulnerabilities

Collecting intelligence is sometimes part of the vulnerability management process. Security teams might use OSINT to develop profiles of potential targets and make data-driven decisions on improving their defenses.

### OSINT Tools

There's an enormous amount of open-source information online. Finding relevant information that can be used to gather intelligence is a challenge. Information can be gathered from a variety of sources, such as search engines, social media, discussion boards, blogs, and more. Several tools also exist that can be used in your intelligence gathering process. Here are just a few examples of tools that you can explore:

| **Tool** | **Description** |
|----------|-----------------|
| [VirusTotal](https://www.virustotal.com/gui/home/upload) | A service that allows anyone to analyse suspicious files, domains, URLs, and IP addresses for malicious content. |
| [MITRE ATT&CK®](https://attack.mitre.org/) | A knowledge base of adversary tactics and techniques based on real-world observations. |
| [OSINT Framework](https://osintframework.com/) | A web-based interface where you can find OSINT tools for almost any kind of source or platform. |
| [Have I been Pwned](https://haveibeenpwned.com/) | A tool that can be used to search for breached email accounts. |

There are numerous other OSINT tools that can be used to find specific types of information. Remember, information can be gathered from a variety of sources. Ultimately, it's your responsibility to thoroughly research any available information that's relevant to the problem you’re trying to solve.

### Key Takeaways

Gathering information and intelligence are important aspects of cybersecurity. OSINT is used to make evidence-based decisions that can be used to prevent attacks. There’s so much information available, which is why it's important for security professionals to be skilled with searching for information. Having familiarity with popular OSINT tools and resources will make your research easier when gathering information and collecting intelligence.

---
# Identify system vulnerabilities
## Vulnerability Assessments

### Introduction

Vulnerability assessments are a crucial aspect of the vulnerability management process. They involve the internal review of an organization's security systems to identify and address weaknesses and flaws. These assessments help prevent attacks and ensure that security controls meet regulatory standards. Security analysts play a key role in conducting and evaluating vulnerability assessments.

### The Process of Vulnerability Assessments

#### Identification

- **Tools and Methods:** Use scanning tools and manual testing to find vulnerabilities.
- **Objective:** Understand the current state of a security system, similar to taking a snapshot of it.
- **Outcome:** A large number of potential vulnerabilities are typically identified.

#### Vulnerability Analysis

- **Role:** Act as a digital detective to find the source of each identified vulnerability.
- **Methods:** Test each vulnerability to determine its nature and impact.
- **Goal:** Gain a deeper understanding of each vulnerability.

#### Risk Assessment

- **Scoring:** Assign a score to each vulnerability based on:
  - **Severity of Impact:** How severe the consequences would be if the vulnerability were exploited.
  - **Likelihood:** The probability of the vulnerability being exploited.
- **Purpose:** Prioritize resources to address the most critical vulnerabilities first.

#### Remediation

- **Collaboration:** Security staff and IT teams work together to fix identified vulnerabilities.
- **Steps:** Implement measures such as enforcing new security procedures, updating operating systems, or applying system patches.
- **Objective:** Address vulnerabilities based on their severity score from the risk assessment step.

### Importance of Vulnerability Assessments

- **Preventive Measure:** Helps organizations identify and address weaknesses before they can be exploited.
- **Regulatory Compliance:** Ensures that security controls meet industry standards and regulatory requirements.
- **Resource Allocation:** Prioritizes vulnerabilities to allocate resources effectively.

### Key Takeaways

- Vulnerability assessments are a continuous process aimed at identifying, analysing, assessing, and remediating security weaknesses.
- They involve a collaborative effort between security and IT teams to ensure comprehensive coverage and effective remediation.
- Regular assessments help maintain a strong security posture by addressing vulnerabilities proactively.

By following this structured approach, organizations can effectively manage vulnerabilities and protect their assets from potential threats.

## Approaches to Vulnerability Scanning

### Introduction
Previously, you learned about vulnerability assessments, which involve the internal review of an organization's security systems to identify weaknesses and prevent attacks. Vulnerability scanning tools are essential in simulating threats by finding vulnerabilities in an attack surface and aiding security teams in implementing remediation strategies.

### What is a Vulnerability Scanner?

A vulnerability scanner is software that automatically compares known vulnerabilities and exposures against the technologies on the network. These tools scan systems to find misconfigurations or programming flaws.

#### Scanning Tools analyse the Five Attack Surfaces:
- **Perimeter Layer:** Authentication systems that validate user access.
- **Network Layer:** Technologies like network firewalls.
- **Endpoint Layer:** Devices on a network, such as laptops, desktops, or servers.
- **Application Layer:** Software that users interact with.
- **Data Layer:** Information that’s stored, in transit, or in use.

When a scan begins, the tool compares findings against databases of security threats, flags any vulnerabilities, and adds them to its reference database. Vulnerability databases are routinely updated by the scanning software's company.

### Performing Scans

Vulnerability scanners are generally non-intrusive, meaning they don't break or exploit a system like an attacker would. Instead, they scan a surface and alert to any potentially unlocked doors in your systems. However, in some cases, a scan can inadvertently cause issues, such as crashing a system.

### Types of Vulnerability Scans

#### External vs. Internal

- **External Scans:** Test the perimeter layer outside of the internal network, analyzing outward-facing systems like websites and firewalls. They can uncover vulnerabilities like open network ports or servers.
- **Internal Scans:** Examine an organization's internal systems, analyzing application software for weaknesses in how it handles user input.

#### Authenticated vs. Unauthenticated

- **Authenticated Scans:** Test a system by logging in with a real user account or even an admin account, checking for vulnerabilities like broken access controls.
- **Unauthenticated Scans:** Simulate external threat actors without access to business resources. For example, they might analyse file shares within the organization to ensure unauthenticated users receive "access denied" results.

#### Limited vs. Comprehensive

- **Limited Scans:** analyse particular devices on a network, like searching for misconfigurations on a firewall.
- **Comprehensive Scans:** analyse all devices connected to a network, including operating systems, user databases, and more.

**Pro Tip:** Discovery scanning should be done before limited or comprehensive scans to get an idea of the computers, devices, and open ports on a network.

### Key Takeaways

- **Diverse Approaches:** Vulnerability scans vary depending on the surfaces being evaluated.
- **Proactive Security:** Seasoned security professionals usually configure and perform these scans to create a security profile of a company. Analysts also play a crucial role in the process.
- **Outcomes:** Results from vulnerability scans often lead to compliance efforts, procedural changes, and system patching.

## The Importance of Updates

### Introduction
At some point, you may have wondered, “Why do my devices constantly need updating?” For consumers, updates improve performance, stability, and introduce new features. From a security standpoint, updates serve a specific purpose: they allow organizations to address security vulnerabilities that can place users, devices, and networks at risk.

### Patching Gaps in Security
An outdated computer is like a house with unlocked doors. Malicious actors exploit these gaps in security to gain unauthorized access. Software updates are similar to locking the doors to keep them out. 

A **patch update** is a software and operating system update that addresses security vulnerabilities within a program or product. Patches usually contain bug fixes that address common security vulnerabilities and exposures (CVEs).

**Note:** Ideally, patches address CVEs before malicious hackers find them. However, patches are sometimes developed as a result of a zero-day exploit, which is a vulnerability that was previously unknown.

### Common Update Strategies
When software updates become available, clients and users have two installation options: manual updates and automatic updates. Each strategy has benefits and disadvantages.

#### Manual Updates
A manual deployment strategy relies on IT departments or users obtaining updates from developers. Home office or small business environments might require individuals to find, download, and install updates themselves. In enterprise settings, the process is usually handled with a configuration management tool, offering a range of options to deploy updates, such as to all clients on a network or a select group of users.

**Advantages:**
- Control: Useful if software updates are not thoroughly tested by developers, which can lead to instability issues.

**Disadvantages:**
- Forgetfulness: Critical updates can be forgotten or disregarded entirely.

#### Automatic Updates
An automatic deployment strategy automates the process of finding, downloading, and installing updates by the system or application.

**Pro Tip:** The Cybersecurity and Infrastructure Security Agency (CISA) recommends using automatic options whenever available.

Certain permissions need to be enabled by users or IT groups before updates can be installed or pushed when they're available. It is up to the developers to adequately test their patches before release.

**Advantages:**
- Simplification: The deployment process is simplified, keeping systems and software current with the latest critical patches.

**Disadvantages:**
- Instability: Issues can occur if patches were not thoroughly tested by the vendor, resulting in performance problems and a poor user experience.

### End-of-Life Software
Sometimes updates are not available for end-of-life (EOL) software. All software has a lifecycle, beginning when it’s produced and ending when a newer version is released. Developers allocate resources to newer versions, leading to EOL software. While older software is still useful, the manufacturer no longer supports it.

**Note:** Patches and updates differ from upgrades. Upgrades refer to completely new versions of hardware or software that can be purchased.

**CISA recommends discontinuing the use of EOL software** because it poses an unfixable risk to systems. However, this recommendation is not always followed due to the cost of replacing EOL technology for businesses and individual users.

The risks that EOL software presents grow as more connected devices enter the marketplace. For example, billions of Internet of Things (IoT) devices, like smart light bulbs, are connected to home and work networks. In some business settings, all an attacker needs is a single unpatched device to gain network access and cause problems.

### Key Takeaways
Updating software and patching vulnerabilities is a critical practice everyone should participate in. Unfortunately, that’s not always the case. Many of the biggest cyber attacks in the world might have been prevented if systems were kept updated. One example is the WannaCry attack of 2017, which affected computers in more than 150 countries and caused an estimated $4 billion in damages. Researchers found that WannaCry could have been prevented if the infected systems were up-to-date with a security patch made available months before the attack. Keeping software updated requires effort, but the benefits make it worthwhile.

### Summary Table

| **Update Strategy**     | **Advantages**                               | **Disadvantages**                                  |
|-------------------------|----------------------------------------------|---------------------------------------------------|
| **Manual Updates**      | Control                                      | Critical updates can be forgotten or disregarded  |
| **Automatic Updates**   | Simplified deployment, keeps systems current | Instability issues if patches aren't thoroughly tested |

**End-of-Life Software:** Use of such software poses unfixable risks, but discontinuation is often not followed due to cost.

**Key Example:** The WannaCry attack could have been prevented with timely updates.

## Penetration Testing

### Introduction

An effective security plan relies on regular testing to identify an organization's weaknesses. Previously, you learned about vulnerability assessments, which are internal reviews of an organization's security systems used to design defence strategies based on system weaknesses. In this reading, you'll learn how security teams evaluate the effectiveness of their defences using penetration testing.

### Penetration Testing

A **penetration test** (pen test) is a simulated attack that helps identify vulnerabilities in systems, networks, websites, applications, and processes. The simulated attack in a pen test involves using the same tools and techniques as malicious actors to mimic a real-life attack. Since a pen test is an authorized attack, it is considered a form of ethical hacking. Unlike a vulnerability assessment that finds weaknesses in a system's security, a pen test exploits those weaknesses to determine the potential consequences if the system is compromised by a threat actor.

**Example:** The cybersecurity team at a financial company might simulate an attack on their banking app to determine if there are weaknesses that would allow an attacker to steal customer information or illegally transfer funds. If the pen test uncovers misconfigurations, the team can address them and improve the overall security of the app.

**Note:** Organizations regulated by PCI DSS, HIPAA, or GDPR must routinely perform penetration testing to maintain compliance standards.

### Learning from Varied Perspectives

These authorized attacks are performed by pen testers skilled in programming and network architecture. Depending on their objectives

# Cyber attacker mindset

## Protect All Entry Points

### Introduction

There's a wide range of vulnerabilities in systems that need to be found. Assessing those weaknesses is a time-consuming process. To position themselves ahead of threats and make the most of their limited resources, companies start by understanding the environment surrounding their operations. An important part of this is getting a sense of their attack surface.

### Attack Surface Analysis

An **attack surface** is all the potential vulnerabilities that a threat actor could exploit. Analyzing the attack surface is usually the first thing security teams do.

**Example:** Imagine being part of a security team of an old castle. Your team would need to decide how to allocate resources to defenses. Giant walls, stone towers, and wooden gates are a few common security controls of these structures. While these are all designed to protect the assets inside from attacks, they don't account for all the possibilities. What if the castle were near the ocean? If it were, these defenses would be vulnerable to long-range attacks by ship. A proper understanding of the attack surface would mean your security team equipped the castle with catapults that could deal with these kinds of threats.

### Physical and Digital Attack Surfaces

Modern organizations need to concern themselves with both a physical and digital attack surface.

**Physical Attack Surface:** The physical attack surface is made up of people and their devices. This surface can be attacked from both inside and outside the organization, which makes it unique.

**Example:** Consider an unattended laptop in a public space, like a coffee shop. The person responsible for it walked away while sensitive company information was visible on the screen. This information is vulnerable to external threats, like a business competitor who can easily record the information and exploit it. An internal threat of this attack surface is often angry employees who might share an organization's private information on purpose.

### Security Hardening

In general, the physical attack surface should be filled with obstacles that deter attacks from happening. This process is called **security hardening**.

**Security Hardening:** Security hardening is the process of strengthening a system to reduce its vulnerabilities and attack surface. In other words, hardening is the act of minimizing the attack surface by limiting its points of entry.

**Note:** Some security controls we've explored previously, like organization policies and access controls, are common ways that organizations harden their physical attack surface.

### Digital Attack Surface

The digital attack surface includes everything beyond an organization's firewall. It includes anything that connects to an organization online.

**Example:** In the past, organizations stored their data in a single location, mainly consisting of servers managed on-site. Accessing the information stored on those servers required connecting to the network the workplace managed. Nowadays, information is accessed outside of an organization's network because it's stored in the cloud. Information can be accessed from anywhere in the world. A person can be in one part of the world, fly to another place, and continue working, all while outside of their organization's network.

### Impact of Cloud Computing

**Cloud Computing:** Cloud computing has essentially expanded the digital attack surface. Quicker access to information is something we all benefit from, but it comes with a cost. Organizations of all sizes are under more pressure to defend against threats coming from different entry points.

### Key Takeaways

Understanding and protecting all entry points is critical for maintaining security. Both physical and digital attack surfaces must be analysed and hardened to prevent unauthorized access. As information and access points increase with technologies like cloud computing, the challenge of securing all entry points becomes more complex.

Approach Cybersecurity with an Attacker Mindset
-----------------------------------------------

### Introduction

Cybersecurity is a continuously changing field. It's a fast-paced environment where new threats and innovative technologies can disrupt your plans at a moment's notice. As a security professional, it’s up to you to be prepared by anticipating change. This all starts with identifying vulnerabilities. In this reading, you will learn how to use the findings of a vulnerability assessment proactively by analysing them from the perspective of an attacker.

### Being Prepared for Anything

Having a plan should things go wrong is important. But how do you figure out what to plan for? Teams often conduct simulations of potential issues as part of their vulnerability management strategy. One way this is done is by applying an attacker mindset to the weaknesses they discover.

**Applying an Attacker Mindset:**
---------------------------------

*   It's like conducting an experiment by causing problems in a controlled environment and evaluating the outcome to gain insights.
*   Offers a different perspective about the challenges you're trying to solve.
*   Helps establish or modify a security plan.

### Simulating Threats

Simulating threats is a method of applying an attacker mindset. These activities are normally performed in two ways: proactively and reactively. Both approaches aim to make systems safer.

**Proactive Simulations:**
--------------------------

*   Assume the role of an attacker by exploiting vulnerabilities and breaking through defences.
*   Known as a red team exercise.
*   Proactive teams spend more time planning attacks than performing them.
*   Example: Persuading staff to disclose their login credentials using fictitious emails to evaluate security awareness.

**Reactive Simulations:**
-------------------------

*   Assume the role of a defender responding to an attack.
*   Known as a blue team exercise.
*   Reactive teams gather information about the assets they're protecting, often using vulnerability scanning tools.

### Scanning for Trouble

A vulnerability scanner is software that automatically compares existing common vulnerabilities and exposures against the technologies on the network. Security teams use various scanning techniques to uncover weaknesses in their defences. Reactive simulations often rely on scan results to weigh risks and determine remediation strategies.

**Steps in a Vulnerability Assessment:**

1.  **Identification:** A vulnerable server is flagged because it's running an outdated operating system (OS).
2.  **Vulnerability Analysis:** Research is done on the outdated OS and its vulnerabilities.
3.  **Risk Assessment:** The severity of each vulnerability is scored, and the impact of not fixing it is evaluated.
4.  **Remediation:** Use gathered information to address the issue.

During such activities, producing a report of findings is essential. Clearly communicating these results to others, like service providers or supervisors, is an important skill.

### Finding Innovative Solutions

Many security controls were created as a reactive response to risks, as criminals continually look for ways to bypass existing defenses. Effectively applying an attacker mindset requires staying knowledgeable of security trends and emerging technologies.

**Pro Tip:** Resources like [NIST's National Vulnerability Database (NVD)](https://nvd.nist.gov/) can help you remain current on common vulnerabilities.

### Key Takeaways

*   Vulnerability assessments are crucial for security risk planning.
*   As an analyst, you'll likely participate in both proactive and reactive simulations.
*   Preparing yourself by researching common vulnerabilities is important, but staying informed about new technologies and thinking innovatively is equally crucial.

## Types of Threat Actors

### Introduction

Anticipating attacks is a crucial skill for an effective security professional. Developing this skill requires an open and flexible mindset about where attacks can come from. Understanding attack surfaces and limiting access to them is key to defending networks, servers, devices, and staff.

### Threat Actors

A **threat actor** is any person or group who presents a security risk. This broad term includes both intentional and accidental threats from inside and outside an organization.

**Categories of Threat Actors:**

1. **Competitors:** Rival companies that might benefit from leaked information.
2. **State Actors:** Government intelligence agencies.
3. **Criminal Syndicates:** Organized groups engaging in criminal activities for profit.
4. **Insider Threats:** Individuals with authorized access who either accidentally or intentionally compromise assets.
5. **Shadow IT:** Individuals using technologies without IT governance, such as personal email for work-related communications.

### Types of Hackers

The term "hacker" can be ambiguous, so it's important to understand the different types based on their intent:

1. **Unauthorized Hackers (Unethical Hackers):**
    
    - Use programming skills for criminal activities.
    - Skill levels vary from script kiddies to highly skilled hackers.
2. **Authorized Hackers (Ethical Hackers):**
    
    - Use skills to improve security.
    - Include internal security team members, external vendors, and freelance hackers participating in bug bounty programs.
3. **Semi-Authorized Hackers:**
    
    - Violate ethical standards but aren't considered malicious.
    - Examples include hacktivists who expose vulnerabilities for political or social causes.

### Advanced Persistent Threats (APTs)

**APTs** refer to instances where a threat actor maintains unauthorized access to a system over an extended period. Often associated with state actors, APTs focus on surveillance and gathering information to manipulate government, defense, financial, and telecom services. Private businesses can also be targeted as stepping stones to larger entities.

### Access Points

Threat actors use various attack vectors to gain access to systems:

1. **Direct Access:** Physical access to a system.
2. **Removable Media:** Portable hardware like USB flash drives.
3. **Social Media:** Communication and content sharing platforms.
4. **Email:** Both personal and business accounts.
5. **Wireless Networks:** On-premises networks.
6. **Cloud Services:** Provided by third-party organizations.
7. **Supply Chains:** Third-party vendors presenting backdoor access.

### Key Takeaways

- Defending an attack surface starts with thinking like a threat actor.
- Understand why someone would pose a threat to organizational assets.
- Recognize that not all threat actors intend to cause harm.
- Match intentions with attack vectors to better defend against potential threats.

## Pathways Through Defenses

### Introduction

To defend against attacks, organizations need more than just an understanding of the digital landscape. They must also understand the types of attacks that can be used against them. This involves analyzing the attack vectors, or pathways, that attackers use to penetrate security defenses.

### Attack Vectors

**Attack vectors** refer to the pathways attackers use to exploit vulnerabilities in security defenses. Examples include social media and removable media like USB drives.

- **Social Media:** Employees might unintentionally or intentionally share sensitive company news.
- **Removable Media:** Devices like USB drives can be used to transfer malicious software into a network.

### Threats Beyond Cyber Criminals

Not only cyber criminals exploit attack vectors. Employees, whether intentionally or unintentionally, can also pose risks.

- **Unintentional Exploits:** Sharing sensitive information on social media.
- **Intentional Exploits:** Disgruntled employees leaking confidential information.

### Practicing an Attacker Mindset

Security professionals use an attacker mindset to anticipate and defend against threats by asking, "How would we exploit this vector?" This involves a step-by-step process:

1. **Identify a Target:** Specific information, systems, people, groups, or the organization.
2. **Determine Access Points:** Identify information available that an attacker might use.
3. **Evaluate Attack Vectors:** Assess which vectors can be exploited to gain entry.
4. **Find Tools and Methods:** Determine the tools and methods attackers might use.

### Implementing Security Controls

By thinking like attackers, security teams gain insights into the best security controls to implement and the vulnerabilities to monitor. Common rules for defending attack vectors include:

#### Educating Users

- **User Education:** Inform users about security vulnerabilities, such as new phishing exploits targeting the organization.

#### Principle of Least Privilege

- **Least Privilege:** Limit access rights to only what is required to perform a task, closing multiple security holes.

#### Security Controls and Tools

- **Security Tools:** Utilize antivirus software and other tools to defend attack vectors and reduce the risk of human error.

#### Diverse Security Team

- **Diverse Team:** Building a diverse security team enhances the ability to apply an attacker's mindset and stay ahead of potential threats.

### Conclusion

Defending an organization's attack surface involves continuous education, applying security principles, using the right tools, and fostering a diverse security team. Staying informed and proactive is essential in this field.

## Fortify Against Brute Force Cyber Attacks

Usernames and passwords are critical security controls, much like door locks that restrict access to networks, services, and data. However, these credentials are vulnerable to being guessed or stolen by attackers.

### A Matter of Trial and Error

Brute force attacks involve trying many combinations to guess a password:

- **Simple Brute Force Attacks:** Attackers guess login credentials by entering any combination of username and password until they find the correct one.
- **Dictionary Attacks:** Attackers use a list of commonly used credentials to access a system.
- **Reverse Brute Force Attacks:** Attackers start with a single credential and try it on various systems until they find a match.
- **Credential Stuffing:** Attackers use stolen login credentials from previous data breaches to access user accounts at another organization.
- **Pass the Hash:** Attackers reuse stolen, unsalted hashed credentials to trick an authentication system.

### Tools of the Trade

Attackers use software to automate the guesswork of brute force attacks. Common tools include:

- **Aircrack-ng:** Tests Wi-Fi network vulnerabilities.
- **Hashcat:** A versatile password cracking tool.
- **John the Ripper:** A fast password cracker.
- **Ophcrack:** Uses rainbow tables to crack passwords.
- **THC Hydra:** Supports numerous protocols for brute force attacks.

### Prevention Measures

Organizations can defend against brute force attacks using technical and managerial controls:

#### Hashing and Salting

- **Hashing:** Converts information into a unique value to determine its integrity.
- **Salting:** Adds random characters to data, increasing the complexity of hash values, making them harder to brute force.

#### Multi-Factor Authentication (MFA)

- **MFA:** Requires a user to verify their identity in two or more ways to access a system, reducing the likelihood of successful brute force attacks.

#### CAPTCHA

- **CAPTCHA:** A challenge-response authentication system that differentiates between humans and automated software. Common CAPTCHA examples include:
    - **Text-based CAPTCHA:** Users enter scrambled letters and/or numbers into a text box.
    - **Image-based CAPTCHA:** Users match images to a randomly generated word.

#### Password Policy

- **Password Policies:** Standardize good password practices, such as:
    - Requiring passwords to be at least 8 characters long and include a letter, number, and symbol.
    - Implementing password lockout policies that limit login attempts and require password changes after a certain period.

### Key Takeaways

Brute force attacks are simple but effective methods to gain unauthorized access. Strong passwords are more resistant to these attacks. As a security professional, recognizing the tactics and tools used in brute force attacks is crucial for implementing effective defences.

# Glossary terms from module 3

**Advanced persistent threat (APT):** An instance when a threat actor maintains unauthorized access to a system for an extended period of time 

**Attack surface:** All the potential vulnerabilities that a threat actor could exploit

**Attack tree:** A diagram that maps threats to assets

**Attack vector:** The pathways attackers use to penetrate security defences 

**Bug bounty:** Programs that encourage freelance hackers to find and report vulnerabilities

**Common Vulnerabilities and Exposures (CVE®) list:** An openly accessible dictionary of known vulnerabilities and exposures

**Common Vulnerability Scoring System (CVSS):** A measurement system that scores the severity of a vulnerability

**CVE Numbering Authority (CNA):** An organization that volunteers to analyse and distribute information on eligible CVEs

**Defence in depth:** A layered approach to vulnerability management that reduces risk

**Exploit:** A way of taking advantage of a vulnerability

**Exposure:** A mistake that can be exploited by a threat

**Hacker:** Any person who uses computers to gain access to computer systems, networks, or data

**MITRE:** A collection of non-profit research and development centers

**Security hardening:** The process of strengthening a system to reduce its vulnerability and attack surface

**Threat actor:** Any person or group who presents a security risk

**Vulnerability:** A weakness that can be exploited by a threat

**Vulnerability assessment:** The internal review process of a company’s security systems

**Vulnerability management:** The process of finding and patching vulnerabilities

**Vulnerability scanner:** Software that automatically compares existing common vulnerabilities and exposures against the technologies on the network

**Zero-day:** An exploit that was previously unknown