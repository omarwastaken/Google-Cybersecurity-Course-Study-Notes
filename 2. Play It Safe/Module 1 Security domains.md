# Manage Security Risks
---
#### In this course, you will:

- Recognize and explain the focus of eight security domains
- Identify the steps of risk management
- Describe the CIA triad
- Identify security principles
- Define and describe the purpose of a playbook
- Explain how entry-level security analysts use SIEM dashboards

#### Skill sets:

- Applying the CIA triad to workplace situations
- Analyzing log data
- Identifying the phases of an incident response playbook

---
## Understanding Cybersecurity through CISSP Security Domains

This information sheet combines key points from the course video and additional resources to explain the eight CISSP security domains. Understanding these domains is essential for anyone interested in cybersecurity, especially security analysts.

**CISSP Security Domains**

These eight domains categorize essential security practices that organizations use to protect their data and assets. Each domain plays a role in an organization's overall security posture, which is its ability to defend itself against threats and adapt to changing security landscapes.

**Domain 1: Security and Risk Management**

- **Focus:** Defining security goals (e.g., protecting personal data), reducing security risks, ensuring compliance with regulations, maintaining operations during security incidents, and acting ethically.
- **Example:** An organization might have a security goal of protecting customer information like names and addresses (Personally Identifiable Information or PII). They may also have a policy requiring employees to report suspicious activity to minimize risks.
- **Key Areas:**
    - **Security Goals and Objectives:** What do you want to achieve with security (e.g., protect data, ensure system availability)?
    - **Risk Mitigation:** How will you reduce the impact of security risks (e.g., backups, security awareness training)?
    - **Compliance:** Following internal rules, external regulations, and industry standards.
    - **Business Continuity:** Maintaining operations during disruptions (e.g., having backup plans for data and systems).
    - **Legal Regulations:** Understanding and following laws related to data privacy and security.

**Domain 2: Asset Security**

- **Focus:** Protecting digital and physical assets, including data storage, maintenance, retention, and destruction.
- **Example:** Ensuring proper disposal of old hard drives to prevent data breaches.
- **Key Areas:**
    - Securing data throughout its lifecycle (from creation to destruction).
    - Knowing where data is stored and who has access to it.
    - Having policies for data handling (storage, transfer, disposal).

**Domain 3: Security Architecture and Engineering**

- **Focus:** Designing and implementing security controls using tools, systems, and processes to protect data.
- **Shared Responsibility:** Everyone in the organization plays a part in security (e.g., reporting suspicious activity).
- **Example:** Encouraging users to report suspicious emails can help identify phishing attempts quickly.
- **Key Areas:**
    - Choosing effective security tools and technologies.
    - Designing secure systems and architectures.
    - Implementing security controls (e.g., firewalls, encryption).
    - Encouraging a culture of security awareness within the organization.

**Domain 4: Communication and Network Security**

- **Focus:** Securing physical networks, wireless communication, and cloud data.
- **Example:** Restricting access to public Wi-Fi or Bluetooth connections to protect employees from insecure networks.
- **Key Areas:**
    - Securing wired and wireless networks.
    - Protecting data during transfer (e.g., using encryption).
    - Securing cloud-based data and applications.

**Domain 5: Identity and Access Management (IAM)**

- **Focus:** Controlling access to data and resources by verifying user identities and granting appropriate permissions.
- **Least Privilege:** Users only have access to what they need to perform their jobs.
- **Example:** Customer service representatives may only need to view a customer's phone number to resolve an issue, not their entire account history.
- **Key Areas:**
    - Verifying user identities ( usernames, passwords, multi-factor authentication).
    - Granting access based on job roles and responsibilities (least privilege).
    - Monitoring user activity to ensure proper data use.

**Domain 6: Security Assessment and Testing**

- **Focus:** Identifying weaknesses in an organization's security posture through testing, data analysis, and security audits.
- **Example:** Regularly testing security controls to identify vulnerabilities that attackers could exploit.
- **Key Areas:**
    - Conducting security control testing to assess existing controls.
    - Collecting and analyzing data to identify potential threats and risks.
    - Performing security audits to ensure overall security posture.

**Domain 7: Security Operations**

- **Focus:** Responding to security incidents and taking preventative measures to avoid future attacks.
- **Incident Response:**
    - Investigate security incidents quickly to minimize damage.
    - Neutralize active attacks and prevent them from escalating.
    - Collect evidence to identify how, when, and why the breach occurred (digital forensics).
    - Implement preventative measures to avoid similar attacks in the future.
- **Key Areas:**
    - Having a plan for responding to security incidents.
    - Investigating security incidents to identify the root cause.
    - Taking steps to prevent future incidents.

**Domain 8: Software Development Security**

- **Focus:** Building secure applications by following secure coding practices throughout the software development lifecycle (SDLC).
- **Secure Development Lifecycle (SDLC):** Efficient process for developing software that integrates security at every stage.
- **Example:** Performing security reviews during design, development, testing, and deployment phases to identify and fix vulnerabilities early on.
- **Key Areas:**
    - Writing secure code using secure coding practices.
    - Integrating security reviews throughout the SDLC.
    - Building security into the software design from the beginning.

**Benefits of Understanding CISSP Security Domains**

- **Improved Security Posture:** By understanding these domains, you can see how they work together to create a strong overall security posture for an organization.
- **Essential Role of Security Teams:** Security teams play a critical role in protecting an organization's sensitive information by implementing these domains effectively.

**Additional Notes:**

- CISSP (Certified Information Systems Security Professional) is a globally recognized cybersecurity certification.
- Information Security (InfoSec) refers to the practices and processes used to secure information.
- There are many design principles used in security architecture and engineering, which will be covered in more detail later in the course.

---
## Cybersecurity Study Notes: Threats, Risks, and Vulnerabilities

This section focuses on how to manage risks associated with cybersecurity threats and vulnerabilities. Understanding these concepts is crucial for anyone entering the cybersecurity field, especially security analysts.

**What are We Protecting?**

- Organizations have valuable assets, both digital (data) and physical (equipment, buildings).
- Examples of digital assets: employee/customer data (Social Security numbers, birthdates), financial information.
- Examples of physical assets: computers, servers, buildings.

**Risk Management: Protecting Our Assets**

- The goal of risk management is to safeguard these assets from harm.
    
- There are different ways to handle risks:
    
    - **Acceptance:** Live with the risk if the cost of fixing it is too high.
    - **Avoidance:** Don't do things that carry the risk (e.g., not using a specific program if it's known to have security issues).
    - **Transfer:** Pay an insurance company to take on the risk.
    - **Mitigation:** Reduce the impact of the risk (e.g., by installing security software).
- Frameworks like NIST RMF and HITRUST help organizations implement risk management processes.
    

**Common Threats, Risks, and Vulnerabilities**

- **Threats:** Events or situations that could harm assets.
    - Examples: disgruntled employees (insider threats), hackers trying to steal data (advanced persistent threats or APTs).
- **Risks:** The chance of a threat happening and causing harm.
    - Example: The risk of a data breach due to outdated software (legacy systems). Factors affecting risk include:
        - **External threats:** Hackers, natural disasters.
        - **Internal threats:** Careless employees, data breaches caused by insiders.
        - **Legacy systems:** Outdated systems with unpatched vulnerabilities.
        - **Multiparty risks:** Sharing data with vendors who might have weak security.
        - **Software compliance/licensing:** Using outdated or unpatched software.
- **Vulnerabilities:** Weaknesses in systems that attackers can exploit.
    - Examples: unpatched software vulnerabilities (ProxyLogon, ZeroLogon, Log4Shell), weaknesses in authentication protocols (PetitPotam).

**Security Analyst's Role: Mitigating Risks**

- Security analysts help identify and address vulnerabilities before they can be exploited by attackers.
- This might involve tasks like:
    - Regularly monitoring systems for vulnerabilities.
    - Applying security patches and updates promptly.
    - Staying up-to-date on current threats and attacker tactics.

**Resources for Further Learning**

- NIST National Vulnerability Database: [https://nvd.nist.gov/vuln](https://nvd.nist.gov/vuln)
- CISA Known Exploited Vulnerabilities Catalog: [https://www.cisa.gov/known-exploited-vulnerabilities-catalog](https://www.cisa.gov/known-exploited-vulnerabilities-catalog)
- OWASP Top 10 Web Application Security Risks: [https://owasp.org/www-project-top-ten/](https://owasp.org/www-project-top-ten/)

**Remember:** Constant vigilance is key in cybersecurity. By understanding and managing risks, you can help organizations protect their valuable assets and information.

---
## Glossary terms from module 1

**Assess:** The fifth step of the NIST RMF that means to determine if established controls are implemented correctly

**Authorize:** The sixth step of the NIST RMF that refers to being accountable for the security and privacy risks that may exist in an organization

**Business continuity:** An organization's ability to maintain their everyday productivity by establishing risk disaster recovery plans

**Categorize:** The second step of the NIST RMF that is used to develop risk management processes and tasks

**External threat:** Anything outside the organization that has the potential to harm organizational assets

**Implement:** The fourth step of the NIST RMF that means to implement security and privacy plans for an organization

**Internal threat:** A current or former employee, external vendor, or trusted partner who poses a security risk

**Monitor**: The seventh step of the NIST RMF that means be aware of how systems are operating

**Prepare:** The first step of the NIST RMF related to activities that are necessary to manage security and privacy risks before a breach occurs

**Ransomware:** A malicious attack where threat actors encrypt an organization’s data and demand payment to restore access 

**Risk:** Anything that can impact the confidentiality, integrity, or availability of an asset

**Risk mitigation:** The process of having the right procedures and rules in place to quickly reduce the impact of a risk like a breach

**Security posture:** An organization’s ability to manage its defense of critical assets and data and react to change

**Select**: The third step of the NIST RMF that means to choose, customize, and capture documentation of the controls that protect an organization

**Shared responsibility:** The idea that all individuals within an organization take an active role in lowering risk and maintaining both physical and virtual security

**Social engineering:** A manipulation technique that exploits human error to gain private information, access, or valuables 

**Vulnerability:** A weakness that can be exploited by a threat


---
