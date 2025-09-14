# Chapter 3: Domain 3—Cloud Platform and Infrastructure Security
The third domain of the Certified Cloud Security Professional (CCSP) Exam Outline concerns the underlying infrastructure of the cloud, including both hardware and software, the concept of pooled resources, and a detailed discussion of identity and access management (IAM).

### Question # 1 - You are in charge of creating the business continuity and disaster recovery (BC/DR) plan and procedures for your organization. Your organization has its production environment hosted in a cloud environment. You are considering using cloud backup services for your BC/DR purposes as well. What would probably be the best strategy for this approach, in terms of redundancy and resiliency?  
A. Have your cloud provider also provide BC/DR backup.  
B. Keep a BC/DR backup on the premises of your corporate headquarters.  
C. Use another cloud provider for the BC/DR backup.  
D. Move your production environment back into your corporate premises, and use your cloud provider to host your BC/DR backup.  
Answer: C. 

It’s best to have your backup at another cloud provider in case whatever causes an interruption in service occurs throughout your primary provider’s environment; **this will be more complicated and expensive, but it provides the best redundancy and resiliency.** 
Using the same provider for production and backup is not a bad option, but it entails the risk of the same contingency affecting both copies of your data. 
Having either the backup or the production environment localized does not provide the best protection, so neither option B nor option D is desirable.

### [important] Question # 2 - You are in charge of creating the business continuity and disaster recovery (BC/DR) plan and procedures for your organization. You decide to have a table top test of the BC/DR activity. Which of the following will offer the best value during the test?  
A. Have all participants conduct their individual activities via remote meeting technology.  
B. Task a moderator well versed in BC/DR actions to supervise and present scenarios to the participants, including randomized special events.  
C. Provide copies of the BC/DR policy to all participants.  
D. Allow all users in your organization to participate.  
Answer: B. 

**A trained and experienced moderator can guide the participants through the activity, enhancing their training and noting pitfalls and areas for improvement.** 

Option A is not preferable because having the participants gathered together ensures their full attention and provides interaction that remote participation might not yield. 

**Option C is a baseline; all participants should have copies of the policy as a matter of course.** 

**Option D is not useful in a tabletop exercise; only critical participants in the organization should take part in the tabletop**.

### [tricky] Question # 3 - You are in charge of creating the business continuity and disaster recovery (BC/DR) plan and procedures for your organization. Your organization has its production environment hosted by a cloud provider, and you have appropriate protections in place. Which of the following is a significant consideration for your BC/DR backup?  
A. Enough personnel at the BC/DR recovery site to ensure proper operations.  
B. Good cryptographic key management.  
C. Access to the servers where the BC/DR backup is stored.  
D. Forensic analysis capabilities.  
Answer: B.

This is a difficult question that requires a great deal of thought. 
[important] Option B is corect because appropriate cloud data security practices will require encrypting a great deal of the data, **and having the keys will be necessary during contingency operations in order to access the backup; without the keys, you won’t be able to access your data.** 

Option A is not correct because using the cloud for BC/DR will allow personnel to access the backup from anywhere they can get broadband connectivity, not specifically a recovery site. 

Option C is not correct because the customer will rarely have physical access to servers in the cloud environment. 

Option D is not correct because forensic analysis is not a significant consideration in BC/DR; it is much more important for incident response.

### [important] Question # 4 - You are in charge of creating the business continuity and disaster recovery (BC/DR) plan and procedures for your organization. You are going to conduct a full test of the BC/DR plan. Which of the following strategies is an optimum technique to avoid major issues?   
A. Have another full backup of the production environment stored prior to the test.    
B. Assign all personnel tasks to perform during the test.    
C. Have the cloud provider implement a simulated disaster at a random moment in order to maximize realistic testing.    
D. Have your regulators present at the test so they can monitor performance.     
Answer: A.    

[important] **A full test will involve both the production environment and the backup data**; 
**it is possible to create an actual disaster during a full test by ruining the availability of both.** 
**Therefore, it is crucial to have a full backup, distinct from the BC/DR backup, in order to roll back from the test in case something goes horribly wrong.** 

Option B is incorrect because not all personnel will have tasks to perform; **most personnel will have to evacuate from the facility only during a full test**. 

Option C is incorrect because the cloud provider should not initiate the test, and the test should not take place at a random moment. 

Option D is not correct because the regulators’ presence will not add any value to the test.

### Question # 5 - A Security Assertion Markup Language (SAML) identity assertion token uses the ___________________.   protocol.   
A. Extensible Markup Language (XML).  
B. Hypertext Transfer Protocol (HTTP).  
C. Hypertext Markup Language (HTML).  
D. American Standard Code for Information Interchange (ASCII).  
Answer: A. 

**Security Assertion Markup Language (SAML) is based on XML.** 
HTTP is used for port 80 web traffic; 
HTML is used to present web pages. 
ASCII is the universal alphanumeric character set.

### Question # 6 - The minimum essential characteristics of a cloud data center are often referred to as “ping, power, pipe.” What does this term mean?  
A. Remote access for customer to racked devices in the data center; electrical utilities; connectivity to an Internet service provider (ISP)/the Internet.    
B. Application suitability; availability; connectivity.   
C. Infrastructure as a service (IaaS); software as a service (SaaS); platform as a service (PaaS).  
D. Anti-malware tools; controls against distributed denial-of-service (DDoS) attacks; physical/environmental security controls, including fire suppression.  
Answer:A. 

Option A is the definition of the term; the other answers are not.

### Question # 7 - To support all aspects of the CIA triad (confidentiality, integrity, availability), all of the following aspects of a cloud data center need to be engineered with redundancies except ___________________.   
A. Power supply.  
B. HVAC.  
C. Administrative offices.  
D. Internet service provider (ISP)/connectivity lines.  
Answer: C. 

The administrative offices of a cloud data center rarely are part of the critical functions of the operation; 
a data center could likely endure the loss of the administrative offices for a considerable length of time, 
so redundancy here is probably not cost effective.
All the other items are part of the critical path and need redundancies.

### Question # 8 - Who is the cloud carrier?    
A. The cloud customer.   
B. The cloud provider.     
C. The regulator overseeing the cloud customer’s industry.    
D. The ISP between the cloud customer and provider.     
Answer: D.    

**Option D is the definition of a cloud carrier, from National Institute of Standards and Technology (NIST) Special Publication (SP) 500-292.**

All the other options are incorrect, as defined by NIST SP 500-292.

### Question # 9 - [important] Which of the following terms describes a means to centralize logical control of all networked nodes in the environment, abstracted from the physical connections to each?   
A. Virtual private network (VPN).     
B. Software-defined network (SDN).    
C. Access control lists (ACLs).    
D. Role-based access control (RBAC).     
Answer: B. 

The question describes a software-defined network (SDN).
A VPN is used for creating an encrypted communications tunnel over an untrusted medium, so option A is incorrect.
ACLs are used as centralized repositories for identification, authentication, and authorization purposes, so option C is incorrect.
RBAC is an access control model used to assign permissions based on job functions within an organization, so option D is incorrect.

### Question # 10 - [important] In software-defined networking (SDN), the northbound interface (NBI) usually handles traffic between the ___________________ and the ___________________.   
A. Cloud customer; ISP.  
B. SDN controllers; SDN applications.  
C. Cloud provider; ISP.  
D. Router; host.  
Answer: B.  

**The NBI usually handles traffic between the SDN controllers and SDN applications.**

Options A and C are incorrect because neither of those options lists any of the SDN infrastructure, be that the controllers or the applications. 
Option D may be arguably correct, as there might be an NBI handling that traffic between those nodes, but option B is more specific and always true for this definition, so it is the better choice.

### Question # 11 - Software-defined networking (SDN) allows network administrators and architects to perform all the following functions except ___________________.       

A. Reroute traffic based on current customer demand.     
B. Create logical subnets without having to change any actual physical connections.       
C. Filter access to resources based on specific rules or settings.       
D. Deliver streaming media content in an efficient manner by placing it closer to the end user.    
Answer: D. 

Option D is really a definition of a CDN (content delivery network).
All the other options are aspects of SDNs.

 ### Question # 12 - Which of the following is a device specially purposed to handle the issuance, distribution, and storage of cryptographic keys?   
A. Key management box (KMB)   
B. Hardware security module (HSM)    
C. Ticket-granting ticket (TGT)    
D. Trusted computing base (TCB)    
Answer: B. 

The question describes an HSM.
KMB is a nonsense term used as a distractor, so it is incorrect.
TGT is a term associated with Kerberos single sign-on systems and is incorrect.
The TCB includes the elements of hardware and software (usually in the operating system) that ensure that a system can only be controlled by those with the proper permissions (i.e., admins with root control), so it is also incorrect.

### Question # 13 - When discussing the cloud, we often segregate the data center into the terms compute, storage, and networking. Compute is made up of ___________________ and ___________________.     
A. Routers; hosts    
B. Application programming interface (APIs); northbound interface (NBIs)     
C. Central processing unit (CPU); random-access memory (RAM)    
D. Virtualized; actual hardware devices   
Answer: C. 

**The compute nodes of a cloud data center can be measured in terms of how many central processing units (CPUs) and how much random access memory (RAM) is available within the center.**

Option A is incorrect because routers would be considered a part of the networking of a data center (and because option C is a better answer).
Option B involves applications and how traffic flows between them and storage controllers; it has nothing to do with the compute nodes and is therefore wrong.
Option D might obliquely be considered correct because it’s technically true (compute nodes will include both virtual and hardware machines), but option C is a much better and more accurate choice.

### Question # 14 - All of the following can be used to properly apportion cloud resources except ___________________.   
A. Reservations    
B. Shares    
C. Cancellations   
D. Limits    
Answer: C.   

Cancellations is not a term used to describe a resource allotment methodology. **All of the other options are such terms.**

### [important and tricky] Question # 15 - Which of the following is a method for apportioning resources that involves setting [guaranteed minimums for all tenants/customers within the environment?]     
A. Reservations    
B. Shares     
C. Cancellations     
D. Limits    
Answer: A.     

The question is the definition of reservations.
Options B and D are also resource apportioning methods, but they do not fall under the definition described in the question.
Option C is incorrect because it has no meaning in this context.

### Question # 16 - Which of the following is a method for apportioning resources that involves setting [maximum usage] amounts for all tenants/customers within the environment?     
A. Reservations         
B. Shares      
C. Cancellations        
D. Limits   
Answer: D. 

The question describes limits.
Options A and B are also resource apportioning methods, but they do not fall under the definition described in the question.
Option C is because it has no meaning in this context.

### [important] Question # 17 - Which of the following is a method for apportioning resources that involves [prioritizing resource requests] to resolve contention situations?       
A. Reservations      
B. Shares         
C. Cancellations         
D. Limits      
Answer: B.      

The question describes shares.
Options A and D are also resource apportioning methods, but they do not fall under the definition described in the question.
Option C is incorrect because it has no meaning in this context.

### Question # 18 - A bare-metal hypervisor is Type ___________________.   
A. 1    
B. 2    
C. 3    
D. 4   
Answer: A. 

**A bare-metal hypervisor is a Type 1 hypervisor.**
Option B describes another type of hypervisor; the other options are incorrect because there is no such thing as a Type 3 or Type 4 hypervisor.

### Question # 19 - A hypervisor that runs inside another operating system (OS) is a Type ___________________ hypervisor.    
A. 1.   
B. 2.   
C. 3.    
D. 4.   
Answer: B. 

The question describes a Type 2 hypervisor.
Option A describes another type of hypervisor; the other options are incorrect because there is no such thing as a Type 3 or Type 4 hypervisor.

### [important tricky] Question # 20 - A Type ___________________ hypervisor is probably more difficult to defend than other hypervisors.     
A. 1     
B. 2     
C. 3     
D. 4    
Answer: B.      

A Type 2 hypervisor relies on the underlying operating system (OS) to operate properly; the underlying OS offers a large attack surface for aggressors.
A Type 1 hypervisor boots directly from the hardware; it’s much easier to secure a machine’s Basic Input/Output System (BIOS) than an entire OS, so option B is better than option A.
Options C and D are incorrect because there is no such thing as a Type 3 or Type 4 hypervisor.

### [very important] Question # 21 - One of the security challenges of operating in the cloud is that additional controls must be placed on file storage systems because ___________________.    
A. File stores are always kept in plain text in the cloud       
B. There is no way to sanitize file storage space in the cloud      
C. Virtualization necessarily prevents the use of application-based security controls      
D. Virtual machines are stored as snapshotted files when not in use      
Answer: D.       

**VMs are snapshotted and simply stored as files when they are not being used; 
an attacker who gains access to those file stores could ostensibly steal entire machines in highly portable, easily copied formats. 
Therefore, these cloud storage spaces must include a significant amount of controls.**

Options A and C are simply untrue.
Option B is untrue when crypto-shredding is utilized.

### Question # 22 - What is the main reason virtualization is used in the cloud?         
A. Virtual machines (VMs) are easier to administer.   
B. If a VM is infected with malware, it can be easily replaced.    
C. With VMs, the cloud provider does not have to deploy an entire hardware device for every new user.    
D. VMs are easier to operate than actual devices.     
Answer: C. 

While options A and B are both also true, C is the most significant reason cloud data centers use VMs. If the cloud provider had to purchase a new box for every user, the cost of cloud services would be as much as running a traditional environment (or likely cost even more), and there would be no reason for any organization to migrate to the cloud, especially considering the risks associated with disclosing data to a third party.
Option D is simply untrue. VMs are not easier to operate than actual devices.

### [important] Question # 23 - Orchestrating resource calls is the job of the ___________________.        
A. Administrator.           
B. Router.        
C. VM.     
D. Hypervisor.       
Answer: D. 

The question describes what the hypervisor does. (Note that the answer “operating system” would also work here but was not one of the options.)
Option A is incorrect; the allocation of resources is not performed manually.
The router directs traffic between networks; it does not apportion resources. Therefore, option B is incorrect.
A VM makes resource calls; option C is incorrect.

### [tricky] Question # 24 - Which of the following terms describes a cloud storage area that uses a filesystem/hierarchy?        
A. Volume storage.   
B. Object storage.    
C. Logical unit number (LUN).   
D. Block storage.    
Answer: B. 

**Object storage is, literally, a means of storing objects in a hierarchy such as a file tree.**
All the other options are terms used to describe cloud storage areas without file structures.

### [important] Question # 25 - Typically, which form of cloud storage is used in the near term for snapshotted virtual machine (VM) images?    
A. Volume storage.   
B. Object storage.    
C. Logical unit number (LUN).   
D. Block storage.    
Answer: B. 

**Snapshotted VM images are usually kept in object storage, as files.**
All the other options are incorrect and option C is not a type of storage.

### Question # 26 - Who operates the management plane?              
A. Regulators.    
B. End consumers.    
C. Privileged users.    
D. Privacy data subjects.    
Answer: C. 

**Only the most trusted administrators and managers will have access to the cloud data center’s management plane.** 
These will usually be cloud provider employees, but some cloud customer personnel may be granted limited access to arrange their organization’s cloud resources.
Regulators do not operate a customer’s management plane, so option A is incorrect.

Option B is ambiguous. However, a consumer of data is unlikely to have been given the elevated privileges necessary of operate the management plane in a cloud environment. Option B is incorrect.

Option D is also an ambiguous answer. Only the most trusted administrators and managers have access to the cloud data center’s management plane. A privacy data subject is neither a most trusted administrator nor a trusted manager. Therefore, option D is incorrect.
	
 ### Question # 27 - [important] What is probably the optimum way to avoid vendor lock-in?    
A. Use nonproprietary data formats.    
B. Use industry-standard media.    
C. Use strong cryptography.
D. Use favorable contract language.     
Answer: D. 

**The contract is probably the cloud customer’s best tool for avoiding vendor lock-in; 
contract terms will establish how easy it is to migrate your organization’s data to another provider in a timely, cost-effective manner.**

Options A and B are also important ways to avoid vendor lock-in, but D is the best answer.
Option C is incorrect and will not aid in avoiding vendor lock-in.
	
### Question # 28 - [confusing] Who will determine whether your organization’s cloud migration is satisfactory from a compliance perspective?   
A. The cloud provider    
B. The cloud customer    
C. The regulator(s)    
D. The Internet service provider (ISP)    
Answer: C.    
**The regulator(s) overseeing your industry/organization will make the final determination as to whether your cloud configuration is suitable to meet their requirements. It is best to coordinate with your regulator(s) when first considering cloud migration.**

Cloud providers, cloud customers, and ISPs are not particularly concerned about whether an organization’s migration is satisfactory from a compliance perspective. The words, “compliance perspective” should automatically bring to mind regulator(s). Options A, B, and D are therefore incorrect answers.
	
### [important] Question # 29 - What is probably the best way to avoid problems associated with vendor lock-out?
A. Use strong contract language.    
B. Use nonproprietary data and media formats.     
C. Use strong cryptography.       
D. Use another provider for backup purposes.        
Answer: D.       

[Important Explanation]
**Vendor lock-out occurs when the provider suddenly leaves the market, as during a bankruptcy or acquisition. 
The risks associated with lock-out include denial of service, because of total unavailability of your data. 
The best way to handle these risks is to have another, full backup of your data with another vendor and the ability to reconstitute your operating environment in a time frame that doesn’t exceed your recovery time objective (RTO).**

The other options do not aid in addressing vendor lock-out.

### [tricky] Question # 30 - In a public cloud services arrangement, who creates governance that will determine which controls are selected for the [data center] and how they are deployed?    
A. The cloud provider    
B. The cloud customer    
C. The regulator(s)    
D. The end user   
Answer: A. 

[important) **Because the cloud provider owns and operates the cloud data center, the provider will craft and promulgate the governance that determines the control selection and usage.** 
This is another risk the cloud customer must consider when migrating into the cloud; 
the customer’s governance will no longer have direct precedence over the environment where the customer’s data is located.
Both the cloud customer and the regulator(s) may have specific control mandates that might require the customer to deploy additional security controls (at the customer side, within the data, as agents on the user devices, or on the provider side or in application programming interfaces [APIs] as allowed by the service model or contract), so options B and C are also partially true, but A is a better answer as it is more general.
Option D untrue because the end user does not determine which controls are selected for the cloud data center and how they are deployed. That is the responsibility of the cloud provider.

### Question # 31 - [important] What is the term that describes the situation when a malicious user or attacker can exit the restrictions of a virtual machine (VM) and access another VM residing on the same host?    
A. Host escape    
B. Guest escape   
C. Provider exit   
D. Escalation of privileges    
Answer: B.   

The question describes a guest escape.
Options A and C are other risks of operating in the cloud. Option D can lead to A or B, but B describes the more specific situation and therefore the correct answer.

### Question # 32 - [important] What is the term that describes the situation when a malicious user or attacker can exit the restrictions of a single host and access other nodes on the network?   
A. Host escape    
B. Guest escape    
C. Provider exit    
D. Escalation of privileges    
Answer: A. 

The question describes host escape.
Options B and C are other risks of operating in the cloud. Option D can lead to A or B, but A is the more specific situation and therefore the correct answer.

### Question # 33 - ___________________ is/are probably the main cause of virtualization sprawl. 
A. Malicious attackers   
B. Lack of provider controls   
C. Lack of customer controls   
D. Ease of use    
Answer: D.  

Because most cloud users don’t see direct costs in creating new VM instances (the bills usually go to a single point of contact in the organization, not the user or the user’s office), they may tend to create additional VMs at a significant rate, without realizing the attendant cost. This is largely because it is so easy to do and has no apparent cost, from their perspective.

All the other options do not cause virtualization sprawl.

### Question # 34 - Sprawl is mainly a(n) ___________________ problem.    
A. Technical   
B. External   
C. Management   
D. Logical    
Answer: C.    

**Sprawl needs to be addressed from a managerial perspective because it is caused by allowed user actions (usually in a completely authorized capacity).**

Options A and D mean the same thing and could be considered as contributing to sprawl because the technological capabilities of virtualization create the ease of use that can cause sprawl. However, option C is a better answer.
Option B is incorrect; sprawl occurs within the organization.

### Question # 35 - Which of the following risks exists in the traditional environment but is dramatically increased by moving into the cloud?   
A. Physical security breaches    
B. Loss of utility power    
C. Financial upheaval    
D. Man-in-the-middle attacks    
Answer: D. 

**Because all cloud access is remote access, the risks to data in transit are dramatically heightened in the cloud.**

The other options exist in both the traditional environment and the cloud but are probably actually reduced in the cloud because cloud providers can use economies of scale to invest in means to reduce those risks in ways that individual organizations would not be able to.

### Question # 36 - A fundamental aspect of security principles, ___________________ should be implemented in the cloud as well as in traditional environments.
A. Continual uptime    
B. Defense in depth     
C. Multifactor authentication     
D. Separation of duties    
Answer: B. 

**Defense in depth, or layered defense, is perhaps the most fundamental characteristic of all security concepts.**
Options A and C are security aspects of some environments, and option A is likely to be a necessary trait of managed cloud services, but they are not fundamentals—they are specifics.
Option D is specifically an administrative control; the question is looking for a fundamental aspect of security. Option B is more general (it applies to all types of security, in all industries and uses) and therefore is the correct choice for this question.

### Question # 37 - From a security perspective, automation of configuration aids in ___________________.     
A. Enhancing performance    
B. Reducing potential attack vectors    
C. Increasing ease of use of the systems    
D. Reducing need for administrative personnel    
Answer: B.     

**A secure baseline configuration, applied and maintained automatically, ensures the optimum security footprint with the least attack surface.**
All the other options are benefits of automated configuration but are not specifically security enhancements.
	

### Question # 38 - ___________________ is the most prevalent protocol used in identity federation.      
A. Hypertext Transfer Protocol (HTTP)    
B. Security Assertion Markup Language (SAML)  
C. File Transfer Protocol (FTP)   
D. WS-Federation    
Answer: B. 

The Security Assertion Markup Language (SAML) is probably the most common protocol being used for identity federation at the moment.
Options A and C are not identity federation protocols.
Option D is a federation specification, but it also uses SAML tokens.

 ### Question # 39 - [important] A user signs on to a cloud-based social media platform. In another browser tab, the user finds an article worth posting to the social media platform. The user clicks on the platform’s icon listed on the article’s website, and the article is automatically posted to the user’s account on the social media platform. This is an example of what?     
A. Single sign-on    
B. Insecure direct identifiers    
C. Identity federation    
D. Cross-site scripting   
Answer: C. 

**This is a very popular function of federated identity.**
**Single sign-on (SSO) is similar to federation,** but it is limited to a single organization; federation is basically SSO across multiple organizations. Option A is incorrect.

**Options B and D are threats listed in the Open Web Application Security Project (OWASP) Top Ten; they are incorrect.**

### [important] Question # 40 - A group of clinics decides to create an identification federation for their users (medical providers and clinicians). If they opt to review each other, for compliance with security governance and standards they all find acceptable, what is this federation model called?  
A. Cross-certification    
B. Proxy    
C. Single sign-on     
D. Regulated    
Answer: A.   

**The cross-certification federation model is also known as a web of trust.**

Proxy is another model for federation, so option B is incorrect.
**Single sign-on is similar to federation, but it is limited to a single organization**; 
option C is incorrect.
Option D does not have relevance in this context and therefore incorrect as an answer.
	
 ### [important] Question # 41 - A group of clinics decides to create an identification federation for their users (medical providers and clinicians). If they opt to hire a third party to review each organization, for compliance with security governance and standards they all find acceptable, what is this federation model called?  
A. Cross-certification   
B. Proxy    
C. Single sign-on    
D. Regulated    
Answer: B. 

**In the proxy federation model, the third party acts on behalf of the member organizations, reviewing each to ensure that they are all acceptable to the others**.

Cross-certification is another model for federation, so option A is incorrect.
Single sign-on is similar to federation, but it is limited to a single organization; option C is incorrect.
Option D does not have relevance in this context and is therefore incorrect as an answer.
	
 ### Question # 42 - [important] A group of clinics decides to create an identification federation for their users (medical providers and clinicians). If they opt to use the web of trust model for federation, who is/are the identity provider(s)?    
A. Each organization    
B. A trusted third party    
C. The regulator overseeing their industry    
D. All of their patients    
Answer: A. 

**In a web of trust federation model, all of the participating organizations are identity providers; each organization will assign identity credentials to its own authorized users, and all the other organizations in the federation will accept those credentials.**

A trusted third party, regulators, and clientele are not involved in the web of trust model, so the other options are incorrect.

 ### Question # 43 - [important] A group of clinics decides to create an identification federation for their users (medical providers and clinicians). If they opt to use the web of trust model for federation, who is/are the service providers?     
A. Each organization    
B. A trusted third party    
C. The regulator overseeing their industry    
D. All of their patients     
Answer: A.    

**In a web of trust model, each member organization usually supplies both the access/identification credentials and the resources that the users want to access, so the organizations are both the identity providers and service providers in a web of trust federation model.**

A trusted third party, regulators, and clientele are not involved in the web of trust model, so the other options are incorrect.

 ### Question # 44 - A group of clinics decides to create an identification federation for their users (medical providers and clinicians). In this federation, all of the participating organizations would need to be in compliance with what U.S. federal regulation?    
A. Gramm-Leach-Bliley Act (GLBA)    
B. Family and Medical Leave Act (FMLA)    
C. Payment Card Industry Data Security Standard (PCI DSS)     
D. Health Information Portability and Accountability Act (HIPAA)    
Answer: D. 

While it’s likely the participating organizations will be subject to other federal regulations, HIPAA covers electronic patient information, so it will definitely be applicable in this case.

**GLBA covers financial and insurance service providers**, so option A is incorrect.
**FMLA dictates how employers give vacation time to employees**, so option B is not correct.
PCI DSS is a contractual, not regulatory, standard, so option C is incorrect.

 ### [easy but tricky] Question # 45 - What is the process of granting access to resources?   
A. Identification    
B. Authentication    
C. Authorization    
D. Federation    
Answer: C.   

The question describes authorization.
Options A and B are part of the overall identity and access management (IAM) process, as is option C, but they do not specifically describe granting access to resources.
Federation is a means of conducting IAM across organizations; option C is more specific, so D is incorrect.
	
### Question # 46 - The process of identity management includes all the following elements except ___________________.   
A. Provisioning     
B. Maintenance     
C. Deprovisioning     
D. Redaction    
Answer: D.     

**Redacting is an editorial process of excising sensitive information from disclosed data.** 
All the other options are elements of identity management.
	
### Question # 47 - Which organizational entity usually performs the verification part of the provisioning element of the identification process?       
A. Information technology (IT)    
B. Security    
C. Human resources (HR)    
D. Sales    
Answer: C.    

This is a complicated question and requires thinking through the portions of the identification process.
Identification of personnel is usually verified during the hiring process, when HR checks identification documents (such as a passport or birth certificate) to confirm the applicant’s identity, often as part of a tax registration process.
Options A and B include offices that may play a role in the identification process, but it is usually HR that does the actual verification.
Option D, “Sales” is untrue. If a Sales department exists in an organization, it does not perform the verification part of the provisioning element of the identification process.
	
### Question # 48 - Of the following options, which is a reason cloud data center audits are often less easy to verify than traditional audits?        
A. Data in the cloud can’t be audited.    
B. Controls in the cloud can’t be audited.     
C. Getting physical access can be difficult.     
D. There are no regulators for cloud operations.         
Answer: C.     

**Cloud providers may be reluctant to grant physical access, even to their customers, on the assumption that allowing access would disclose information about security controls**. 
In some cases, cloud customers won’t even know the location(s) of the data center(s) where their data is stored.
The other options are all untrue. Data in the cloud and controls in the cloud can most certainly be audited. So, options A and B are incorrect. D is untrue; there are regulators for all industries, including those that operate in the cloud.
	
### Question # 49 - Of the following options, which is a reason cloud data center audits are often less easy to verify than traditional audits?     
A. Cryptography is present.    
B. Auditors don’t like the cloud.         
C. Cloud equipment is resistant to audit.      
D. They often rely on data the provider chooses to disclose.      
Answer: D.      

In many circumstances, a cloud audit will depend on which information a cloud provider discloses, which makes auditing difficult and less trustworthy.

Option A is incorrect because cryptography is sometimes present in traditional environments and audits still take place.

Option B is incorrect; auditors’ opinions are not relevant.

Option C is untrue; equipment does not resist auditing—it is inanimate and unfeeling.

### Question # 50 - Of the following options, which is a reason cloud data center audits are often less easy to verify than audits in standard data centers?  
A. They frequently rely on third parties.    
B. The standards are too difficult to follow.     
C. The paperwork is cumbersome.     
D. There aren’t enough auditors.     
Answer: A.      

Because cloud audits are often the result of third-party assertions, recipients of cloud audit reports may be more skeptical of the results than they would have been of traditional audits, in which the recipients may have performed firsthand.

Option B is untrue. The difficulty of standards is not a hindrance to audit.

Option C is untrue. Paperwork does not hinder audits.

Option D is not only untrue, but also hilarious. If you have ever been involved in an audit, you know that there are plenty of auditors to go around.

### Question # 51 - The cloud customer will usually not have physical access to the cloud data center. This enhances security by ___________________.     
A. Reducing the need for qualified personnel    
B. Limiting access to sensitive information     
C. Reducing jurisdictional exposure     
D. Ensuring statutory compliance     
Answer: B.       

The “sensitive information,” in this case, is whatever knowledge of the data center’s security controls and processes might be gathered by physically visiting the data center. Even though a cloud customer cannot get access to the facility, this also means that other cloud customers (some of whom may be inimical to another customer’s interests) also will not have access, so none would have advantage over the other(s).

Option A is incorrect because qualified personnel are still required whether a cloud environment has limited access to their data center or not. In fact, security may be degraded by having unqualified personnel rather than qualified personnel working in the cloud data center.

Option C is incorrect because reducing jurisdictional exposure does not enhance security.
There may be a correlation between ensuring statutory compliance and enhancing security as it applies to limiting access to the cloud data center. However, option B is a better answer because it is certainly true. Therefore, option D is not the best answer to the question.

### Question # 52 - Which of the following controls would be useful to build into a virtual machine baseline image for a cloud environment?      
A. GPS tracking/locator     
B. Automated vulnerability scan on system startup     
C. Access control list (ACL) of authorized personnel       
D. Write protection       
Answer: B. 

Because VMs don’t take updates when they are not in use (snapshotted and saved as image files) and updates may be pushed while the VMs are saved, it’s important to ensure that they receive updates when they are next instantiated.

A physical tracking mechanism won’t be of much aid for virtual devices because they aren’t physically stolen like hardware boxes, so option A is incorrect.
Having an ACL in the image baseline would create a situation where every user from every cloud customer could access every VM in the data center; option C is incorrect.
Write protection is used in forensic analysis of machines (virtual or otherwise); it would not be useful in an operational baseline. Option D is incorrect.

### Question # 53 - Which of the following controls would be useful to build into a virtual machine baseline image for a cloud environment?       
A. Automatic registration with the configuration management system      
B. Enhanced user training and awareness media         
C. Mechanisms that prevent the file from being copied       
D. Keystroke loggers       
Answer: A. 

Version control can be difficult in a virtual environment because saved VMs don’t receive updates. Ensuring that each VM is the correct version is a function of configuration management (CM), and CM controls can be built into the baseline.
Each organization will have its own training and awareness program, and there is no one-size-fits-all solution that is appropriate; this does not belong in the baseline. Option B is incorrect.

Having a baseline that cannot be copied is pointless; option C is incorrect.

Keystroke loggers will create a huge volume of detailed, stored data that will pose more of a security risk (and may actually be a violation of customer privacy regulations) than any benefit it offers; 

option D is incorrect.

### Question # 54 - Virtual machine (VM) configuration management (CM) tools should probably include ___________________.      
A. Biometric recognition        
B. Anti-tampering mechanisms        
C. Log file generation       
D. Hackback capabilities      
Answer: C.      

Event logging is essential for incident management and resolution; this can be set as an automated function of the CM tools.
Not all systems need or can utilize biometrics; option A is incorrect.
Usually, tampering refers to physical intrusion of a device; since the question is about VMs, it is probably not applicable. Option B is incorrect.
Hackback is illegal in many jurisdictions; option D is incorrect.

### Question # 55 - Using a virtual machine baseline image could be very useful for which of the following options?        
A. Physical security       
B. Auditing       
C. Training       
D. Customization       
Answer: B.        

A specified configuration built to defined standards and with a controlled process can be used to demonstrate that all VMs within an environment include certain controls; this can greatly enhance the efficiency of an audit process.
The VM’s image has very little to do with physical security or training; options A and C are incorrect.
Baseline images are the opposite of customization; option D is incorrect.

### Question # 56 - What can be revealed by an audit of a baseline virtual image, used in a cloud environment?       
A. Adequate physical protections in the data center       
B. Potential criminal activity before it occurs      
C. Whether necessary security controls are in place and functioning properly      
D. Lack of user training and awareness        
Answer: C. 

The baseline will contain the suite of security controls applied uniformly throughout the environment.
A VM image audit is unlikely to involve any form of physical security; A is incorrect.
Baselines won’t predictively show malicious activity; B is incorrect.
Baselines also do not have anything to do with user training and awareness; option D is incorrect.

### Question # 57 - Using one cloud provider for your operational environment and another for your BC/DR backup will also give you the additional benefit of ___________________.     
A. Allowing any custom VM builds you use to be instantly ported to another environment     
B. Avoiding vendor lock-in/lock-out      
C. Increased performance      
D. Lower cost     
Answer: B. 

Having an additional backup with a different provider means that if your primary provider becomes unusable for any reason (including bankruptcy or unfavorable contract terms), your data is not held hostage or lost.
Custom VMs may or may not work in a new environment; this is actually a risk when porting data out of the production environment; option A is incorrect.
Performance probably will not increase if data is replicated to another cloud provider; in fact, you will probably lose some load balancing capability you might have had if you kept the data and backups together. Option C is incorrect.
Having two providers will always be more costly than a single provider; option D is incorrect.

### Question # 58 - Having your BC/DR backup stored with the same cloud provider as your production environment can help you ___________________.      
A. Maintain regulatory compliance      
B. Spend less of your budget on traveling     
C. Train your users about security awareness     
D. Recover quickly from minor incidents     
Answer: D. 

Having the backup within the same environment can allow easy rollback to a last known good state or to reinstantiate clean VM images after minor incidents (e.g., a malware infection in certain VMs).
Ease of compliance will not be determined by the location of the backup, so option A is incorrect.
Traveling should not be a major cost for cloud usage; option B is incorrect.
The location of the backups won’t have any effect on user training; option C is incorrect.

### Question # 59 - If you use the cloud for BC/DR purposes, even if you don’t operate your production environment in the cloud, you can cut costs by eliminating your ___________________.      
A. Security personnel       
B. BC/DR policy     
C. Old access credentials       
D. Need for a physical hot site/warm site      
Answer: D.      

Having your data backed up and accessible in the cloud eliminates any need for having a distinct hot site/warm site separate from your primary operating environment; instead, your personnel can recover operations from anywhere with a good broadband connection.
Cloud BC/DR capability does not remove the necessity of security personnel and appropriate policies; both options A and B are incorrect.
Option C makes no sense as an answer to the question. It is unclear how you can cut costs by eliminating your old access credentials. In fact, it is difficult to imagine how that is a true statement. Therefore, option C is a poor choice and option D is the best choice.

### Question # 60 - If the cloud is used for BC/DR purposes, the loss of ___________________ could gravely affect your organization’s RTO.      
A. Any cloud administrator     
B. A specific VM     
C. Your policy and contract documentation      
D. ISP connectivity      
Answer: D. 

Without ISP connectivity, nobody will be able to use the Internet and, thus, the cloud. Of course, realistically, without Internet connectivity not much business will get done anyway, for most organizations, regardless of whether they were operating in the cloud or on-premise.

Option A is incorrect because the loss of any, single, cloud administrator is unlikely to gravely affect your organization’s RTO.

The loss of a specific VM will probably not gravely affect your organization’s RTO. VMs can be reinstantiated with ease. Option B is incorrect.

The loss of your policy and contract documentation cannot gravely affect your organization’s RTO. Option C is untrue.

### Question # 61 - What is the most important asset to protect in cloud BC/DR activities?      
A. Intellectual property     
B. Hardware at the cloud data center     
C. Personnel     
D. Data on portable media       
Answer: C.      

Health and human safety is always paramount in all security activity.
All the other options are assets that should be protected, but nothing is as important as option C, so they are incorrect answers for this question.

### [important]Question # 62 - When considering cloud data replication strategies (i.e., whether you are making backups at the block, file, or database level), which element of your organization’s BC/DR plan will be most affected by your choice?      
A. Recovery time objective     
B. Recovery point objective     
C. Maximum allowable downtime      
D. Mean time to failure     
Answer: B.      

[important] **The recovery point objective (RPO) is a measure of data that can be lost in an outage without irreparably damaging the organization. Data replication strategies will most affect this metric, as the choice of strategy will determine how much recent data is available for recovery purposes**.

Recovery time objective (RTO) is a measure of how long an organization can endure an outage without irreparable harm. This may be affected by the replication strategy, but not as much as the RPO. Option 

A is incorrect.

*#The maximum allowable downtime (MAD) is how long an organization can suffer an outage before ceasing to be an organization**. 
This is not dependent on the RPO, and the data replication strategy won’t have much effect on it at all. Option C is incorrect.

The mean time to failure (MTTF) is a measure of how long an asset is expected to last (usually hardware), as determined by the manufacturer/vendor. The data replication strategy will have no bearing on this whatsoever. Option D is incorrect.

### Question # 63 - In addition to BC/DR, what other benefit can your data archive/backup provide?     
A. Physical security enforcement      
B. Access control methodology     
C. Security control against data breach     
D. Availability for data lost accidentally      
Answer: D.       

A data backup/archive can offer your organization an operational “reachback” capability, where admins can assist users in recovering data lost by accident or carelessness.
The backup/archive does not aid in any of the areas in the other options. So, options A, B, and C are incorrect.

### Question # 64 - Which of the following risks is probably most significant when choosing to use one cloud provider for your operational environment and another for BC/DR backup/archive?     
A. Physical intrusion     
B. Proprietary formats/lack of interoperability     
C. Vendor lock-in/lock-out     
D. Natural disasters      
Answer: B.     

When using two different cloud providers, a cloud customer runs the risk that data/software formats used in the operational environment can’t be readily adapted to the other provider’s service, thus causing delays during an actual failover.
Risks of physical intrusion are neither obviated nor enhanced by choosing to use two cloud providers; option A is incorrect.
Using a different cloud provider for backup/archiving actually reduces the risks of outages due to vendor lock-in/lock-out and natural disasters, so options C and D are not correct.

### Question # 65 - Return to normal operations is a phase in BC/DR activity when the emergency is over and regular production can resume. Which of the following can sometimes be the result when the organization uses two different cloud providers for the production and BC/DR environments?       
A. Both providers are affected by the emergency, extending the time before return to normal can occur.     
B. The BC/DR provider becomes the new normal production environment.     
C. Regulators will find the organization in violation of compliance guidance.       
 D. All data is lost irretrievably.       
Answer: B. 

Theoretically, all the options are possibly true. However, option B is the most likely to occur and is fairly common in practice; the cost and risk of moving operations from one environment/provider to another is sizable, so staying with the secondary provider (making them the new primary) is a good way to reduce some of the risk involved in returning to normal.

### Question # 66 - Which of these determines the critical assets, recovery time objective (RTO), and recover point objective (RPO) for BC/DR purposes?      
A. Business drivers      
B. User input     
C. Regulator mandate     
 D. Industry standards      
Answer: A.     

The business requirements will determine the crucial aspects of BC/DR.
All the other options may constitute some input that will influence the BC/DR, but they are not the prevailing factors, so are incorrect.

### Question # 67 - What artifact—which should already exist within the organization—can be used to determine the critical assets necessary to protect in the BC/DR activity?     
A. Quantitative risk analysis     
B. Qualitative risk analysis      
C. Business impact analysis     
D. Risk appetite      
Answer: C.      

The business impact analysis (BIA) is designed for this purpose: to determine the critical path of assets/resources/data within the organization. It is a perfect tool to use in shaping the BC/DR plan.
The risk analyses options and the risk appetite option may provide input for the BIA, but they are not what is used to determine the critical assets necessary to protect in the BC/DR activity. So, options A, B, and D are incorrect.

### Question # 68 - Which of the following is probably the most important element to address if your organization is using two different cloud providers for the production and BC/DR environments?      
A. Do they cost the same?     
B. Do they have similar facility protections in place?     
C. What level of end-user support do they each offer?       
D. Can the backup provider meet the same SLA requirements as the primary?      
Answer: D.      

If the contingency operation will last for any extended period of time, it is important to know whether all the same service expectations can be met by the backup provider as were available in the production environment.
All the other questions are important, but not as crucial as option D, so they are incorrect.

### Question # 69 - In a managed cloud services arrangement, who invokes a BC/DR action?      
A. The cloud provider     
B. The cloud customer       
C. Depends on the contract       
D. Any user      
Answer: C. 

BC/DR responsibilities must be negotiated and codified in the contract; initiation could be something performed by provider or customer, depending on circumstances, so the parties must agree before those circumstances are realized.
It is exceedingly unlikely that “any user” in a managed cloud services arrangement can invoke a BC/DR action. Option D is therefore a poor choice for the answer to the question.

### Question # 70 - What do you need to do in order to fully ensure that a BC/DR action will function during a contingency?      
A. Audit all performance functions.     
B. Audit all security functions.     
C. Perform a full-scale test.     
D. Mandate this capability in the contract.      
Answer: C. 

Without a full test, you can’t be sure the BC/DR plan/process will work the way it is intended.
Audits are good, but they will not demonstrate actual performance the way a test will, so options A and B are incorrect.
It is important that the BC/DR capacity and performance be included in the contract, but that will not truly ensure that the functionality exists; a test is required, so option D is incorrect.

### Question # 71 - Which of the following is probably the most important activity, of those listed?      
A. Regularly update the BC/DR plan/process.     
B. Have contact information for all personnel in the organization.      
C. Have contact information for essential BC/DR personnel.      
D. Have contact information for local law enforcement.     
Answer: A.      

All of these are important, but without regular updates, the information will soon become outdated and a lot less useful.

### Question # 72 - The BC/DR plan/policy should include all of the following except ___________________.      
A. Tasking for the office responsible for maintaining/enforcing the plan     
B. Contact information for essential entities, including BC/DR personnel and emergency services agencies      
C. Copies of the laws/regulations/standards governing specific elements of the plan      
D. Checklists for BC/DR personnel to follow      
Answer: C.     

This is not an easy question, because every plan/policy should include mention of the governance documents that drive the formation of the plan/policy; however, these can be included by reference only—you don’t need to include full copies of these governance documents.
All the other options should be included in the BC/DR plan/policy.

### Question # 73 - The BC/DR plan/process should be written and documented in such a way that it can be used by ___________________.           
A. Users     
B. Essential BC/DR team members       
C. Regulators       
D. Someone with the requisite skills      
Answer: D.        

This question is difficult. You want your BC/DR plan/process to include sufficient detail such that it could be followed by someone with the right background (perhaps IT for certain roles, security for others, etc.) but without any experience or specific training in that role. This is because a contingency of the scope that would require initiation of BC/DR activities might involve dramatic, significant external forces to the point where the personnel normally tasked with BC/DR actions are not available (for instance, natural disasters, fire, civil disruption, etc.), so the tasks may need to be completed by whoever is available at the time.
The BC/DR plan/process should be written and documented in such a way that someone with the requisite skills can use it. It is unlikely that typical users or regulators have the requisite skills to perform many of the BC/DR activities. Therefore options A and C are poor choices for answers to the question.
It is tempting to choose option B, however, option D is a better answer because it ensures that someone with the requisite skills will be able to read the BC/DR plan and perform the activities they document. Having to rely on essential BC/DR team members being present and available to follow the plan is risky. So option B is incorrect.

### Question # 74 - Which of the following probably poses the most significant risk to the organization?     
A. Not having essential BC/DR personnel available during a contingency     
B. Not including all BC/DR elements in the cloud contract     
C. Returning to normal operations too soon      
D. Telecommunications outages     
Answer: C.      

A premature return to normal operations can jeopardize not only production, but personnel; if the contingency that caused the BC/DR action is not fully complete/addressed, there may still be danger remaining.
The BC/DR plan/process should take into account both the absence of essential personnel and telecommunications capabilities, so options A and D are incorrect.
Option B does present a serious problem for the organization, but C is still a greater risk, so B is incorrect.

### Question # 75 - Which of the following probably poses the most significant risk to the organization?     
A. Lack of data confidentiality during a contingency    
B. Lack of regulatory compliance during a contingency      
C. Returning to normal operations too late      
D. Lack of encrypted communications during a contingency       
Answer: C. 

Not returning to normal operations in a timely fashion can cause you to exceed the RTO and the MAD.
During a contingency, some of the requirements your organization faces may relax somewhat; for instance, if a life-threatening natural disaster occurs, regulators will likely understand if some of the normal compliance activities/controls are not fully incorporated while personnel and assets are moved to safety (depending on the nature of the industry, of course). Options A and B are therefore incorrect; option C poses a greater risk.

Option D is a distractor; not all organizations need encrypted communications during contingencies.

### Question # 76 - Why does the physical location of your data backup and/or BC/DR failover environment matter?       
A. It may affect regulatory compliance.     
B. Lack of physical security.      
C. Environmental factors such as humidity.      
D. It doesn’t matter. Data can be saved anywhere without consequence.       
Answer: A.       

Depending on your industry and the nature of your data, moving information into another jurisdiction may affect or invalidate your regulatory compliance.
Cloud providers, wherever they are located, should compensate for environmental and physical security factors, so this should have no impact on your potential risk; options B and C are incorrect.

Option D is incorrect because it is blanket statement that is not always true. In fact, for some organizations, the physical location where their data is stored can have serious regulatory consequences.

### Question # 77 - According to the European Union Agency for Network and Information Security (ENISA), a cloud risk assessment should provide a means for customers to accomplish all these assurance tasks except ___________________.      
A. Assess risks associated with cloud migration    
B. Compare offerings from different cloud providers      
C. Reduce the risk of regulatory noncompliance     
D. Reduce the assurance burden on cloud providers      
Answer: C.     

ENISA’s approach to cloud risk assessments does not specifically address this type of assurance, probably because of the wide variety of possible regulators and the difficulty in crafting a risk assessment that would address them all.
All the other options are assurance efforts that ENISA’s cloud risk assessment is meant to enhance, so they are incorrect answers for this question.

### Question # 78 - The European Union Agency for Network and Information Security’s (ENISA’s) definition of cloud computing differs slightly from the definition offered by (ISC)2 (and, for instance, NIST). What is one of the characteristics listed by ENISA but not included in the (ISC)2 definition?        
A. Metered service      
B. Shared resources      
C. Scalability     
D. Programmatic management       
Answer: D.      

ENISA includes “programmatic management” as a defining trait of cloud computing, even specifying “through WS API.” This is not included in the definition published by (ISC)2 (or by NIST).
All the other characteristics are included in the (ISC)2 (and NIST) definitions.

### Question # 79 - Risk should always be considered from a business perspective. Risk is often balanced by corresponding ___________________.      
A. Profit      
B. Performance        
C. Cost          
D. Opportunity       
Answer: D.      

The only reason organizations accept any level of risk is because of the potential benefit also afforded by a risky activity.
Profit is not the hallmark of every opportunity (or every organization—many organizations are nonprofit or government-based), so option A is incorrect.
Likewise, not all risky activities offer a chance to enhance performance, so option B is incorrect.
Cost is not a benefit, so that doesn’t even make sense in the context of the question; option C is not correct and a distractor.

### Question # 80 - When considering the option to migrate from an on-premise environment to a hosted cloud service, an organization should weigh the risks of allowing external entities to access the cloud data for collaborative purposes against ___________________.      
A. Not securing the data in the traditional environment     
B. Disclosing the data publicly      
C. Inviting external personnel into the traditional workspace in order to enhance collaboration       
D. Sending the data outside the traditional environment for collaborative purposes          
Answer: D.       

The cloud greatly enhances opportunities for collaboration between organizations, mostly by giving external parties some limited access to the owner’s data in the cloud. While there is risk in this situation, the truly comparable risk in the traditional environment would result from sending data outside the organization to external collaborators. (Furthermore, the organization has to balance this risk against the cost of business of not being able to collaborate, if data is never shared with third parties.)

Option A is ridiculous; data should be secured whether it is in an on-premise environment or in the cloud.

Option B does not create a true equivalence; disclosing data under controlled conditions is not the same as public disclosure.

Option C is not equivalent to the costs/benefits of the other forms of collaboration; it would be too cumbersome for the organization to truly benefit from collaboration in a modern business environment.

### Question # 81 - There are many ways to handle risk. However, the usual methods for addressing risk are not all possible in the cloud because ___________________.      
A. Cloud data risks cannot be mitigated     
B. Migrating into a cloud environment necessarily means you are accepting all risks      
C. Some risks cannot be transferred to a cloud provider       
D. Cloud providers cannot avoid risk      
Answer: C. 

Under current legal frameworks, some risks (such as legal liability for privacy data breaches) cannot be transferred to a contracted party, so the data owners (that is, cloud customers) will still retain those risks.

Option A is ridiculous; risks can and should be mitigated, even in the cloud.

Option B is not correct; cloud migration will require some risk acceptance, but that is true for everything except avoided risk.

Option D is incorrect; cloud providers can choose not to offer services or not to accept certain clients.

### Question # 82 - In which cloud service model does the customer lose the most control over governance?      
A. Infrastructure as a service (IaaS)      
B. Platform as a service (PaaS)      
C. Software as a service (SaaS)         
D. Private cloud       
Answer: C.      

As the models increase in level of abstraction and service, the customer’s control over the environment decreases.

### Question # 83 - Which of the following poses a new risk in the cloud, not affecting the traditional, on-premise IT environment?     
A. Internal threats     
B. Multitenancy      
C. Natural disasters     
D. Distributed denial-of-service (DDoS) attacks      
Answer: B.       
Sharing resources with other, unknown customers (some of whom may be competitors of or even hostile to the organization) is a risk not faced by organizations that maintain their own, on-premise data centers.
All the other answers are threats that exist in both environments and are therefore incorrect.

### Question # 84 - In addition to the security offered by the cloud provider, a cloud customer must consider the security offered by ___________________.      
A. The respective regulator      
B. The end user(s)     
C. Any vendor the cloud customer previously used in the on-premise environment        
D. Any third parties the provider depends on      
Answer: D. 

Because supply chain dependencies can affect service, the cloud customer will need assurance that any third-party reliance is secure.
Regulators and end users do not provide security to the enterprise, so options A and B are incorrect.
The vendors used for on-premise security will no longer affect the data, so option C is incorrect.

### Question # 85 - Which of the following poses a new risk in the cloud, not affecting the traditional, on-premise IT environment?       
A. User carelessness     
B. Inadvertent breach       
C. Device failure       
D. Resource exhaustion      
Answer: D. 

It is possible that a cloud provider will be unable to handle an increased load during contingency situations where all its customers are demanding additional resources far beyond their usual contracted rate. While this is unlikely (many cloud providers, especially the major operators in the market, have resources that greatly exceed any possible demand by their customers), it could conceivably occur if a significant number of customers experience an immediate and dramatic need for capacity, such as during a major BC/DR event (a region-wide natural disaster or a physical attack on a city). This is not something that would affect an on-premise solution; your organization’s data center is not affected by others’ demand for resources (although the on-premise environment may be affected by the same contingency that causes cloud resource exhaustion, of course).
All the other options portray risks faced by both cloud and on-premise environments.

### Question # 86 - Where is isolation failure probably least likely to pose a significant risk?       
A. Public cloud      
B. Private cloud       
C. PaaS environment       
D. SaaS environment      
Answer: B.     

Guest escape (a malicious user leaving the confines of a VM and able to access other VMs on the same machine) is less likely to occur and to have a significant impact in an environment provisioned for and used by a single customer.

In a public cloud, this is more likely and would be more significant, so option A is incorrect.
The service model doesn’t specifically dictate the likelihood of occurrence or impact (both PaaS and IaaS could be in a private or public cloud, which is the more important factor), so both options C and 
D are incorrect.

### Question # 87 - Which of the following poses a new risk in the cloud, not affecting the traditional, on-premise environment?      
A. Fire     
B. Legal seizure of another firm’s assets        
C. Mandatory privacy data breach notifications       
D. Flooding       
Answer: B.       

Because of multitenancy and shared resources in the cloud, law enforcement may seize a cloud customer’s assets (a physical device, a data set, etc.) and inadvertently capture assets belonging to another, unsuspected/innocent organization. This could not happen in a situation where all individual organizations only kept their own assets on their own premises.
All the other options include risks that exist in the traditional, on-premise environment, as well as the cloud, so they are incorrect.

### Question # 88 - Which of these does the cloud customer need to ensure protection of intellectual property created in the cloud?      
A. Digital rights management (DRM) solutions        
B. Identity and access management (IAM) solutions       
C. Strong contractual clauses        
D. Crypto-shredding        
Answer:  C.       

This is not an easy question; the simple answer seems to be option A, which is true for data stored/saved/migrated to the cloud (and property that already has been created in the cloud), but for new intellectual property created in the cloud, strong contract language in favor of the customer’s rights is very necessary. Without clear-language support about the customer’s ownership of all intellectual property created in the cloud data center, the cloud provider could, ostensibly, make a claim on such property, as the provider’s resources were used in a collaborative effort to create that property.

Options B and D are security controls used to protect all sorts of assets, including intellectual property, but they are not as specifically addressing the creation of new intellectual property in the cloud the way explicit contract clauses would, so option C is still the better answer.

### Question # 89 - What could be the result of failure of the cloud provider to secure the hypervisor in such a way that one user on a virtual machine can see the resource calls of another user’s virtual machine?     
A. Unauthorized data disclosure    
B. Inference attacks    
C. Social engineering    
D. Physical intrusion   
Answer: B.     

While it is possible that one guest VM seeing the resource calls of another VM could possibly allow one guest to see the other’s data, it’s much more likely that a user seeing another user’s use of resources, rather than raw data, would allow the viewer to infer something about the victim’s behavior/usage/assets.
Likewise, it may be possible for the viewer to leverage knowledge of this usage as part of a social engineering attack, but that would be subsequent to the inference itself; option B is still better than C.
Lack of resource isolation does not affect physical intrusions, which is just a distractor here.

### Question # 90 - Key generation in a cloud environment might have less entropy than the traditional environment for all the following reasons except ___________________.      
A. Lack of direct input devices     
B. No social factors     
C. Uniform build     
D. Virtualization     
Answer: B.     

Social factors should not/don’t affect the level of entropy in a random number generator.
However, all the other factors listed in the other answers do, and that means that a malicious user in the cloud would be more likely (statistically) to guess/predict the random number used to create/seed an encryption key made in that same cloud environment. Cloud customers should take this into account when designing/planning their cloud configuration.

### Question # 91 - Lack of industry-wide standards for cloud computing creates a potential for ___________________.      
A. Privacy data breach      
B. Privacy data disclosure      
C. vendor lock-in     
D. vendor lock-out    
Answer: C.     

Without uniformity of data formats and service mechanisms, there is no assurance that a customer would be able to easily move their cloud operation from one provider to another; this can result in lock-in.
All the other options are not affected by lack of standards.

### Question # 92 - What can hamper the ability of a cloud customer to protect their assets in a managed services arrangement?     
A. Prohibitions on port scanning and penetration testing      
B. Geographical dispersion      
C. Rules against training users     
D. Laws that prevent them from doing so        
Answer:  A.      

Many cloud providers prohibit activities that are common for administrative and security purposes but can also be construed/used for hacking; this includes port scanning and penetration testing. These restrictions can reduce the customer’s ability to perform basic security functions.
While geographical dispersion of cloud assets might make securing those assets more difficult in the notional sense (customer administrators can’t physically visit the devices that host their data), remoteness does not necessarily inhibit good security practices, which can be performed at a remove. This is not as detrimental as rules against port scanning/pen testing, so option B is incorrect.
There are no rules against user training or laws against securing your own assets, in the cloud or otherwise; options C and D are incorrect.

### Question # 93 - Cloud administration almost necessarily violates the principles of the ___________________ security model.      
A. Brewer-Nash (Chinese Wall)   
B. Graham-Denning   
C. Bell-LaPadula    
D. Biba    
Answer: A.     

Brewer-Nash was specifically created for managed services arrangements, where an administrator for a given customer might also have access to a competitor’s data/environment; the model requires that administrators not be assigned to competing customers. In the modern cloud provider model, a cloud data center administrator will almost definitely have access to many customers from the same industry (i.e., competitors) but probably won’t even know it.
All the other options are access control security models; cloud administrators will not (or should not) be assigning access rights, so all these options are wrong.

### Question # 94 - The physical layout of a cloud data center campus should include redundancies of all the following except ___________________.    
A. Physical perimeter security controls (fences, lights, walls, etc.)    
B. The administration/support staff building    
C. Electrical utility lines          
D. Communications connectivity lines     
Answer:  B. 

Administrative and support staff are usually not part of the critical path of a data center; they are nonfunctional-requirement elements, not functional requirements.
All the other options are mission-critical elements of the cloud data center and must have redundancy capabilities.

### Question # 95 - Best practice for planning the physical resiliency for a cloud data center facility includes ___________________.    
A. Having one point of egress for personnel     
B. Ensuring that any cabling/connectivity enters the facility from different sides of the building/property      
C. Ensuring that all parking areas are near generators so that personnel in high-traffic areas are always illuminated by emergency lighting, even when utility power is not available       
D. Ensuring that the foundation of the facility is rated to withstand earthquake tremors        
Answer: B. 

To avoid a situation where severing a given physical connection results in severing its backup as well (such as construction/landscaping, etc.), have redundant lines enter on different sides of the building.
For health and human safety, multiple egress points from each facility is preferred (and often required by law); option A is incorrect.
Emergency lighting should receive power regardless of their proximity to the power source, and parking vehicles near generators is a bad idea from a safety perspective; option C is incorrect.
Not all facilities need to withstand earthquakes; this may be true of data centers in California, but not in Sydney, so it is not an industry-wide best practice. Option D is incorrect.

### Question # 96 - The physical layout of a cloud data center campus should include redundancies of all the following except ___________________.     
A. Generators    
B. HVAC units     
C. Generator fuel storage        
D. Points of personnel ingress      
Answer: D.      

People entering the facility can be vectored through a single security checkpoint as a means of enhancing access control; multiple lines of ingress are not necessary (although multiple lines of egress are essential to ensure health and human safety).
All the other options are facility elements that require redundancy.

### Question # 97 - There are two reasons to conduct a test of the organization’s recovery from backup in an environment other than the primary production environment. Which of the following is one of them?     
A. It costs more to conduct a test at the same location as the primary workplace.    
B. You don’t want to waste travel budget on what is only a test.    
C. The risk of negative impact to both production and backup is too high.    
D. There won’t be enough room for everyone to sit in the primary facility.      
Answer: C. 

A recovery from backup into the production environment carries the risk of failure of both data sets—the production set and the backup set. This can cause cataclysmic harm to the organization.
Recovering in the primary facility would probably be cheaper than having a different test facility, so option A is incorrect.
A proper test is worth the financial expenditure, so option B is incorrect.
Option D is incorrect because any BCDR plan would account for sufficient personnel workspace.

### Question # 98 - There are two reasons to conduct a test of the organization’s recovery from backup in an environment other than the primary production environment. Which of the following is one of them?    
A. It is good to invest in more than one community.    
B. You want to approximate contingency conditions, which includes not operating in the primary location.      
C. It is good for your personnel to see other places occasionally.      
D. Your regulators won’t follow you off-site, so you’ll be unobserved during your test.      
Answer: B.      

Assuming your facility is not available during contingency operations allows you to better approximate an emergency situation, which adds realism to the test.
Though option A is an act of benevolence on the part of the organization towards the community, option B is still a better answer for the question.
Option C is an act of benevolence on the part of the organization towards the employee, option B is still a better answer for the question.
Option D is incorrect because it makes assumptions that cannot be counted upon. Regulatory oversight should not be avoided, and should always be assumed.

### Question # 99 - In an IaaS arrangement, who accepts responsibility for securing cloud-based applications?     
A. The cloud provider     
B. The cloud customer      
C. The regulator        
D. The end user/client     
Answer: B.      

In an infrastructure as a service (IaaS) model, the provider is only responsible for provisioning the devices and computing/storage capacity; the customer is responsible for everything else, including the security of the applications.
All the other answers are incorrect because those individuals/organizations do not accept responsibility for securing cloud-based applications.

### Question # 100 - Industry best practices dictate that cloud customers do not ___________________.     
A. Create their own identity and access management (IAM) solutions   
B. Create contract language that favors them over the provider   
C. Retrain personnel for cloud operations    
D. Encrypt data before it reaches the cloud    
Answer: A.     

According to ENISA, custom IAM builds can become weak if not properly implemented.
Strong contract language in favor of the customer is always desirable for the customer, so option B is incorrect.
Training for specific conditions is always advisable, so option C is incorrect.
There is nothing wrong with having encryption take place before data is sent to the cloud, so option D is incorrect.

### Question # 101 - It is possible for the cloud customer to transfer ___________________ risk to the provider, but the cloud customer always retains ultimate legal risk.    
A. Market     
B. Perception      
C. Data     
D. Financial     
Answer: D.     

With strong contract terms, the cloud customer may be able to recover monetary damages (and even penalties) from the cloud provider as a result of a loss suffered by the customer; however, legal liability remains with the cloud customer.
The other answers are not relevant in this context.

### Question # 102 - A process for ___________________ can aid in protecting against data disclosure due to lost devices.      
A. User punishment        
B. Credential revocation         
C. Law enforcement notification      
D. Device tracking        
Answer: B.      

Revoking credentials that might be lost when a device goes missing is a way to mitigate the possibility of those credentials being used by an unauthorized person.
Punishing a user and notifying law enforcement does not prevent data from being disclosed; options A and C are incorrect.
Tracking devices may assist recovery efforts, but it won’t protect against data disclosures during the period the device is not under the organization’s control; option D is incorrect.

### Question # 103 - All of the following can be used in the process of anomaly detection except ___________________.     
A. The ratio of failed to successful logins    
B. Transactions completed successfully      
C. Event time of day           
D. Multiple concurrent logins      
Answer: B. 

Of all these options, only B is not something that will reveal untoward behavior.

### Question # 104 - Critical components should be protected with ___________________.     
A. Strong passwords    
B. Chain-link fences     
C. Homomorphic encryption      
D. Multifactor authentication      
Answer: D.      

Multifactor authentication offers additional protections for assets that are critical to the organization.
All logins should utilize strong passwords, whether they are critical or not, so option A is incorrect.
Some form of physical perimeter security is useful, but not necessarily chain-link fences, and not only for critical assets (perimeter security will protect all assets on the campus), so option B is incorrect.
Homomorphic encryption is a theoretical technology; option C is incorrect.

### Question # 105 - It’s important to maintain a current asset inventory list, including surveying your environment on a regular basis, in order to ___________________.     
A. Prevent unknown, unpatched assets from being used as back doors to the environment      
B. Ensure that any lost devices are automatically entered into the acquisition system for repurchasing and replacement     
C. Maintain user morale by having their devices properly catalogued and annotated     
D. Ensure that billing for all devices is handled by the appropriate departments     
Answer: A. 

An asset that is not tracked will not be maintained properly, and an improperly maintained asset provides an avenue for attack.

Options B and D are management issues, not security issues; option A is preferable to both of them.

Option C is incorrect; users don’t care if their devices are catalogued and annotated. Option C is a poor choice for an answer to the question.

### Question # 106 - Which of the following can enhance data portability?   
A. Interoperable export formats    
B. Egress monitoring solutions    
C. Strong physical protections   
D. Agile business intelligence    
Answer: A.     

Data formatted in a manner that allows its reuse in other environments is essential for portability.
None of the other options are relevant to the issue of data portability.

### Question # 107 - Which of the following can enhance application portability?     
A. Using the same cloud provider for the production environment and archiving     
B. Conducting service trials in an alternate cloud provider environment     
C. Providing cloud-usage training for all users     
D. Tuning web application firewalls (WAFs) to detect anomalous activity in inbound communications     
Answer: B. 

Testing is a great way to enhance assurance that applications will work in the new environment.
None of the other options are relevant to the issue of application portability.

### Question # 108 - What should the cloud customer do to ensure that disaster recovery activities don’t exceed the maximum allowable downtime (MAD)?    
A. Make sure any alternate provider can support the application needs of the organization.     
B. Ensure that contact information for all first responder agencies are correct and up-to-date at all times.     
C. Select an appropriate recovery time objective (RTO).     
D. Regularly review all regulatory directives for disaster response.      
Answer: C. 

The RTO must always be less than the MAD.
It is good to know that services will operate in the alternate environment and that first response contact info is current, but neither determines the speed with which services and data will be available during contingency operations; options A and B are incorrect.
Regulators will usually not dictate MAD/RTO for a given organization; option D is incorrect.

### Question # 109 - Which of the following would probably best aid an organization in deciding whether to migrate from a traditional environment to a particular cloud provider?    
A. Rate sheets comparing a cloud provider to other cloud providers    
B. Cloud provider offers to provide engineering assistance during the migration    
C. The cost/benefit measure of closing the organization’s relocation site (hot site/warm site) and using the cloud for disaster recovery instead      
D. SLA satisfaction surveys from other (current and past) cloud customers     
Answer: D. 

Of the listed options, knowing how other customers feel about a provider may be the most valuable data point; it is the most realistic depiction of whether an organization realized projected/anticipated benefits after a migration.

Options A and B are just marketing materials and should not, by themselves, be all that convincing for making a migration decision.

Option C is a good factor to consider, but it is only a very small piece of what migration entails; D is still a much better option.

### Question # 110 - A cloud provider will probably require all of the following except ___________________ before a customer conducts a penetration test.    
A. Notice   
B. Description of scope of the test        
C. Physical location of the launch point      
D. Knowledge of time frame/duration     
Answer: C.      

Because cloud access is remote access, pen tests will be remote tests; it doesn’t really matter what the physical origin of the simulated attack is.
All the other options are items the provider will want to know before the customer launches the test.

### Question # 111 - Cloud providers will probably not allow ___________________ as part of a customer’s penetration test.     
A. Network mapping          
B. Vulnerability scanning      
C. Reconnaissance      
D. Social engineering      
Answer: D.      

Performing live deception and trickery against employees of the cloud provider (or its suppliers/vendors) could be construed as unethical and possibly illegal, especially without their knowledge and/or consent. Social engineering probably won’t be involved in penetration tests run by customers.
All the other options are legitimate activities a customer might perform during a penetration test (with provider permission).

### Question # 112 - A cloud customer performing a penetration test without the provider’s permission is risking ___________________.      
A. Malware contamination    
B. Excessive fees for SLA violations    
C. Loss of market share     
D. Prosecution     
Answer: D. 

In most jurisdictions, the activity involved in penetration testing would be considered criminal, and quite serious, and the provider would be justified in seeking law enforcement involvement and prosecution.
None of the other answers make sense with respect to the question.

### Question # 113 - When a customer performs a penetration test in the cloud, why isn’t the test an optimum simulation of attack conditions?     
A. Attackers don’t use remote access for cloud activity.    
B. Advanced notice removes the element of surprise.     
C. When cloud customers use malware, it’s not the same as when attackers use malware.     
D. Regulator involvement changes the attack surface.     
Answer: B. 

Because all penetration tests launched by the customer require notifying the provider beforehand (and getting permission), the simulation loses quite a bit of realism. In the traditional environment, where the organization had full control over its own assets, penetration tests could involve double-blind status, which was much more realistic.
Everyone uses remote access for cloud activity, so option A is incorrect.
Cloud customers will not be able to deploy malware as part of a test because that is a crime, so option C is wrong.
Regulators are not involved in penetration tests, so option D is incorrect.

### Question # 114 - Managed cloud services exist because the service is less expensive for each customer than creating the same services for themselves in a traditional environment. What is the technology that creates most of the cost savings in the cloud environment?    
A. Emulation               
B. Secure remote access      
C. Crypto-shredding      
D. Virtualization      
Answer: D. 

Virtualization allows for the scalability and cost reduction available in managed cloud services.
All the other options are incorrect because they do not cite the technology that creates most of the cost saving in the cloud environment. Only virtualization provides this cost savings.

### Question # 115 - Managed cloud services exist because the service is less expensive for each customer than creating the same services for themselves in a traditional environment. From the customer perspective, most of the cost differential created between the traditional environment and the cloud through virtualization is achieved by removing ___________________.     
A. External risks     
B. Internal risks         
C. Regulatory compliance      
D. Sunk capital investment     
Answer: D. 

In the traditional environment, the cloud customer must pay for a device for every user, which requires additional capacity that is almost never fully used; this represents a cost with no associated benefit. Moving into a virtualized environment allows the organization to only pay for resources that are utilized and not for underutilized or unused capacity.
The risks and regulatory requirements for an organization do not go away when the organization moves into the cloud, so there is no cost savings associated with these elements. Therefore, all of the other options are incorrect.

### Question # 116 - Managed cloud services exist because the service is less expensive for each customer than creating the same services for themselves in a traditional environment. Using a managed service allows the customer to realize significant cost savings through the reduction of ___________________.      
A. Risk    
B. Security controls     
C. Personnel     
D. Data     
Answer: C. 

An organization operating in the cloud should not need as many IT personnel as would be required to operate a traditional enterprise with the same level of services for users; this can represent a significant cost savings.
Moving into the cloud reduces neither risk nor data; options A and D are incorrect.
Arguably, the cloud customer may realize some cost savings through cloud migration because the customer will not be solely responsible for acquiring, deploying, and managing security controls. However, security controls still exist—they are, instead, the responsibility of the cloud provider, and the price of applying them is enclosed in the cost of the cloud service. Moreover, this savings is not nearly as significant as the savings realized through reduction in personnel, so option C is still preferable.
 
### Question # 117 - Which of the following is a risk posed by the use of virtualization?       
A. Internal threats interrupting service through physical accidents (spilling drinks, tripping over cables, etc.)       
B. The ease of transporting stolen virtual machine images      
C. Increased susceptibility of virtual systems to malware       
D. Electromagnetic pulse     
Answer: B. 

Because virtual machine images are stored as imaged files, an attacker able to access the stored files would have a much easier time transporting those files than transporting actual drives/machines.
Option A actually represents a risk in the physical environment that is reduced by the use of virtual machines and is incorrect.
VMs are not any more or less susceptible to malware or EMP, so options C and D are incorrect.

### Question # 118 - The tasks performed by the hypervisor in the virtual environment can be most likened to the tasks of the ___________________ in the traditional environment.      
A. Central processing unit (CPU)     
B. Security team         
C. Operating system (OS)      
D. Pretty Good Privacy (PGP)      
Answer: C. 

Both the hypervisor and the OS orchestrate access to resources (the hypervisor coordinates requests from VMs, and the OS coordinates requests from applications).
Option A is incorrect because the CPU in a traditional environment performs calculations, while the operating system manages resources and performs process scheduling.
The security team in a traditional environment has a narrow and focused role, not like the operating system that manages the entire system and its resources.
Pretty Good Privacy is an application that performs a specific, limited role. Option D is incorrect.

### Question # 119 - Mass storage in the cloud will most likely currently involve ___________________.      
A. Spinning platters     
B. Tape drives     
C. Magnetic disks     
D. Solid-state drives (SSDs)     
Answer: D. 

Solid-state drives (SSDs) are currently the most efficient and durable storage technology, so cloud providers will favor them.
All the other options are older technologies that employ magnetic media in one form or another, while SSD employs electronic circuitry to store data.

### Question # 120 - What is the type of cloud storage arrangement that involves the use of associating metadata with the saved data?     
A. Volume   
B. Block    
C. Object    
D. Redundant     
Answer: C. 

In object storage, data objects/files are saved in the storage space along with relevant metadata such as content type and creation date.
Options A and B are different names for the same type of storage arrangement and incorrect.
Option D has no meaning in this context.

### Question # 121 - According to the NIST Cloud Computing Reference Architecture, which of the following is most likely a cloud carrier?     
A. Amazon Web Services    
B. Netflix    
C. Verizon     
D. Nessus     
Answer: C.     

NIST’s definition of cloud carrier is “an intermediary that provides connectivity and transport of cloud services from Cloud Providers to Cloud Consumers.”
Of the choices, option C best represents this definition.

### Question # 122 - Resolving resource contentions in the cloud will most likely be the job of the ___________________.     
A. Router    
B. Emulator    
C. Regulator     
D. Hypervisor    
Answer: D.     

The hypervisor orchestrates assignment of resources and is responsible for avoiding and resolving contention.
The router manages traffic flow, which might be considered as resolving contention issues for resource requests outside the local device (for example, from a given device to the storage cluster) but wouldn’t handle resource requests inside a given device (such as a VM on the device making a request to the device CPU), so option D is a better answer.
An emulator virtualizes programs, not machines, and is not responsible for orchestrating resource calls, so option B is incorrect.
Regulators do not manage resources, so option C is incorrect.

### Question # 123 - Security controls installed on a guest virtual machine operating system (VM OS) will not function when ___________________.    
A. The user is accessing the VM remotely    
B. The OS is not scanned for vulnerabilities    
C. The OS is not subject to version control     
D. The VM is not active while in storage     
Answer: D.     

Security controls operating on a guest VM OS are only active while the VM is active; when the VM is stored, it is snapshotted and saved as a file, so those controls won’t be active either.
All user access to the VMs will be done remotely; option A is simply incorrect.
Security controls on OSs that are not scanned or subject to version control may be out of date or not optimized, but they will still function (just not as well), so option D is still preferable to B and C.

### Question # 124 - Typically, SSDs are ___________________.    
A. More expensive than spinning platters    
B. Larger than tape backup     
C. Heavier than tape libraries     
D. More subject to malware than legacy drives     
Answer: A. 

Solid-state drives (SSDs) are usually more expensive, per drive, than their counterparts. However, as the industry matures, this is changing rapidly. Moreover, cloud providers are usually buying devices at such a scale and under such a budget that individual price differentials for device types is not the main criteria for making purchase decisions.
Size and shape are not defining criteria of SSDs or tapes; options B and C are irrelevant (and also somewhat wrong).
The physical nature of the drive does not affect its vulnerability to malware; option D is incorrect.

### Question # 125 - Typically, SSDs are ___________________.     
A. Harder to install than magnetic memory     
B. Faster than magnetic drives   
C. Harder to administer than tape libraries     
D. More likely to fail than spinning platters     
Answer: B. 

SSD technology offers a great increase in speed and efficiency.
SSDs are not typically more difficult to install or administer than traditional technology, nor are they more likely to fail than other storage devices, so all the other options are incorrect.

### Question # 126 - Typically, SSDs are ___________________.      
A. Impossible to destroy physically     
B. Not vulnerable to degaussing      
C. Subject to a longer warranty          
D. Protected by international trade laws     
Answer: B. 

Because SSDs do not use magnetic properties to store data, degaussing is not a suitable means of sanitizing SSDs.
All the other options are untrue and are therefore inappropriate answers.

### Question # 127 - Of the following control techniques/solutions, which can be combined to enhance the protections offered by each?     
A. Fences/firewalls     
B. Asset inventories/personnel training      
C. Data dispersion/encryption      
D. Intrusion prevention solutions/intrusion detection solutions      
Answer: C. 

Theoretically, all combinations of security controls are preferable to any one security control used by itself (this is the principle of layered defense). All of the potential responses are therefore true. However, of this list, the pairing that makes the most sense is option C, because encrypting the data while also spreading it across multiple storage devices/locations increases the protection each one offers against certain common threats (in this case, physical theft of a storage device, failure of a device, legal seizure of a device in a multitenant environment, etc.).

### Question # 128 - Of the following control techniques/solutions, which can be combined to enhance the protections offered by each?      
A. Razor tape/background checks     
B. Least privilege/generators     
C. DLP/DRM    
D. Personnel badging/secure baselines      
Answer: C. 

Theoretically, all combinations of security controls are preferable to any one security control used by itself (this is the principle of layered defense). All of the potential responses are therefore true. However, of this list, the pairing that makes the most sense is option C, because adding another layer of access control on objects while also detecting outbound motion of objects increases the protection each one offers against certain common threats (in this case, internal threats, escalation of privilege, unauthorized or inadvertent dissemination of data, etc.).

### Question # 129 - Risk assessment is the responsibility of ___________________.     
A. Companies offering managed cloud services    
B. Regulatory bodies    
C. Every organization    
D. Legislative entities    
Answer: C. 

Every organization is responsible for performing its own risk assessment for its own particular business needs.
Cloud providers will not perform risk assessments on behalf of their customers.
Regulatory bodies and legislative entities do not perform risk assessments.

### Question # 130 - Which entity can best aid the organization in avoiding vendor lock-in?      
A. Senior management       
B. The IT security office     
C. General counsel     
D. The cloud security representative      
Answer: C. 

The best method for avoiding vendor lock-in is to have strong contract language favorable to the customer; the entity best equipped to craft contracts is the office of the general counsel.
Senior management can assist the organization to avoid vendor lock-in by tasking the correct resources (offices/personnel) to perform vendor selection activities, but option A is not as accurate as C.
Security personnel will have the technical skills and knowledge to properly determine the organization’s IT needs and can inform general counsel as to what services/resources will best meet the organization’s needs, but these entities are not as adept and trained at crafting contract language as the attorneys. Options B and D are not preferable to C.

### Question # 131 - Perhaps the best method for avoiding vendor lock-out is also a means for enhancing BC/DR capabilities. This is ___________________.     
A. Having a warm site within 250 miles of the primary production environment         
B. Using one cloud provider for primary production and another for backup purposes     
C. Building a data center above the flood plain    
D. Cross-training all personnel    
Answer: B. 

Using distinct cloud providers for production and backup ensures that the loss of one provider, for any reason, will not result in a total loss of the organization’s data.
None of the other options address vendor lock-out and are therefore unsuitable as answers.

### Question # 132 - ___________________ can often be the result of inadvertent activity.    
A. DDoS   
B. Phishing    
C. Sprawl    
D. Disasters    
Answer: C.     

Users in a cloud environment may not realize the attendant costs that come along with creating many new virtual instances, and the ease with which new instances are created allows users to do so without much effort.
While DDoS and phishing may include an element of user gullibility and ignorance, at least one party (the attacker) is not engaged in inadvertent activity—their behavior is very purposeful. Options A and B are incorrect.
While inadvertent action can often result in incidents, disasters are usually at a much greater scale and aren’t as likely to be the result of unknowing action; option D is incorrect.

### Question # 133 - Of the following, which is probably the most significant risk in a managed cloud environment?    
A. DDoS    
B. Management plane breach     
C. Guest escape    
D. Physical attack on the utility service lines     
Answer: B.    

Management plane breach allows an attacker to gain full control of the environment and can affect all aspects of the CIA triad.
DDoS and physically attacking the utility lines, options A and D, only affect availability, which is a significant negative impact but not as bad as option B, which can affect integrity and confidentiality as well.
Guest escape is a breach limited to a specific device and the virtual machines on that device; this is not as much impact as breaching the management plane, which gives full access to the entire environment.

### Question # 134 - What is the optimal number of entrances to the cloud data center campus?     
A. One     
B. Two     
C. Three      
D. Four     
Answer: A.     

Controlling access is optimized by minimizing access.
All the other options are incorrect.

### Question # 135 - The cloud data center campus physical access point should include all of the following except ___________________.    
A. Reception area      
B. Video surveillance      
C. Badging procedure      
D. Mantrap structures     
Answer: D. 

Usually, mantrap areas control access to sensitive locations within a facility, not an entrance to the facility.
None of the other options address vendor lock-out and are therefore unsuitable as answers.

### Question # 136 - Where should multiple egress points be included?     
A. At the power distribution substation   
B. Within the data center            
C. In every building on the campus      
D. In the security operations center    
Answer: C. 

Health and human safety is a paramount goal of security; all facilities must have multiple emergency egress points.
All the other options are distractors as they are included in option C.

### Question # 137 - Which of the following is a risk in the cloud environment that does not exist or is not as prevalent in the traditional environment?     
A. DDoS   
B. Isolation failure    
C. External attack    
D. Internal attack    
Answer: B.    

In the traditional environment, when all resources are owned, controlled, and used by the organization’s personnel, loss of isolation will only expose data to other members of the organization; isolation failure in the cloud environment may expose data to people outside the organization, a more significant impact.
All the other options are risks that have similar likelihoods and impacts in the cloud and traditional environments and are therefore incorrect.

### Question # 138 - All security controls necessarily ___________________.      
A. Are expensive    
B. Degrade performance      
 C. Require senior management approval      
D. Will work in the cloud environment as well as they worked in the traditional environment        
Answer: B. 

Security and productivity/operations are always trade-offs.
Option A is a generalization that may or may not be true depending on several variables. Some security controls are inexpensive to implement.
Senior management approval may be required before security controls can be implemented, however, some may not need prior approval. It depends on the organization and how it is managed. Option C is incorrect.
Option D is another generalization that may or may not be true. Whether a security control will work in the cloud environment as well as they worked in the traditional environment depends on the control and how it is implemented. Option B is a better choice.

### Question # 139 - Which of the following is a risk in the cloud environment that does not exist or is not as prevalent in the traditional environment?     
A. Legal liability in multiple jurisdictions    
B. Loss of productivity due to DDoS     
C. Ability of users to gain access to their physical workplace       
D. Fire      
Answer: A. 

Because cloud providers may use data centers that span state (or even national) borders, new legal risks may be introduced to the customer’s organization after cloud migration.
All the other options are risks faced by organizations in both the cloud and traditional environments and are therefore incorrect.

### Question # 140 - Which of the following is a risk in the cloud environment that does not exist or is not as prevalent in the traditional environment?     
A. Loss of availability due to DDoS     
B. Loss of value due to DDoS           
C. Loss of confidentiality due to DDoS       
D. Loss of liability due to DDoS    
Answer: A. 

In the traditional environment, if DDoS prevented the organization’s connectivity with the Internet or other organizations, users still had access to their own data but simply could not share it or use it in external transactions; this hampered productivity, but not availability. In the cloud, without connectivity outside the organization, users cannot reach their data, which is an availability issue.
DDoS does not affect value, confidentiality, or liability; all the other options are incorrect.

### Question # 141 - DDoS attacks do not affect ___________________ for cloud customers.      
A. Productivity     
B. Availability     
C. Connectivity     
D. Integrity     
Answer: D.     

DDoS prevents all these things except for data integrity. DDoS only prevents communication; it does not usually result in modified data.

### Question # 142 - Sprawl in the cloud can lead to significant additional costs to the organization because of ___________________.        
A. Larger necessary physical footprint    
B. Much larger utility consumption     
C. Software licensing     
D. Requisite additional training     
Answer: C.     

In some instances, more virtualized machines will entail a relative increase in the number of software seat licenses, which can be a significant expense.
Typically, cloud customers do not pay extra for additional consumption of floor space or power usage for the number of virtual machines; these costs are rolled into the per-instance price, so options A and B are incorrect.
Option D is incorrect; users don’t require more training if they have more virtual assets.

### Question # 143 -  It is best to use variables in ___________________.          
A. Baseline configurations            
B. Security control implementations        
C. Contract language       
D. BC/DR tests       
Answer: D.      

When performing BC/DR tests, it is useful to create scenarios that are unpredictable and vary from previous tests so as to better approximate conditions of an actual disaster.
All the other answers represent elements that should avoid variables as much as possible and are incorrect.
