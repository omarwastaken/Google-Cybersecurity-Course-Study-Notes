## The Future of SIEM Tools

This reading explores how Security Information and Event Management (SIEM) tools are evolving to address modern cybersecurity threats.

**Current SIEM Solutions**

- SIEM tools collect and analyse log data for security monitoring.
- They provide real-time analysis of potential security threats, risks, and vulnerabilities.
- Dashboards help security teams manage and monitor this data.
- However, current SIEM solutions require human intervention for security event analysis.

**The Future of SIEM Tools**

- **Cloud Adoption:** SIEM tools are adapting to cloud environments.
    - **Cloud-Hosted SIEM:** Managed by vendors, accessed via the internet (ideal for organizations without dedicated infrastructure).
    - **Cloud-Native SIEM:** Fully managed by vendors, designed to leverage cloud capabilities (scalability, flexibility).
- **Addressing Evolving Threats:** SIEM tools are expected to adapt to:
    - **Internet of Things (IoT):** The growing number of interconnected devices will increase the attack surface and data volume for threat actors.
    - **Advanced Threats:** SIEM tools will leverage AI and Machine Learning (ML) for improved threat detection, visualization, and data storage.
- **Increased Automation:** Security Orchestration, Automation, and Response (SOAR) will automate responses to common security incidents, freeing analysts for more complex tasks.
- **Improved Platform Integration:** Better communication and interaction between cybersecurity platforms are anticipated.

**Key Takeaways**

- Understanding SIEM tools is crucial for entry-level security analysts (e.g., monitoring dashboards).
- Staying updated on SIEM advancements is essential for adapting to the evolving cybersecurity landscape.
- Cloud adoption, SIEM integration, and automation are key trends in future SIEM development.

---

## Common SIEM Tools

This video introduces several industry-leading SIEM tools and explores the different deployment options available for organizations.

**Types of SIEM Tools (Deployment Options):**

- **Self-Hosted SIEM:**
    - Requires on-premise infrastructure (servers) for installation, operation, and maintenance by the organization's IT department.
    - Ideal for maintaining physical control over sensitive data.
- **Cloud-Hosted SIEM:**
    - Managed by the SIEM vendor and accessed via the internet.
    - Ideal for organizations without the resources to maintain their own infrastructure.
- **Hybrid SIEM:**
    - Combines self-hosted and cloud-hosted deployments for a balance between cloud benefits and physical data control.

**Common SIEM Tools:**

- **Splunk:**
    - A data analysis platform offering SIEM solutions through two products:
        - **Splunk Enterprise:** Self-hosted SIEM tool for log data retention, analysis, and real-time security insights.
        - **Splunk Cloud:** Cloud-hosted SIEM tool for log data collection, search, and monitoring in hybrid or cloud environments.
- **Chronicle:**
    - A cloud-native SIEM tool by Google for data retention, analysis, search, log monitoring, and data collection.
    - Like cloud-hosted tools, it's fully managed by the vendor but specifically designed for cloud environments (scalability, flexibility).

**Key Takeaways**

- Organizations use a variety of SIEM tools to defend against evolving cyber threats.
- SIEM tools are just one component of an organization's cybersecurity strategy.
- This course will provide hands-on experience with Splunk Cloud and Chronicle later in the program.

## Open-Source vs. Proprietary Cybersecurity Tools

This reading explores the differences between open-source and proprietary cybersecurity tools, highlighting their advantages and disadvantages.

**Open-Source Tools**

- **Free and User-Friendly:** Often free to use with a focus on usability and collaboration.
- **Security & Customization:** Public development fosters security and allows users to customize tools for specific needs.
- **Transparency & Improvement:** Source code and training materials are readily available for user modification and improvement.

**Proprietary Tools**

- **Development & Ownership:** Developed and owned by a single entity (person or company).
- **Cost & Access:** Users typically pay a fee for usage, training, and updates. Limited access to source code restricts user modifications.
- **Examples:** Splunk® and Chronicle SIEM tools.

**Common Misconceptions**

- Open-source tools are not inherently less effective or secure than proprietary tools.
- Open-source development allows for quicker identification and resolution of security vulnerabilities.

**Examples of Open-Source Tools**

- **Linux:** A widely used open-source operating system offering customization through a command-line interface.
- **Suricata:** An open-source network analysis and threat detection tool used to inspect network traffic for suspicious activity.

**Key Takeaways**

- Open-source tools are prevalent in cybersecurity.
- This program will provide opportunities to explore both open-source and proprietary tools.

## Using SIEM Tools to Protect Organizations

This reading explores how Security Information and Event Management (SIEM) tools and their dashboards help cybersecurity professionals identify potential threats, risks, and vulnerabilities within an organization.

**SIEM Dashboards and Purposes**

SIEM tools offer various dashboards to visualize security data for different purposes:

- **Security Posture Dashboard (Splunk & Chronicle):**
    - Monitors security events and trends over the past 24 hours.
    - Helps assess security infrastructure and policy effectiveness.
    - Enables real-time investigation of suspicious activity (e.g., suspicious IP addresses).
- **Executive Summary Dashboard (Splunk):**
    - Analyses overall security health over time.
    - Supports security teams in improving security measures and reducing risk.
    - Provides high-level security insights to stakeholders (e.g., security incident trends).
- **Incident Review Dashboard (Splunk):**
    - Assists in identifying suspicious patterns during security incidents.
    - Highlights high-risk items for immediate review by analysts.
    - Provides a visual timeline of events leading up to an incident.
- **Risk Analysis Dashboard (Splunk):**
    - Helps identify risks associated with specific assets (users, computers, IP addresses).
    - Shows changes in risk-related activity (e.g., unusual login times, high network traffic).
    - Enables prioritizing risk mitigation efforts based on potential impact of vulnerabilities.

**Chronicle Dashboards and Purposes**

- **Enterprise Insights Dashboard:**
    - Highlights recent security alerts and identifies suspicious domain names (IOCs) in logs.
    - Uses confidence scores and severity levels to indicate threat likelihood and significance.
    - Helps monitor login/data access attempts from unusual locations or devices for critical assets.
- **Data Ingestion and Health Dashboard:**
    - Shows the number of event logs, log sources, and success rates of data processing.
    - Ensures logs are received without errors and that log sources are configured correctly.
    - Identifies and addresses log-related issues to maintain access to necessary data.
- **IOC Matches Dashboard:**
    - Identifies the top threats, risks, and vulnerabilities affecting the organization.
    - Enables monitoring of domain names, IP addresses, and device IOCs over time for trend analysis.
    - Helps prioritize security efforts by focusing on the highest threats.
- **Main Dashboard:**
    - Provides a high-level overview of data ingestion, alerting, and event activity.
    - Offers a timeline of security events (e.g., failed login attempts) across various data sources.
    - Assists in identifying threat trends across logs, devices, locations, and IP addresses.
- **Rule Detections Dashboard:**
    - Provides statistics on security incidents with the highest occurrences, severities, and detections.
    - Offers a list of alerts triggered by specific detection rules (e.g., opening malicious email attachments).
    - Helps manage recurring incidents and establish mitigation tactics to reduce risk.
- **User Sign In Overview Dashboard:**
    - Provides information about user access behaviour across the organization.
    - Enables identifying unusual activity (e.g., simultaneous logins from multiple locations).
    - Helps mitigate threats, risks, and vulnerabilities to user accounts and applications.

**Key Takeaways**

SIEM dashboards are crucial for organizing and prioritizing security tasks. They empower security professionals to identify, analyse, and address high-priority threats efficiently, minimizing risk. Later in the program, you will gain hands-on experience using SIEM tool features and search queries.

---
## Glossary terms from module 3

**Chronicle:** A cloud-native tool designed to retain, analyse, and search data

**Incident response:** An organization’s quick attempt to identify an attack, contain the damage, and correct the effects of a security breach

**Log:** A record of events that occur within an organization’s systems 

**Metrics:** Key technical attributes such as response time, availability, and failure rate, which are used to assess the performance of a software application

**Operating system (OS):** The interface between computer hardware and the user

**Playbook:** A manual that provides details about any operational action

**Security information and event management (SIEM):** An application that collects and analyses log data to monitor critical activities in an organization

**Security orchestration, automation, and response (SOAR):** A collection of applications, tools, and workflows that use automation to respond to security events

**SIEM tools:** A software platform that collects, analyses, and correlates security data from various sources across your IT infrastructure that helps identify and respond to security threats in real-time, investigate security incidents, and comply with security regulations

**Splunk Cloud:** A cloud-hosted tool used to collect, search, and monitor log data

**Splunk Enterprise:** A self-hosted tool used to retain, analyse, and search an organization's log data to provide security information and alerts in real-time