# Safeguard Information

## Security Controls

### Introduction
In today’s digital age, information is omnipresent, making it imperative for organizations to implement effective security controls to safeguard information from theft or exposure. Security controls are measures designed to mitigate specific security risks, encompassing various tools that protect assets before, during, and after an event.

### Types of Security Controls
Security controls are categorized into three main types: technical, operational, and managerial.

#### 1. Technical Controls
Technical controls involve technologies used to protect assets.

| Control Type         | Examples                                                                 |
|----------------------|--------------------------------------------------------------------------|
| **Technical Controls** | Encryption, authentication systems, firewalls, anti-malware software     |

#### 2. Operational Controls
Operational controls pertain to maintaining the day-to-day security environment, typically performed by people.

| Control Type          | Examples                                                                            |
|-----------------------|-------------------------------------------------------------------------------------|
| **Operational Controls** | Awareness training, incident response, security patrols, access management         |

#### 3. Managerial Controls
Managerial controls focus on how technical and operational controls reduce risk.

| Control Type           | Examples                                             |
|------------------------|------------------------------------------------------|
| **Managerial Controls** | Policies, standards, procedures, risk assessments    |

### Information Privacy and Security Policy
Organizations’ security policies define the necessary controls to achieve their security goals, with a strong emphasis on information privacy. Information privacy is about protecting data from unauthorized access and distribution, ensuring the right to choose how private information is shared.

### Example Scenario
Consider using a travel app to book a flight:

- **Personal Information Entered:** Name, email, credit card number
- **Access Expectation:** Airline company accesses this information to complete the reservation.

#### Principle of Least Privilege
Not everyone at the company should have access to your information. For instance:
- **Marketing Department:** No access to credit card information.
- **Customer Support Agent:** Access only during reservation assistance.

Security controls limit access based on the user and situation, adhering to the principle of least privilege.

### Data Owners and Data Custodians
Effective security controls distinguish between data owners and data custodians.

| Role              | Description                                                                                           |
|-------------------|-------------------------------------------------------------------------------------------------------|
| **Data Owner**    | Decides who can access, edit, use, or destroy information. Can be straightforward or involve multiple owners (e.g., intellectual property). |
| **Data Custodian**| Responsible for safe handling, transport, and storage of information. Includes people, organizations, and systems.                            |

### Additional Considerations
Data is an asset requiring proper classification and handling. As we continue, we'll explore more security controls that facilitate this process.

### Key Takeaways
- **Security Controls:** Measures to mitigate security risks, categorized into technical, operational, and managerial types.
- **Information Privacy:** Ensures unauthorized access and distribution are prevented.
- **Principle of Least Privilege:** Limits access based on the user’s role and situation.
- **Data Owners vs. Data Custodians:** Differentiates responsibilities for managing and safeguarding information.

## Principle of Least Privilege

### Introduction
Security controls are crucial for keeping sensitive data private and safe. One of the most common controls is the principle of least privilege (PoLP). PoLP is a security concept where a user is granted the minimum level of access and authorization required to complete a task or function.

### Importance of Least Privilege
Least privilege supports the confidentiality, integrity, and availability (CIA) triad of information security. It reduces risk by:

- Limiting access to sensitive information
- Reducing accidental data modification, tampering, or loss
- Supporting system monitoring and administration

By connecting specific resources to specific users and placing limits on what they can do, least privilege minimizes the likelihood of successful attacks.

### Determining Access and Authorization
To implement least privilege effectively, access and authorization must be determined by asking:
1. Who is the user?
2. How much access do they need to a specific resource?

Users can be people (customers, employees, vendors), devices, or software connected to the business network. Each user should have their own account, managed within the organization’s directory service.

#### Common Types of User Accounts
| Account Type       | Description                                                                                             |
|--------------------|---------------------------------------------------------------------------------------------------------|
| **Guest Accounts**   | Provided to external users like customers, clients, contractors, or business partners.                  |
| **User Accounts**    | Assigned to staff based on their job duties.                                                            |
| **Service Accounts** | Granted to applications or software needing to interact with other software on the network.              |
| **Privileged Accounts** | Have elevated permissions or administrative access.                                                   |

### Implementing Least Privilege
- Determine a baseline access level for each account type.
- Access levels may change based on current tasks. For example, a customer support representative should only access your data while assisting you.
- Consistently monitor and audit user accounts to maintain least privilege.

### Auditing Account Privileges
Setting up user accounts and assigning appropriate privileges is the first step. Periodic auditing is essential to keep systems secure.

#### Common Approaches to Auditing User Accounts
| Audit Type           | Description                                                                                             |
|----------------------|---------------------------------------------------------------------------------------------------------|
| **Usage Audits**       | Review which resources each account is accessing and the actions taken. Identify if permissions can be revoked. |
| **Privilege Audits**   | Assess if a user's role aligns with the resources they access to prevent privilege creep.                |
| **Account Change Audits** | Check logs for suspicious activity like multiple password change attempts. Ensure changes are authorized.      |

Most directory services can alert system administrators to suspicious activity, enhancing security.

### Key Takeaways
- **Principle of Least Privilege (PoLP):** Reduces the risk of unauthorized access by granting minimum necessary access.
- **User Accounts:** Properly configured and regularly audited user accounts are essential for maintaining security.
- **Audits:** Conducting usage, privilege, and account change audits helps maintain the confidentiality, integrity, and availability of information.

## The Data Lifecycle

### Introduction
Organizations handle a vast amount of data that must be kept private. Data can be vulnerable whether at rest, in use, or in transit. Information should always be kept private by limiting access and authorization.

### The Data Lifecycle
The data lifecycle is a model that maps data vulnerabilities and plays a crucial role in maintaining the confidentiality, integrity, and availability (CIA) triad. It influences policies and the technologies used to make information accessible. The lifecycle consists of five stages:

| Stage    | Description                                                                 |
|----------|-----------------------------------------------------------------------------|
| **Collect** | Data is gathered from various sources.                                      |
| **Store**   | Data is stored in databases or other storage systems.                       |
| **Use**     | Data is accessed and utilized for various operations.                      |
| **Archive** | Data is moved to long-term storage for retention.                           |
| **Destroy** | Data is securely deleted or destroyed when it is no longer needed.          |

![Five stages of the data lifecycle: collection, storage, usage, archival, and destruction.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/Sx9FANHTQYK_Emc4x9cBsA_4dad354c13cc4354b9caef4a1b05d2f1_CS_R-091_ive-stages-of-the-data-lifecycle.png?expiry=1715990400000&hmac=F9bFocfEm7RVmjITXune9cpxM7wOrisj695iwLireWY)

### Data Governance
Data governance is a structured approach to managing information. It includes policies to keep data private, accurate, available, and secure throughout its lifecycle. Effective data governance relies on people and assigns specific roles:

| Role           | Description                                                                                              |
|----------------|----------------------------------------------------------------------------------------------------------|
| **Data Owner**    | Decides who can access, edit, use, or destroy their information.                                        |
| **Data Custodian**| Responsible for safe handling, transport, and storage of information.                                   |
| **Data Steward**  | Maintains and implements data governance policies set by an organization.                               |

### Protecting Data at Every Stage
Security plans include a data governance policy that outlines how information will be managed. These policies define procedures and place limits on data access. Security professionals, especially data custodians, play a key role in ensuring data isn’t damaged, stolen, or misused.

### Legally Protected Information
Data can represent personal thoughts, actions, and choices. Protecting a person's data privacy decisions is crucial. Different types of information have specific regulatory requirements:

| Type  | Description                                                                                                     |
|-------|-----------------------------------------------------------------------------------------------------------------|
| **PII**  | Personally identifiable information used to infer an individual's identity, such as contact or location data.   |
| **PHI**  | Protected health information regulated by laws like HIPAA in the U.S. and GDPR in the EU, relating to health data. |
| **SPII** | Sensitive personally identifiable information requiring stricter handling, such as bank account numbers.        |

### Key Takeaways
- **Data Governance:** Essential for managing and protecting data throughout its lifecycle.
- **Data Custodians:** Play a crucial role in maintaining data security and privacy.
- **Legal Requirements:** Understanding and adhering to regulations for PII, PHI, and SPII is vital.

Effective data management and security controls are fundamental for protecting information in an increasingly digital world.

## Information Privacy: Regulations and Compliance

### Introduction
Security and privacy are closely related concepts. People have the right to control how their personal data is collected and used, and organizations have a responsibility to protect this information from being compromised or misused. As a security professional, you will be involved in these efforts.

### Information Security vs. Information Privacy
- **Information Privacy:** Protection from unauthorized access and distribution of data. Provides people with control over their personal information and how it is shared.
- **Information Security (InfoSec):** Keeping data in all states away from unauthorized users. Protects people's choices and keeps their information safe from potential threats.

Example: A retail company collecting customer data for marketing must disclose how this data will be used and provide an opt-out option. Implementing security controls ensures this data remains private and secure.

### Why Privacy Matters in Security
- **Late 1990s:** Companies began storing and using data for business purposes, leading to concerns about data privacy and security.
- **Global Conversation:** Organizations became more transparent and implemented more security measures to protect data privacy.
- **Data Vulnerability:** The more data collected, stored, and used, the more vulnerable it is to breaches and threats.

### Notable Privacy Regulations
Regulations are rules set by governments or authorities to control how something is done. Privacy regulations protect users from having their information collected, used, or shared without consent.

| Regulation | Description                                                                                                           |
|------------|-----------------------------------------------------------------------------------------------------------------------|
| **GDPR**   | Developed by the EU, GDPR gives data owners control over their personal information. Applies to any business handling data of EU citizens. |
| **PCI DSS**| Security standards formed by major financial organizations to secure credit and debit card transactions against theft and fraud. |
| **HIPAA**  | U.S. law requiring the protection of sensitive patient health information. Prohibits disclosure without knowledge and consent. |

### Security Assessments and Audits
Compliance with regulations is essential for businesses. This involves a continual process of security audits and assessments.

| Evaluation Type       | Description                                                                                           |
|-----------------------|-------------------------------------------------------------------------------------------------------|
| **Security Audit**    | Review of security controls, policies, and procedures against a set of expectations. Conducted less frequently, about once per year. |
| **Security Assessment** | Check to determine how resilient current security implementations are against threats. Conducted more frequently, every three to six months. |

Example: If MFA is required by a regulation, an audit checks for compliance. An assessment might reveal weak passwords, leading to the decision to enable MFA for all user accounts.

### Key Takeaways
- **Privacy and Governance:** Protecting and governing the use of sensitive data is essential for maintaining customer trust.
- **Assessments and Audits:** Evaluate gaps in security plans. Regular assessments and audits ensure effective protection of privacy.
- **Consequences:** Overlooking or delaying assessment results can lead to fines or data breaches.

By understanding and implementing these privacy regulations and compliance measures, security professionals can help organizations protect sensitive data and maintain robust security practices.

---

# Encryption methods

## Fundamentals of Cryptography

### Introduction
The internet is an open, public system with a vast amount of data flowing through it. Some information, such as personally identifiable information (PII), needs to be kept private. PII includes details that can infer an individual's identity, like names, medical and financial information, photos, emails, or fingerprints.

### Cryptography: The Basics
Maintaining the privacy of PII online is challenging and requires the right security controls. Cryptography is a primary security control that protects information by transforming it into a form that unintended readers cannot understand. The process involves two steps: encryption to hide the information and decryption to unhide it.

### Encryption and Decryption
- **Plaintext:** Original, readable form of data.
- **Ciphertext:** Unreadable form of data after encryption.

Example: Sending an email to a friend:
1. **Encryption:** Converts plaintext into ciphertext.
2. **Decryption:** Converts ciphertext back into plaintext.

### Historical Cryptography: Caesar's Cipher
One of the earliest cryptographic methods is Caesar's cipher, named after Julius Caesar. This simple algorithm shifts letters in the Roman alphabet forward by a fixed number of spaces. 

| Original | Encrypted (Shift 3) |
|----------|---------------------|
| A        | D                   |
| B        | E                   |
| C        | F                   |
| ...      | ...                 |
| hello    | khoor               |

### Cryptographic Key
A cryptographic key decrypts ciphertext. In Caesar's cipher, the key indicates the number of shifts. For example, a shift of 3 encrypts "hello" as "khoor."

### Modern Cryptography
Caesar's cipher is not widely used today due to its flaws:
1. **Brute Force Attack:** Simple trial-and-error process of shifting letters 26 ways in the English alphabet.
2. **Single Key Dependence:** If the key is lost or stolen, the information can be easily accessed.

Proper management of cryptographic keys is crucial:
- **Secure Storage:** Do not store keys in public places.
- **Separate Sharing:** Share keys separately from the information they decrypt.

### Moving to Modern Algorithms
Modern algorithms are more complex and secure than Caesar's cipher. They address the limitations of simple ciphers and provide robust methods for protecting information online.

### Key Takeaways
- **Cryptography:** Essential for protecting PII by transforming data into unreadable forms.
- **Encryption and Decryption:** Critical processes for hiding and revealing information.
- **Historical Example:** Caesar's cipher illustrates basic encryption concepts but is outdated due to its simplicity.
- **Modern Security:** Advanced algorithms and proper key management are necessary for effective cryptographic security.

By understanding the fundamentals of cryptography, security professionals can better protect sensitive information in today's digital world.

## Public Key Infrastructure

### Introduction
Public Key Infrastructure (PKI) is an encryption framework that secures online information exchange. It ensures fast, easy, and secure access to information by managing encryption keys.

### How PKI Works
PKI is a two-step process involving asymmetric and symmetric encryption.

#### Asymmetric Encryption
- **Definition:** Uses a pair of keys, public and private, for encryption and decryption.
- **Public Key:** Can be shared and used to add items to a secure "box" but not remove them.
- **Private Key:** Kept by the owner to decrypt and access the contents of the "box".

| Key Type    | Function                            | Security                              |
|-------------|-------------------------------------|---------------------------------------|
| **Public Key**  | Encrypts data (adds items to the "box")   | Can be shared widely                   |
| **Private Key** | Decrypts data (removes items from the "box") | Kept secret, only with the owner        |

- **Strengths:** Secure for information exchange.
- **Weakness:** Slower due to two-key system.

#### Symmetric Encryption
- **Definition:** Uses a single secret key for both encryption and decryption.
- **Key:** Same key is used to lock and unlock the "box".

| Key Type        | Function                           | Security                              |
|-----------------|------------------------------------|---------------------------------------|
| **Secret Key**  | Encrypts and decrypts data          | Shared with authorized users only     |

- **Strengths:** Faster and simpler.
- **Weakness:** Less secure due to single key use.

### Combining Asymmetric and Symmetric Encryption
PKI can use both encryption methods depending on the priority of speed or security. For instance:
- **Asymmetric Encryption:** Used to establish secure connections initially.
- **Symmetric Encryption:** Used for faster communication thereafter.

### Establishing Trust
A common vulnerability in encryption is establishing trust between sender and receiver. PKI addresses this by using digital certificates.

#### Digital Certificates
- **Definition:** Files that verify the identity of a public key holder.
- **Purpose:** Establish trust in online communications.

| Component               | Function                                                       |
|-------------------------|----------------------------------------------------------------|
| **Certificate Authority (CA)** | Verifies and authenticates entities requesting certificates     |
| **Digital Certificate** | Contains encrypted data and CA’s digital signature              |

### Example of Digital Certificate Creation
1. **Domain Registration:** Business registers domain with hosting company.
2. **Information Sent to CA:** Hosting company sends business details and public key to CA.
3. **Verification:** CA verifies the company’s identity using the provided data.
4. **Creation of Certificate:** CA encrypts the verified data and adds its digital signature.
5. **Digital Certificate Issued:** Business receives the digital certificate to establish trust.

### Key Takeaways
- **Public Key Infrastructure (PKI):** Manages encryption keys for secure information exchange.
- **Asymmetric and Symmetric Encryption:** Used for security and speed, respectively.
- **Digital Certificates:** Establish trust in online communications by verifying identities.
- **Role of Certificate Authorities (CAs):** Authenticate and issue digital certificates to maintain trust.

## Symmetric and Asymmetric Encryption

### Introduction
Encryption transforms data from a readable format to an encoded format to keep it private and secure. Public key infrastructure (PKI) secures online information exchanges, and ciphers are algorithms that encrypt information. This guide compares symmetric and asymmetric encryption and discusses well-known algorithms for each.

### Types of Encryption
There are two main types of encryption:

#### Symmetric Encryption
- **Definition:** Uses a single secret key for both encryption and decryption.
- **Mechanism:** Sender and receiver must know the secret key to lock or unlock the cipher.

#### Asymmetric Encryption
- **Definition:** Uses a public and private key pair for encryption and decryption.
- **Mechanism:** Public key encrypts data, and the private key decrypts it. The private key is only given to authorized users.

### The Importance of Key Length
Ciphers are vulnerable to brute force attacks, which involve trying every possible key until the correct one is found. Longer key lengths are more secure but result in slower processing times. Balancing fast data communication and security is crucial.

### Approved Algorithms
Many web applications use a combination of symmetric and asymmetric encryption to balance user experience with safeguarding information.

#### Symmetric Algorithms
| Algorithm        | Description                                                                                                     |
|------------------|-----------------------------------------------------------------------------------------------------------------|
| **Triple DES (3DES)** | A block cipher that converts plaintext into ciphertext in “blocks.” Generates 192-bit keys.                   |
| **Advanced Encryption Standard (AES)** | One of the most secure symmetric algorithms today. Generates keys of 128, 192, or 256 bits.   |

#### Asymmetric Algorithms
| Algorithm               | Description                                                                                               |
|-------------------------|-----------------------------------------------------------------------------------------------------------|
| **Rivest Shamir Adleman (RSA)** | Produces a public and private key pair. Key sizes are 1,024, 2,048, or 4,096 bits. Protects highly sensitive data. |
| **Digital Signature Algorithm (DSA)** | Generates key lengths of 2,048 bits. Complements RSA in public key infrastructure.              |

### Generating Keys
Organizations implement these algorithms using tools like OpenSSL, an open-source command line tool that generates public and private keys. OpenSSL is commonly used to verify digital certificates exchanged as part of PKI.

**Note:** OpenSSL disclosed a vulnerability known as the Heartbleed bug in 2014, which was later patched. Secure versions of OpenSSL are now widely used.

### Obscurity is Not Security
According to Kerchoff’s principle, cryptographic algorithms should be secure even if all details, except the private key, are known. Encryption systems must be proven unbreakable to be considered secure. Custom algorithms that rely on secrecy often fail once made public.

**Pro Tip:** A cryptographic system should not require secrecy around its working mechanisms to be secure.

### Encryption in Practice
Companies use both symmetric and asymmetric encryption, often in combination. For example:
- **Asymmetric Encryption:** Secures small blocks of data (e.g., usernames and passwords) during login requests.
- **Symmetric Encryption:** Used for the rest of the web session for speed.

### Legal Requirements
Regulations like the Federal Information Processing Standards (FIPS 140-3) and the General Data Protection Regulation (GDPR) require data encryption to ensure compliance and demonstrate responsible data handling.

### Key Takeaways
- **Symmetric Encryption:** Uses a single secret key.
- **Asymmetric Encryption:** Uses a public and private key pair.
- **Key Length:** Longer keys are more secure but slower.
- **Compliance:** Encryption is required to meet legal standards and protect data.

## Non-Repudiation and Hashing

### Introduction
Security professionals focus on vulnerabilities to stay ahead of threats. We've explored encryption forms that produce keys shared during communication, which can be vulnerable to loss or theft. Another security control that addresses this weakness is hashing.

### Hash Functions
A hash function is an algorithm that produces a code that can't be decrypted. Unlike asymmetric and symmetric algorithms, hash functions are one-way processes that do not generate decryption keys. Instead, they produce a unique identifier known as a hash value or digest.

#### Example:
Imagine a company has an internal application stored in a shared drive. After passing through a hashing function, the program receives its hash value. If an attacker replaces the program with a modified version, even one line of code change will result in a different hash value. Comparing hash values helps validate that the programs are different.

### Uses of Hashes in Security
- **Integrity Verification:** Hashes determine the integrity of files and applications.
- **Non-Repudiation:** Ensures that the authenticity of information can't be denied.

### Data Integrity
Data integrity relates to the accuracy and consistency of information. Non-repudiation ensures that the authenticity of information can't be denied. Hash functions are critical security controls that make proven data integrity possible.

### Generating and Comparing Hash Values
Security analysts use hash values to compare files or applications against known malicious files. Here's how to generate a hash value using the Linux command line with the SHA-256 algorithm:

1. Launch a shell.
2. Type the name of the hashing algorithm (e.g., `sha256`).
3. Enter the file name to hash (e.g., `newfile.txt`).
4. Press Enter to generate the unique hash value.

### Practical Tools
Security practitioners use tools like VirusTotal to analyse suspicious files, domains, IPs, and URLs. VirusTotal allows comparison of hash values with known online viruses.

### Importance of Hash Functions
Hash functions ensure that even the slightest change in input results in a totally different hash value. This design helps with non-repudiation by providing a quick and easy way to compare input and output values and validate data integrity.

### Key Takeaways
- **Hash Functions:** Produce non-decryptable codes (hash values) to ensure data integrity and non-repudiation.
- **Integrity Verification:** Used to compare files and applications against known malicious files.
- **Non-Repudiation:** Ensures the authenticity of information can't be denied.
- **Practical Tools:** Tools like VirusTotal are used to analyse and compare hash values with known viruses.

## The Evolution of Hash Functions

### Introduction
Hash functions are crucial controls in a company's security strategy, used for authentication and non-repudiation. Hash functions convert information into unique values to determine its integrity.

### Origins of Hashing
Hash functions date back to the early days of computing, initially created for quick data searching. These algorithms represent data of any size as small, fixed-size values or digests.

#### Example: MD5
- **Developer:** Professor Ronald Rivest, MIT, early 1990s.
- **Function:** Converts data into a 128-bit value.
- **Purpose:** Verify file integrity over a network.

#### Bit and Hash Values
- **Bit:** The smallest unit of data measurement in a computer (0 or 1).
- **Hash Value:** A string of characters generated from input data. Any change in the input results in a different hash value.

### Hash Collisions
All hash functions map any input into a fixed-size value. Due to finite output possibilities, different inputs can produce the same hash value, known as a hash collision.

- **Vulnerability:** MD5 values are 32 characters long, making them susceptible to collisions.
- **Impact:** Collisions can allow attackers to impersonate authentic data.

### Next-Generation Hashing
To reduce the risk of hash collisions, functions that generate longer values were developed, known as Secure Hashing Algorithms (SHAs), approved by NIST.

#### SHA Family of Algorithms
| Algorithm   | Digest Size (bits) |
|-------------|--------------------|
| **SHA-1**   | 160                |
| **SHA-224** | 224                |
| **SHA-256** | 256                |
| **SHA-384** | 384                |
| **SHA-512** | 512                |

### Secure Password Storage
Passwords stored in databases must be protected from attackers. Hashing passwords adds a layer of security as hash values cannot be reversed.

### Rainbow Tables
A rainbow table contains pre-generated hash values and their associated plaintext. Attackers can use these tables to compare stolen hashes and find matching plaintext values.

### Adding Some “Salt”
**Salting** strengthens hash functions by adding a random string of characters to data before hashing, creating more unique hash values.

#### Example: Salting Passwords
- **Without Salt:** Multiple entries of the password "password" will have the same hash.
- **With Salt:** Each entry will have a different hash value, preventing rainbow table attacks.

### Key Takeaways
- **Hash Functions:** Validate data integrity and reduce data breach chances.
- **MD5 Vulnerabilities:** Shorter keys like MD5 are more susceptible to rainbow table attacks.
- **SHA Algorithms:** Provide longer, more secure hash values.
- **Salting:** Enhances security by creating unique hash values, even for identical inputs.

---
# Authentication, authorization, and accounting

## Access Controls and Authentication Systems

### Introduction
Protecting data is a fundamental aspect of security controls. Hashing and encryption are powerful tools but managing who or what has access to information is also crucial. Access controls are security controls that manage access, authorization, and accountability of information. When done well, they maintain data confidentiality, integrity, and availability.

### Access Control Functions
Access control systems are commonly broken down into three related functions: authentication, authorization, and accounting. Each control has its own protocols and systems.

### Authentication
Authentication systems are access controls that verify the identity of anything attempting to access information.

#### Factors of Authentication
Authentication responses can be based on three factors:

| Factor         | Description                                                            | Example                                         |
|----------------|------------------------------------------------------------------------|-------------------------------------------------|
| **Knowledge**  | Something the user knows                                               | Password, security question                      |
| **Ownership**  | Something the user possesses                                           | One-time passcode (OTP) sent via text or email   |
| **Characteristic** | Something the user is                                              | Biometrics (fingerprint scan, facial recognition)|

The information provided during authentication must match the information on file for access to be granted. If the credentials do not match, access is denied.

#### Single Sign-On (SSO)
Single sign-on (SSO) combines several different logins into one, establishing a user's identity once and allowing faster access to company resources. While SSO is convenient, it presents a vulnerability when used alone.

#### Multi-Factor Authentication (MFA)
Multi-factor authentication (MFA) requires a user to verify their identity in two or more ways to access a system or network. MFA combines independent credentials like knowledge and ownership to strengthen security.

| Authentication Method | Description                                                                                  |
|-----------------------|----------------------------------------------------------------------------------------------|
| **Single Sign-On (SSO)**  | Combines several logins into one, simplifying the authentication process                     |
| **Multi-Factor Authentication (MFA)** | Requires multiple credentials, enhancing security by combining different authentication factors |

SSO and MFA are often used together to provide both convenience and security.

### Key Takeaways
- **Access Controls:** Manage access, authorization, and accountability of information.
- **Authentication:** Verifies the identity of users attempting to access information.
- **Factors of Authentication:** Include knowledge, ownership, and characteristic.
- **Single Sign-On (SSO):** Simplifies authentication but can be vulnerable when used alone.
- **Multi-Factor Authentication (MFA):** Combines multiple authentication factors to enhance security.
- **Combination:** SSO and MFA are used together to ensure both convenient and secure access.

## The Rise of SSO and MFA

### Introduction
Most companies use authentication systems to keep their data secure. Usernames and passwords are commonly used, but are they enough? Managing user access and authorization is crucial for information security.

### Factors of Authentication
Previously, we learned about the three factors of authentication:
1. **Knowledge:** Something the user knows (e.g., password).
2. **Ownership:** Something the user possesses (e.g., one-time passcode).
3. **Characteristic:** Something the user is (e.g., biometrics).

Single sign-on (SSO) and multi-factor authentication (MFA) are popular technologies for implementing these authentication factors.

### A Better Approach to Authentication

#### Single Sign-On (SSO)
SSO combines several logins into one. Companies adopt SSO for three main reasons:
1. **Improves User Experience:** Eliminates the need to remember multiple usernames and passwords.
2. **Lowers Costs:** Streamlines the management of connected services.
3. **Enhances Security:** Reduces the number of access points for attackers.

SSO emerged in the mid-1990s to combat password fatigue, the tendency to reuse passwords across services.

### How SSO Works
SSO automates trust establishment between a user and a service provider using encrypted access tokens exchanged between identity providers and service providers.

![One user connects to multiple applications with one access token.](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/IaWbLEaURvGv7k6ZSOjbRg_c43ff4ecdca147cca2f5351aaaa917f1_image2.png?expiry=1715990400000&hmac=P5G5cRbWqri15Y9cxpC2Ro_pnSk7q-nMgHegdROCmB4)

#### Authentication Protocols
| Protocol | Use Case                          |
|----------|-----------------------------------|
| **LDAP** | Transmitting information on-premises |
| **SAML** | Transmitting information off-premises (cloud) |

**Note:** LDAP and SAML are often used together.

### Limitations of SSO
While SSO offers many benefits, relying solely on usernames and passwords is not always secure. A lost or stolen password can expose information across multiple services.

### MFA to the Rescue

#### Multi-Factor Authentication (MFA)
MFA requires users to verify their identity in two or more ways. It strengthens authentication by requiring multiple proofs of identity.

#### Authentication Factors
| Factor                    | Example                                     |
|---------------------------|---------------------------------------------|
| **Something a user knows** | Username and password                        |
| **Something a user has**   | One-time passcode (OTP) sent via SMS         |
| **Something a user is**    | Physical characteristics (fingerprints, facial scans) |

### Strengthening Authentication
MFA builds on the benefits of SSO by requiring additional forms of identification. This is especially effective in cloud environments, where it can be difficult to ensure that users are not threat actors.

### Key Takeaways
- **SSO:** Improves user experience, lowers costs, and enhances security by reducing access points.
- **MFA:** Adds multiple layers of authentication, making it harder for unauthorized users to access systems.
- **Combination:** Implementing both SSO and MFA improves security without sacrificing user experience.

## The Mechanisms of Authorization

### Introduction
Access control is as much about authorization as it is about authentication. One of the most important functions of access controls is assigning responsibility for systems and processes. Authorization mechanisms determine what authenticated users are allowed to do.

### Authorization and Authentication
While authentication validates who the user is, authorization determines what the user is allowed to do. Both principles work closely together within the authentication, authorization, and accounting (AAA) framework to protect private information.

### Principles of Authorization
- **Principle of Least Privilege:** Access to information only lasts as long as needed.
- **Separation of Duties:** Users should not have authorization levels that allow them to misuse a system, reducing the risk of system failures and inappropriate behavior.

### Example of Separation of Duties
A customer service representative should not be authorized to rate their own performance. Similarly, a person authorized to develop and test a security system might overlook its weaknesses.

### Scope of Authorization
Authorization applies to:
- People
- Networks
- Databases
- Processes
- Any other aspect of an organization

### Frequently Used Access Controls
Two common access controls used for securing data over a network are HTTP Basic Auth and OAuth.

#### HTTP Basic Auth
- **Definition:** Technology used to establish a user's request to access a server via hypertext transfer protocol (HTTP).
- **Mechanism:** Sends an identifier every time a user communicates with a webpage.
- **Vulnerability:** Transmits usernames and passwords openly over the network.
- **Secure Alternative:** Most websites use HTTPS (hypertext transfer protocol secure) to prevent exposing sensitive information.

#### OAuth
- **Definition:** Open-standard authorization protocol that shares designated access between applications.
- **Mechanism:** Uses API tokens to verify access between a user and a service provider, avoiding the need to transmit sensitive usernames and passwords.

### API Tokens
- **Definition:** Small blocks of encrypted code containing user information such as identity and site permissions.
- **Function:** OAuth uses API tokens to send and receive access requests securely between servers and user devices.

### Example of OAuth in Action
When authorizing a site to create an account using your Google profile, Google's login protocols remain active, including multi-factor authentication (MFA). API tokens provide an additional layer of encryption, keeping your Google password safe even if another platform is breached.

### Key Takeaways
- **Authorization Mechanisms:** Determine what authenticated users are allowed to do.
- **Principles:** Least privilege and separation of duties help minimize risks.
- **Common Controls:** HTTP Basic Auth and OAuth are examples of authorization tools designed to enhance security.
- **API Tokens:** Secure method for exchanging access information, minimizing risks associated with transmitting sensitive data.

## Why We Audit User Activity

### Introduction
Auditing user activity is an essential function within the authentication, authorization, and accounting (AAA) framework. Accounting involves monitoring access logs to track user activity within a system.

### The Role of Accounting
Accounting involves keeping records of system access, including who accessed the system, when they accessed it, and what resources they used. Security analysts rely heavily on these access logs to identify trends, detect unauthorized access, and investigate security incidents like data breaches.

### Access Logs
Access logs are records of user sessions within a system, capturing the moment a user enters until they leave.

### Sessions and Session IDs
- **Session:** A sequence of network HTTP basic auth requests and responses associated with the same user.
- **Session ID:** A unique token identifying a user and their device during a session. Created at the start of a session and attached to the user until they close their browser or the session times out.

### Session Cookies
- **Definition:** Tokens exchanged between a server and a user's device to validate a session and determine its duration.
- **Purpose:** Ensure safer and more efficient web sessions by preventing the exchange of sensitive information like usernames and passwords.
- **Vulnerability:** Stolen cookies can lead to session hijacking, where attackers impersonate a user by using their session token.

### Session Hijacking
- **Definition:** An event where attackers obtain a legitimate user's session ID to impersonate them.
- **Consequences:** Attackers can steal money, private data, and access additional systems using stolen single sign-on (SSO) credentials.

### Importance of Auditing
- **Detecting Unusual Activity:** Monitoring access logs can reveal unusual activity, indicating potential unauthorized access or data theft.
- **Insight and Safety:** Regular auditing of session logs provides valuable insights that help enhance information security.

### Key Takeaways
- **Accounting:** Involves monitoring and analyzing access logs to track user activity and detect security incidents.
- **Sessions and IDs:** Sessions start with the creation of a session ID and the exchange of session cookies, which ensure secure and efficient user access.
- **Session Hijacking:** A significant threat where attackers use stolen session tokens to impersonate users.
- **Auditing:** Crucial for detecting unusual activity, ensuring the security of user sessions, and protecting sensitive information.

## Identity and Access Management

Security is more than just combining processes and technologies to protect assets. It is about ensuring these processes and technologies create a secure environment supporting a defense strategy. Two fundamental security principles that limit access to organizational resources are:

- **Principle of Least Privilege:** Users are granted the minimum level of access and authorization required to complete a task or function.
- **Separation of Duties:** Users should not be given levels of authorization that allow them to misuse a system.

These principles support each other. Least privilege limits the access an individual receives, while separation of duties divides responsibilities among multiple people to prevent any one person from having too much control.

### Identity and Access Management (IAM)

IAM is a collection of processes and technologies that help organizations manage digital identities. Both AAA and IAM systems are designed to authenticate users, determine their access privileges, and track their activities within a system. These systems ensure the right user is granted access to the right resources at the right time and for the right reasons, as determined by organizational policies and processes.

### Authenticating Users

To ensure the right user is accessing a resource, some form of proof is required. Authentication factors include:
- **Knowledge:** Something the user knows (e.g., password).
- **Ownership:** Something the user possesses (e.g., one-time passcode).
- **Characteristic:** Something the user is (e.g., biometrics).

Common tools for authentication include:
- **Single Sign-On (SSO):** Combines several logins into one.
- **Multi-Factor Authentication (MFA):** Requires a user to verify their identity in two or more ways.

### User Provisioning

User provisioning involves creating and maintaining a user's digital identity. This process ensures that users have appropriate access rights. Deprovisioning is equally important, removing access rights when they are no longer needed.

### Granting Authorization

If the right user has been authenticated, the network ensures the right resources are made available. Three common frameworks handle this step:

#### Mandatory Access Control (MAC)
- **Definition:** The strictest framework, granting access on a need-to-know basis, typically in government and military environments.
- **Control:** Managed by a central authority.

#### Discretionary Access Control (DAC)
- **Definition:** Allows data owners to decide access levels, such as sharing access in Google Drive.
- **Control:** Managed by the data owner.

#### Role-Based Access Control (RBAC)
- **Definition:** Grants access based on a user's role within an organization.
- **Control:** Managed according to predefined roles.

### Access Control Technologies

Access control technologies offer speed and automation needed by administrators to monitor and modify access rights, decreasing errors and potential risks. Organizations might develop customized access control technologies or license third-party solutions for a comprehensive suite of tools.

### Key Takeaways

- **Principles:** Least privilege and separation of duties are fundamental for controlling access.
- **Frameworks:** IAM and AAA are common frameworks for implementing these principles.
- **Responsibilities:** Security analysts may handle user provisioning and collaborate with IAM or AAA teams to help organizations achieve security objectives.

---
# Glossary terms from module 2

 **Terms and definitions from Course 5, Module 2**

**Access controls:** Security controls that manage access, authorization, and accountability of information

**Algorithm:** A set of rules used to solve a problem

**Application programming interface (API) token:** A small block of encrypted code that contains information about a user

**Asymmetric encryption:** The use of a public and private key pair for encryption and decryption of data   

**Basic auth:** The technology used to establish a user’s request to access a server

**Bit:** The smallest unit of data measurement on a computer

**Brute force attack:** The trial and error process of discovering private information

**Cipher:** An algorithm that encrypts information

**Cryptographic key:** A mechanism that decrypts ciphertext

**Cryptography:** The process of transforming information into a form that unintended readers can’t understand

**Data custodian:** Anyone or anything that’s responsible for the safe handling, transport, and storage of information

**Data owner:** The person that decides who can access, edit, use, or destroy their information

**Digital certificate:** A file that verifies the identity of a public key holder

**Encryption:** The process of converting data from a readable format to an encoded format

**Hash collision:** An instance when different inputs produce the same hash value

**Hash function:** An algorithm that produces a code that can’t be decrypted

**Hash table:** A data structure that's used to store and reference hash values

**Identity and access management (IAM):** A collection of processes and technologies that helps organizations manage digital identities in their environment 

**Information privacy:** The protection of unauthorized access and distribution of data

**Multi-factor authentication (MFA):** A security measure that requires a user to verify their identity in two or more ways to access a system or network

**Non-repudiation:** The concept that the authenticity of information can’t be denied

**OAuth:** An open-standard authorization protocol that shares designated access between applications

**Payment Card Industry Data Security Standards (PCI DSS):** A set of security standards formed by major organizations in the financial industry

**Personally identifiable information (PII):** Any information used to infer an individual's identity

**Principle of least privilege:** The concept of granting only the minimal access and authorization required to complete a task or function

**Protected health information (PHI):** Information that relates to the past, present, or future physical or mental health or condition of an individual

**Public key infrastructure (PKI):** An encryption framework that secures the exchange of online information

**Rainbow table:** A file of pre-generated hash values and their associated plaintext

**Salting:** An additional safeguard that’s used to strengthen hash functions

**Security assessment:** A check to determine how resilient current security implementations are against threats

**Security audit:** A review of an organization's security controls, policies, and procedures against a set of expectations

**Security controls:** Safeguards designed to reduce specific security risks 

**Separation of duties:** The principle that users should not be given levels of authorization that would allow them to misuse a system

**Session:** A sequence of network HTTP basic auth requests and responses associated with the same user

**Session cookie:** A token that websites use to validate a session and determine how long that session should last

**Session hijacking:** An event when attackers obtain a legitimate user’s session ID

**Session ID:** A unique token that identifies a user and their device while accessing a system 

**Single Sign-On (SSO):** A technology that combines several different logins into one

**Symmetric encryption:** The use of a single secret key to exchange information

**User provisioning:** The process of creating and maintaining a user's digital identity