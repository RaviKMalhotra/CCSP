# Domain 4 - Cloud Applications Security Questions and Use Caess

### Question # 1 - Dynamic testing of software is perhaps most useful for _______________.  
	A. Simulating negative test cases  
	B. Finding errors in the source code  
	C. Determining the effect of social engineering  
	D. Penetration tests  
		Answer: A  
		Running the software and allowing users to operate it is a great form of dynamic testing, which simulates both known good and known bad inputs.  

### Question # 1 - ISO 27034 mandates a framework for application security within an organization. According to the standard, each organization should have a(n) _______________, and each application within the organization should have its own _______________.  
	A. Organizational Normative Framework (ONF), Application Normative Framework (ANF)  
	B. Application Normative Framework (ANF), Organizational Normative Framework (ONF)  
	C. Standard Application Security (SAS), Application Normative Framework (ANF)  
	D. Organizational Normative Framework (ONF), Standard Application Security (SAS)  
 	Answer: A
   	The ONF lists all the controls used in all the applications within an organization; each ANF lists the particular controls used in each application the 		organization has.
### Question # 2 - According to ISO 27034, there is one Organizational Normative Framework (ONF) in the organization, and _______________ Application Normative Framework (ANF[s]) for each application within that organization.
	A. Many
	B. Three
	C. No
	D. One
	Answer: D
  	Each application will have its own ANF, derived from the organization’s ONF. This can be a difficult question because there are many ANFs in the 
   	organization, but only one for each application.
	
### Question # 3 - What language is used in the Simple Object Access Protocol (SOAP) application design protocol?
	A. Hypertext Markup Language (HTML)
	B. X.509
	C. Extensible Markup Language (XML)
	D. Hypertext Transfer Protocol (HTTP)
	Answer: C. 
 	SOAP necessarily uses XML.
	HTML is a language used to tag text files so that they can be displayed with different fonts, colors, graphics and hyperlinks. HTML is not used in SOAP. 		Option A is incorrect.
	Option B is incorrect because X.509 is a standard and the question is about a programming language.
	Option D is incorrect because HTTP is protocol and the question is about a programming language.
	
 ### Question # 4 - Typically, representational state transfer (REST) interactions do not require _______________.
	A. Credentials
	B. Sessions
	C. Servers
	D. Clients
	Answer: B. 
 	Generally, a REST interaction involves the client asking the server (through an application programming interface [API]) for data, sometimes as the result 	
  	of processing; the server processes the request and returns the result. In REST, an enduring session, where the server has to store some temporary data 	
   	about the client, is not necessary.
	These interactions obviously involve servers and clients, so options C and D are not correct.
	Using REST does not eliminate the need for credentials, so option A is not correct.
	
 ### Question # 5 - Representational state transfer (REST) application programming interfaces (APIs) use _______________ protocol verbs.
	A. Hypertext Markup Language (HTML)
	B. Hypertext Transfer Protocol (HTTP)
	C. Extensible Markup Language (XML)
	D. American Standard Code for Information Interchange (ASCII)
	Answer: B. 
 	Roy Fielding, the author of the PhD dissertation that created REST, was also the author of HTTP, so it’s no surprise the command set is the same.
	All the other options are incorrect because the REST APIs do not use HTML, XML or ASCII as protocol verbs.

### Question #  6 - The architecture of the World Wide Web, as it works today, is _______________.
	A. JavaScript Open Notation (JSON)
	B. Denial of service (DoS)
	C. Representational state transfer (REST)
	D. Extensible Markup Language (XML)
	Answer: C. 
 	The web is mainly HTTP, which is a RESTful protocol.
	All the other options are incorrect because they do not answer the question about the architecture of the World Wide Web.

### Question # 7 - RESTful responses can come from the server in _______________ or _______________ formats.
	A. Extensible Markup Language (XML), JavaScript Open Notation (JSON)
	B. Hypertext Transfer Protocol (HTTP), X.509
	C. American Standard Code for Information Interchange (ASCII), text
	D. Hypertext Markup Language (HTML), Extensible Markup Language (XML)
	Answer: A. 
 	Servers can return REST requests to clients in a number of formats, including XML and JSON.
	X.509 certificates are used for passing session encryption information, not data requests, so option B is incorrect.
	Servers usually return data requests in some sort of display format, not plain text or ASCII, so option C is incorrect.
	HTML responses would simply be an entire web page, not specific data, so option D is incorrect.

### Question # 8 - Which of the following is an informal industry term for moving applications from a traditional environment into the cloud?
	A. Instantiation
	B. Porting
	C. Grandslamming
	D. Forklifting
	Answer: D. 
 	All the other options are simply words used in other contexts. They are incorrect.

### Question # 9 - Developers creating software for the cloud environment should bear in mind cloud-specific risks such as _______________ and _______________.
	A. DoS and DDoS (denial of service and distributed denial of service)
	B. Multitenancy and third-party administrators
	C. Unprotected servers and unprotected clients
	D. Default configurations and user error
	Answer: B. 
 	All the other options are risks that exist in the traditional environment as well as the cloud.

### Question # 10 - When an organization considers cloud migrations, the organization’s software developers will need to know which _______________ and which _______________ the organization will be using, in order to properly and securely create suitable applications.
	A. Geographic location, native language
	B. Legal restrictions, specific ISP
	C. Service model, deployment model
	D. Available bandwidth, telecommunications country code
	Answer: C. 
 	In order for developers to properly create and secure applications, they will need to understand the extent of resource sharing 	
  	(public/private/hybrid/community) and level of control (infrastructure as a service [IaaS], platform as a service [PaaS], software as a service [SaaS]) the 
   	organization will expect in the cloud environment.
	Each of the other options includes at least one element that programmers don’t need to know (specifically, the native language, Internet service provider 	
 	[ISP], country code) and is therefore incorrect.

### Question # 11 - Which of the following is perhaps the best method for reducing the risk of a specific application not delivering the proper level of functionality and performance when it is moved from the traditional environment into the cloud?
	A. Remove the application from the organization’s production environment and replace it with something else.
	B. Negotiate and conduct a trial run in the cloud environment for that application before permanently migrating.
	C. Make sure the application is fully updated and patched according to all vendor specifications.
	D. Run the application in an emulator.
	Answer: B. 
 	A trial run in the cloud will reveal any functionality/performance loss before a permanent cloud migration.
	Option A doesn’t reduce any risk for a specific application; it trades the risk of one application not operating correctly with the risk of another 	
 	application not working correctly. This answer is wrong.
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

### Question # 13 - In a platform as a service (PaaS) model, who should most likely be responsible for the security of the applications in the production environment?
	A. Cloud customer
	B. Cloud provider
	C. Regulator
	D. Programmers
	Answer: A. 
 	In PaaS, the customer is responsible for the administration (and security) of applications.
	Neither regulators nor programmers are responsible for the security of the applications in the production environment. That is the responsibility of the 	
 	cloud customer.
	It may appear as though the cloud provider should be responsible for application security, however, as the cloud customer acquires more responsibility for 	
 	their cloud environment, the cloud provider assumes less responsibility. Option B is incorrect.

### Question # 14 - In the testing phase of the software development lifecycle (SDLC), software performance and _______________ should both be reviewed.
	A. Quality
	B. Brevity
	C. Requirements
	D. Security
	Answer: D. 
 	Performance and security both need to be reviewed for adequacy.
	In this context, quality would be synonymous with performance and requirements, so D is a better answer than A or C.
	Brevity is not a trait we look for in testing, even though it may be desirable in programming, so B is incorrect.

### Question # 15 - Regardless of which model the organization uses for system development, in which phase of the software development lifecycle (SDLC) will user input be requested and considered?
	A. Define
	B. Design
	C. Develop
	D. Detect
	Answer: A. 
 	In the Define phase, we’re trying to determine the purpose of the software, in terms of meeting the users’ needs; therefore, we may solicit input from the 	
  	user community in order to figure out what they really want.
	Options B and C are other phases of the SDLC, but not all SDLC models incorporate user input in these phases, so the options are not correct.
	Option D is not a phase of the SDLC and is incorrect.

### Question # 16 - Which phase of the software development lifecycle (SDLC) is most likely to involve crypto-shredding?
	A. Define
	B. Design
	C. Test
	D. Disposal
	Answer:D. 
 	Disposal is the only phase concerned with the sanitization of media or destruction of data.
	All the other options are also SDLC phases, however, crypto-shredding is much more likely to be used in the disposal phase.

### Question # 17 - Where are business requirements most likely to be mapped to software construction?
	A. Define
	B. Design
	C. Test
	D. Secure Operations
	Answer: B. 
 	Design is the correct answer, as this is where the requirements gathered during the Define phase are mapped to system designs.
	All the other options are SDLC phases where requirements are not mapped to software construction.

### Question # 18 - All of the following are usually nonfunctional requirements except _______________.
	A. Color
	B. Sound
	C. Security
	D. Function
	Answer: D. 
 	Function is usually the functional requirement, describing what action the tool/process satisfies.
	All the others are usually nonfunctional requirements. Exceptions to this are when the characteristic listed is the actual desired function. For instance, 	
 	if the product is a tool that enunciates text so that a blind user can hear the words, then sound would be the functional requirement. If the product is a 	
  	security tool such as a firewall or data loss prevention (DLP) solution, then security would be a functional requirement. Otherwise, these are nonfunctional 	requirements for standard products.

### Question # 19 - Designers making applications for the cloud have to take into consideration risks and operational constraints that did not exist or were not as pronounced in the traditional environment. Which of the following is an element cloud app designers may have to consider incorporating in software for the cloud that may not have been as important in the traditional environment?
	A. Identity and access management (IAM) capability
	B. Distributed denial of service (DDoS) resistance
	C. Encryption for data at rest and in motion
	D. Field validation
	Answer: C. 
 	Traditional apps won’t usually require encryption in all phases of the data lifecycle because data is protected in several stages in the traditional 	
  	environment without the need for additional controls. In the cloud environment, however, data exposed at any point in the lifecycle might constitute an 
   	inadvertent disclosure, so cloud apps require encryption for data at rest and in motion (and usually in use as well).
	Even traditional apps require IAM and field validation functions, so options A and D are incorrect.
	Most anti-DDoS activity will be performed by hardware and communication software run by the cloud provider or Internet service provider (ISP); developers 	
 	should not typically need to include anti-DDoS elements in their programs. Option B is incorrect.

### Question # 20 - Designers making applications for the cloud have to take into consideration risks and operational constraints that did not exist or were not as pronounced in the traditional environment. Which of the following is an element cloud app designers may have to consider incorporating in software for the cloud that might not have been as important in the traditional environment?
	A. Application isolation
	B. Inference framing
	C. Known secure library components
	D. Testing that uses known bad data
	Answer: A. 
 	Because the cloud is a multitenant environment, one of the concerns that developers should consider is how well the application prevents other 	
  	applications/users from observing its operation and resource calls. In the traditional environment, this is not usually required because the organization 	
   	owns the underlying infrastructure (as a single tenant) and there is very little risk in exposing the application’s functionality.
	Inference framing is a nonsense term, used here only as a distractor.
	Software should include known secure components, and testing should include known bad data (fuzz testing), whether it is going to be used in the cloud or in 	a traditional environment, so options C and D are incorrect.

### Question # 21 - Designers making applications for the cloud have to take into consideration risks and operational constraints that did not exist or were not as pronounced in the traditional environment. Which of the following is an element cloud app designers may not be able to use as readily in the cloud environment as it was deployed in the traditional environment?
		A. Cryptography
		B. STRIDE testing
		C. Field validation
		D. Logging
Answer:
D. The cloud provider may have controls that restrict logging, or the delivery of log data, in the environment; this can make it complicated for cloud developers to include that functionality/security element in cloud apps.
All the other options are things that can (and should) be done with software whether the application is being used in traditional or cloud environments, so those options are incorrect.

### Question # 22 - All of these can affect the quality of service expected from an application except _______________.
		A. Encryption
		B. Egress monitoring
		C. Anti-malware tools
		D. Use of known secure libraries/components
Answer:
D. Using only known secure libraries and components in software design may slow down development efforts but shouldn’t impact how the application runs.
All the other options are security controls that will degrade performance because they require additional overhead; these options are incorrect.

### Question # 23 - The possibility that a user could gain access or control of an application so as to take on administrator or management capabilities is called _______________.
		A. Inversion
		B. Spoofing
		C. Repudiation
		D. Escalation of privilege
Answer:
D. This is the definition of escalation of privilege (sometimes referred to as “elevation of privilege”).
Inversion is a nonsense term in this context and just a distractor.
Options B and C are threat modeling elements but are not correct answers for this question.

### Question # 24 - Which of the following is not checked when using the STRIDE threat model?
		A. The ability of users to gain administrative access rights without proper permission
		B. The ability of internal personnel to trigger business continuity/disaster recovery activities
		C. The ability of a participant in a transaction to refute that they’ve taken part in the transaction
		D. The ability of an unauthorized user to pretend to be an authorized user
Answer:
A. The STRIDE threat model does not deal with business continuity and disaster recovery (BC/DR) actions.
All the other options are elements of STRIDE (escalation of privilege, repudiation, and spoofing, respectively) and are therefore not correct.

### Question # 25 - It is very likely that your organization’s users will use unapproved application programming interfaces (APIs), especially in a bring your own device (BYOD) environment, because _______________.
		A. Users are constantly trying to break the security of your environment
		B. APIs can’t ever be secure
		C. Hackers are constantly infiltrating all APIs
		D. Users enhance their productivity however they can
Answer:
D. Users in the production environment will leverage whatever tools and techniques they can in order to get their job done in a better, faster way, often regardless of whether this complies with security policies.
All the other options are untrue and therefore cannot be the correct answer. For test-taking purposes, be very suspicious of words like, “constantly” and “can’t ever” in answer choices.

### Question # 26 - Some current software developers are not aware of security problems within the programs they’re creating because _______________.
		A. Young programmers are not nearly as disciplined in their coding practices as older programmers
		B. Some current programmers don’t write code line by line and instead use code component libraries
		C. Coding languages have not been secure for 20 years
		D. Users are not clear in defining their requirements at the outset of the software development lifecycle (SDLC)
Answer:
B. Because many programs are currently constructed from “building block” components found in code libraries, any security issues within specific components may not be understood or identified by coders who don’t know the code inside the component.
Option A is an unfair generalization.
Option C is another broad generalization that may or may not be true. Option B is a better answer.
Option D does not relate to the question about the SDLC and is therefore a poor choice for an answer.

### Question # 27 - What is the most secure form of code testing and review?
		A. Open source
		B. Proprietary/internal
		C. Neither open source nor proprietary
		D. Combination of open source and proprietary
Answer:
D. Obviously, using multiple forms of code review will produce more secure results than any one form of review, in the same way that having multiple forms of security controls (physical, logical, administrative, etc.) will provide better security than just one type.
The question is which is the “most” secure form of code testing and review. That would be the most extensive. Since the correct answer is a combination of open source and proprietary, the least secure would be least extensive. Option A is strictly open source so that is incorrect. Option C is neither open source nor proprietary, which is even less extensive. Option C is incorrect. Proprietary/internal is also less extensive than Option D. So Option B is incorrect.

### Question # 28 - What is the major difference between authentication and authorization?
		A. Code verification/code implementation
		B. Identity validation/access permission
		C. Inverse incantation/obverse instantiation
		D. User access/privileged access
Answer:
B. This is the textbook definition of these terms. All the other options are incorrect answers.

### Question # 29 - Access should be based on _______________.
		A. Regulatory mandates
		B. Business needs and acceptable risk
		C. User requirements and management requests
		D. Optimum performance and security provision
Answer:
B. Business needs and risk acceptable to senior management should drive all organizational decisions, including access. Specific user or object access will, of course, be delegated down from senior management to a manageable layer of the organization, but the principle applies.
This decision, however, should be informed by pertinent externalities, which include regulatory mandates (option A), user requirements and management requests (option C), and, to some degree, the trade-off of performance and security (option D, and both characteristics should also be dictated by senior management as an aspect of acceptable risk). While these externalities and options all play a part in determining appropriate access, they are all subordinate to business needs and acceptable risk, which are paramount; B is still the best answer to this question.

### Question # 30 - Who should determine which users have access to which specific objects?
		A. The cloud provider
		B. Senior management
		C. Data owners
		D. System administrators
Answer:
C. The data owner is responsible for the disposition of the data under their control; this includes access decisions.
The cloud provider is not typically the data owner; option A is incorrect.
Ostensibly, senior management is the data owner (the organization, as a whole, is the legal owner of the data, and the senior managers are the legal representatives of the organization). However, in practice, this responsibility can be (and usually is) delegated down to a manageable level, where the data owner for a given data set understands it best and can provide a sufficiently granular control of that data set. This is rarely senior management and is more likely department heads, branch managers, or some other form of middle management. Option C is preferable to B.
System administrators will usually be the literal granters of access, insofar as admins will modify access control systems that allow or disallow access for specific individuals or roles. However, the sysadmin does not make the decision of who is granted access and instead responds to direction from data owners (middle management); again, option C is preferable to D.

### Question # 31 - All of the following are identity federation standards commonly found in use today except _______________.
		A. WS-Federation
		B. OpenID
		C. OAuth (Open Authorization)
		D. Pretty Good Privacy (PGP)
Answer:
D. PGP is an email encryption tool, not an identity federation standard. All the other options are federation standards.

### Question # 32 - Which of the following is a federation standard/protocol that does not rely on Simple Object Access Protocol (SOAP), Security Assertion Markup Language (SAML), or Extensible Markup Language (XML)?
		A. WS-Federation
		B. OpenID Connect
		C. Service Organization Control (SOC) 2
		D. Open Web Application Security Project (OWASP)
Answer:
B. OpenID Connect is a federation protocol that uses representational state transfer (REST) and JavaScript Object Notation (JSON); it was specifically designed with mobile apps in mind, instead of only web-based federation.
WS-Federation is a federation protocol that is part of the WS-Security family of standards and reliant on Simple Object Access Protocol (SOAP), so option A is incorrect.
Option C is incorrect; SOC 2 is a type of Statement on Standards for Attestation Engagements (SSAE) 18 audit report, not a federation standard.
OWASP is a volunteer group of and for web app developers, not a federation standard or protocol, so option D is incorrect.

### Question # 33 - Authentication mechanisms typically include any or all of the following except _______________.
		A. Something you know
		B. Someone you know
		C. Something you have
		D. Something you are
Answer:
B. Because there is no transitive property of identification and authentication, knowing a trusted entity is not sufficient for validating an identity assertion.
All the other options are typical authentication mechanisms and so are incorrect.

### Question # 34 - Which of the following constitutes a multifactor authentication process or procedure?
		A. Using an automated teller machine (ATM) to get cash with your credit or debit card
		B. Using a password and personal identification number (PIN) to log into a website
		C. Presenting a voice sample and fingerprint to access a secure facility
		D. Displaying a birth certificate and a credit card
Answer:
A. At the ATM, the customer will use the card (something you have) and enter a PIN (something you know). This is true multifactor authentication.
A password and PIN are both something you know, so option B is incorrect.
Using a voice sample and fingerprint are two forms of something you are, so option C is incorrect.
A birth certificate and credit card are both something you have, so option D is incorrect.

### Question # 35 - Typically, multifactor authentication should be used _______________.
		A. In every IT transaction
		B. For high-risk operations and data that is particularly sensitive
		C. When remote users are logging into the cloud environment
		D. Only in the traditional environment
Answer:
B. Multifactor authentication should be considered for operations that have a significant risk or that deal with highly sensitive data (for instance, privileged user logins or when handling financial transactions).
Requiring multifactor authentication for every transaction is an undue burden on both the users and the systems and is a needless addition of extra overhead, so option A is incorrect.
All cloud access will entail remote login; this is a common operation, so adding multifactor authentication is an unnecessary burden in most cases. Option C is incorrect.
The decision to use multifactor authentication should be based on the risk of the operation and the sensitivity of the data, not on whether it takes place in the traditional or online environment, so option D is incorrect.

### Question # 36 - A web application firewall (WAF) usually operates at Layer _______________ of the Open Systems Interconnection (OSI) model.
		A. 2
		B. 3
		C. 7
		D. Q
Answer:
C. A WAF is a Layer 7 tool.
All the other options are incorrect.

### Question # 37 - A web application firewall (WAF) can understand and act on _______________ traffic.
		A. Malicious
		B. Simple Mail Transfer Protocol (SMTP)
		C. Internet Control Message Protocol (ICMP)
		D. Hypertext Transfer Protocol (HTTP)
Answer:
D. WAFs recognize HTTP traffic and can respond to traffic that matches prohibited rulesets or conditions.
Option A is technically correct; a WAF can be given a ruleset that recognizes certain forms of attack traffic. However, this answer is too general, and D is a much better response for this question.
Options B and C are protocols not usually inspected by WAFs and are therefore incorrect.

### Question # 38 - WAFs can be used to reduce the likelihood that _______________ attacks will be successful.
		A. Social engineering
		B. Physical theft
		C. Obverse inflection
		D. Cross-site scripting
Answer:
D. WAFs can be used to attenuate the possibility that cross-site scripting attacks will be successful.
WAFs do not protect against social engineering or physical attacks in any way, so options A and B are incorrect.
Option C is a nonsense term and is therefore incorrect.

### Question # 39 - A database activity monitor (DAM) tool usually operates at Layer _______________ of the Open Systems Interconnection (OSI) model.
		A. 2
		B. 3
		C. 7
		D. Q
Answer:
C. A DAM is a Layer 7 tool.
All the other options are incorrect.

### Question # 40 - Database activity monitors (DAMs) can be used to reduce the potential success of _______________ attacks.
		A. SQL injection
		B. Cross-site scripting
		C. Insecure direct-object reference
		D. Social engineering
Answer:
A. DAMs can be used to reduce the possibility that SQL injection attacks will be successful.
DAMs do not protect against cross-site scripting, insecure direct-object reference, or social engineering attacks in any way, so options B, C, and D are incorrect.

### Question # 41 - Which security tool can perform content inspection of Secure File Transfer Protocol (SFTP) communications?
		A. Web application firewall (WAF)
		B. Database activity monitor (DAM)
		C. Extensible Markup Language (XML) gateway
		D. Single sign-on (SSO)
Answer:
C. The XML gateway can provide this functionality; it acts as a reverse proxy and can perform content inspection on many traffic protocols.
The WAF and DAM are also security tools that inspect traffic but do not usually handle SFTP content, so options A and B are incorrect.
Option D, single sign-on, concerns authentication functions, not communications traffic, and is only a distractor in this context.

### Question # 42 - To deploy a set of microservices to clients instead of building one monolithic application, it is best to use a(n) _______________ to coordinate client requests.
		A. Extensible Markup Language (XML) gateway
		B. Application programming interface (API) gateway
		C. Web application firewall (WAF)
		D. Database activity monitor (DAM)
Answer:
B. An API gateway translates requests from clients into multiple requests to many microservices and delivers the content as a whole via an API it assigns to that client/session.
XML gateways, WAFs, and DAMs are also tools used frequently in cloud-based enterprises, but they do not handle microservice requests in a meaningful way.

### Question # 43 - Firewalls can detect attack traffic by using all these methods except _______________.
		A. Known past behavior in the environment
		B. Identity of the malicious user
		C. Point of origination
		D. Signature matching
Answer:
B. While it would be wonderful, for security purposes, to know the identity of attackers before or while they’re making an attack, this is information the attacker doesn’t usually share.
All the other options are methods firewalls can use to recognize attacks.

### Question # 44 - Transport Layer Security (TLS) provides _______________ and _______________ for communications.
		A. Privacy, security
		B. Security, optimization
		C. Privacy, integrity
		D. Enhancement, privacy
Answer:
C. TLS maintains the confidentiality and integrity of communications, often between a web browser and a server.
In this context, privacy and security mean much the same thing; privacy is synonymous with confidentiality, which is a subset of the overall topic of security. Therefore, option A is repetitive and not correct.
TLS does not optimize performance or add any sort of enhancement, so options B and D are incorrect.

### Question # 45 - Transport Layer Security (TLS) uses a new _______________ for each secure connection.
		A. Symmetric key
		B. Asymmetric key
		C. Public-private key pair
		D. Inverse comparison
Answer:
A. TLS uses symmetric key crypto for each communications session in order to secure the connection; the session key is uniquely generated each time a new connection is made.
Options B and C are names for another type of encryption. Asymmetric encryption is also used in establishing a secure TLS connection; however, the keys used in this portion of the process will not change from session to session, and therefore these options are incorrect.
Option D is a nonsense term and is therefore incorrect.

### Question # 46 - A virtual private network (VPN) is used to protect data in transit by _______________.
		A. Securing each end of a client-server connection
		B. Creating an encrypted tunnel between two endpoints
		C. Encrypting databases
		D. Restricting key access to only eight parties
Answer:
B. A VPN is a temporary, synthetic encrypted tunnel between two endpoints (often a client and a server).
Option A is subtly misleading; the VPN secures the connection between two endpoints, not the ends of the connection. This option is incorrect.
Option C is not correct; VPN is not used for encrypting databases—it is used for encrypting communications.
Option D is incorrect; the symmetric key used in VPN is shared only between two parties (the endpoints), and the elements of the asymmetric key pair are either held by only one party (the owner of each private key) or by anyone at all (public key).
### Question # 47 - The employment of users in dynamic software testing should best be augmented by _______________.
		A. Having the developers review the code
		B. Having the developers perform dynamic testing
		C. Using automated agents to perform dynamic testing
		D. Social engineering
Answer:
C. Users may not offer enough coverage for larger software products that have a great deal of functionality; it can be useful to also use automated agents to checks paths that users might not often attempt or utilize.
The developers should not be involved in any form of testing the software as they have an inherent conflict of interest, so options A and B are incorrect.
Dynamic testing does not involve social engineering; option D is incorrect.

### Question # 48 - Why do developers have an inherent conflict of interest in testing software they’ve created?
		A. They are notoriously bad, as a group, at testing.
		B. They work for the same department as the testing personnel.
		C. They have a vested interest in having the software perform well.
		D. They are never trained on testing procedures.
Answer:
C. This is the definition of “conflict of interest.”
All the other answers are incorrect.

### Question # 49 - Sandboxing can often be used for _______________.
		A. Optimizing the production environment by moving processes that are not frequently used into the sandbox
		B. Allowing secure remote access for users who need resources in the cloud environment
		C. Running malware for analysis purposes
		D. Creating secure subnets of the production environment
Answer:
C. A sandbox can be used to run malware for analysis purposes as it won’t affect (or infect) the production environment; it’s worth noting, though, that some malware is sandbox-aware, so additional anti-malware measures are advisable.
Options A, B, and D are not correct because the sandbox should be completely disconnected (air-gapped) from the production environment so that users can’t perform productive activity there.

### Question # 50 - Sandboxing can often be used for _______________.
		A. Testing user awareness and training
		B. Testing security response capabilities
		C. Testing software before putting it into production
		D. Testing regulatory response to new configurations and modifications
Answer:
C. Software that has either been purchased from a vendor or developed internally can be tested in a sandboxed environment that mimics the production environment in order to determine whether there will be any interoperability problems when it is installed into actual production.
All the other options aren’t uses for sandboxes and are incorrect.

### Question # 51 - Application virtualization can typically be used for _______________.
		A. Running an application in a non-native environment
		B. Installing updates to a system’s operating system (OS)
		C. Preventing escalation of privilege by untrusted users
		D. Enhancing performance of systems
Answer:
A. Virtualized applications can run on platforms that wouldn’t otherwise allow them to function, such as running Microsoft apps on a Linux box.
Because the virtualization engine encapsulates the application from the native runtime environment, patches can’t be applied through virtualized programs; option B is incorrect.
Virtualization really doesn’t have anything to do with access control; option C is incorrect.
The overhead of running a software virtualization engine will actually add to system overhead, not decrease it, so option D is incorrect.

### Question # 52 - Application virtualization can typically be used for _______________.
		A. Denying access to untrusted users
		B. Detecting and mitigating distributed denial of service (DDoS) attacks
		C. Replacing encryption as a necessary control
		D. Running an application on an endpoint without installing it
Answer:
D. Application virtualization allows the software to run on a simulated environment on the device without the need to install it on the device.
Virtualization really doesn’t have anything to do with access control; option A is incorrect.
Virtualization neither detects nor responds to DDoS; option B is incorrect.
Virtualization does not replace encryption; if data needs to be secure within the virtualization environment, encryption may still have to be utilized. Option C is incorrect.

### Question # 53 - Any organization that complies with ISO 27034 will have a maximum of _______________ Organizational Normative Framework(s) (ONF)(s).
		A. 0
		B. 1
		C. 5
		D. 25
Answer:
B. ISO 27034 dictates that an organization will have a collection of security controls used for all software within that organization; this collection is called the ONF.
All the other options are distractors and incorrect.
Under ISO 27034<img width="1122" height="15388" alt="image" src="https://github.com/user-attachments/assets/2bb4afc4-359c-457d-9a5b-8a06d25e0e3a" />


❓1. Dynamic testing of software is perhaps most useful for _______________.
✔️[Answer] Simulating negative test cases

 The inclusion of security controls in the software design process is dictated by _______________.
 ISO 27034

 Software that includes security elements from the outset of the software development lifecycle (SDLC) process will _______________.
 Be less expensive to operate securely in the production environment
 When security is created as an aspect of the software itself, there is less need to acquire and apply additional security controls to mitigate risks after  
 deployment.


- ❓# 106. Software that includes security elements from the outset of the software development lifecycle (SDLC) process will be _______________.
		A. More secure in deployment
  		B. Less secure in deployment
  		C. More likely to malfunction
		D. Less likely to malfunction
Answer:
A. It is important to verify and validate the program at each stage of the SDLC.
Adding functionality at each stage of the SDLC is the definition of scope creep, which is what we’d like to avoid. Option A is incorrect.
Management should not have to shepherd software through the development process; this is the process of the development team. Option B is incorrect.
Option D makes no sense: you can’t repurpose something that has just been developed.
<img width="1148" height="307" alt="image" src="https://github.com/user-attachments/assets/db45347c-4c26-4367-801e-176f8e2ab370" />

