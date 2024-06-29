#### In this course, you will:

- Explain security’s role in mitigating organizational risk
- Describe the defense in depth strategy
- Explain how vulnerability assessments are used to assess potential risk
- Develop an attacker mindset to recognize threats
- Discuss the role encryption and hashing play in securing assets
- Identify forms of social engineering, malware, and web-based exploits

#### Skill sets:

- Classifying assets
- Decrypting a message
- Searching the CVE database for vulnerable applications
- Analyzing attack surfaces
- Applying the PASTA threat modeling framework

---
# Introduction to assets

## The What, Why, and How of Asset Security

### Introduction
Understanding asset security is crucial for maintaining a robust security posture. This section delves into the concepts of assets, threats, and vulnerabilities, forming the foundation of security planning.

### The Importance of Practice
- **Security as a Skill:** Just like painting, sports, or playing an instrument, security requires continuous practice.
- **Core Skill:** Planning for the future is essential in security and requires time, dedication, and focus.

### Dealing with Uncertainty
- **Anticipation:** We all try to solve problems before they arise, such as planning a trip.
- **Example:** Packing coats and sweaters for a cold destination.
- **Organizational Planning:** Businesses also plan ahead by analyzing risk to ensure security.

### Focus on Risk
- **Definition of Risk:** In security, risk is anything that can impact the confidentiality, integrity, or availability of an asset.
- **CIA Triad:** The primary focus is on maintaining:
  - **Confidentiality**
  - **Integrity**
  - **Availability**

### Elements of Security Plans
- **Three Elements:**
  - **Assets:** Items perceived as valuable to an organization.
  - **Threats:** Circumstances or events that can negatively impact assets.
  - **Vulnerabilities:** Weaknesses that can be exploited by threats.
- **Objective:** Measure security risk by analyzing how these elements affect confidentiality, integrity, and availability.

### Assets
- **Definition:** Items of value to an organization.
- **Examples:** Buildings, equipment, data, people.
- **Home Analogy:** 
  - **Inside Assets:** People, personal belongings.
  - **Outside Assets:** Walls, roof, windows, doors.
- **Protection Priorities:** Security plans prioritize resources to protect assets efficiently.

### Threats
- **Definition:** Any circumstance or event that can negatively impact assets.
- **Examples:** Burglars, accidents, natural events.
- **Home Analogy:** 
  - **Burglars:** Trying to gain access.
  - **Accidents:** Strong winds blowing doors open, kids damaging windows.

### Vulnerabilities
- **Definition:** Weaknesses within assets that can be exploited by threats.
- **Examples:** Weak locks, old and cracked wood.
- **Home Analogy:** 
  - **Weak Lock:** Exploitable by burglars.
  - **Old Wood:** Vulnerable to storm damage.

### Conclusion
- **Comprehensive Planning:** Effective security plans account for a wide range of assets, threats, and vulnerabilities.
- **Future Focus:** Security teams continuously plan and adapt to protect the organization's assets.

## Understand Risks, Threats, and Vulnerabilities

### Introduction
When security events occur, effective coordination and clear communication are essential to address problems swiftly. Understanding the distinctions between risk, threat, and vulnerability is fundamental for security professionals. This guide delves into these key concepts and their interrelationships.

### Foundational Security Terms
- **Risk:** Anything that can impact the confidentiality, integrity, or availability of an asset.
- **Threat:** Any circumstance or event that can negatively impact assets.
- **Vulnerability:** A weakness that can be exploited by a threat.

These terms, while often used interchangeably in everyday language, have specific meanings in the context of security.

### Security Risk
Security plans revolve around how an organization defines risk. The interpretation and approach to risk can vary significantly between organizations.

- **Risk Definition:** Anything that can impact the confidentiality, integrity, or availability of an asset.
- **Risk Calculation:** 
  \[
  \text{Likelihood} \times \text{Impact} = \text{Risk}
  \]
  
#### Example:
- **Scenario:** Driving a car to work.
- **Likelihood:** Getting a flat tire.
- **Impact:** Being late to work, potentially losing your job.
  
Organizations calculate risk to:
- Prevent costly and disruptive events.
- Identify system and process improvements.
- Determine tolerable risks.
- Prioritize critical assets requiring attention.

The business impact of a negative event depends on the asset and the situation. Security professionals focus on the likelihood aspect by addressing factors that increase the odds of a problem.

### Risk Factors
Risk factors in security are broadly classified into:
- **Threats**
- **Vulnerabilities**

The risk of an asset being harmed depends on whether a threat exploits a vulnerability.

#### Example:
- **Scenario:** Being late to work.
- **Threat:** Nail puncturing a tire.
- **Vulnerability:** Tires are susceptible to sharp objects.
- **Mitigation:** Driving on clean roads to reduce the risk.

### Categories of Threats
Threats are circumstances or events that can negatively impact assets. They are categorized as:
- **Intentional Threats:** Deliberate actions aimed at causing harm.
  - **Example:** A malicious hacker targeting a misconfigured application to gain access to sensitive information.
- **Unintentional Threats:** Accidental events that cause harm.
  - **Example:** An employee unknowingly holding the door open for an unauthorized person.

### Categories of Vulnerabilities
Vulnerabilities are weaknesses that can be exploited by threats. They are grouped into:
- **Technical Vulnerabilities:** Flaws in systems or software.
  - **Example:** Misconfigured software allowing unauthorized data access.
- **Human Vulnerabilities:** Human errors or actions.
  - **Example:** An employee losing their access card.

### Key Takeaways
- **Understanding Terms:** Knowing the specific meanings of risks, threats, and vulnerabilities helps build a strong foundation in security.
- **Interrelationships:** Understanding how these elements interact enhances your credibility and demonstrates working knowledge in the field.
- **Professional Growth:** Mastering these concepts signals to colleagues that you are a knowledgeable member of the global security community.

## Security Starts with Asset Classification

### Introduction
Security begins with understanding and managing the assets that need protection. Just like losing your keys can be stressful, organizations face similar challenges when tracking their valuable assets. Effective security management starts with asset classification.

### The Challenge of Asset Management
- **Everyday Stress:** Difficulty in finding important items like keys can be frustrating.
- **Organizational Parallel:** Businesses, too, must keep track of numerous important assets.

#### Example Scenario:
- **New Security Team Member:** You join a small online retailer’s security team.
- **Growing Business:** The company’s expanding customer base increases the number of assets.
- **Responsibility:** Each team member is responsible for 10 assets, highlighting the need for robust asset management.

### Importance of Asset Management
- **Fundamental Truth:** You can only protect what you can account for.
- **Asset Management Definition:** The process of tracking assets and the risks affecting them.
- **Core Security Element:** Asset management is central to all security plans.

### Asset Inventory
- **Definition:** A catalog of assets needing protection.
- **Purpose:** Prevents organizations from losing track of important assets.

#### Analogy:
- **Shepherd and Sheep:** Knowing the exact number of sheep helps allocate resources and alerts if one goes missing.

### Asset Classification
- **Practice:** Labeling assets based on their sensitivity and importance to the organization.
- **Example Ranking:** Wallet is more important than shoes.

#### Classification Scheme:
- **Public:** Shared with anyone.
- **Internal-Only:** Shared within the organization but not outside.
- **Confidential:** Accessed only by those working on a specific project.
- **Restricted:** Highly sensitive, protected, and need-to-know basis.

### Detailed Classification Examples
- **Public Assets:** Information that can be freely shared.
- **Internal-Only Assets:** Internal company communications and documents.
- **Confidential Assets:** Project-specific documents and communications.
- **Restricted Assets:** Intellectual property, health information, and payment information.

#### Practical Applications:
- **Internal Emails:** Marked as confidential for new product development.
- **Office Doors:** Labelled restricted to prevent unauthorized access.

### Impact of Classification
- **Disclosure:** Determines who can access the asset.
- **Alteration:** Specifies who can modify the asset.
- **Destruction:** Indicates how and when an asset can be disposed of.

### Continuous Process of Asset Management
- **Ongoing Practice:** Regularly reviewing and updating asset records.
- **Uncovering Gaps:** Identifies potential security risks and gaps.
- **Essential Part of Security Planning:** Ensures comprehensive protection of all organizational assets.

### Summary
Asset management and classification are critical components of a robust security strategy. By accurately cataloguing and classifying assets, organizations can effectively allocate resources, mitigate risks, and ensure the protection of valuable information and resources.

## Common Classification Requirements

### Introduction
Asset management is essential for tracking assets and the risks affecting them. Effective asset management requires identifying, tracking, and classifying assets. This guide delves into the purpose and benefits of asset classification, including common classification levels.

### Why Asset Management Matters
A workable system to protect assets ensures businesses operate smoothly. Detailed knowledge of assets is crucial for setting up these systems. For example, a bank needs to secure its money, ensuring availability and protection from unauthorized access.

#### Examples of Different Assets:
- **Digital Assets:** Customer data, financial records.
- **Information Systems:** Networks, software.
- **Physical Assets:** Facilities, equipment, supplies.
- **Intangible Assets:** Brand reputation, intellectual property.

Every asset, regardless of type, should be classified and accounted for. Asset classification involves labeling assets based on sensitivity and importance to an organization.

### Determining Asset Characteristics
To classify assets effectively, organizations need to know:
- **What you have**
- **Where it is**
- **Who owns it**
- **How important it is**

This information helps determine the sensitivity and value of an asset.

### Common Asset Classifications
Asset classification aids in effective risk management, prioritizing security resources, reducing IT costs, and complying with legal regulations. The most common classification scheme includes four levels: restricted, confidential, internal-only, and public.

| Classification Level | Description                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| Restricted           | Highest level; reserved for highly sensitive assets (need-to-know information). |
| Confidential         | Assets whose disclosure may lead to significant negative impact.            |
| Internal-only        | Assets available to employees and business partners.                        |
| Public               | Lowest level; no negative consequences if released.                         |

### Application of Classification
How the classification scheme is applied depends on the characteristics of an asset. Identifying an asset’s owner can be particularly challenging.

#### Ownership Challenges:
- **Straightforward:** Owners of physical assets like buildings.
- **Complex:** Information assets, such as a business-issued laptop used for personal matters.

### Challenges of Classifying Information
Classifying information poses unique challenges due to the complexity of ownership and multiple classification values.

#### Example:
- **Business-Issued Laptop:** Assumed to be owned by the business but may contain personal data like photos.
- **Letter Example:** Contains public information (your name) and confidential information (your address).

### Key Takeaways
- **Business Specifics:** Each business has unique requirements for its security strategy.
- **Importance of Information:** Information is one of the most critical assets, requiring protection from damage, disclosure, and misuse.
- **Challenges:** Recognizing and addressing the challenges of classifying information helps in developing effective security solutions.
---

# Digital and physical assets

## Assets in a Digital World

### Introduction
Welcome back! We've explored organizational assets, their importance, and the tremendous amount of assets security teams protect. Asset classification based on value is crucial, and understanding what makes an asset valuable is key. In today's digital world, information is often the most valuable asset. 

### What Makes an Asset Valuable?
- **Information as Value:** Most valuable assets today are in the form of information.
- **Data:** Information that is translated, processed, or stored by a computer.

### Digital Assets and Their Challenges
- **Connected World:** Billions of devices globally are linked to the internet, constantly exchanging data.
- **Protection Based on State:** Protecting data depends on its state and activity.

### Three States of Data
Security teams protect data in three different states: in use, in transit, and at rest. 

#### Data in Use
- **Definition:** Data being accessed by one or more users.
- **Example:** Checking email on a laptop at a park. When you log in, your inbox is considered to be in use.

#### Data in Transit
- **Definition:** Data traveling from one point to another.
- **Example:** Sending an email reply. When you click send, the email becomes data in transit.

#### Data at Rest
- **Definition:** Data not currently being accessed, typically stored on a physical device.
- **Example:** Closing your laptop after checking email and packing it up. The data on your laptop is at rest.

### Information Security (InfoSec)
- **Purpose:** Protecting data in all states from unauthorized users.
- **Consequences of Weak InfoSec:**
  - **Identity Theft**
  - **Financial Loss**
  - **Reputational Damage**
- **Impact:** These issues can harm organizations, their partners, and their customers.

### Evolving Understanding of Data at Rest
- **Cloud Storage:** Data stored in the cloud means it's not necessarily at rest even if the physical device is not in use.
- **New Vulnerabilities:** Increased connectivity leads to new vulnerabilities that need continuous monitoring.

### Asset Management and Data States
- **Importance:** Understanding the three states of data helps in analyzing risk and determining an asset management plan.
- **Security Plan:** Keeping track of where data is and what it’s doing is part of a comprehensive security strategy.

### Key Takeaways
- **Data States:** Recognizing the states of data (in use, in transit, at rest) is crucial for effective data protection.
- **InfoSec:** Strong information security practices are essential to prevent identity theft, financial loss, and reputational damage.
- **Adaptation:** Continuously adapt security measures to address new vulnerabilities in an increasingly connected world.
- **Asset Management:** Effective asset management requires understanding the state of data and implementing appropriate protections.

## The Emergence of Cloud Security

### Introduction
Cloud computing is one of the most significant technological developments of this century. According to the United Kingdom's National Cyber Security Centre, cloud computing is “an on-demand, massively scalable service, hosted on shared infrastructure, accessible via the internet.” As businesses move their data to the cloud, they face new challenges and opportunities in keeping information safe.

### Soaring into the Cloud
Starting an online business was once a complex and costly process, requiring companies to build and maintain internal solutions. Cloud technologies have drastically changed this landscape, allowing businesses to scale and adapt quickly while lowering costs. However, the shift to cloud-based services has introduced new cybersecurity challenges.

### Cloud-Based Services
Cloud-based services are web-based business solutions available on demand. These services can range from website hosting to application development environments and entire back-end infrastructure. 

#### Three Main Categories of Cloud-Based Services
| Category                    | Description                                                                                         | Examples                                                                                          |
|-----------------------------|-----------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|
| **Software as a Service (SaaS)** | Front-end applications accessed via a web browser. Providers host, manage, and maintain back-end systems. | Gmail™, Slack, Zoom                                                                                |
| **Platform as a Service (PaaS)** | Back-end application development tools accessed online. Developers build, manage, and deploy their apps.   | Google App Engine™, Heroku®, VMware Cloud Foundry                                                 |
| **Infrastructure as a Service (IaaS)** | Remote access to back-end systems hosted by the provider. Resources are licensed as needed.              | Google Cloud Platform, Microsoft Azure                                                            |

Cloud-based services enable companies to connect with customers, employees, and business partners over the internet.

### Cloud Security
Moving applications and infrastructure to the cloud facilitates online business operations but complicates data privacy and safety. Cloud security focuses on protecting data, applications, and infrastructure in the cloud.

#### Traditional vs. Cloud Security
In traditional models, organizations had their IT infrastructure on premises, with internal security teams responsible for protection. In the cloud, responsibilities are shared between clients and providers.

#### Shared Responsibility Model
- **Clients:** Secure anything directly within their control (e.g., identity and access management, resource configuration, data handling).
- **Providers:** Maintain the security of the shared infrastructure (e.g., servers).

The division of responsibility varies depending on the type of service (SaaS, PaaS, IaaS).

### Cloud Security Challenges
Several challenges arise from storing data in the cloud and accessing it over the internet:

| Challenge                | Description                                                                                                         |
|--------------------------|---------------------------------------------------------------------------------------------------------------------|
| **Misconfiguration**     | Customers are responsible for configuring their own security environment. Out-of-the-box configurations often fall short. |
| **Cloud-Native Breaches**| More likely due to misconfigured services.                                                                           |
| **Monitoring Access**    | Varies depending on the client and level of service.                                                                |
| **Regulatory Standards** | Meeting standards like HIPAA, PCI DSS, and GDPR can be challenging.                                                 |

These challenges highlight the need for cloud security professionals to address the growing number of risks associated with cloud-based services.

### Key Takeaways
The global marketplace has largely shifted to cloud-based services, resulting in new security models and challenges. Familiarity with cloud technologies and services is crucial for supporting organizational efforts to protect information online.

---
# Risk and asset security

## Elements of a Security Plan

### Introduction
Security encompasses people, processes, and technology, requiring a collective effort from the entire organization. It’s a culture with shared values extending to employees, vendors, and customers. Protecting digital and physical assets involves everyone’s participation.

### The Purpose of Security Plans
- **Common Goal:** Be prepared for risks when they happen.
- **Focus on People:** Considering diverse backgrounds ensures no one is left out during incidents.
- **Risk Definition:** Anything that impacts the confidentiality, integrity, or availability of an asset.

### Common Risk Categories and Factors
- **Categories:**
  - Damage
  - Disclosure
  - Loss of information
- **Factors:**
  - Physical damage
  - Device malfunctions
  - Attacks
  - Human error

#### Example:
- **New School Teacher:** Signs a contract warning against human error, such as using personal email for sensitive information.

### Elements of a Security Plan
Security plans consist of three basic elements: policies, standards, and procedures. These elements share the security plans within an organization, each serving a specific function.

#### 1. Policies
- **Definition:** A set of rules that reduce risk and protect information.
- **Function:** Foundation of every security plan, providing guidance.
- **Focus:** Strategic side, identifying scope, objectives, and limitations.

#### Example:
- **Acceptable Use Policy (AUP):** Newly hired employees sign off on provisions outlining secure ways to access corporate systems.

#### 2. Standards
- **Definition:** Tactical references that inform how to set policies.
- **Function:** Create a point of reference.
- **Focus:** How well assets are protected.

#### Example:
- **Password Management Standard:** NIST Special Publication 800-63B specifies employees’ passwords must be at least eight characters long.

#### 3. Procedures
- **Definition:** Step-by-step instructions to perform a specific security task.
- **Function:** Ensure accountability, consistency, and efficiency.
- **Focus:** Clear, actionable instructions.

#### Example:
- **Procedure Documents:** Instructions on choosing secure passwords or securely resetting a locked password.

### Understanding the Structure
Policies, standards, and procedures are tailored to each organization’s goals. Understanding their structure is essential for making security a team effort.

| Element     | Definition                                                | Function                                          | Focus                   | Example                                                                                  |
|-------------|------------------------------------------------------------|--------------------------------------------------|-------------------------|------------------------------------------------------------------------------------------|
| **Policy**  | Set of rules that reduce risk and protect information      | Foundation of security plan, providing guidance   | Strategic side          | Acceptable Use Policy (AUP)                                                              |
| **Standard**| Tactical references informing policy settings              | Point of reference                                | How well assets protected| NIST Special Publication 800-63B for password management                                 |
| **Procedure**| Step-by-step instructions for specific security tasks     | Ensure accountability, consistency, and efficiency| Clear, actionable tasks | Instructions for choosing secure passwords or securely resetting a locked password       |

### Key Takeaways
- **Security Culture:** Involves everyone’s participation and extends across all organizational levels.
- **Preparedness:** Effective security plans prepare for risks by focusing on people and addressing diverse perspectives.
- **Policies, Standards, Procedures:** Essential elements tailored to organizational goals, ensuring a structured and effective security plan.

## The NIST Cybersecurity Framework

### Introduction
Having a plan is just one part of securing assets. The other crucial part is ensuring everyone follows the plan, which in security is called compliance.

### Compliance
- **Definition:** The process of adhering to internal standards and external regulations.
- **Importance:** Maintaining trust, reputation, safety, and data integrity. Compliance is crucial to avoid fines, penalties, and lawsuits, especially in highly regulated industries like healthcare, energy, and finance.
- **Impact:** Non-compliance can have long-lasting financial and reputational effects.

### Regulations
- **Definition:** Rules set by a government or other authority to control the way something is done.
- **Purpose:** Protect people and their information on a larger scale, similar to policies but more comprehensive and authoritative.

### The NIST Cybersecurity Framework (CSF)
The NIST Cybersecurity Framework is a voluntary framework consisting of standards, guidelines, and best practices to manage cybersecurity risk. It is designed to help businesses secure one of their most important assets: information. The CSF consists of three main components: the core, tiers, and profiles.

### Components of the NIST Cybersecurity Framework

#### 1. The Core
The core is a simplified version of the functions or duties of a security plan. It identifies five broad functions, which act as a security checklist:

| Function  | Description                                                      |
|-----------|------------------------------------------------------------------|
| **Identify** | Develop an understanding to manage cybersecurity risk to systems, assets, data, and capabilities. |
| **Protect**  | Implement appropriate safeguards to ensure delivery of critical infrastructure services. |
| **Detect**   | Implement appropriate activities to identify the occurrence of a cybersecurity event. |
| **Respond**  | Take action regarding a detected cybersecurity incident.       |
| **Recover**  | Maintain plans for resilience and restore any capabilities or services impaired due to a cybersecurity incident. |

#### 2. The Tiers
Tiers provide security teams with a way to measure performance across each of the five functions of the core. They range from Level-1 to Level-4:

| Tier     | Description                                                                                       |
|----------|---------------------------------------------------------------------------------------------------|
| **Level-1 (Partial)**  | Risk management practices are not formalized and risk is managed in an ad hoc manner. |
| **Level-2 (Risk Informed)** | Risk management practices are approved by management but not established as organization-wide policy. |
| **Level-3 (Repeatable)**  | Risk management practices are formally established and organizationally implemented. |
| **Level-4 (Adaptive)**    | Risk management practices are continually improving and adapting. |

Tiers are designed to show organizations what is and isn't working with their security plans, allowing for continuous improvement.

#### 3. The Profiles
Profiles provide insight into the current state of a security plan. They act like photos capturing a moment in time, allowing organizations to compare their security posture at different points to gain insights and track changes over time.

### Revisiting the Core Functions
- **Identify:** Our previous discussions on asset management and risk assessment relate to this function.
- **Protect:** The next focus will be on many of the categories of the protect function.

### Key Takeaways
- **Compliance:** Ensures adherence to standards and regulations, avoiding financial and reputational damage.
- **Regulations:** Protect information on a larger scale.
- **NIST CSF Components:** Core functions, tiers, and profiles are essential elements that help manage and improve cybersecurity practices.

By understanding and implementing the NIST Cybersecurity Framework, organizations can enhance their cybersecurity posture, ensuring better protection of their information and assets.

## Security Guidelines in Action

### Introduction
Organizations often face overwhelming amounts of risk, making it challenging to develop a comprehensive security plan from scratch. Security frameworks, such as the NIST Cybersecurity Framework (CSF), provide a structured approach to managing cybersecurity risks. The NIST CSF is flexible and applicable to any industry, aiding organizations in implementing effective security measures.

![The NIST CSFs five functions: identify, protect, detect, respond, and recover.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/EkOObSH4SXm2So4UnlEsXg_61119b639bf84caeb75133fc91847df1_CS_V-037_S25G008-Edited.png?expiry=1715990400000&hmac=zUJZYAM5K1qkC7XSMrEpLeJeYo73qHNqUX_kpDmj9JU)

### Origins of the Framework
- **Release Year:** 2014
- **Developer:** National Institute of Standards and Technology (NIST)
- **Purpose:** Protect critical infrastructure in the United States
- **Adaptation:** Modified for public and private sector businesses to make it flexible and easier to adopt, especially for small businesses.

### Components of the CSF
The NIST CSF consists of three main components: the core, tiers, and profiles.

#### Core
The CSF core is a set of desired cybersecurity outcomes helping organizations customize their security plans. It consists of five functions:

| Function  | Description                                                                  |
|-----------|------------------------------------------------------------------------------|
| Identify  | Develop an understanding to manage cybersecurity risks to systems, assets, data, and capabilities. |
| Protect   | Implement appropriate safeguards to ensure delivery of critical infrastructure services. |
| Detect    | Implement activities to identify the occurrence of a cybersecurity event.    |
| Respond   | Take action regarding a detected cybersecurity incident.                     |
| Recover   | Maintain plans for resilience and restore any capabilities or services impaired due to a cybersecurity incident. |

#### Tiers
The CSF tiers measure the sophistication of an organization's cybersecurity program, ranging from Level-1 to Level-4:

| Tier                   | Description                                                                                       |
|------------------------|---------------------------------------------------------------------------------------------------|
| **Tier 1 (Partial)**   | Risk management practices are not formalized; risk is managed in an ad hoc manner.                 |
| **Tier 2 (Risk Informed)** | Risk management practices are approved by management but not established as organization-wide policy. |
| **Tier 3 (Repeatable)**| Risk management practices are formally established and organizationally implemented.               |
| **Tier 4 (Adaptive)**  | Risk management practices are continually improving and adapting.                                 |

#### Profiles
CSF profiles are pre-made templates tailored to address specific risks of an organization or industry. They serve as a baseline for developing cybersecurity plans or comparing current cybersecurity posture to industry standards.

### Implementing the CSF
Compliance is the process of adhering to internal standards and external regulations. The NIST CSF helps organizations achieve compliance with various regulations.

#### Steps for Implementation
1. **Create a current profile** of the security operations and outline the specific needs of your business.
2. **Perform a risk assessment** to identify which of your current operations are meeting business and regulatory standards.
3. **analyse and prioritize existing gaps** in security operations that place the business's assets at risk.
4. **Implement a plan of action** to achieve your organization’s goals and objectives.

**Pro Tip:** Always consider current risk, threat, and vulnerability trends when using the NIST CSF.

### Industries Embracing the CSF
The NIST CSF has evolved since its introduction, influenced by the standards and best practices of major companies worldwide. Its flexibility and alignment with security practices help organizations meet regulatory compliance, mitigating financial and reputational risks.

### Key Takeaways
- **Flexibility:** The NIST CSF is a versatile resource for assessing and improving security posture.
- **Best Practices:** Combines security best practices from various industries.
- **Compliance:** Helps businesses meet regulatory compliance requirements to avoid financial and reputational risks.

---
## Glossary terms from module 1

**Asset:** An item perceived as having value to an organization

**Asset classification:** The practice of labelling assets based on sensitivity and importance to an organization

**Asset inventory:** A catalogue of assets that need to be protected

**Asset management:** The process of tracking assets and the risks that affect them 

**Compliance:** The process of adhering to internal standards and external regulations

**Data:** Information that is translated, processed, or stored by a computer

**Data at rest:** Data not currently being accessed

**Data in transit:** Data traveling from one point to another

**Data in use:** Data being accessed by one or more users

**Information security (InfoSec):** The practice of keeping data in all states away from unauthorized users

**National Institute of Standards and Technology (NIST) Cybersecurity Framework (CSF):** A voluntary framework that consists of standards, guidelines, and best practices to manage cybersecurity risk

**Policy:** A set of rules that reduce risk and protect information

**Procedures:** Step-by-step instructions to perform a specific security task

**Regulations:** Rules set by a government or other authority to control the way something is done

**Risk**: Anything that can impact confidentiality, integrity, or availability of an asset

**Standards:** References that inform how to set policies

**Threat:** Any circumstance or event that can negatively impact assets

**Vulnerability:** A weakness that can be exploited by a threat