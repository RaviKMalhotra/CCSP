# Notes from the Book - 
CCSP For Dummies—Book + 2 Practice Tests + 100 Flashcards Online, 2nd Edition
978-1-394-21281-1
Arthur J. Deane
CISSP, CCSP

# Strting your CCSP Journey

# Chapter # 2 - Identifying Informatino Security Fundamentals
Overview of this chapter. Following topics will be coverd in this chapter:
1. Bullet Recognizing the pillars of information security
2. Bullet Identifying threats, vulnerabilities, and risks
3. Bullet Discovering how to control access to your data
4. Bullet Exploring encryption
5. Bullet Planning for and responding to security incidents

## Exploring the Pillars of Information Security

### Confidentiality
- > Confidentiality entails limiting access to data to authorized users and systems. In other words, confidentiality prevents exposure of information to anyone
  > who is not an intended party.
  > The concept of confidentiality is closely related to the security best practice of least privilege, which asserts that access to systems or information
  > should only be granted on a need to know basis.

In order to enforce the principle of least privilege and maintain confidentiality, it’s important that you classify (or categorize) data by its sensitivity level. You explore data classification in Chapter 5, but for this chapter, keep in mind that it plays a critical role in ensuring confidentiality. 
You must know what data you own and how sensitive it is before determining how to protect it and who to protect it from.

 🍎:TIP  Privacy is a hot topic that focuses on the confidentiality of personal data.

### Integrity
Integrity involves maintaining the **accuracy, validity, and completeness** of information and systems. It ensures that data is not tampered with by anyone other than an authorized party for an authorized purpose. A che****cksum is a value derived from a piece of data that uniquely identifies that data and is used to detect changes that may have been introduced during storage or transmission. Checksums are generated based on cryptographic hashing algorithms and help you validate the integrity of data

### Availability
Availability is all about ensuring that authorized users can access required systems and data when and where they need it. Availability has a special place in the cloud given that easy access to data is often a major selling point for cloud services. If your letter gets lost in the mail, then availability is a clear issue — the message that was intended for you to read is no longer accessible for you to read.

One of the most common attacks on availability is Distributed Denial of Service, or DDoS, which is a **coordinated attack** by multiple compromised machines causing disruption to a system’s availability. Another common and rapidly growing attack on availability is **ransomware**, which involves an attacker blocking system or data owners from accessing their own systems and data **until a sum of money is paid.** Aside from sophisticated cyber-attacks, something as simple as accidentally deleting a file can compromise availability.

 REMEMBER  Availability is a major consideration for cloud systems.

### Security controls

So, you know all about confidentiality, integrity, and availability — that’s great! Now, how do you enforce those concepts in your systems? -- said another
way, security controls protect the confidentiality, integrity, and availability of your systems and data.


TIP  You’ll often see “security controls” referenced as just “controls.”
Security controls can be categorized in a couple of ways: by their type and by their function.

- Types of security control include
 - Technical controls use technology (shocking, I know!) to protect information systems and data. Things like firewalls, data loss prevention (DLP) systems, and
   encryption fall under this category.
 - Physical controls involve the use of physical measures to protect an organization’s assets. This can include things like doors, gates, surveillance cameras,
   and physical disposal of sensitive information (including things like shredding and degaussing).
 - Administrative controls include the set of policies, procedures, guidelines, and practices that govern the protection of systems and data. This can be
   anything from incident response plans (see later in this chapter) to security awareness training.

- Functions of security controls include
 - **Preventative controls** keep negative security events from **happening**. This includes things like security awareness training, locked doors, and
   encryption.
 - Detective controls **identify** negative security events when they do happen. Examples of detective controls include log monitoring and video surveillance.
 - Corrective controls fix or reduce damages associated with a negative security event and may include measures to prevent the same negative event from happening
   again. Backups and system recovery features are the most common examples of corrective controls.
 
## Threats, Vulnerabilities, and Risks … Oh My!

Threats, vulnerabilities, and risks are **interrelated** terms describing things that may compromise the pillars of information security for a given system or an asset (the thing you’re protecting).

**The field of risk management deals with identifying threats and vulnerabilities and quantifying and addressing the risk associated with them**. 
Being able to recognize threats, vulnerabilities, and risks is a critical skill for information security professionals. 
It’s important that you’re able to identify the things that may cause your systems and data harm in order to better plan, design, and implement protections against them.

### Threats
**A threat is anything capable of intentionally or accidentally compromising an asset’s security**. Some examples of common threats include
 - **Natural disasters:** Earthquakes, hurricanes, floods, and fires can cause physical damage to critical infrastructure, leading to loss of connectivity, power
   outages, or even complete destruction of systems.
 - **Malware:** Malicious software such as viruses, worms, and ransomware can infect systems, steal data, or disrupt normal business operations.
 - **Phishing attacks:** Deceptive emails, messages, or websites designed to trick individuals into revealing sensitive information like passwords, credit card
   numbers, or personal data.
 - **Denial of service (DOS) attacks:** Deliberate attempts to overload a network, server, or website with excessive traffic, making it unavailable to legitimate
   users.
Though only a few examples, the preceding short list shows how threats can come in all shapes and sizes, and how they can be natural or manmade, malicious or accidental.

### Vulnerabilities

A vulnerability is a weakness or gap existing **within a system**; it’s something that, if not taken care of, may be exploited in order to compromise an asset’s confidentiality, integrity, or availability.

Examples of vulnerabilities include
 - Unpatched software: Failure to install updates or patches for operating systems, applications, or firmware, leaving security vulnerabilities open to
   exploitation.
 - Lack of environmental protection: Missing or faulty fire suppression systems or other physical protections, leaving infrastructure vulnerable to natural
   disasters and other environmental threats.
- Insecure passwords: The use of commonly used or otherwise insecure passwords, making it easier for attackers to gain unauthorized access to accounts or
  systems.
- Untrained employees: Lack of security awareness training for employees and system users, leaving them susceptible to phishing attacks.

⭐ **Threats are pretty harmless without an associated vulnerability, and vice versa.** 
A good fire detection and suppression system gives your data center a fighting chance, just like (you hope) thorough security awareness training for your organization’s employees will neutralize the threat of an employee clicking on a link in a phishing email.

### Risks

**Risk is the intersection of threat and vulnerability** that **defines the likelihood of a vulnerability being exploited** (by a threat actor) **and the impact should that exploit occur**. 

In other words, risk is used to define the potential for damage or loss of an asset. Some examples of risks include
 - A fire wipes out your data center, making service unavailable for five days.
 - A hacker steals half of your customer’s credit card numbers, causing significant reputational damage to your company.
 - An attacker gains root privilege through a phishing email and steals your agency’s Top Secret defense intelligence.

 **REMEMBER  Risk = Threat x Vulnerability.** 
 **This simple equation is the cornerstone of risk management.** 
 
 
## Understand Identity and Access Management

So much of information security requires you to first have a strong understanding of who your users are and then controlling their actions based on their identity. 
Think about it this way: The principle of confidentiality is pretty hard to enforce if you don’t first understand who does and doesn’t qualify as an authorized user, right?

IAM consists of **four** key **elements**: **identification, authentication, authorization, and accountability**.

- Identification is the act of establishing who (or what) someone (or something) is. In computing, identification is the process by which you associate an entity (i.e., a system or user) with a unique identity or name, such as a username or email address.
- Authentication takes identification a step further and validates a user’s identity. During authentication, you answer the question “Are you who you say you are?” before authorizing access to a system. Passwords are the most obvious and common forms of authentication, but authenticators (things used to verify identity) can vary. Authenticators generally fit into one of three factors (or methods):
  1. Something you know: Passwords and PINs (Personal Identification Numbers) fall into this category.
  2. Something you have: Security tokens and smart cards are examples of this factor.
  3. Something you are: Examples of this factor include fingerprints, iris scans, voice analysis, and other biometric methods.

REMEMBER  Due to the imperfect nature of any one of the preceding factors, many organizations require Two-Factor Authentication (2FA) or Multifactor Authentication (MFA). MFA has become standard practice for enforcing stronger validation of a user’s identity. Because passwords can be hacked and security tokens can be stolen, **the idea here is to require more than one form of authentication to reduce the risk of granting access to someone impersonating someone else**.

Once you verify a user’s identity, you can determine what access to grant them. Authorization is the process of granting access to a user based on their authenticated identity and the policies you’ve set for them. You can control access to systems and data in many ways, but that topic is largely outside the scope of this book.

The final major element in IAM is accountability, **which involves assigning and holding an entity responsible for their actions within an information system**. **Accountability requires establishing unique user identities, enforcing strong authentication, and maintaining thorough logs to track user actions.**

## Deciphering Cryptography

Cryptography is the science of encrypting and decrypting information **to protect its confidentiality and/or integrity**.

### Encryption and decryption
Encryption is the process of using an algorithm (or cipher) to convert plaintext (or the original information) into ciphertext. The ciphertext is unreadable unless it goes through the reverse process, known as decryption, which then allows an authorized party to convert the ciphertext back to its original form **using the appropriate encryption key(s)**. 

An encryption key is a piece of information that allows the holder to encrypt and/or decrypt data.

### Types of encryption
Encryption can either be **symmetric-key** or **asymmetric-key**.

**Symmetric-key encryption** (sometimes referred to as **<ins>secret-key encryption</ins>**) uses the same key (called a secret key) for both encryption and decryption (see Figure 2-2). Using a single key means the party encrypting the information must give that key to the recipient before they can decrypt the information. **<ins>The secret key is typically sent to the intended recipient as a message separate from the ciphertext</ins>**. Symmetric-key encryption is **simple, fast, and relatively cheap**.

 WARNING  A notable drawback of symmetric-key encryption is it requires a secure channel for the initial key exchange between the encrypting party and the recipient. If your secret key is compromised, the encrypted information is as good posted on a billboard.

 **Asymmetric-key encryption (more commonly known as <ins>public-key encryption<ins>)** **operates by using two keys** — one **public** and one **private**. The public key, as you might guess, is made publicly available for anyone to encrypt messages. The private key remains a secret of the owner and is required to decrypt messages that come from anyone else (see Figure 2-3). Although public-key encryption is typically slower than its counterpart, **it removes the need to secretly distribute keys and also has some very important uses** (see the next section).

Lastly, in cloud environments, there are different ways that asymmetric keys are generated and even managed. Each has their own benefits and drawbacks. This is covered in Chapter 5.

Figure: Using a symmetric-key for both encryption and decryption.
<img width="580" height="224" alt="image" src="https://github.com/user-attachments/assets/80b6c5c8-02a9-4834-b49f-e104ecab3ee7" />

Figure: Utilizing asymmetric-key (or public key) encryption and decryption.
<img width="580" height="285" alt="image" src="https://github.com/user-attachments/assets/cd08ef92-3967-4ade-9396-a2daf8c9718a" />

### Common uses of encryption
Encryption plays an important part in protecting information systems, and its applications are wide ranging. This section discusses some of the most common uses of encryption.

#### Data protection
Arguably the most widely used application of encryption **is to protect the confidentiality of data**. You’ll typically see encryption used for data protection for both data-at-rest (things like files on a hard drive or in a database) and data-in-motion (communication over a network, for example). Both symmetric-key and asymmetric-key encryption are commonly used in data protection applications.

#### Authentication and authorization
Usernames and passwords are often sent to some remote system for authentication and authorization. Encryption is commonly used to protect these sensitive credentials **from eavesdroppers on the network who would intercept the credentials in transit and utilize them to impersonate an authorized user**. **Authentication is a standard use case for public-key encryption**.

#### Network security
**Transport Layer Security (TLS) is the standard technology** used **to encrypt traffic over a network**, and **it creates an encrypted link ensuring that all traffic between two points remains private**. TLS has replaced its longstanding predecessor, Secure Sockets Layer (SSL), as the de facto standard and **is used widely when privacy and data integrity need to be maintained between two systems**. you need to know that **TLS connections use a combination of symmetric- and asymmetric-key encryption**.

**(HTTPS) is TLS over HTTP** and is the **gold standard for protecting web communications**. HTTPS is incredibly important for banking and other websites where users send and receive sensitive information and is now commonly used as a standard practice. Keep an eye on your browser’s address bar for https:// to ensure your session is encrypted.

#### Digital signatures
- Much like your handwritten signature is used to verify your identity, a digital signature is a piece of information that asserts or proves the identity of a user.
- **Digital signatures operate on a public-key scheme** and **require a sender to use their private key to electronically sign a message**. Recipients can then use the sender’s public key to verify their identity. In addition to helping to identify users, **digital signatures support the principle of nonrepudiation**, which is the information security concept that **ensures that a party cannot deny the integrity or authenticity of a digital communication or transaction**. **Nonrepudiation provides assurance that the communication or transaction took place and that the parties involved cannot later deny their involvement.**

#### Virtual private networks (VPNs)
A virtual private network **(VPN) encrypts communication between the two networks**, over the Internet, to create a secure tunnel for communication. You commonly see VPNs used for people who telework by connecting to their organization’s network from home. Similar to the network security example in the earlier section, **VPNs use a mix of symmetric-key and asymmetric-key encryption**.

#### Crypto-shredding
Standard data deletion involves overwriting data with a series of zeroes, ones, or both. This process is both slow and not completely effective at ensuring bits and pieces of data aren’t left behind. **A better process, known as crypto-shredding**, **involves encrypting data and then destroying the keys. With no key left behind to decrypt the data, it’s effectively considered deleted.**

 TIP: If you guessed that symmetric-key encryption is best for crypto-shredding, you’d be correct! In addition to being simpler, faster, and cheaper, there’s only one key to delete!

## Grasping Physical Security

“I’m an IT gal/guy. Why should I care about physical security?” I’m glad you asked! While most information security discussions focus on using technical controls to protect the data that resides on machines, the protection of physical assets is just as important.

An uncontrolled fire wiping out your data center may not compromise your data’s confidentiality or integrity, but what about availability? If it impacts one or more of the three pillars of information security, then you, as a security professional, definitely care about it. (For more on this topic, see the section “Exploring the Pillars of Information Security,” earlier in this chapter.)

 REMEMBER  Information security professionals are concerned with anything that impacts the confidentiality, integrity, or availability of data or systems. **Don’t ignore legitimate risks that are present outside of the computer hardware and software.**

In addition to the environmental considerations that come with physical security, keep in mind that you can spend all your time throwing sophisticated technical protections at your systems, but it means nothing if an attacker can simply pick the lock to your data center and walk out with a server! You can find out more about secure physical design in Chapter 11.


## Realizing the Importance of Business Continuity and Disaster Recovery

You can’t always stop bad things from happening. The unfortunate reality is some factors will always be outside of your control — and when bad things do happen, business continuity and disaster recovery are paramount.

Business continuity (BC) refers to the policies, procedures, and tools you put in place to ensure critical business functions continue during and after a disaster or crisis. The goal of business continuity is to allow essential personnel the ability to access important systems and data until the crisis is resolved. REMEMBER  When you think of disasters and crises, you’re not only concerned with malicious cyberattacks, but also accidental disruptions, natural disasters, and major system failures.

Disaster recovery (DR) is a subset of business continuity focusing on (you guessed it!) recovering your IT systems that are lost or damaged during a disaster.

In other words, DR is the part of BC focused on restoring full operation of and access to hardware, software, and data as quickly as possible after a disaster. 

Unlike business continuity — whose focus is on making a business operational — disaster recovery focuses on activities like recovering off-site backups, for example.

 WARNING  Though business continuity and disaster recovery **are closely related, they’re not the same**. Business continuity broadly focuses on the procedures and systems you have in place to keep a business up and running during and after a disaster. Disaster recovery more narrowly focuses on getting your systems and data back after a crisis hits. The terms are often misused, so make note of the distinction.

You need to be aware of a couple important related metrics:
- **Recovery Time Objective (RTO)** -- is the amount of **time** **within** which business processes **must** be **restored** in order to avoid significant consequences associated with the disaster. In other words, RTO answers the question “How much time can pass before an outage or disruption has unacceptably affected my business?”

- **Recovery Point Objective (RPO)** -- **is the maximum amount of data loss that’s tolerable to your organization**. It answers the question “How much data can I lose before my business is unacceptably impacted by a disaster?”
  - **RPO plays an important role in determining frequency of backups**.

Business continuity and disaster recovery are typically big selling points of cloud computing. The cloud’s robust infrastructure and redundancy features contribute to increased reliability and resilience, making cloud computing a central part of many organization’s business continuity and disaster recovery plans.
As a cloud security professional, there are a couple things you should keep in mind regarding business continuity and disaster recovery:

You should ensure that the cloud infrastructure and applications being used have appropriate security measures in place to protect systems and data during both normal operations and disaster scenarios. This includes ensuring encryption, access controls, and other mechanisms remain in place during a disaster.

 You should maintain integrity and availability throughout the disaster recovery process with regular backups, testing, and validation procedures to verify that the backups remain reliable and can be restored successfully, when needed.

 WARNING  Cloud providers commonly advertise their uptime and other availability metrics, but cloud infrastructures and applications are not immune from availability risks. You should conduct regular audits and compliance checks of your cloud services to ensure that their disaster recovery and business continuity plans align with industry regulations and your organization’s own requirements.

## Understanding Logging and Monitoring

Logging and monitoring are separate, but related, practices that your organization uses to help **detect, escalate, and respond to security events.**
Logging is the process of **recording and storing the key actions**, **activities, and events** that occur within an information system. 
Logging involves capturing important information and storing it in files (or logs) for future reference and analysis.

Examples of key log types include
1. System logs that capture events related to the operating system, such as startups and shutdowns, logins and logouts, system errors and warnings.
2. Security logs that capture things like failed login attempts, changes to access permissions, intrusion attempts, and other suspicious activities that may
   indicate a security incident.
3. Network logs that capture information about network traffic, such as connection information, source and destination IP addresses, and traffic volumes.
4. Database logs that capture changes made to a database, including access, modifications, and queries.
TIP  The log types that you should be aware of depends on your particular environment and use cases. The list here is only a starting point.

**Logging is great and all, but logs serve little purpose if they are not actively monitored.** 

Just like a bank might have security personnel who actively monitor the surveillance systems, monitoring, in the context of information security, involves continuously observing and analyzing your information systems. **By monitoring your systems, you can detect and respond to security events in a timely manner**.

Monitoring activities include: 
  vulnerability scanning, 
  intrusion detection (through the use of intrusion detection systems, or IDS), 
  threat intelligence analysis, and 
  log analysis.

TECHNICAL STUFF  The amount of log data in even a small organization can quickly become overwhelming and impossible to analyze manually. Security Information and Event Management (SIEM) is a category of tools used to collect, centralize, and analyze large volumes of log data from all over your environment. A SIEM tool can help automatically correlate security events and logs from various sources and enable your organization to conduct real-time threat detection and incident response.

## Implementing Incident Handling


It would be great if you could just do your security magic, and nothing bad would ever happen. Unfortunately, you can’t fix every vulnerability or stop every threat … so it’s important that you’re prepared to handle whatever comes your way. The field of incident handling deals with preparing for, addressing, and recovering from security incidents.

I want to define some important terms up front. NIST SP 800-61 defines the following:

 An event is any observable occurrence in a system or network.

 Adverse events are events with negative consequences.

 A computer security incident is a violation or imminent threat of violation of computer security policies, acceptable use policies, or standard security practices.

 TIP  While the focus in this section is specifically on computer security incidents, keep in mind that these principles apply to power failures, natural disasters, and so on.

Though every incident starts as an event (or multiple events), every event is not necessarily an incident. To take the distinction even further, not every event is even considered adverse or negative. Some examples of events include

 A website visitor downloads a file.

 A user enters an incorrect password.

 An administrator is granted root access to a router.

 A firewall rejects a connection attempt.

 A server crashes.

Of the preceding events, only the last one is inherently adverse — and without further information, you can’t call any of them incidents. The following list includes some examples of incidents:

 A hacker encrypts all your sensitive data and demands a ransom for the keys (i.e., a ransomware attack).

 A user inside your organization steals your customers’ credit card data.

 An administrator at your company is tricked into clicking on a link inside a phishing email, resulting in a backdoor connection for an attacker.

 Your HR system is taken offline by a Distributed Denial of Service (DDoS) attack.

 WARNING  Make sure you don’t use the terms event and incident interchangeably — they’re not the same. I have heard IT professionals refer to simple events and/or alerts as incidents, and that’s a great way to sound alarms that don’t need to be sounded!

Incident handling starts well before an incident even occurs and ends even after things are back to normal. The Incident Response (IR) lifecycle (shown in Figure 2-4) describes the steps you take before, during, and after an incident. The key components of the IR lifecycle are

 Preparation

 Detection

 Containment

 Eradication

 Recovery

 Post-Mortem

Figure 2-4: The Incident Response (IR) lifecycle.
A flow diagram depicts the incident response lifecycle. It illustrates the following: Preparation, detection, containment, eradication, recovery, and post-mortem.
I cover the preceding concepts in the remaining sections.

Preparing for incidents
You can easily overlook preparation as part of the incident response process, but it’s a critical step for the rapid response to and recovery from incidents. This phase of incident handling includes things like

 Developing an incident response plan. Your incident response plan identifies procedures to follow when an incident occurs, as well as roles and responsibilities of all stakeholders.

 Periodically testing your incident response plan. Determine your plan’s effectiveness by conducting table-top exercises and incident simulations.

 Implementing preventative measures to keep the number of incidents as low as possible. This process includes finding vulnerabilities in your systems, conducting threat assessments, and applying a layered approach to security controls (things like network security, host-based security, and so on) to minimize risk.

 Setting up incident analysis equipment. This process can include forensic workstations, backup media, and evidence-gathering accessories (cameras, notebooks and pens, and storage bags/bins to preserve crucial evidence and maintain chain of custody).

Detecting incidents
During this phase, you acknowledge that an incident has indeed occurred, and you feverishly put your IR Plan into action. This phase is all about gathering as much information as possible and analyzing it to gain insights into the origin and impact of the incident. Some examples of activities during this phase are

 Conducting log analysis and seeking unusual behavior. A good Security Information and Event Management (SIEM) tool can help aggregate different log sources and provide more intelligent data for your analysis. You’re looking for the smoking gun, or at least a trail of breadcrumbs, that can alert you to how the attack took place.

 Identifying the impact of the incident. Which systems were impacted? What data was impacted? How many customers were impacted?

 Notifying the appropriate individuals. Your IR Plan should detail who to contact for specific types of incidents. During this phase, you’ll need to enact your communications plan to alert proper teams and stakeholders.

 Documenting the findings. The situation will likely be frantic, so organization is critical. You want to keep detailed notes of your findings, actions taken, chain of custody, and other relevant information. This activity helps with your post-mortem reporting later on and also helps you keep track of important details that can assist in tracing the attack back to its origin. In addition, many incidents require reporting to law enforcement, regulators, or other external parties. Thorough notes and a strong chain of custody help support any investigations that may arise.

 TIP  Depending on various factors (the nature of the incident, your industry, or any contractual obligations), you may be responsible for notifying customers, law enforcement, regulators, or even US-CERT (part of Department of Homeland Security). Make sure that you keep a comprehensive list of parties to notify in case of a breach.

Containing incidents
The last thing you want to deal with during an incident is an even bigger incident. Containment is extremely important to stop the bleeding and prevent further damage. It also allows you to use your incident response resources more efficiently and avoid exhausting your analysis and remediation capacity. Some common containment activities include:

 Disabling Internet connectivity for affected systems

 Isolating/quarantining malware-infected systems from the rest of your network

 Reviewing and/or changing potentially compromised passwords

 Capturing forensic images and memory dumps from impacted systems

Eradicating incidents
By the time you reach this phase, your primary mission is to remove the threat from your systems. Eradication involves eliminating any components of the incident that remain. Depending on the number of impacted hosts, this phase can be fairly short or last for quite some time. Here are some key activities during this phase:

 Securely removing all traces of malware

 Disabling or re-creating impacted user and system accounts

 Identifying and patching all vulnerabilities (starting with the ones that led to the breach!)

 Restoring known good backups

 Wiping or rebuilding critically damaged systems

Recovering from incidents
The objective of the Recovery phase is to bring impacted systems back into your operational environment and fully resume business as usual. Depending on your organization’s IR Plan, this phase may be closely aligned or share steps with the Eradication phase. It can take several months to fully recover from a large-scale compromise, so you need to have both short-term and long-term recovery objectives that align with your organization’s needs. Some common recovery activities include:

 Confirming vulnerabilities have been patched and fully remediated

 Validating systems are functioning normally

 Restoring systems to normal operations (for example, reconnecting Internet access, restoring connection to your production network, and so on)

 Closely monitoring systems for any remaining signs of undesirable activity

Conducting a post-mortem
After your systems are back up and running and the worst is over, you need to focus your attention on the lessons learned from the incident. The primary objective of the Post-Mortem phase is to document the lessons and implement the changes required to prevent a similar type of incident from happening in the future. All members of the Incident Response Team (and supporting personnel) should meet to discuss what worked, what didn’t work, and what needs to change within the organization moving forward. Here are some questions to consider during post-mortem discovery and documentation:

 What vulnerability (technical or otherwise) did this breach exploit?

 What could have been done differently to prevent this incident or decrease its impact on your organization?

 How can you respond more effectively during future incidents?

 What policies need to be updated, and with what content?

 How should you train your employees differently?

 What security controls need to be modified or implemented?

 Do you have proper funding to ensure that you are prepared to handle future breaches?

 TIP  For a more in-depth review of handling security incidents, refer to NIST’s Computer Security Incident Handling Guide (SP 800-61).


 ## Utilizing Defense-in-Depth
One final security concept to explore is defense-in-depth, or layered security. These two terms describe the same idea of applying multiple, distinct layers of security technologies and strategies for greater overall protection. The thought behind this concept is that each layer has its own strengths and weaknesses, which you’d like to complement one another. A weakness in one layer can be compensated by the strengths in other layers. By applying two or more of the control mechanisms discussed in this chapter (access control, cryptography, and physical security), you can implement defense-in-depth and gain greater overall protection. (I cover additional security controls that support defense-in-depth throughout the remainder of this book.)

Of course, this approach isn’t foolproof — vulnerabilities will still exist. However, a well-executed defense-in-depth approach makes it much harder for attackers to find and exploit vulnerabilities in your system, and much easier for you to detect an incident sooner rather than later. You explore the concept of defense-in-depth as it relates to the cloud throughout the rest of this book.

# Domain # 1 - Cloud Concepts, Architecture, and Design
- Domain 1 represents 17 percent of the CCSP certification exam

## Understanding Cloud Computing Concepts

### Defining cloud computing terms

**According to NIST**, “Cloud computing is a model for enabling ubiquitous, convenient, on-demand network access to a shared pool of configurable computing resources (e.g., networks, servers, storage, applications, and services) that can be rapidly provisioned and released with minimal management effort or service provider interaction. This cloud model is composed of **five essential characteristics**, **three service models (IaaS, PaaS, SaaS, FaaS)**, and **four deployment models (public, private, community, and hybrid)**.”

The following list is **based on ISO/IEC 17788**, “Cloud Computing — Overview and Vocabulary” and defines some important terms used in the cloud computing industry. 
- **Cloud application**: An application that is accessed via the Internet rather than installed and accessed locally.
- **Cloud data portability**: The ability to easily move data from one cloud provider to another.
- **Cloud deployment model**: The way in which cloud services are made available through specific configurations that control the sharing of cloud resources
  with cloud users. The cloud deployment models are public, private, community, and hybrid.
- **Cloud resources:** Compute, storage, and networking capabilities that a cloud provider shares with a cloud user.
  - These resources include the physical equipment located in the cloud provider’s data centers
  - as well as virtual resources like operating systems and applications.
- **Cloud service:** Capabilities made available to a cloud user by a cloud provider through a published interface (a management console or command line, for
  example).
- **Cloud service category:** A collection of cloud services that share a common set of features or qualities.
  - Cloud service categories are labelled XaaS (where the X can be Anything as a Service).

- **Cloud service customer data:** Any data objects **under the control of the cloud service customer** and that were input to the cloud service by the cloud
  customer or generated by the cloud service on behalf of the cloud customer.
- **Cloud service derived data:** Any data objects **under the control of the cloud service provider** and that were derived by interaction of the cloud customer
  with the cloud service. Derived data may include access logs, utilization information, and other forms of metadata (or data about data).
- **Cloud service provider data:** Any data objects related to the operation of the cloud service and that are fully under the control of the cloud service
  provider. Provider data may include cloud service operational data, information generated by the cloud service provider to provide services, and similar data
  not owned or related to any specific cloud customer.
TIP: The topic of data ownership in the cloud can be a contentious one, and has many legal and compliance implications. It’s important that cloud providers share clear terms as to what data they own and what the customer owns, as this has an effect on who is responsible for securing what.

- **Community cloud:** Cloud deployment model where cloud services are provided **to a group of cloud service customers** with **similar requirements**.
  - It is common for at least one member of the community to control the cloud resources for the group.

- **Data portability:** The ability to easily move data from one system to another, without needing to re-enter the data.
- **Hybrid cloud:** Cloud deployment model that uses a combination of **at least two** **different cloud deployment models** (public, private, or community).
  - **Infrastructure as a service (IaaS):** Cloud service category **that provides infrastructure capabilities to the cloud service customer**.
  - **Measured service:** Delivery of cloud services in such a way that its usage can be **monitored, accurately reported, and precisely billed.**
  - **Multitenancy:** Allocation of cloud resources such that multiple tenants and their data are inaccessible from other tenants who share those resources.
  - **On-demand self-service:** A characteristic of cloud that allows a cloud service customer to provision cloud resources and capabilities with little or no
    interaction with the cloud service provider.
  - **Platform as a service (PaaS):** Cloud service category that **provides platform capabilities to the cloud service customer**.
  - **Private cloud:** Cloud deployment model where cloud **services are provided to a single cloud service customer** who controls their own cloud resources.
  - **Public cloud:** Cloud deployment model where cloud resources are controlled by the cloud service provider and **cloud services are made available to any
    cloud service customer**.
  - **Resource pooling:** Aggregation of a cloud service provider’s resources to provide cloud service to one or more cloud service customers.
  - **Reversibility: Capability for a cloud service customer to retrieve their cloud service customer data and for the cloud service provider to delete this data
    after a specified period or upon request.**

- **Software as a service (SaaS):** Cloud service category that provides software/application capabilities to the cloud service customer.
- **Tenant:** One or more cloud service users sharing access to a set of cloud resources.

Identifying cloud computing roles and responsibilities
When you (or your customers) move data into the cloud, questions like “Who does what?” may arise. It’s important that you become familiar with the common roles in cloud computing environments and understand how the various roles work together to keep cloud data secure:

 Cloud auditor: A cloud service partner who is responsible for conducting an audit of the use of cloud services. An audit may be for general security hygiene, but is often for legal or compliance purposes.

 Cloud service broker: A cloud service partner who negotiates relationships between cloud service providers and cloud service customers.

 Cloud service customer: A person or group that is in a business relationship to provision and use cloud services from a cloud service provider.

 Cloud service partner: A person or group that supports the provision, use, or other activities of the cloud service provider, the cloud service customer, or both.

 Cloud service provider (CSP): An entity making cloud services available for use. I refer to cloud service provider as the CSP in this book.

 Cloud service user: A person or entity (which may be a device, for example) that uses cloud services on behalf of the cloud service customer.

Recognizing key cloud computing characteristics
Five characteristics must be present for a service or offering to be considered cloud:

 On-demand self-service

 Broad network access

 Resource pooling

 Rapid elasticity

 Measured service

Looking at these five essential cloud characteristics, you can see some major themes: convenience, efficiency, and transparency, among others. While cloud has evolved to present a strong case for being secure and cutting-edge, keep in mind that the heart of cloud computing is really all about making resources easy to access, manage, and monitor.

 TECHNICAL STUFF  Although the features described are the five key cloud computing characteristics, a sixth characteristic is worth mentioning: multitenancy. Multitenancy is a feature of most clouds that involves having multiple customers sharing physical hardware. Whereas traditional data centers rely on cages and physically separate servers and network devices to segregate customers, cloud environments rely on logical technologies (like encryption, virtualization, segmentation, and so on) to keep one customer’s data virtually separated from others. While this is very standard in cloud computing, I explain an exception when I discuss the private cloud deployment model in the “Cloud deployment models” section.

If the five key characteristics are not present in a service or offering, then it is not true cloud computing. Some of these features are defined in the previous sections, but I cover them all in depth in the following sections.

#### On-demand self-service
By design, cloud service providers allow customers to procure and provision cloud resources by anyone who wants or needs them. 
On-demand self-service means that a customer can request, set up, and use cloud services in an automated fashion and without interacting with another human. 
On-demand self-service **allows full cloud usage without approval from your manager, legal team, or finance department**.

The upside to on-demand self-service is the **tremendous ease of procurement**. 
Cloud computing is designed to be easy to get started with; if you can pay for it, you can use it. 
Though self-service is helpful for productivity, security teams should be aware of the risks that come with it and implement policies and procedures to help govern the use of cloud services.

 TECHNICAL STUFF **Shadow IT refers to the use of unsanctioned or unauthorized technology (such as cloud services) within an IT environment, which may lead to unauthorized sharing of information with unapproved third parties**. 
**Shadow IT is one of the key risks related to on-demand self-service in cloud computing and poses significant security risks to your organization’s data governance and compliance efforts.**

#### Broad network access
Cloud resources should be accessible to any authorized cloud user with an Internet connection. 
The principle behind this characteristic is that **cloud computing should make resources and data ubiquitous** and **easily accessed when and where** they’re required.

Mature cloud offerings make accessing their resources device-agnostic, allowing cloud users the ability to connect to their cloud services from a variety of endpoint devices that include laptops, desktops, tablets, and even smartphones. 
From a security standpoint, this ability gives customers deploying cloud applications some additional considerations, as cloud computing extends their data to a variety of devices, that may not be within the enterprise’s control. For this reason, many companies need to examine their mobile device management policies when moving to or operating in the cloud.

 WARNING Bring your own device (BYOD) has become increasingly common and means that companies are allowing employees to connect their own smartphones, tablets, and laptops to corporate systems. BYOD has the benefit of enabling broad access to cloud systems from many devices, but adds concerns regarding device management and secure access methods. Fortunately, cloud computing mitigates some risk of BYOD because it encourages users to store their data in cloud storage rather than on their devices. Additionally, cloud computing can also extend security capabilities (like device checks and monitoring) onto your BYOD devices. Even still, be mindful of your company’s BYOD policies and consider how cloud systems might impact them.

### Resource pooling
One of the most critical concepts in cloud computing, 
resource pooling occurs when a **CSP groups (or pools) its cloud resources for shared use between multiple cloud customers**. 
What resource pooling allows the CSP to do is scale resources up and down, on a per-customer basis, as each customer’s resource needs increase or decrease. 
**CSPs can have many thousands of servers, networking devices, and other resources available; pooling allows them to efficiently manage those resources between customers, with minimal waste.**

 TIP  Some organizations prefer or require maintaining segregation between their data and other organizations’ data, which goes against the concept of resource pooling. **Private clouds and some community clouds address this concern with data segregation or isolation needs.**

Resource pooling works closely with rapid elasticity to provide cloud customers a dynamic set of compute, storage, and network resources that are allocated based on each customer’s needs.

Rapid elasticity
At the core of cloud computing, rapid elasticity allows a cloud customer to quickly obtain additional cloud resources as the user’s needs require. Think of a retail website during the Black Friday or Cyber Monday shopping frenzy. Rapid elasticity allows that website to seamlessly accommodate a sudden spike in traffic, without the cloud customer’s intervention, by automatically scaling and provisioning (referred to as auto-scaling and auto-provisioning) resource based on load.

 TIP  It’s not uncommon for many businesses to have peak-hours or peak-seasons, during which their resource utilization may drastically increase. Outside of these peaks, many businesses can see their resource demands plummet for long periods of time. Rapid elasticity and resource pooling work together to give cloud customers as much compute, storage, and networking power as needed, and nothing more. This capability is important because cloud also leverages a pay-as-you-use model.

Measured service
Cloud computing makes it exceedingly easy for cloud customers to monitor, measure, control, and report on their resource usage. Measured service works in a similar manner to how you might have a measured (or metered) use for your water or electric bill. Similar to these home utilities, CSPs charge customers only for the resources that they use. As such, providing measured services that allows full transparency between a CSP and cloud customer is paramount.

 TIP  Measured service allows your organization to continuously monitor resource utilization in your cloud environment and can help you detect unusual activity (such as Shadow IT or suspiciously high usage volumes resulting from certain compromises). Measured service provides detailed usage logs that assist with security audits and incident investigations.

Building block technologies
Many technologies at the heart of cloud computing architectures are very familiar if you’ve worked with traditional IT hardware and software. Any cloud computing environment, at the most fundamental level, consists of compute (CPU), memory (RAM), storage, networking, virtualization, and orchestration technologies. The customer will have greater or lesser responsibility over these building block technologies, depending on the cloud service category. The following sections explore some of the key building block technologies that exist in cloud environments.

Storage
Cloud storage technologies include object storage (ideal for unstructured data like documents and images) and block storage (ideal for high-performance use cases like virtual machines and databases).

Modern cloud providers offer a wide range of database storage services that support relational databases (such as MySQL, SQL Server, and PostgreSQL) and NoSQL databases (such as DynamoDB, MongoDB, and Cassandra).

Networking
Key cloud networking technologies include virtual networks, firewalls, load balancers, VPNs, and content delivery networks (CDNs). These networking technologies enable secure and efficient communication in the cloud, and they support several of the key cloud computing characteristics mentioned in the previous section.

Virtualization
Virtualization is a central concept in cloud computing involving the creation of virtual instances that simulate the behavior of physical hardware, including servers, storage devices, and networking equipment. Virtualization abstracts the underlying hardware and allows multiple virtual computing environments to run on a single physical machine.

 REMEMBER  Virtual machines (VMs) are the most easily identifiable form of virtualization, but you should know that storage, networking, compute, and memory resources are all virtualized in a cloud environment.

#### Orchestration
Orchestration, in cloud computing, refers to the **coordination** and management of cloud resources and services. 
Orchestration involves **creating and executing workflows** to provision, deploy, scale, and manage cloud infrastructure and applications.
Orchestration tools help streamline the management of complex cloud environments, enabling efficient resource allocation and ensuring consistent deployment and operations.

TECHNICAL STUFF  **AWS CloudFormation**, **Azure Automation**, **Puppet Bolt**, and **Terraform** are a **few popular cloud orchestration tools**, but there are many others.

TIP **Cloud automation is a subset of cloud orchestration** that involves programming repetitive tasks, such as spinning up and configuring virtual machines. Cloud automation helps you achieve repetitive tasks with minimal human intervention, while cloud orchestration involves coordinating and managing a collection of automated tasks.


## Describing Cloud Reference Architecture

Several key components fit together to create the complete picture of a cloud architecture and implementation. These components include the activities and capabilities required to develop and manage a cloud environment, as well as the cloud service categories and cloud deployment models that describe how the service is delivered, configured, and managed.

### Cloud computing activities : 
Similar to traditional computing environments, cloud computing requires a number of activities to be performed by several parties in order to build, deploy, secure, audit, and manage systems and data. This section serves as a high-level overview of the key activities performed by the cloud service provider, cloud service customer, and cloud service partner.

Cloud service **provider**: The following are key roles and activities performed by the cloud service provider:
  - Cloud service operations manager: Oversees and manages the operation and performance of cloud services provided to customers.
  - Technical account manager: Provides account support and high-level technical guidance to cloud customers.
Cloud service **customer**: The following are key roles and activities performed by the cloud service customer:
  - Cloud architect: Evaluates cloud technologies and services and designs the overall architecture of the cloud deployment to meet organizational requirements.
  - Cloud service user: Uses services provided by the CSP.
  - Cloud service administrator: Configures, manages, and monitors the use of cloud services.
Cloud service **partner**: The following are key roles and activities performed by the cloud service partner:
  - Cloud auditor: Performs audits of cloud environments and provides audit reports.
  - Cloud service broker: Provides a marketplace for approved services, manages contracting, and securely integrates cloud services with on-prem applications.

### Cloud service capabilities
You should familiarize yourself with three primary cloud service **capabilities**:
1. Infrastructure service capability: The cloud customer can provision and maintain granular control over compute, storage, and network resources.
2. Platform service capability: The cloud customer can run code and develop applications using programming libraries that are managed and controlled by the cloud service provider.
3. Software service capability: The cloud customer can use applications that are fully developed and managed by the cloud service provider.

### Cloud service categories
Cloud service categories generally fall into three main groups:
1. Infrastructure as a service (IaaS)
2. Platform as a service (PaaS)
3. Software as a service (SaaS)

### Infrastructure as a service (IaaS)
Infrastructure as a service, or IaaS, **is in many ways what people first think of when they hear cloud computing**. It’s the service category where the CSP provides compute, storage, and networking resources and the **customer has the greatest level of control and customization over those resources**. Think of things like virtual machines and storage containers or buckets — that’s IaaS.

NIST 800-145 describes IaaS as “the capability provided to the consumer is to provision processing, storage, networks, and other fundamental computing resources where the consumer is able to deploy and run arbitrary software, which can include operating systems and applications. The consumer does not manage or control the underlying cloud infrastructure but has control over operating systems, storage, and deployed applications; and possibly limited control of select networking components (e.g., host firewalls).”

**IaaS key characteristics and benefits include**
1. **Cost efficiency:**
  - By using the IaaS service model, **customers do not need to spend money on buying and managing hardware up front** or as the need for additional resources
    grow.
    - With IaaS, **customers can trade Capital Expenditure (CapEx) for Operational Expenditure (OpEx)**.
  - In addition, **customers also benefit from the cloud provider paying for and managing physical security of the datacenter**s.

2. **Availability and reliability:**
  - Infrastructure as a service provides customers with options for load balancing and redundancy across vast infrastructures that can span many regions or even
   countries. These vast infrastructures provide customers with assurance that their resources will be highly available and resilient against availability
   threats (DDoS and others).

3. **Scalability:**
  - With IaaS service models, additional resources can be procured, provisioned, and expanded quickly and with ease to support growing demand.
  - Whereas on-premise solutions would require a customer to purchase and set up new servers to support increased utilization,
  - IaaS allows automatic scaling when necessary.

### Platform as a service (PaaS)

Platform as a service, or PaaS, sits on top of the IaaS layer in the cloud stack and begins to shift control (and responsibility) over resources away from the cloud customer and back to the cloud provider. 
In PaaS offerings, the user is generally **building their own application or solution using prepackaged libraries and features provided by the cloud provider.** 

Having the **infrastructure and development environment** **taken care of by the CSP** **allows the customer to focus on development rather than managing servers, virtual machines, and other granular resources**. 

As a result of PaaS offerings, the barrier to entry for software development continues to fall. 

**Developers, large and small, spend less time and money developing infrastructures and managing resources and more time on being innovative**.

 TIP  You may be familiar with terms like up the stack and down the stack from TCP/IP discussions, and they carry over to the cloud computing world. In cloud, these terms refer to the way the three cloud service categories stack on top of each other to provide full cloud functionality. **IaaS sits at the bottom of the stack and moves up to PaaS, followed by SaaS at the top.**

**NIST 800-145** describes PaaS as “the capability provided to the consumer is to deploy onto the cloud infrastructure consumer-created or acquired applications created using programming languages, **libraries, services, and tools supported by the provider**. The consumer does not manage or control the underlying cloud infrastructure including network, servers, operating systems, or storage, but has control over the deployed applications and possibly configuration settings for the application-hosting environment.”

**Though PaaS customers inherit many of the same benefits of IaaS, some will be unique to PaaS**.

**PaaS key characteristics and benefits include**

1. **Cost efficiency:**
  - Similar to IaaS, the PaaS service category offers cost savings **because application developers pay only for the systems and resources they use**.
  - As customers progress through the development cycle, they can scale up or down with ease and without incurring unnecessary costs.

3. **Flexibility:**
  - Developers receive a great deal of flexibility during their application development lifecycle when they use PaaS cloud offerings.
  - Within a given cloud environment, **developers can often easily switch between operating systems and software versions to suit their needs**.
  - Many cloud providers provide open source environments and applications for developers, which prevents vendor lock-in and affords them the ease of moving
    between environments, platforms, and even cloud providers.

5. Simplicity: With the underlying infrastructure and operating systems being managed by the cloud provider, hardware and software upgrades and system patches are handled for the developer. Upgrading to the latest version of software is commonly as simple as clicking a few buttons, which minimizes downtime and lets developers focus on creating their applications rather than managing systems.

6. Ease of access: Being cloud-based means that development platforms and tools are easily accessed from anywhere in the world. This ease of access makes it incredibly easy for global development teams to collaborate on projects, as opposed to on-prem development platforms that may require out of band collaboration (like emailing updated files or using less reliable technologies like shared drives).

TECHNICAL STUFF Serverless computing is a cloud computing model that allows developers to run their code without needing to provision or manage servers. A serverless function is a small piece of code that is executed in response to an event or trigger. In serverless computing, developers just need to write and deploy their application code and define event-driven functions. The CSP takes care of all of the infrastructure and scaling needs.

Function as a service (FaaS)
The increased adoption of serverless computing has given rise to another popular cloud service category, Function as a Service (FaaS). FaaS is similar to PaaS in that it provides a platform for developers to create, run, and manage application code while hiding infrastructure management from the developers. While PaaS requires you to manage servers and scaling, FaaS (and serverless) is more focused on code execution, and it doesn’t require any server process to constantly run; application code only executes when a function is invoked.

Serverless computing has been around for some time, but FaaS was first made popular with the announcement of AWS Lambda in 2014. Since then, Microsoft Azure, Google Cloud Platform, and other CSPs, large and small, have launched serverless offerings that continue to grow in adoption.

Software as a service (SaaS)
Software as a service, or SaaS, sits at the top of the cloud stack and provides fully operational software applications to the customer. SaaS moves the majority of resource management to the cloud provider, allowing the end user to simply use the provided application to meet their needs. Examples of SaaS offerings include Google Docs, Dropbox, and DocuSign; these cloud-based applications require little to no configuration by the customer.

NIST 800-145 describes SaaS as “the capability provided to the consumer is to use the provider’s applications running on a cloud infrastructure. The applications are accessible from various client devices through either a thin client interface, such as a web browser (e.g., web-based email), or a program interface. The consumer does not manage or control the underlying cloud infrastructure including network, servers, operating systems, storage, or even individual application capabilities, with the possible exception of limited user specific application configuration settings.”

SaaS customers inherit many of the previously mentioned benefits from IaaS and PaaS, but SaaS does have some unique features and benefits.

SaaS key characteristics and benefits include

 Cost efficiency: You’re probably seeing a theme here: Cloud helps customers cut costs. Similar to IaaS and PaaS, software as a service helps customers manage costs by eliminating the need for system administrators and dedicated hardware and software. For SaaS applications, customers only need a device to access the given application and an Internet connection.

 Licensing: With SaaS, customers effectively lease or borrow licenses as they use software. Leasing eliminates the need for customers to purchase full sets of licenses, which may go underutilized for long periods of time. Cloud providers, due to the scale of their environments, can take advantage of friendlier licensing fees from third-party vendors, and some of those savings are able to be realized by the end user.

 Standardization: By nature, cloud applications are standardized regardless of who’s accessing or where they’re accessing the application from. From an application standpoint, standardization helps ensure consistent experiences from one user to another and makes sure that all users are using the latest and greatest software versions, with little to no action taken by the customer.

Cloud deployment models
Four main types of cloud deployment models exist:

 Public

 Private

 Community

 Hybrid

These deployment models describe how cloud services are hosted, who controls and operates them, and what cloud customers may access them. Table 3-2 highlights the main features of the four main types of cloud deployment.

Table 3-2: Overview of the Cloud Deployment Models
Public

Private

Community

Hybrid

Open to the general public

Used exclusively by a single organization

Used exclusively by a community of similar organizations (like government agencies)

Shares features of two or more cloud models

May be owned by a private company, government organization, academic institution, or a combination

May be owned by the organization, a third party, or co-owned

May be owned by a community member, a third party, or co-owned

Allows customers to have control over their most critical systems

Highly scalable resources

May exist on- or off-premises

Supports disaster recovery for customers considering private cloud

Customer maintains increased ownership and control over their resources

Public cloud deployment
According to NIST SP 800-145, “[public] cloud infrastructure is provisioned for open use by the general public. It may be owned, managed, and operated by a business, academic, or government organization, or some combination of them. It exists on the premises of the cloud provider.” In English, public cloud is a set of computing services that can be accessed by anyone willing and able to pay for them.

With enterprise offerings from tech giants like Google, Amazon, and Microsoft — as well as Apple’s consumer cloud product, iCloud — public cloud is typically what consumers think of when they think about “the cloud.”

Public cloud benefits and uses include

 Easy to set up and manage: In public cloud deployments, the cloud service provider owns and operates the infrastructure, which means the customer isn’t responsible to manage infrastructure like data center facilities, networking hardware, and operational expenses. In addition, public cloud commonly offers streamlined access to resources through easy-to-use interfaces.

 Highly scalable resources: Public clouds typically have vast infrastructures that are ready and able to handle heavy workloads.

 Resource efficiency and cost-effective: Customers don’t have to worry about wasted resources, as public clouds automatically scale a customer’s resources up or down, based on their usage and bill them only for what they use. Unused resources from one customer can be used (and paid for) by another.

Private cloud deployment
According to NIST SP 800-145, “[private] cloud infrastructure is provisioned for exclusive use by a single organization comprising multiple consumers (e.g., business units). It may be owned, managed, and operated by the organization, a third party, or some combination of them, and it may exist on or off premises.” In other words, private cloud offers similar services to those offered by public cloud, but private cloud can only be accessed by members of a single organization.

Private cloud is sometimes referred to as an internal cloud and is often used for legal, compliance, or security purposes. In certain highly regulated industries, customers often want the convenience and features that cloud provides, without their data being mixed (or comingling) with other customers’ data.

Private cloud benefits and uses include

 Increased ownership: With private clouds, the customer/user is the same party that owns and operates it. As such, private clouds give users a greater level of ownership and the ability to control everything about it. One common example is for customers with data location requirements — for example, a bank may have regulations that require its data remains within the European Union (EU). The standard way to satisfy this requirement has historically been to build or use a private cloud that allows that bank to only let data travel to data centers within the EU. Newer offerings from some public cloud infrastructures are now allowing these customers to meet these types of requirements without managing their own private cloud.

 High level of system and data control: Similar to the point mentioned in the previous bullet, private clouds give customers increased control over all resources. Private cloud customers can control things like bandwidth, system patching, and software/application availability, whereas these things are often only controlled by the CSP in public clouds.

Community cloud deployment
According to NIST SP 800-145, “[community] cloud infrastructure is provisioned for exclusive use by a specific community of consumers from organizations that have shared concerns (e.g., mission, security requirements, policy, and compliance considerations). It may be owned, managed, and operated by one or more of the organizations in the community, a third party, or some combination of them, and it may exist on or off premises.” Think of community clouds as private clouds that are extended to a limited set of related organizations.

Community clouds are common in highly regulated industries. Government customers, for example, will often seek out the moniker GovCloud for assurance that only government data resides within a given cloud. While the term GovCloud may entail a bit of marketing, it’s a great example of the intent of the community cloud deployment model.

Community cloud benefits typically mirror those of public clouds. The added benefit comes from all members of the cloud user base sharing a common set of privacy, security, or compliance requirements. A community of users with the same (or highly similar) set of requirements can ensure that the cloud meets their requirements exactly.

Hybrid cloud deployment
According to NIST SP 800-145, “[hybrid] cloud infrastructure is a composition of two or more distinct cloud infrastructures (private, community, or public) that remain unique entities, but are bound together by standardized or proprietary technology that enables data and application portability (e.g., cloud bursting for load balancing between clouds).” Simply put, hybrid cloud consists of some combination of public, private, and/or community cloud features.

As you may expect, hybrid cloud models attempt to bring the best of multiple worlds together; when using a hybrid cloud deployment, customers are generally seeking public cloud features and scalability with private or community cloud control.

Hybrid cloud benefits include

 Re-use of existing infrastructure and technology: Many customers want the benefits and features that public clouds provide, but they may already have an expensive infrastructure that’s up and running. A hybrid cloud allows customers to reap the benefits of public clouds while still utilizing their private clouds, as necessary. A hybrid cloud is sometimes a stepping stone for customers dipping their toe in the cloud waters, but there are often compliance, legal, or other business reasons for customers maintaining private cloud (or on-premises) infrastructure.

 Control over critical or sensitive systems: With hybrid cloud deployment models, customers are able to keep data that they are most concerned about in their private cloud, while moving less sensitive data to a public cloud. By sharing characteristics of public and private (or community) clouds, customers are able to maintain a high level of control and ownership without missing out on the benefits that public cloud provides.

 Disaster recovery support: One common use case for hybrid cloud is in supporting disaster recovery. Customers already running on a fully functional private cloud can benefit from the redundancy and reliability assurance that many public clouds provide. Customers can continue to use their private clouds as normal, but can configure their resources to failover to the public cloud in the event of a disaster. Because the public cloud would be used only in case of emergency, customers will usually incur little to no costs under normal circumstances (because you’re billed for what you use).

 TECHNICAL STUFF  The hybrid cloud deployment model shares similarities with the concept of multi-cloud. Multi-cloud refers to a strategy where an organization uses multiple CSPs rather than just a single cloud provider. This often includes the use of multiple public cloud providers — so while all hybrid cloud deployments are multi-cloud, not all multi-cloud deployments are hybrid.

Cloud shared considerations
Cloud computing involves organizations outsourcing the management and maintenance of their computing infrastructure to one or more third-party cloud providers. As such, moving to the cloud is not only a technology decision, but also a business decision. As with any business decision, you must consider several factors before moving forward. In this section, you explore several universal cross-cutting aspects that anyone thinking about moving their data to the cloud should consider.

Interoperability
Interoperability is the ability for two or more systems to seamlessly work together by sharing information and using that information as necessary. In cloud systems, interoperability ensures that cloud services can understand standard data formats, APIs, configurations, and identification and authorization mechanisms so that these cloud-based systems can work with the organization’s existing technologies or even other clouds.

Portability and reversibility
Portability is the ease with which a party can move or reuse application or service components. Portability means that the service provider, underlying platform, operating system, API structure, format of data, or other factors do not present obstacles to seamlessly moving services from one solution to another.

Vendor lock-in occurs when any of these factors prevents a customer from moving from one cloud provider to another. Portability ensures that an organization is able to easily move between cloud providers or cloud deployment models (from public to private cloud, for example), and host some or all of those components in different environments. Highly interoperable systems provide customers flexibility as their needs change and also tend to keep cloud providers on their toes because customers are able to migrate at any time.

Availability
As discussed in Chapter 2, availability is one of the pillars of information security and one of the greatest considerations for organizations moving to the cloud. In many ways, the availability of resources and systems can make or break a cloud provider’s success and their reputation. When an organization relies on a cloud provider for their infrastructure, platforms, or applications, the cloud provider’s failure to deliver can mean substantial impact to the customer’s business. It’s not uncommon for CSPs to commit to 99.9 percent (or higher) availability. Failure to meet this commitment can result in penalties, loss of customers, and degraded brand reputation.

Resiliency
Resiliency measures the ability of a cloud provider to continue providing fully functioning services in the event of disruption. In many ways, resiliency goes hand in hand with availability. As you learn in Chapter 2, disaster recovery and business continuity planning are two key reasons users move to the cloud. Given that CSPs commonly have incredibly vast amounts of resources (servers, storage, networking equipment, bandwidth, and so on), it’s easier for cloud-based systems to be highly redundant and resilient in the event of natural disaster, power failure, or other equipment outage. Potential cloud adopters should pay close attention to any resiliency commitments made in their contracts or SLAs.

Security and privacy
Security is often the top concern for potential cloud customers, and it can either be a major selling point or a barrier to adoption for any given CSP. For many organizations — especially smaller ones — moving to the cloud can significantly increase security capabilities, because large scale cloud providers are able to provide world-class security controls that some organizations either cannot afford or are not yet sophisticated enough to implement.

Many cloud providers will publicly state their baseline levels of security or share some of their most marketable security features, but they will typically fall short of listing specific security controls to avoid arming potential attackers with sensitive information that could lead them to compromising the CSP’s security. In general, the most mature cloud providers are able to offer just about any security feature a customer could want, but additional security can often incur additional costs.

 WARNING  Not all cloud providers are created equally, and not all are able to meet the same levels of security standards. As cloud security professionals, it’s important to not only understand what security features are available, but also which ones are enabled by default. Too many cloud breaches occur because users falsely assume that an advertised security feature is enabled without their action.

If security is concern 1A, privacy is often 1B for potential users of cloud services. The very nature of cloud means that customers’ data is not always 100 percent within their control. Remember that the global nature of cloud means that a customer’s data may exist in multiple locations around the world. Privacy laws and regulations are increasingly influencing CSPs’ behavior, but no universal or international set of laws or directives currently consistently enforce privacy standards from one CSP to another, across different geographical locations. Depending on a customer’s privacy needs, it may be necessary to negotiate specific requirements as part of contracts or SLAs. (I cover SLAs later in the section “Service-level agreements.”)

It might go without saying that cloud computing and high performance are intertwined. Few customers will select or stay with a cloud provider that can’t deliver consistently strong performance. The largest CSPs have been in a bit of an “arms race” for years and are releasing stronger, better, and faster compute, memory, and storage capabilities at least every year.

In the upcoming section “Impact of related technologies,” you can see some key emerging applications for cloud computing that rely on high performance.

Governance
Governance relates to the policies, procedures, roles, and responsibilities in place to ensure security, privacy, resiliency, and performance. Governance is required at the start of any cloud migration and continues through the entire lifetime of a cloud deployment. In other words, governance activities are ongoing from day zero until cloud services are no longer being used.

Many cloud providers make governance easier than it is with traditional data center models because they offer tools to generate reports and monitor relevant statistics and metrics. The ability to schedule and automate reporting enhances governance activities and allows customers to focus on their mission.

Service-level agreements
In cloud, a service-level agreement (SLA) is an agreement between a cloud service provider and cloud customer that identifies the minimum level of service that must be maintained.

SLAs can include anything from amount of uptime to minimum response time to customer service inquiries. In many ways, an SLA serves as a warranty when a customer moves to the cloud. Similar to the warranty you get when purchasing a car, a cloud SLA gives customers assurance that they are getting what they expect and provides remedies (like fee reimbursement) if those agreed upon expectations aren’t met.

Here are some examples of things you should look for in a service-level agreement. Keep in mind that this list is not exhaustive:

 Availability: How much uptime is the CSP committing to? The standard is 99.9 percent or more, but pay attention to the period of time over which this guarantee is made.

 Performance: What are standard and maximum response times?

 Data ownership: Who owns your data once it’s in the cloud?

 Location of the data: What geographical locations might your data be located? The location may have privacy or compliance implications.

 Portability of the data: Are you able to move your data to another provider whenever you choose?

 Data security and privacy: Is data encrypted at rest? In transit? Who is permitted to access your data?

 Disaster recovery: What solutions and processes are in place for DR and backup?

Maintenance and versioning
The cloud service category being used will determine just how much consideration a customer must give to maintenance and versioning. With SaaS offerings, the CSP is responsible for just about all patching, maintenance, and versioning. Moving up the stack to PaaS and even more with IaaS, the customer has increasing responsibility for these actions.

Maintenance and versioning responsibilities should be agreed upon and understood early on, and they should be specifically called out in contracts and SLAs. With versioning, customers should be aware of what ability the CSP grants for rolling back to previous versions, and what responsibility they have to upgrade (or rollback) from one version to another.

Regulatory compliance
Regulatory compliance is the requirement for an organization to meet or satisfy regulations, guidelines, policies, and laws relevant to its business. A company failing to meet these requirements may face financial penalties, legal action, or even termination of business operations. As a result, regulatory compliance is a major concern for potential cloud users, and it’s important to note that the nature of cloud means satisfying compliance is a shared responsibility between a CSP and its customer.

 TIP  Having worked on compliance teams at two of the largest cloud providers, I can say firsthand that cloud customers often struggle to understand what is commonly called the Shared Responsibility Model. As a CCSP, it’s paramount that you understand what your organization is responsible for securing and what your CSP or customer is responsible for. The most transparent CSPs will provide substantial documentation to support your understanding of the Shared Responsibility Model; if this documentation is not readily available, it’s best to ask for sufficient details.

Many, many regulations and laws impact technology. Some key examples that impact cloud-based environments include Health Insurance Portability and Accountability Act (HIPAA), Payment Card Industry Data Security Standard (PCI DSS), System and Organization Controls (SOC), the Federal Information Security Management Act (FISMA), and the Federal Risk and Authorization Management Program (FedRAMP), among others. It’s important that cloud security professionals understand how their industry influences which of these or other regulations they are required to satisfy.

 TIP  In the context of regulatory compliance, you may see SOC (i.e., SOC 1, SOC 2, or SOC 3) described as either System and Organization Controls or Service Organization Controls.

Auditability
As a CCSP candidate, auditability in the cloud is an area you should pay very close attention to because of the Shared Responsibility Model. Because customers do not have full control over the cloud environment the way they would in a traditional data center model, it’s important that they’re able to audit their compliance with various regulatory requirements, as well as monitor important user and system activity.

The CSP is responsible for providing logging and auditing capabilities to the customer and demonstrating that they are capturing and reporting on any events the customer may want to audit. Most mature cloud service providers offer a wealth of auditing and reporting capabilities, but it is up to the customer to use them in accordance with their compliance obligations.

Impact of related technologies
One of the recently updated sections to the CCSP Common Body of Knowledge (CBK) addresses critical technologies that cloud security professionals should stay abreast of. The following list of emerging technologies are closely related to cloud and represent some of the fastest growing applications of cloud computing.

Artificial Intelligence (AI) and machine learning (ML)
Broadly speaking, Artificial Intelligence is the field devoted to helping machines process things in a smart manner; AI involves giving machines the ability to imitate intelligent human behavior. AI burst onto the public scene in a big way with the release of the AI-enabled chat app, ChatGPT, at the end of 2022. As of this writing in 2023, ChatGPT has over 100 million active users and generates 1.8 billion visitors per month, demonstrating the meteoric rise of mainstream AI, which has been enabled and driven by cloud computing.

Machine learning is a subset of AI that focuses on allowing machines to alter themselves as they are exposed to additional data. Much like a child learns language by being exposed to different words in different contexts over time, ML occurs when a machine learns new information without requiring it to be explicitly programmed.

Cloud providers like Amazon Web Services (AWS), Google Cloud Platform, and Microsoft Azure offer services that make it easy for organizations and users to access AI and ML capabilities without requiring advanced skills in data science. Many of these services offer pre-built machine learning models and large datasets from which those models can begin “learning” for your application.

Data science
Data science is a multidisciplinary approach to studying large and complex datasets and extracting meaningful insights using machine learning and various statistical techniques. Cloud computing plays a significant role in data science by providing scalable and flexible infrastructure and computational resources, allowing data scientists to store and process huge amounts of data using cutting-edge ML capabilities.

Blockchain
In April 2021, the price of 1 Bitcoin peaked at close to a whopping $65,000! Since then (as of this writing), the price has trended downward, but interest in cryptocurrencies and other blockchain applications continues strong. In simplest terms, a blockchain is a string of digital information that is chained together by cryptography. Each block of information contains a cryptographic hash of the previous block, transaction data, and a timestamp. Several industry leading cloud providers now offer platforms to help users build their blockchain-based applications without needing PhDs in cryptography.

Internet of things (IoT)
Internet of things is a fancy way of describing everyday devices that are connected to the Internet. My TVs, refrigerator, oven range, and dishwasher are all equipped with devices that connect to the Internet and that allow them to send and receive data (hopefully not to Skynet). Outside of the home, IoT has many commercial and industrial applications; you can find entire warehouses run by Internet-connected devices. Because these devices collect and generate a large amount of data, cloud systems play a pivotal role in drawing insights from IoT systems. For systems with thousands or even millions of IoT sensors, cloud computing allows data to be aggregated, processed, and analyzed more quickly and efficiently.

Edge computing
In simple terms, edge computing is a form of computing that involves capturing, processing, and analyzing data at its source. Edge computing reduces latency and improves performance by bringing the power of the cloud to the edge of the networks and doing all of the processing on-site instead of sending data to a central cloud data center. In a smart home, for example, edge computing can be used to process and control devices like security cameras and thermostats directly in the home instead of sending all data to a cloud server.

Confidential computing
Confidential computing is a cloud-based technology focused on protecting sensitive data by isolating it in a protected central processing unit (CPU) during processing. Confidential computing keeps sensitive data encrypted in a secure enclave that is separate from the rest of the environment, offering assurance that even the cloud provider cannot access the data in plaintext.

Containers
Containers are a growing technology that involves logically decoupling an application from its environment so that the containerized application can be developed, deployed, and run consistently in different environments (public cloud, private cloud, or even a personal laptop). Containers were made popular with the development of Kubernetes, an open-source platform for managing containerized workloads. With Kubernetes and other container platforms, cloud users are able to develop applications and seamlessly move and run them from one platform to another. Containers are particularly useful in hybrid cloud deployments, for example, where a customer might run the same application on-prem and in the cloud.

Quantum computing
In October 2019, Google announced that it had achieved quantum supremacy — basically, the ability of a quantum computer to solve a problem that a classical computer could not solve in a practical amount of time. Though quantum computing is still in its infancy, tech giants like Google, IBM, and Microsoft are pushing forward with solutions to bring the power of quantum computing to cloud applications.

 TECHNICAL STUFF  The field of quantum computing revolves around using the principle of quantum mechanical superposition to process information exponentially faster than even modern supercomputers. The physics behind quantum mechanics and quantum computing is outside the scope of this book, but worth further research if you find yourself working on cloud-based quantum applications.

DevSecOps
DevSecOps is a software development practice aimed at combining security and IT operations into every stage of the software development lifecycle (SDLC). Cloud computing plays an important role in supporting and enabling DevSecOps practices in modern technology environments. The scalability, flexibility, and automation features within cloud environments support automating security processes and enabling development teams to include security throughout the entire development lifecycle.

