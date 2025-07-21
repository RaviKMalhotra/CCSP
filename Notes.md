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

