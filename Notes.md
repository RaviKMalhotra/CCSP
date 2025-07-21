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
 
 
