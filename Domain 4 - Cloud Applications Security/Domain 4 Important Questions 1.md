# CCSP: Chapter 4: Domain 4—Cloud Application Security
# Chapter 4: Domain 4—Cloud Application Security
The fourth domain of the Certified Cloud Security Professional (CCSP) Exam Outline covers applications in the cloud, from software development to challenges involved in migrating apps from the traditional IT environment. It also addresses software security and performance testing methods as well as proper identity and access management (IAM) principles. Because it is weighted less than the previous domains (according to this table published by (ISC)2,  https://cccure.training/m/articles/view/CISSP-domains-weight-percentage-on-the-real-exam), there are considerably fewer questions in this chapter.
	
### Question # 1 - ISO 27034 mandates a framework for application security within an organization. According to the standard, each organization should have a(n) _______________, and each application within the organization should have its own _______________.  
A. Organizational Normative Framework (ONF), Application Normative Framework (ANF)  
B. Application Normative Framework (ANF), Organizational Normative Framework (ONF)  
C. Standard Application Security (SAS), Application Normative Framework (ANF)  
D. Organizational Normative Framework (ONF), Standard Application Security (SAS)  
Answer: A.   

The **ONF** lists all the controls **used in all the applications within an organization**; 
And each **ANF** lists the **particular controls used in each application the organization has**. 
Standard Application Security is a made-up term therefore options C and D are incorrect.

### Question # 2 - According to ISO 27034, there is one Organizational Normative Framework (ONF) in the organization, and _______________ Application Normative Framework (ANF[s]) for each application within that organization.    
A. Many    
B. Three    
C. No    
D. One     
Answer: D. 

Each application will have its own ANF, derived from the organization’s ONF. This can be a difficult question because there are many ANFs in the organization, but only one for each application. The reader needs to examine the question carefully.

### Question # 3 - What language is used in the Simple Object Access Protocol (SOAP) application design protocol?   
A. Hypertext Markup Language (HTML).  
B. X.509.  
C. Extensible Markup Language (XML).     D. Hypertext Transfer Protocol (HTTP).  
Answer: C. 

**SOAP necessarily uses XML.**
HTML is a language used to tag text files so that they can be displayed with different fonts, colors, graphics and hyperlinks. **HTML is not used in SOAP.** Option A is incorrect.
Option B is incorrect because X.509 is a standard and the question is about a programming language.
Option D is incorrect because HTTP is protocol and the question is about a programming language.

### [Important] Question # 4 - Typically, representational state transfer (REST) interactions do not require.   _______________.
A. Credentials.   
B. Sessions.    
C. Servers.    
D. Clients.    
Answer: B.     

Generally, a REST interaction involves the client asking the server (through an application programming interface [API]) for data, sometimes as the result of processing; the server processes the request and returns the result. 
**In REST, an enduring session, where the server has to store some temporary data about the client, is not necessary.**
These interactions obviously involve servers and clients, so options C and D are not correct.
Using REST does not eliminate the need for credentials, so option A is not correct.

### Question # 5 - Representational state transfer (REST) application programming interfaces (APIs) use _______________ protocol verbs.     
A. Hypertext Markup Language (HTML).  
B. Hypertext Transfer Protocol (HTTP).  
C. Extensible Markup Language (XML).       D. American Standard Code for Information.  Interchange (ASCII).  
Answer: B.    

Roy Fielding, the author of the PhD dissertation **that created REST, was also the author of HTTP**, so it’s no surprise the command set is the same.
All the other options are incorrect because the **REST APIs do not use HTML, XML or ASCII as protocol verbs.**

### Question # 6 - The architecture of the World Wide Web, as it works today, is _______________.    b
A. JavaScript Open Notation (JSON).  
B. Denial of service (DoS).  
C. Representational state transfer (REST).  
D. Extensible Markup Language (XML).  
Answer: C.   

**The web is mainly HTTP, which is a RESTful protocol.**
All the other options are incorrect because they do not answer the question about the architecture of the World Wide Web.
	
### Question # 7 - RESTful responses can come from the server in _______________ or _______________ formats.   
A. Extensible Markup Language (XML), JavaScript Open Notation (JSON).  
B. Hypertext Transfer Protocol (HTTP), X.509.   
C. American Standard Code for Information Interchange (ASCII), text.   
D. Hypertext Markup Language (HTML), Extensible Markup Language (XML).   
Answer: A.    

**Servers can return REST requests to clients in a number of formats, including XML and JSON**.
**X.509 certificates are used for passing session encryption information, not data requests**, so option B is incorrect.
Servers usually return data requests in some sort of display format, not plain text or ASCII, so option C is incorrect.
HTML responses would simply be an entire web page, not specific data, so option D is incorrect.
	
### Question # 8 - Which of the following is an informal industry term for moving applications from a traditional environment into the cloud?    
A. Instantiation.  
B. Porting.   
C. Grandslamming.   
D. Forklifting.   
Answer: D. 

All the other options are simply words used in other contexts. They are incorrect.

### Question # 9 - Developers creating software for the cloud environment should bear in mind cloud-specific risks such as _______________ and _______________.   
A. DoS and DDoS (denial of service and distributed denial of service).  
B. Multitenancy and third-party administrators.   
C. Unprotected servers and unprotected clients.   
D. Default configurations and user error.  
Answer: B. 

All the other options are risks that exist in the traditional environment as well as the cloud.

### Question # 10 - When an organization considers cloud migrations, the organization’s software developers will need to know which _______________ and which _______________ the organization will be using, in order to properly and securely create suitable applications.   
A. Geographic location, native language. 
B. Legal restrictions, specific ISP. 
C. Service model, deployment model.  
D. Available bandwidth, telecommunications country code.  
Answer: C.   

In order for developers to properly create and secure applications, they will need to understand the extent of resource sharing (public/private/hybrid/community) and level of control (infrastructure as a service [IaaS], platform as a service [PaaS], software as a service [SaaS]) the organization will expect in the cloud environment.

Each of the other options includes at least one element that programmers don’t need to know (specifically, the native language, Internet service provider [ISP], country code) and is therefore incorrect.

### Question # 11 - Which of the following is perhaps the best method for reducing the risk of a specific application not delivering the proper level of functionality and performance when it is moved from the traditional environment into the cloud?    
A. Remove the application from the organization’s production environment and replace it with something else.   
B. Negotiate and conduct a trial run in the cloud environment for that application before permanently migrating.   
C. Make sure the application is fully updated and patched according to all vendor specifications.   
D. Run the application in an emulator.   
Answer: B.    

A trial run in the cloud will reveal any functionality/performance loss before a permanent cloud migration.
Option A doesn’t reduce any risk for a specific application; it trades the risk of one application not operating correctly with the risk of another application not working correctly. This answer is wrong.
All applications should be reasonably patched and updated, whether it is in the traditional environment or the cloud. Option C is incorrect.
An emulator won’t reduce the risk of degraded performance; it will probably result in degraded performance. Option D is incorrect.

### Question # 12 - Software developers designing applications for the cloud should expect to include options to ensure all of the following capabilities except _______________.  
A. Encryption of data at rest   
B. Encryption of data in transit    
C. Data masking    
D. Hashing database fields    
Answer: D. 

Not all programs (or organizations) will require database access, or even use databases, and hashing is not a common requirement.
All the other functions are expected in the majority of cloud operations.

### Question # 13 - In a platform as a service (PaaS) model, who should most likely be responsible for the security of the applications in the production.   environment?   
A. Cloud customer.  
B. Cloud provider.  
C. Regulator.  
D. Programmers.  
Answer: A.   

**In PaaS, the customer is responsible for the administration (and security) of applications.**
Neither regulators nor programmers are responsible for the security of the applications in the production environment. That is the responsibility of the cloud customer.
It may appear as though the cloud provider should be responsible for application security, however, as the cloud customer acquires more responsibility for their cloud environment, the cloud provider assumes less responsibility. Option B is incorrect.
	
### Question # 14 - In the testing phase of the software development lifecycle (SDLC), software performance and _______________ should both be reviewed.    
A. Quality.  
B. Brevity.  
C. Requirements.   
D. Security.  
Answer: D. 

Performance and security both need to be reviewed for adequacy.
In this context, quality would be synonymous with performance and requirements, so D is a better answer than A or C.
Brevity is not a trait we look for in testing, even though it may be desirable in programming, so B is incorrect.

### Question # 15 - Regardless of which model the organization uses for system development, in which phase of the software development lifecycle (SDLC) will user input be requested and considered?  
A. Define.  
B. Design.  
C. Develop.  
D. Detect. 
Answer: A. 

In the Define phase, we’re trying to determine the purpose of the software, in terms of meeting the users’ needs; therefore, we may solicit input from the user community in order to figure out what they really want.

Options B and C are other phases of the SDLC, but not all SDLC models incorporate user input in these phases, so the options are not correct.
Option D is not a phase of the SDLC and is incorrect.

### Question # 16 - Which phase of the software development lifecycle (SDLC) is most likely to involve crypto-shredding?   
A. Define.  
B. Design. 
C. Test.  
D. Disposal.  
Answer: D. 

Disposal is the only phase concerned with the sanitization of media or destruction of data.
All the other options are also SDLC phases, however, **crypto-shredding is much more likely to be used in the disposal phase.**

### Question # 17 - Where are business requirements most likely to be mapped to software construction?   
A. Define.  
B. Design.  
C. Test.  
D. Secure Operations.  
Answer: B. 

Design is the correct answer, as this is where the requirements gathered during the Define phase are mapped to system designs.
All the other options are SDLC phases where requirements are not mapped to software construction.

### Question # 18 - [important] All of the following are usually nonfunctional requirements except _______________.   
A. Color.  
B. Sound.  
C. Security.   
D. Function.  
Answer: D. 

**Function is usually the functional requirement, describing what action the tool/process satisfies.**

All the others are usually nonfunctional requirements. Exceptions to this are when the characteristic listed is the actual desired function. For instance, if the product is a tool that enunciates text so that a blind user can hear the words, then sound would be the functional requirement. If the product is a security tool such as a firewall or data loss prevention (DLP) solution, then security would be a functional requirement. Otherwise, these are nonfunctional requirements for standard products.

### Question # 19 - Designers making applications for the cloud have to take into consideration risks and operational constraints that did not exist or were not as pronounced in the traditional environment. Which of the following is an element cloud app designers may have to consider incorporating in software for the cloud that may not have been as important in the traditional environment?    
A. Identity and access management (IAM) capability.  
B. Distributed denial of service (DDoS) resistance.   
C. Encryption for data at rest and in motion.   
D. Field validation.  
Answer: C. 

Traditional apps won’t usually require encryption in all phases of the data lifecycle because data is protected in several stages in the traditional environment without the need for additional controls. In the cloud environment, however, data exposed at any point in the lifecycle might constitute an inadvertent disclosure, **so cloud apps require encryption for data at rest and in motion (and usually in use as well).**

Even traditional apps require IAM and field validation functions, so options A and D are incorrect.
Most anti-DDoS activity will be performed by hardware and communication software run by the cloud provider or Internet service provider (ISP); developers should not typically need to include anti-DDoS elements in their programs. Option B is incorrect.
	
### Question # 20 - Designers making applications for the cloud have to take into consideration risks and operational constraints that did not exist or were not as pronounced in the traditional environment. Which of the following is an element cloud app designers may have to consider incorporating in software for the cloud that might not have been as important in the traditional environment?  
A. Application isolation.  
B. Inference framing.  
C. Known secure library components.  
D. Testing that uses known bad data.  
Answer: A. 

Because the cloud is a multitenant environment, one of the concerns that developers should consider is how well the application prevents other applications/users from observing its operation and resource calls. In the traditional environment, **this is not usually required because the organization owns the underlying infrastructure (as a single tenant) and there is very little risk in exposing the application’s functionality.**

Inference framing is a nonsense term, used here only as a distractor.
Software should include known secure components, and testing should include known bad data (fuzz testing), whether it is going to be used in the cloud or in a traditional environment, so options C and D are incorrect.

### Question # 21 - Designers making applications for the cloud have to take into consideration risks and operational constraints that did not exist or were not as pronounced in the traditional environment. Which of the following is an element cloud app designers may not be able to use as readily in the cloud environment as it was deployed in the traditional environment?   
A. Cryptography.  
B. STRIDE testing.  
C. Field validation.  
D. Logging.  
Answer: D. 

The cloud provider may have controls that restrict logging, or the delivery of log data, in the environment; this can make it complicated for cloud developers to include that functionality/security element in cloud apps.

All the other options are things that can (and should) be done with software whether the application is being used in traditional or cloud environments, so those options are incorrect.

### Question # 22 - All of these can affect the quality of service expected from an application except _______________.   
A. Encryption.  
B. Egress monitoring.  
C. Anti-malware tools.  
D. Use of known secure libraries/components.  
Answer: D. 

Using only known secure libraries and components in software design **may slow down development efforts but shouldn’t impact how the application runs.**

All the other options are security controls that will degrade performance because they require additional overhead; these options are incorrect.

### Question # 23 - The possibility that a user could gain access or control of an application so as to take on administrator or management capabilities is called.  _______________.  
A. Inversion  
B. Spoofing  
C. Repudiation  
D. Escalation of privilege  
Answer: D.     

This is the definition of escalation of privilege (sometimes referred to as “elevation of privilege”).
Inversion is a nonsense term in this context and just a distractor.
Options B and C are threat modeling elements but are not correct answers for this question.
	
### Question # 24 - Which of the following is not checked when using the STRIDE threat model?     
A. The ability of users to gain administrative access rights without proper permission.   
B. The ability of internal personnel to trigger business continuity/disaster recovery activities.   
C. The ability of a participant in a transaction to refute that they’ve taken part in the transaction.   
D. The ability of an unauthorized user to pretend to be an authorized user.   
Answer: B   

**The STRIDE threat model does not deal with business continuity and disaster recovery (BC/DR) actions.**
All the other options are elements of STRIDE (escalation of privilege, repudiation, and spoofing, respectively) and are therefore not correct.
STRIDE stands for:
	S: Spoofing
 	T: Tempering
	R: Repudiation
 	I: Information Disclosure
  	D: Denial of Service
   	E: Elevation of Privileges
	
### Question # 25 - It is very likely that your organization’s users will use unapproved application programming interfaces (APIs), especially in a bring your own device (BYOD) environment, because _______________.   
A. Users are constantly trying to break the security of your environment.  
B. APIs can’t ever be secure.  
C. Hackers are constantly infiltrating all APIs.  
D. Users enhance their productivity however they can.  
Answer: D. 

**Users in the production environment will leverage whatever tools and techniques they can in order to get their job done in a better, faster way, often regardless of whether this complies with security policies**.

All the other options are untrue and therefore cannot be the correct answer. For test-taking purposes, be very suspicious of words like, “constantly” and “can’t ever” in answer choices.

### Question # 26 - Some current software developers are not aware of security problems within the programs they’re creating because _______________.     

A. Young programmers are not nearly as disciplined in their coding practices as older programmers.                            

B. Some current programmers don’t write code line by line and instead use code component libraries.  

C. Coding languages have not been secure for 20 years. 

D. Users are not clear in defining their requirements at the outset of the software development lifecycle (SDLC).   

Answer: B.   

Because many programs are currently constructed from “building block” components found in code libraries, any security issues within specific components may not be understood or identified by coders who don’t know the code inside the component.

Option A is an unfair generalization.
Option C is another broad generalization that may or may not be true. Option B is a better answer.
Option D does not relate to the question about the SDLC and is therefore a poor choice for an answer.

### Question # 27 - What is the most secure form of code testing and review?   
A. Open source.   
B. Proprietary/internal.    
C. Neither open source nor proprietary.     
D. Combination of open source and proprietary.     
Answer: D.      

Obviously, using multiple forms of code review will produce more secure results than any one form of review, in the same way that having multiple forms of security controls (physical, logical, administrative, etc.) will provide better security than just one type.
The question is which is the “most” secure form of code testing and review. That would be the most extensive. Since the correct answer is a combination of open source and proprietary, the least secure would be least extensive. Option A is strictly open source so that is incorrect. Option C is neither open source nor proprietary, which is even less extensive. Option C is incorrect. Proprietary/internal is also less extensive than Option D. So Option B is incorrect.
	
### Question # 28 - What is the major difference between authentication and authorization?     
A. Code verification/code implementation.   
B. Identity validation/access permission.   
C. Inverse incantation/obverse instantiation.    
D. User access/privileged access.    
Answer: B.     

This is the textbook definition of these terms. All the other options are incorrect answers.

### Question # 29. Access should be based on _______________.  
A. Regulatory mandates.   
B. Business needs and acceptable risk.   
C. User requirements and management requests.    
D. Optimum performance and security provision.    

Answer: B. 

Business needs and risk acceptable to senior management should drive all organizational decisions, including access. Specific user or object access will, of course, be delegated down from senior management to a manageable layer of the organization, but the principle applies.
This decision, however, should be informed by pertinent externalities, which include regulatory mandates (option A), user requirements and management requests (option C), and, to some degree, the trade-off of performance and security (option D, and both characteristics should also be dictated by senior management as an aspect of acceptable risk). While these externalities and options all play a part in determining appropriate access, they are all subordinate to business needs and acceptable risk, which are paramount; B is still the best answer to this question.
	
### Question # 30 - Who should determine which users have access to which specific objects?    
A. The cloud provider.    
B. Senior management.    
C. Data owners.    
D. System administrators.    
Answer: C.    

The data owner is responsible for the disposition of the data under their control; this includes access decisions.
The cloud provider is not typically the data owner; option A is incorrect.
Ostensibly, senior management is the data owner (the organization, as a whole, is the legal owner of the data, and the senior managers are the legal representatives of the organization). However, in practice, this responsibility can be (and usually is) delegated down to a manageable level, where the data owner for a given data set understands it best and can provide a sufficiently granular control of that data set. This is rarely senior management and is more likely department heads, branch managers, or some other form of middle management. 

Option C is preferable to B.
System administrators will usually be the literal granters of access, insofar as admins will modify access control systems that allow or disallow access for specific individuals or roles. 

However, the sysadmin does not make the decision of who is granted access and instead responds to direction from data owners (middle management); again, option C is preferable to D.
	
### Question # 31 - All of the following are identity federation standards commonly found in use today except _______________.  
A. WS-Federation. 
B. OpenID. 
C. OAuth (Open Authorization). 
D. Pretty Good Privacy (PGP). 
Answer: D. 

PGP is an email encryption tool, not an identity federation standard. All the other options are federation standards.
	
### Question # 32 - Which of the following is a federation standard/protocol that does not rely on Simple Object Access Protocol (SOAP), Security Assertion Markup Language (SAML), or Extensible Markup Language (XML)?  
A. WS-Federation. 
B. OpenID Connect. 
C. Service Organization Control (SOC) 2. 
D. Open Web Application Security Project (OWASP). 
Answer: B. 

OpenID Connect is a federation protocol that uses representational state transfer (REST) and JavaScript Object Notation (JSON); it was specifically designed with mobile apps in mind, instead of only web-based federation.
WS-Federation is a federation protocol that is part of the WS-Security family of standards and reliant on Simple Object Access Protocol (SOAP), so option A is incorrect.
Option C is incorrect; SOC 2 is a type of Statement on Standards for Attestation Engagements (SSAE) 18 audit report, not a federation standard.
OWASP is a volunteer group of and for web app developers, not a federation standard or protocol, so option D is incorrect.
	
### Question # 33 - Authentication mechanisms typically include any or all of the following except _______________.  
A. Something you know. 
B. Someone you know. 
C. Something you have. 
D. Something you are. 
Answer: B. 

Because there is no transitive property of identification and authentication, knowing a trusted entity is not sufficient for validating an identity assertion.
All the other options are typical authentication mechanisms and so are incorrect.
	
### Question # 34 - Which of the following constitutes a multifactor authentication process or procedure?     
A. Using an automated teller machine (ATM) to get cash with your credit or debit card. 
B. Using a password and personal identification number (PIN) to log into a website. 
C. Presenting a voice sample and fingerprint to access a secure facility. 
D. Displaying a birth certificate and a credit card. 
Answer: A. 

At the ATM, the customer will use the card (something you have) and enter a PIN (something you know). This is true multifactor authentication.
A password and PIN are both something you know, so option B is incorrect.
Using a voice sample and fingerprint are two forms of something you are, so option C is incorrect.
A birth certificate and credit card are both something you have, so option D is incorrect.
	
### Question # 35 - Typically, multifactor authentication should be used _______________.   
A. In every IT transaction. 
B. For high-risk operations and data that is particularly sensitive. 
C. When remote users are logging into the cloud environment. 
D. Only in the traditional environment. 
Answer: B. 

Multifactor authentication should be considered for operations that have a significant risk or that deal with highly sensitive data (for instance, privileged user logins or when handling financial transactions).
Requiring multifactor authentication for every transaction is an undue burden on both the users and the systems and is a needless addition of extra overhead, so option A is incorrect.
All cloud access will entail remote login; this is a common operation, so adding multifactor authentication is an unnecessary burden in most cases. Option C is incorrect.
The decision to use multifactor authentication should be based on the risk of the operation and the sensitivity of the data, not on whether it takes place in the traditional or online environment, so option D is incorrect.
	
### Question # 36 - A web application firewall (WAF) usually operates at Layer _______________ of the Open Systems Interconnection (OSI) model.   
A. 2.  
B. 3.  
C. 7.  
D. Q.  
Answer: C. 

A WAF is a Layer 7 tool.
All the other options are incorrect.

### Question # 37 - A web application firewall (WAF) can understand and act on _______________ traffic.  
	A. Malicious. 
	B. Simple Mail Transfer Protocol (SMTP). 
	C. Internet Control Message Protocol (ICMP). 
	D. Hypertext Transfer Protocol (HTTP).  
Answer: D. 

WAFs recognize HTTP traffic and can respond to traffic that matches prohibited rulesets or conditions.
Option A is technically correct; a WAF can be given a ruleset that recognizes certain forms of attack traffic. However, this answer is too general, and D is a much better response for this question.
Options B and C are protocols not usually inspected by WAFs and are therefore incorrect.
	
### Question # 38 - WAFs can be used to reduce the likelihood that _______________ attacks will be successful.  
A. Social engineering. 
B. Physical theft. 
C. Obverse inflection. 
D. Cross-site scripting. 
Answer: D. 

WAFs can be used to attenuate the possibility that cross-site scripting attacks will be successful.
WAFs do not protect against social engineering or physical attacks in any way, so options A and B are incorrect.
Option C is a nonsense term and is therefore incorrect.
	
### Question # 39 - A database activity monitor (DAM) tool usually operates at Layer _______________ of the Open Systems Interconnection (OSI) model.  
A. 2. 
B. 3. 
C. 7. 
D. Q. 
Answer: C. 

A DAM is a Layer 7 tool.
All the other options are incorrect.
	
### Question # 40 - Database activity monitors (DAMs) can be used to reduce the potential success of _______________ attacks.   
A. SQL injection. 
B. Cross-site scripting. 
C. Insecure direct-object reference. 
D. Social engineering. 
Answer: A. 

DAMs can be used to reduce the possibility that SQL injection attacks will be successful.
DAMs do not protect against cross-site scripting, insecure direct-object reference, or social engineering attacks in any way, so options B, C, and D are incorrect.
	
### Question # 41 - Which security tool can perform content inspection of Secure File Transfer Protocol (SFTP) communications?  
A. Web application firewall (WAF). 
B. Database activity monitor (DAM). 
C. Extensible Markup Language (XML).   gateway.  
D. Single sign-on (SSO).  
Answer: C. 

The XML gateway can provide this functionality; it acts as a reverse proxy and can perform content inspection on many traffic protocols.
The WAF and DAM are also security tools that inspect traffic but do not usually handle SFTP content, so options A and B are incorrect.
Option D, single sign-on, concerns authentication functions, not communications traffic, and is only a distractor in this context.
	
### Question # 42 - To deploy a set of microservices to clients instead of building one monolithic application, it is best to use a(n) _______________ to coordinate client requests.   
A. Extensible Markup Language (XML) gateway. 
B. Application programming interface (API) gateway. 
C. Web application firewall (WAF). 
D. Database activity monitor (DAM). 
Answer: B. 

An API gateway translates requests from clients into multiple requests to many microservices and delivers the content as a whole via an API it assigns to that client/session.
XML gateways, WAFs, and DAMs are also tools used frequently in cloud-based enterprises, but they do not handle microservice requests in a meaningful way.
	
### Question # 43 - Firewalls can detect attack traffic by using all these methods except _______________.  
A. Known past behavior in the environment. 
B. Identity of the malicious user. 
C. Point of origination. 
D. Signature matching. 
Answer: B. 

While it would be wonderful, for security purposes, to know the identity of attackers before or while they’re making an attack, this is information the attacker doesn’t usually share.
All the other options are methods firewalls can use to recognize attacks.
	
### Question # 44 - Transport Layer Security (TLS) provides _______________ and _______________ for communications.  
A. Privacy, security. 
B. Security, optimization. 
C. Privacy, integrity. 
D. Enhancement, privacy. 
Answer: C. 

TLS maintains the confidentiality and integrity of communications, often between a web browser and a server.
In this context, privacy and security mean much the same thing; privacy is synonymous with confidentiality, which is a subset of the overall topic of security. Therefore, option A is repetitive and not correct.
TLS does not optimize performance or add any sort of enhancement, so options B and D are incorrect.
	
### Question # 45 - Transport Layer Security (TLS) uses a new _______________ for each secure connection.   
A. Symmetric key. 
B. Asymmetric key. 
C. Public-private key pair. 
D. Inverse comparison. 
Answer: A. 

TLS uses symmetric key crypto for each communications session in order to secure the connection; the session key is uniquely generated each time a new connection is made.
Options B and C are names for another type of encryption. Asymmetric encryption is also used in establishing a secure TLS connection; however, the keys used in this portion of the process will not change from session to session, and therefore these options are incorrect.
Option D is a nonsense term and is therefore incorrect.
	
### Question # 46 - A virtual private network (VPN) is used to protect data in transit by _______________.   
A. Securing each end of a client-server connection. 
B. Creating an encrypted tunnel between two endpoints. 
C. Encrypting databases. 
D. Restricting key access to only eight parties. 
Answer: B. 

A VPN is a temporary, synthetic encrypted tunnel between two endpoints (often a client and a server).

Option A is subtly misleading; the VPN secures the connection between two endpoints, not the ends of the connection. This option is incorrect.

Option C is not correct; VPN is not used for encrypting databases—it is used for encrypting communications.

Option D is incorrect; the symmetric key used in VPN is shared only between two parties (the endpoints), and the elements of the asymmetric key pair are either held by only one party (the owner of each private key) or by anyone at all (public key).
	
### Question # 47 - The employment of users in dynamic software testing should best be augmented by _______________.   
A. Having the developers review the code. 
B. Having the developers perform dynamic testing. 
C. Using automated agents to perform dynamic testing. 
D. Social engineering. 
Answer: C. 

Users may not offer enough coverage for larger software products that have a great deal of functionality; it can be useful to also use automated agents to checks paths that users might not often attempt or utilize.
The developers should not be involved in any form of testing the software as they have an inherent conflict of interest, so options A and B are incorrect.
Dynamic testing does not involve social engineering; option D is incorrect.
	
### Question # 48 - Why do developers have an inherent conflict of interest in testing software they’ve created?   
A. They are notoriously bad, as a group, at testing.   
B. They work for the same department as the testing personnel.   
C. They have a vested interest in having the software perform well.   
D. They are never trained on testing procedures.   
Answer: C. 

This is the definition of “conflict of interest.”
All the other answers are incorrect.
	
### Question # 49 - Sandboxing can often be used for _______________.   
A. Optimizing the production environment by moving processes that are not frequently used into the sandbox. 
B. Allowing secure remote access for users who need resources in the cloud environment.  
C. Running malware for analysis purposes. 
D. Creating secure subnets of the production environment. 
Answer: C. 

A sandbox can be used to run malware for analysis purposes as it won’t affect (or infect) the production environment; it’s worth noting, though, that some malware is sandbox-aware, so additional anti-malware measures are advisable.
Options A, B, and D are not correct because the sandbox should be completely disconnected (air-gapped) from the production environment so that users can’t perform productive activity there.
	
### Question # 50. Sandboxing can often be used for _______________.      
A. Testing user awareness and training   
B. Testing security response capabilities    
C. Testing software before putting it into production    
D. Testing regulatory response to new configurations and modifications    
Answer: C. 

Software that has either been purchased from a vendor or developed internally can be tested in a sandboxed environment that mimics the production environment in order to determine whether there will be any interoperability problems when it is installed into actual production.
All the other options aren’t uses for sandboxes and are incorrect.
	
### Question # 51 - Application virtualization can typically be used for _______________.       
A. Running an application in a non-native environment    
B. Installing updates to a system’s operating system (OS)    
C. Preventing escalation of privilege by untrusted users    
D. Enhancing performance of systems    
Answer: A. 

Virtualized applications can run on platforms that wouldn’t otherwise allow them to function, such as running Microsoft apps on a Linux box.
Because the virtualization engine encapsulates the application from the native runtime environment, patches can’t be applied through virtualized programs; option B is incorrect.
Virtualization really doesn’t have anything to do with access control; option C is incorrect.
The overhead of running a software virtualization engine will actually add to system overhead, not decrease it, so option D is incorrect.
	
### Question # 52. Application virtualization can typically be used for _______________.         
A. Denying access to untrusted users    
B. Detecting and mitigating distributed denial of service (DDoS) attacks    
C. Replacing encryption as a necessary control    
D. Running an application on an endpoint without installing it    
Answer: D. 

Application virtualization allows the software to run on a simulated environment on the device without the need to install it on the device. 
Virtualization really doesn’t have anything to do with access control; option A is incorrect.
Virtualization neither detects nor responds to DDoS; option B is incorrect.
Virtualization does not replace encryption; if data needs to be secure within the virtualization environment, encryption may still have to be utilized. Option C is incorrect.
 
### Question # 53. Any organization that complies with ISO 27034 will have a maximum of _______________ Organizational Normative Framework(s) (ONF)(s).     
A. 0   
B. 1    
C. 5    
D. 25    
Answer: B.    

ISO 27034 dictates that an organization will have a collection of security controls used for all software within that organization; this collection is called the ONF.
All the other options are distractors and incorrect.
	
### Question # 54. Under ISO 27034, every application within a given organization will have an attendant set of controls assigned to it; the controls for a given application are listed in the _______________.      
A. ONF    
B. ANF    
C. TTF    
D. FTP    
Answer: B.     

Each application in an organization compliant with ISO 27034 will be assigned an Application Normative Framework (ANF), which lists all the controls assigned to that application.
Technically, the controls for each application within an organization compliant with ISO 27034 will be listed in the Organizational Normative Framework (ONF), because the ONF is the list of all controls for all applications; however, for a given application, only the controls used for that application are listed in an ANF, so option B is a preferable answer to A.
TTF (time to failure) has no meaning in this context, so option C is incorrect.
FTP (File Transfer Protocol) is a protocol for transferring files and not applicable here; option D is incorrect.
	
### Question # 55. Static application security testing (SAST) is usually considered a _______________ form of testing.       
A. White-box   
B. Black-box    
C. Gray-box    
D. Parched field    
Answer: A. 

SAST is often referred to as white-box testing.
Black-box testing does not include access to source code, which is required for SAST. Option B is therefore incorrect.
Option C is a combination of black-box and white-box testing so option C is an incorrect answer for this question.
Option D has no meaning in this context.
	
### Question # 56. Static application security testing (SAST) examines _______________.       
A. Software outcomes    
B. User performance    
C. System durability    
D. Source code    
Answer: D. 

In SAST, testers review the source code of an application in order to determine security flaws and operational errors.
While determining “software outcomes” may be considered a possible goal of SAST, “source code” is a much better answer as it is more specific and applicable to the question. Option D is still preferable.
SAST does not check user performance or system durability; options B and C are incorrect.
	
### Question # 57. Dynamic application security testing (DAST) is usually considered a _______________ form of testing.      
A. White-box    
B. Black-box    
C. Gray-box    
D. Parched field    
Answer: B. 

DAST is often referred to as black-box testing.
White-box testing requires the tester to have access to source code, which is not provided in DAST. Option A is therefore incorrect.
Option C is a combination of black-box and white-box testing so option C is an incorrect answer for this question.
Option D has no meaning in this context.
	
### Question # 58. Dynamic application security testing (DAST) checks software functionality in _______________.       
A. The production environment    
B. A runtime state    
C. The cloud    
D. An IaaS configuration    
Answer: B.     

DAST is performed while the application is running.
Software testing should not take place in the production environment; option A is incorrect.
DAST, like other forms of testing, may or may not take place in the cloud and is not confined to any particular service model (although it is unlikely to occur in software as a service [SaaS] environments); options C and D are incorrect.
	
### Question # 59. Vulnerability scans are dependent on _______________ in order to function.      
A. Privileged access    
B. Vulnerability signatures    
C. Malware libraries    
D. Forensic analysis    
Answer: B.    

Vulnerability scans use signatures of known vulnerabilities to detect and report those vulnerabilities.
Vulnerability scans do not typically require administrative access to function; option A is incorrect.
Both malware libraries and forensic analysis of existing vulnerabilities may be used to create the signatures that vulnerability scanning tools utilize to detect and report vulnerabilities; however, these answers are too specific (limiting the answer), making option B a better answer than either C or D.
	
### Question # 60. Due to their reliance on vulnerability signatures, vulnerability scanners will not detect _______________.      
A. User error    
B. Improper control selection    
C. Cloud vulnerabilities   
D. Unknown vulnerabilities     
Answer: D.    

Because vulnerability scanning tools require vulnerability signatures to operate effectively, unknown vulnerabilities that might exist in the scanned system won’t be detected (no signature has been created by vendors until a vulnerability is known). User errors are not detected by vulnerability scans; option A is incorrect. Scans can’t tell you whether you’ve picked the optimum security controls for your environment; option B is incorrect. Vulnerability scanning tools may or may not detect cloud-based vulnerabilities, depending on the tool used, the level of access to the target environment, and the settings applied to the scanner; option C is less accurate than option D.

### Question # 61. Penetration testing is a(n) _______________ form of security assessment.       
A. Active    
B. Comprehensive    
C. Total    
D. Inexpensive    
Answer: A. 

A penetration test requires the tester to analyze the security of an environment from the perspective of an attacker; this also includes actually taking action that would result in breaching that environment.
Penetration tests may or may not be comprehensive, depending on the intended scope and area of analysis. Option B is incorrect.
While it’s nice to think of any security assessment as total, that is an extreme term, like all or never; such terms can rarely be used in security because there are no absolutes when dealing with risk, and it has no meaning in this context. Option C is not correct.
Although the cost of a penetration test will vary according to a vast range of variables, it will rarely be considered inexpensive, especially relative to other forms of security testing. Option D is not correct.
	
### Question # 62. Dynamic software security testing should include _______________.      
A. Source code review    
B. User training    
C. Penetration testing    
D. Known bad data    
Answer: D. 

Also called fuzz testing, dynamic testing methods should include known bad inputs in order to determine how the program will handle the “wrong” data (will it fail into a state that is less secure than normal operations, etc.).
Source code review is not part of dynamic testing; option A is incorrect.
For accurate quality testing, user familiarity with the target software should be minimal and should not be assessed; option B is not correct.
Penetration includes active steps to overcome security measures; this is rarely the purpose of software testing; option C is not the best answer.
	
### Question # 63. According to Open Web Application Security Project (OWASP) recommendations, active software security testing should include all of the following except _______________.          
A. Information gathering   
B. User surveys   
C. Configuration and deployment management testing    
D. Identity management testing    
Answer: B. 

User surveys are not an element of active security testing, although they might be used in acceptance testing. All of the other options are included in the OWASP guide to active security testing.
	
### Question # 64. According to Open Web Application Security Project (OWASP) recommendations, active software security testing should include all of the following except _______________.      
A. Authentication testing   
B. Authorization testing    
C. Session management testing   
D. Privacy review testing    
Answer: D. 

Privacy review testing is not included in the OWASP guide to active security testing, although it might be included as an aspect of compliance testing (for organizations in highly regulated industries). All of the other options are included in the OWASP guide to active security testing.
	
### Question # 65. According to Open Web Application Security Project (OWASP) recommendations, active software security testing should include all of the following except _______________.       
A. Session initiation testing   
B. Input validation testing    
C. Testing for error handling    
D. Testing for weak cryptography     
Answer: A. 

While session management testing is included in the OWASP guide to active software security testing, session initiation is not. All of the other options are included in the OWASP guide to active security testing.
	
### Question # 66. According to Open Web Application Security Project (OWASP) recommendations, active software security testing should include all of the following except _______________.      
A. Business logic testing   
B. Client-side testing   
C. Intuition testing   
D. Information gathering    
Answer: C.     

Intuition testing is not part of the OWASP guide to active security testing. All of the other options are included in the OWASP guide to active security testing.
	
### Question # 67. Static software security testing typically uses _______________ as a measure of how thorough the testing was.     
A. Number of testers    
B. Flaws detected    
C. Code coverage    
D. Malware hits    
Answer: C.     

This metric is usually expressed as a percentage of lines of code. For example, “SAST covered 90% of the source code.”
The number of testers involved means very little when discussing testing coverage; this is a distractor and not correct.
In some cases, testing reports might include a statistic representing the number of flaws discovered in the code; however, this is usually not a pertinent metric (undetected flaws can’t be measured, so counting the ones that have doesn’t add to your surety the code is secure), and code coverage is used more often. Option C is preferable to option B.
Testing should first occur in an environment where the software has not even been exposed to the possibility of malware infection. Option D is incorrect.

### Question # 68. Dynamic software security testing typically uses _______________ as a measure of how thorough the testing was.      
A. User coverage    
B. Code coverage    
C. Path coverage    
D. Total coverage     
Answer: C. 

In dynamic software security testing, the objective is to test a significant sample of the possible logical paths from data input to output.
User coverage is a distractor and has no real meaning in this context; option A is incorrect.
Code coverage is the metric used in static testing, making option B incorrect.
While it would be nice to test each and every data pathway through an application, with both known good and known bad data, that could be unrealistic, depending on the number of possible branches in the application; this goes up exponentially every time another option/choice is added to the program. Total coverage is not a metric—it’s a hope. Option D is incorrect.

### Question # 69. Software security testing should involve both known good and known bad data in order to simulate both _______________ and _______________.     
A. Managers, users    
B. Regulators, users   
C. Vendors, users    
D. Users, attackers     
Answer: D. 

Known good data is used to determine if the software fulfills the business requirements for which it was acquired. Known bad data tests the ability of the software to handle inputs and conditions that might put it into a fail state; these inputs and conditions can be invoked either purposefully (by attackers) or inadvertently (by users who make mistakes).
Testing does not attempt to mimic managers, regulators, or vendors, so the other answers are incorrect.

### Question # 70. Training programs should be tracked and monitored in order to fulfill both _______________ and _______________ requirements. Choose the best response.     
A. Business, security    
B. Regulatory, legal    
C. User, managerial    
D. Vendor, supplier    
Answer: B. 

This is not a simple question, and more than one answer could be construed as correct, but option B is the best answer. Tracking and monitoring personnel training is absolutely vital in order to demonstrate regulatory requirements (and many, if not all, organizations are obligated to comply with some regulation that mandates user training) and legal requirements (as an element of due diligence in the modern workplace).
Option A is the other answer that could be perceived as accurate, but there is a bit of nuance that makes it less preferable than B. Security is a business requirement—it may not be a functional requirement, but it is a requirement nonetheless. Therefore, these two terms are repetitive; security requirements are just a subset of business requirements. Option B is still the better answer.
Options C and D do not make sense in this context.

### Question # 71. Task-centric training is typically for _______________.         
A. All personnel    
B. Specific personnel    
C. Management personnel     
D. HR personnel     
Answer: B. 

Training is usually a formal process involving detailed information. This is for those personnel who are involved with the specific topic or task for which the training is intended (for example, personnel involved in business continuity and disaster recovery [BC/DR] activities should get specific, detailed training on how to perform those actions).
Option A incorrect because not all personnel require task-centric training. Training required for all personnel in an organization cannot be task-centric training, by definition (not all personnel perform the same tasks).
Options C and D are incorrect because they would only answer a subset of the question. Management personnel would receive management training and HR personnel would receive HR training. The correct answer is task-centric training is for specific personnel.
 
 ### Question # 72. Awareness training is typically for _______________.     
A. All personnel    
B. Specific personnel     
C. Management personnel    
D. HR personnel     
Answer: A. 

Awareness efforts are usually intended to reach as wide an audience as possible within the organization, for generalized information. For instance, fire drills are awareness exercises; everyone in the facility needs to know how to get out and where to go.
Specific personnel, management personnel, and HR personnel would all receive task-centric training in addition to the awareness instruction that all personnel receive. Options B, C, and D are incorrect.

### Question # 73. Why is cloud security training particularly important for software developers?
A. Software developers are the mainstay of every cloud environment.     
B. You can’t have a cloud environment without software developers.    
C. Security controls cannot be added to software after the fact and must be included from the very first steps of software development.     
D. Many modern software developers don’t understand how the code underlying the libraries they use actually works.     
Answer: D.    

Modern developers usually aren’t writing code—they are recombining library components in novel ways to create new functionality. They may not understand the security risks associated with their work, especially for the cloud environment, which entails a different set of challenges from the traditional environment, which the developers might be more familiar with.
Options A and B are actually the same concept, reworded, which is patently untrue: depending on the cloud deployment and service models the organization chooses to use, software developers may or may not be crucial (for instance, in a software as a service [SaaS] public cloud, many organizations won’t even need internal development teams).
Option C is just wrong: security controls can be added to software after it has been fielded. This is just not a best practice, as it is usually less effective and more expensive (in terms of both money and overhead).

### Question # 74. Software developers should receive cloud-specific training that highlights the challenges involved with having a production environment that operates in the cloud. One of these challenges is _______________.     
A. The massive additional hacking threat, especially from foreign sources     
B. The prevalent use of encryption in all data life-cycle phases    
C. Drastic increase of risk due to distributed denial of service (DDoS) attacks      
D. Additional regulatory mandates     
Answer: B. 

Because cloud operations are so dependent on encryption protections in all data life-cycle phases, developers will have to accommodate the additional overhead and interoperability encryption requires.
The hacking threat (foreign or otherwise) does not change whether the target is the cloud or the (connected) traditional environment; option A is incorrect.
Likewise, the threat of DDoS attacks does not increase; if anything, it may decrease, because the cloud provider may be more resistant to such attacks than individual organizations would be. Option C is not correct.
Regulatory requirements may or may not change when moving into the cloud. Moreover, developers are not likely to be the ones interpreting and responding to these new mandates; that is a level of abstraction above developer insight into software requirements. Option D is not preferable to B.

### Question # 75. Software developers should receive cloud-specific training that highlights the challenges involved with having a production environment that operates in the cloud. One of these challenges is _______________.     
A. Lack of management oversight    
B. Additional workload in creating governance for two environments (the cloud data center and client devices)    
C. Increased threat of malware     
D. The need for process isolation    
Answer: D. 

Because shared resources in the cloud may mean increased opportunity for side-channel attacks, developers will have to design programs to function in a way that ensures process isolation.
Management oversight should not change from a policy perspective, regardless of where the processing is taking place; option A is incorrect.
There is no additional workload resulting from cloud migration; in fact, the load should decrease, because the cloud customer cannot impose governance on the cloud provider. Option B is wrong.
Malware threat does not increase or decrease in the cloud environment; option C is incorrect.

### Question # 76. Which security technique is most preferable when creating a limited functionality for customer service personnel to review account data related to sales made to your clientele?     
A. Anonymization   
B. Masking    
C. Encryption    
D. Training   
Answer: B. 

Masking allows customer service representatives to review clients’ sales and account information without revealing the entirety of those records (for instance, obscuring credit card numbers except for the last four digits).
Anonymization strips out identifying information from a record. This would not aid in limiting customer service personnel from viewing sensitive data, but it would make it impossible for customer service personnel to know who they were communicating with and leave them unable to identify customers, which would defeat the purpose of their existence. Option A is incorrect.
Encryption of sales/account records would not limit customer service personnel in their review of account records. It would either disallow them to see the records at all or allow them to see the entirety of the records (depending on whether the representatives were given keys to that encrypted data). Option C is incorrect.
Training does not limit access; option D is incorrect.

### Question # 77. At which phase of the software development lifecycle (SDLC) is user involvement most crucial?     
A. Define    
B. Design    
C. Develop    
D. Test    
Answer: A. 

While some development models allow for user involvement in the entirety of the process, user input is most necessary in the Define phase, where developers can understand the business/user requirements—what the system/software is actually supposed to produce, in terms of function and performance. All the other options are beneficial phases to gauge user input, but not as crucial as option A.

### Question # 78. At which phase of the software development lifecycle (SDLC) should security personnel first be involved?     
A. Define    
B. Design    
C. Develop     
D. Test    
Answer: A.     

The earlier security inputs are included in the project, the more efficient and less costly security controls are overall. The Define phase is the earliest part of the SDLC. All the other options are later phases and incorrect.

### Question # 79. At which phase of the software development lifecycle (SDLC) is it probably most useful to involve third-party personnel?
A. Define    
B. Design    
C. Develop    
D. Test    
Answer: D.    

During testing, getting outside perspective is invaluable, for both performance and security purposes; internal development and review capabilities are enhanced by augmentation from external parties.
All the other phases are not normally appropriate for external participation.

### Question # 80. In software development lifecycle (SDLC) implementations that include a Secure Operations phase, which of the following security techniques or tools are implemented during that phase?    
A. Vulnerability assessments and penetration testing    
B. Performance testing and security control validation    
C. Requirements fulfillment testing    
D. Threat modeling and secure design review       
Answer: A. 

Once the system is deployed operationally, continuous security monitoring, including periodic vulnerability assessments and penetration testing, is recommended. All the other options are security functions that should take place in phases prior to the system’s deployment.

### Question # 81. A cloud environment that lacks security controls is vulnerable to exploitation, data loss, and interruptions. Conversely, excessive use of security controls _______________.      
A. Can lead to data breaches    
B. Causes electromagnetic interference   
C. Will affect quality of service    
D. Can cause regulatory noncompliance     
Answer: C. 

Security and operations are always inversely related; excessive controls necessarily degrade performance.
Excessive use of controls should not lead to more data breaches; if anything, it may reduce their occurrence. However, it is more likely that there will be no effect. Option A is incorrect.
Many controls don’t affect the electromagnetic spectrum in any way. Option B is incorrect.
Regulations don’t usually mandate a maximum set of controls but rather a minimum. Option D is incorrect.

### Question # 82. A cloud environment that lacks security controls is vulnerable to exploitation, data loss, and interruptions. Conversely, excessive use of security controls _______________.    
A. Can lead to distributed denial of service (DDoS)   
B. Allows malware infections    
C. Increases the risk of adverse environmental effects    
D. Is an unnecessary expense     
Answer: D. 

From a simple financial perspective (which is often the managerial perspective), money spent on excessive anything is money wasted; spending to no good effect is detrimental.
Overuse of controls should not result in greater risks of DDoS, malware, or environmental threats in any way. Options A, B, and C are incorrect.

### Question # 83. A cloud environment that lacks security controls is vulnerable to exploitation, data loss, and interruptions. Conversely, excessive use of security controls _______________.    
A. Can lead to customer dissatisfaction    
B. Is a risk to health and human safety     
C. Brings down the organization’s stock price     
D. Negates the need for insurance     
Answer: A. 

If excessive controls impact the user/customer experience to the extent that system response speeds and results are delayed significantly, and performance is degraded to the point where competitors’ systems are far superior, customer dissatisfaction can be a severe problem.
Some security controls (particularly physical controls) can affect health and human safety, such as if extraneous fencing/walls/barriers are put in place to control access/egress, and this hinders emergency escape from facilities. However, not all security controls pose this risk, so option B is a bit too specific; option A is still preferable.
Security controls should not affect stock price or, in and of themselves, negate insurance needs (risk mitigation does not automatically offset the benefits of risk transference). Options C and D are incorrect.

### Question # 84. You are the security manager for an online retail sales company with 100 employees and a production environment hosted in a platform as a service (PaaS) model with a major cloud provider. According to your company policies, personnel are allowed to work equally from the company offices and their own homes or other locations, using their personal IT devices. The policies also dictate which application programming interfaces (APIs) can be used to access and manipulate company data and the process for getting an API added to the list of approved programs. You conduct an approved scan of the company data set in the cloud, with the provider’s permission. This allows you to catalog all APIs that have accessed and manipulated company data through authorized user accounts in the last month. The scan reveals that 300 different APIs were used by authorized personnel. Of these, 30 had been approved by the company and were on the list. Of the following, what is the most reasonable immediate action?    
A. Delete accounts of all users who had utilized unapproved APIs to access company data.      
B. Suspend access for all users who had utilized unapproved APIs to access company data.     
C. Block all unapproved APIs from accessing company data.     
D. Notify whomever you report to in the company hierarchy, and suggest bringing the matter to the attention of senior management immediately.     
Answer: D.     

The problem in this case is not so much that policies have been violated or that, in a more literal sense, the unapproved APIs are being used to access the data, the problem is that the violations are so pervasive and extensive that taking any immediate direct action (such as the responses in options A, B, and C) might interfere with business activity in a drastic and potentially harmful way. Because of this, the matter needs to be dealt with as a business decision and requires that senior management make a determination before action is taken.

### Question # 85. You are the security manager for an online retail sales company with 100 employees and a production environment hosted in a platform as a service (PaaS) model with a major cloud provider. According to your company policies, personnel are allowed to work equally from the company offices and their own homes or other locations, using their personal IT devices. The policies also dictate which application programming interfaces (APIs) can be used to access and manipulate company data and the process for getting an API added to the list of approved programs. You conduct an approved scan of the company data set in the cloud, with the provider’s permission. This allows you to catalog all APIs that have accessed and manipulated company data through authorized user accounts in the last month. The scan reveals that 300 different APIs were used by authorized personnel. Of these, 30 had been approved by the company and were on the list. You’ve brought the matter to the attention of the chief executive officer (CEO), who understands the issue and asks for your recommendation. What is probably the best suggestion?    
A. Gather more data about how users are utilizing the APIs and for what purposes.     
B. Delete accounts of all users who had utilized unapproved APIs to access company data.    
C. Suspend access for all users who had utilized unapproved APIs to access company data.    
D. Block all unapproved APIs from accessing company data.     
Answer: A. 

Again, before taking any action that might impact operations, it would probably be best to figure out the actual user needs being met by the unapproved APIs, and the severity of impact if they were removed from service, before performing the actions described in options B, C, and D.

### Question # 86. You are the security manager for an online retail sales company with 100 employees and a production environment hosted in a platform as a service (PaaS) model with a major cloud provider. According to your company policies, personnel are allowed to work equally from the company offices and their own homes or other locations, using their personal IT devices. The policies also dictate which application programming interfaces (APIs) can be utilized to access and manipulate company data and the process for getting an API added to the list of approved programs. You conduct an approved scan of the company data set in the cloud, with the provider’s permission. This allows you to catalog all APIs that have accessed and manipulated company data through authorized user accounts in the last month. The scan reveals that 300 different APIs were used by authorized personnel. Of these, 30 had been approved by the company and were on the list. Upon performing an information-gathering investigation at the behest of the chief executive officer (CEO), you determine that these APIs increased productivity 387 percent over the period since they were adopted, at a cost that is negligible compared to getting even one API through the company’s current approval process. What is your suggestion on how to handle the situation?     
A. Retroactively put all the APIs currently in use through the formal approval process, and require that all future APIs users want to install also get approved.   
B. Have the CEO waive formal approval processing for all APIs currently in use, granting them approval, but require all future APIs be approved through that process.  
C. Punish all employees who have installed or used any of the rogue APIs for violating company policy.     
D. Change the policy.     
Answer: D.    

It’s hard to argue with success; operational capability and security are always a trade-off, but this kind of productivity increase with little attendant cost is probably too good to pass up. It also seems evident that the existing policy is far too restrictive and limiting and that it is not being accepted by a significant number of users; trying to mandate its acceptance, and enforcing it with punitive measures, especially in the face of the overwhelming success of the violations, is most likely counter to the company’s overall interests. It is best to revisit the policy itself, determine why it didn’t meet user needs originally, and modify it so as to meet the demands of both the users and senior management (as well as whatever other externalities may have been the foundation of the policy). Options A, B, and C may be attractive, but they are all less preferable than D.

### Question # 87. You are the security manager for an online retail sales company with 100 employees and a production environment hosted in a platform as a service (PaaS) model with a major cloud provider. According to your company policies, personnel are allowed to work equally from the company offices and their own homes or other locations, using their personal IT devices. The policies also dictate which application programming interfaces (APIs) can be utilized to access and manipulate company data and the process for getting an API added to the list of approved programs. You conduct an approved scan of the company data set in the cloud, with the provider’s permission. This allows you to catalog all APIs that have accessed and manipulated company data through authorized user accounts in the last month. The scan reveals that 300 different APIs were used by authorized personnel. Of these, 30 had been approved by the company and were on the list. As a subject matter expert, what should you also recommend to the chief executive officer (CEO)?     
A. Reward the users who committed the infractions, for aiding the company even when they were violating the policy.     
B. Replace all the personnel that violated the policy, and have the new personnel use the new policy from their start of hire.      
C. Restrict user access to possible APIs.    
D. Augment the current set of security controls used by the company in order to offset risks posed by the anticipated use of even more APIs from unknown sources.    
Answer: D.   

APIs chosen by users may or may not have integral security and probably weren’t chosen according to how secure they are; because the company will continue to be exposed to additional risks from these (and future) APIs, additional security controls are absolutely necessary.
However, personnel actions and draconian enforcement efforts at this point would be pointless and vindictive, and probably counter to the company’s interests. Options A, B, and C are incorrect.

### Question # 88. You are the security manager for an online retail sales company with 100 employees and a production environment hosted in a platform as a service (PaaS) model with a major cloud provider. According to your company policies, personnel are allowed to work equally from the company offices and their own homes or other locations, using their personal IT devices. The policies also allow users to select which application programming interfaces (APIs) they install and use on their own devices in order to access and manipulate company data. Of the following, what is a security control you’d like to implement to offset the risk(s) incurred by this practice?     
A. Encrypt all routers between mobile users and the cloud.     
B. Use additional anti-malware detection capabilities on both user devices and the environment to which they connect.     
C. Implement strong multifactor authentication on all user-owned devices.      
D. Employ regular performance monitoring in the cloud environment to ensure that the cloud provider is meeting the service level agreement (SLA) targets.     
Answer: B.      

Because untrusted APIs may not be secured sufficiently, increased vigilance for the possibility of introducing malware into the production environment is essential.
It is impossible to encrypt devices that don’t belong to the organization. Option A is incorrect.
Securing access to user-owned devices is admirable, but it has no effect at all on securing the device (or production environment) from risks due to installed APIs; option C is incorrect.
This is a security question, and option D addresses performance; this is incorrect.

### Question # 89. You are the security manager for an online retail sales company with 100 employees and a production environment hosted in a platform as a service (PaaS) model with a major cloud provider. According to your company policies, personnel are allowed to work equally from the company offices and their own homes or other locations, using their personal IT devices. The policies also allow users to select which application programming interfaces (APIs) they install and use on their own devices in order to access and manipulate company data. Of the following, what is a security control you’d like to implement to offset the risk(s) incurred by this practice?    
A. Regular and widespread integrity checks on sampled data throughout the managed environment     
B. More extensive and granular background checks on all employees, particularly new hires     
C. Inclusion of references to all applicable regulations in the policy documents.     
D. Increased enforcement of separation of duties for all workflows      
Answer: A.    

In order to detect possible erroneous or malicious modification of the organization’s data by unauthorized or security-deficient APIs, it’s important to take representative samples of the production data on a continual basis and perform integrity checks.
Additional personnel security measures will not, in this case, yield any relevant security benefit; options B and D are not correct.
It is always good to refer to regulations in policies; this isn’t something to be performed in response to the policy change but should have been included when the policy was created. Option C is incorrect.     

### Question # 90 - You are the security manager for an online retail sales company with 100 employees and a production environment hosted in a platform as a service (PaaS) model with a major cloud provider. According to your company policies, personnel are allowed to work equally from the company offices and their own homes or other locations, using their personal IT devices. The policies also allow users to select which application programming interfaces (APIs) they install and use on their own devices in order to access and manipulate company data. Of the following, what is a security control you’d like to implement to offset the risk(s) incurred by this practice?       
A. Enact secure connections between the user devices and the cloud environment using end-to-end encryption.   
B. Enact secure connections between the user devices and the cloud environment using link encryption.   
C. Employ additional user training.   
D. Tunnel all connections with a virtual private network (VPN).   
Answer: C.   

Additional user training would be helpful in this situation, particularly any information that helps users understand the reasons APIs from unknown sources might be less secure and the potential impacts from using them.
All the other answers are incorrect; securing the connection between endpoints and the cloud is irrelevant in protecting against risks caused by software installed on the client devices.

### Question # 91. Users in your organization have been leveraging application programming interfaces (APIs) for enhancing their productivity in the cloud environment. To ensure that you are securing API access to the production environment, you should deploy _______________ and _______________.    
A. Secure Sockets Layer (SSL) and message-level cryptography   
B. Transport Layer Security (TLS) and message-level cryptography    
C. SSL and whole drive encryption     
D. TLS and whole drive encryption    
Answer: B. 

Cryptography for the two main types of APIs is required; this is TLS for representational state transfer (REST) and message-level encryption for Simple Object Access Protocol (SOAP).
SSL has been deprecated because of severe vulnerabilities; this eliminates options A and C. Whole drive encryption protects against loss or theft of a device but does not secure API access to the data, which eliminates option D.

### Question # 92. You implement identity and access management (IAM) in order to control access between subjects and objects. What is the ultimate purpose of this effort?    
A. Identification. Determine who the specific, individual subjects are.
B. Authentication. Verify and validate any identification assertions.
C. Authorization. Grant subjects permissions to objects once they’ve been authenticated.
D. Accountability. Be able to reconstruct a narrative of who accessed what.
Answer: D. 

Accountability is the end purpose of all IAM efforts; all the other options are the elements of IAM that support this effort.

### Question # 93. _______________ is perhaps the main external factor driving identity and access management (IAM) efforts.    
A. Regulation   
B. Business need    
C. The evolving threat landscape   
D. Monetary value     
Answer: A.    

Regulatory compliance has historically driven IAM efforts. All the other options can to some extent drive IAM efforts, however, they do not have as much influence as regulatory factors. Therefore options B, C, and D are incorrect answers.

### Question # 94. Whether in a cloud or traditional environment, it is important to implement both _______________ and _______________ access controls.       
A. Internal and managed   
B. Provider and customer    
C. Physical and logical     
D. Administrative and technical    
Answer: C. 

Both physical and logical controls are possible (and necessary) to implement in both environments.
Options A and B are really only feasible if the organization is using a cloud service (or other managed service); the terms managed and provider suggest this. This makes these options less desirable for a question that also includes the traditional environment.
It is not reasonable to expect that the organization can impose administrative controls in a cloud environment (for the provider environment), so option D is not correct.

### Question # 95. Access to specific data sets should be granted by _______________.    
A. The data subjects    
B. The data owners    
C. The data processors    
D. The data regulators    
Answer: B.    

The data owner is most familiar with the risks and impacts associated with the data sets under their control.
The data subject may grant permission for a data owner to have the subject’s data but will not govern the granular assignment of access rights. Option A is incorrect.
The data processor does not have the right to grant data access and must only act at the direction of the data owner. Option C is incorrect.
Regulators dictate how data must be secured, and possibly in what manner, but do not supervise explicit access to that data. Option D is incorrect.

### Question # 96. Access should be granted based on all of the following except _______________.        
A. Policy    
B. Business needs   
C. Performance   
D. Acceptable risk   
Answer: C. 

Performance should not determine who gets access to which data; all the other options are the factors for making this determination.

### Question # 97. Federation allows _______________ across organizations.     
A. Role replication     
B. Encryption    
C. Policy    
D. Access   
Answer: D. 

Federation allows users from multiple member organizations to access resources owned by various members.
All the other answers are simply not correct.

### Question # 98. Federation should be _______________ to the users.      
A. Hostile    
B. Proportional    
C. Transparent    
D. Expensive    
Answer: C. 

Federation allows ease of use for access to multiple resource providers; this provides a transparent user mechanism.
The goal of federation is to enhance the user experience, the exact opposite of making the environment more hostile to them. Option A is incorrect.
Option B is incorrect because it is meaningless in this context.
Option D is incorrect. Users typically do not pay for the organization’s IT environment.

### Question # 99. A web application firewall (WAF) understands which protocol(s)?    
A. All protocols that use the Internet as a medium    
B. Transport Layer Security (TLS)   
C. Hypertext Transfer Protocol (HTTP)   
D. File Transfer Protocol (FTP)   
Answer: C. 

WAFs apply rulesets to web traffic, which uses HTTP. All the other answers are incorrect.

### Question # 100. Web application firewalls and database activity monitors function at levels _______________ and _______________ of the Open Systems Interconnection (OSI) model, respectively.          
A. 1 and 7.      
B. 7 and 1.      
C. 7 and 7.    
D. 3 and 4.     
Answer: C.     

These are both Layer 7 tools. All the other answers are incorrect.

### Question # 101. What can tokenization be used for?     
A. Encryption.     
B. Compliance with the Payment Card.  Industry Data Security Standard (PCI DSS).     
C. Enhancing the user experience.  
D. Giving management oversight to e-commerce functions.      
Answer: B.    

Aside from encryption, PCI DSS allows for tokenization as a means to protect account and cardholder data at rest.
Tokenization is not encryption; there is no encryption engine and no key involved in the process. Option A is incorrect.
Tokenization does not necessarily enhance or detract from the user experience; option C is incorrect.
Management is not allowed any additional oversight into any particular function by tokenization; option D is incorrect.

### Question # 102. Merchants who accept credit card payments can avoid some of the compliance burden for the Payment Card Industry Data Security Standard (PCI DSS) by outsourcing the tokenization function to _______________.    
A. A third party    
B. The data owner    
C. The data subject    
D. The PCI Security Standards Council    
Answer: A.    

By offloading privacy data to a tokenizing third party, merchants can free themselves of the contractual burdens for protecting cardholder data at rest.
The data owner is the merchants themselves, and the data subject is the person to whom the privacy data applies, so privacy data cannot be outsourced to either of these, and options B and C are incorrect.
The PCI Council is the body that promulgates and enforces the PCI DSS; they will not process data on behalf of any merchant. Option D is incorrect.

### Question # 103. Which of the following is an example of useful and sufficient data masking of the string “CCSP”?    
A. XCSP.    
B. PSCC.     
C. TtLp.     
D. 3X91.     
Answer: C.    

This answer requires some thought about how the original data is displayed and its properties.
Option A masks only one letter in a four-letter string; this is not sufficient because the original string could be identified with a very low-work factor, brute-force attack of only 26 possible combinations.
Option B is likewise easy to break; it only reverses the content of the string, which is very simple to determine, and would allow easy recovery of any other similar strings in the data set.
Option D mixes numeric characters into what was originally only an alphabetic string; this may detract from the utility of the string if the masked version is to be used for software testing.
Option C completely obscures the original content but retains the qualities of the original (all alphabetic characters). It may affect the use of the string by mixing uppercase and lowercase, but this is still the best choice of the four possible answers.

### Question # 104. A cloud-based sandbox should not be used for _______________.    
A. Application interoperability testing    
B. Processing sensitive data    
C. Application security testing    
D. Malware analysis    
Answer: D. 

Installing malware on systems owned by someone else may be illegal in many jurisdictions. While on-premises sandboxes are fine for this purpose, it may be a felony if performed in the cloud.
All the other options are good uses of cloud-based sandboxes.

### Question # 105. Which of the following should occur at each stage of the software development lifecycle (SDLC)?     
A. Added functionality     
B. Management review    
C. Verification and validation    
D. Repurposing of any newly developed components    
Answer: C.     

It is important to verify and validate the program at each stage of the SDLC.
Adding functionality at each stage of the SDLC is the definition of scope creep, which is what we’d like to avoid. Option A is incorrect.
Management should not have to shepherd software through the development process; this is the process of the development team. Option B is incorrect.
Option D is a distractor and makes no actual sense.

### Question # 106. Software that includes security elements from the outset of the software development lifecycle (SDLC) process will be _______________.    
A. More secure in deployment    
B. Less secure in deployment    
C. More likely to malfunction    
D. Less likely to malfunction    
Answer: A. 

It is important to verify and validate the program at each stage of the SDLC.
Adding functionality at each stage of the SDLC is the definition of scope creep, which is what we’d like to avoid. Option A is incorrect.
Management should not have to shepherd software through the development process; this is the process of the development team. Option B is incorrect.
Option D makes no sense: you can’t repurpose something that has just been developed.

### Question # 107. Software that includes security elements from the outset of the software development lifecycle (SDLC) process will _______________.     
A. Be less expensive to operate securely in the production environment    
B. Be more expensive to operate securely in the production environment     
C. Not be interoperable with other software and systems in the production environment    
D. Have a greater likelihood of interoperability with other software and systems in the production environment    
Answer: A.    

When security is created as an aspect of the software itself, there is less need to acquire and apply additional security controls to mitigate risks after deployment. Option B is also wrong for this same reason.
Options C and D are incorrect because the inclusion of security aspects in software design should not affect interoperability in any significant way.

### Question # 108. The inclusion of security controls in the software design process is dictated by _______________.    
A. The National Institute of Standards and Technology (NIST) 800-37     
B. The American Institute of Certified Public Accountants (AICPA)      
C. ISO 27034     
D. The Health Insurance Portability and Accountability Act (HIPAA)       
Answer: C.     

ISO 27034 addresses the sets of controls used in software throughout the environment.
800-37 is the Risk Management Framework, which is about the organization’s overall security, not software development, so option A is incorrect.
The AICPA is a standards-making body, not a standard itself, so option B is incorrect.
HIPAA deals with health care privacy, so option D is incorrect.

### Question # 109. Software development should be perceived as _______________.       
A. Including all members of the organization    
B. The paramount goal of the organization    
C. The greatest risk to the organization    
D. A lifecycle    
Answer: D.   

It is important to consider software development as having a defined process and an eventual endpoint for the useful life of the product.
Not every organization is a software development company. Even in software development companies, not everyone participates in development (there are other departments/offices, such as sales, accounting, etc.). Option A is a poor choice.
Option B is only a correct answer if the organization is a software development company. Otherwise, it is not a correct answer. Option B is incorrect.
If software development poses the most significant risk to your organization, you probably shouldn’t be doing software development. Option C is incorrect.

### Question # 110. Dynamic testing of software is perhaps most useful for _______________.      
A. Simulating negative test cases    
B. Finding errors in the source code     
C. Determining the effect of social engineering      
D. Penetration tests     
Answer: A.

Dynamic testing does not involve source code review or social engineering; options B and C are incorrect.
Penetration tests occur in the production environment, not on pre-deployment software; option D is incorrect.
