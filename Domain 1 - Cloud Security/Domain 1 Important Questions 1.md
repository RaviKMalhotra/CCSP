# Chapter 1: Domain 1—Cloud Concepts, Architecture, and Design

Domain 1 of the Certified Cloud Security Professional (CCSP) Exam Outline is an introductory section that touches on almost every other element of the exam outline so you’ll find a wide breadth of content and subject matter ranging over many topics. The questions in this chapter will reflect that broad scope but will also get into some level of detail on certain aspects you’ll find pertinent to the exam.

### Question # 1 - Alice is the CEO for a software company; she is considering migrating the operation from the current traditional on-premises environment into the cloud. Which cloud service model should she most likely consider for her company’s purposes?   
A. Platform as a service (PaaS)  
B. Software as a service (SaaS)  
C. Backup as a service (Baas)  
D. Infrastructure as a service (IaaS)   
Answer: A. 

PaaS will allow her developers to create and design their software on a variety of operating systems (OSs), increasing the breadth of the market she can sell to. Also, she can use geographically dispersed programmers to work on projects concurrently, and the provider will be responsible for maintaining and updating the OSs as necessary. 

IaaS is a less attractive option because it would retain the need for Alice’s company to administer the OSs in addition to building their software; it might be less expensive in terms of paying the cloud provider, but the time and effort and personnel necessary to maintain the OSs would offset that cost, probably in a net-negative way. SaaS is not an option; Alice wants her company to build software, not rent it or buy it. Backup as a Service (BaaS) would not be useful for creating, designing, or deploying Alice’s company’s software.

### Question # 2 - Alice is the CEO for a software company; she is considering migrating the operation from the current traditional on-premises environment into the cloud. Which aspect of cloud computing should she be most concerned about, in terms of security issues?    
A. Multitenancy   
B. Metered service    
C. Service-level agreement (SLA)    
D. Remote access    
Answer: A. 

Of these four options, multitenancy poses the greatest risk to software developers in the cloud, because developers need to be concerned with two things: protecting their intellectual property (the software they’re making) and protecting resource calls their software makes to the underlying infrastructure (which, if detectable by other cloud customers, could provide information that constitutes a side-channel attack). Metered service doesn’t pose much of a security risk. 

The SLA might include some security aspects (such as response time), but it’s usually more of a performance-ensuring tool, and this choice is not as good as option A. Remote access, in this particular case, provides more benefit than risk: Alice can utilize work from developers located across the country or across the planet. 

While she does have to consider the risks inherent in all remote access, those risks are not as significant as the risks due to multitenancy, so option A is still preferable.

### Question # 3 - Alice is the CEO for a software company; she is considering migrating the operation from the current traditional on-premises environment into the cloud. In order to protect her company’s intellectual property, Alice might want to consider implementing all these techniques/solutions except ____________.    
A. Egress monitoring    
B. Encryption    
C. Turnstiles     
D. Digital watermarking     
Answer: C.    

Turnstiles are a physical security barrier to prevent piggybacking/tailgating (an unauthorized person coming through an entrance behind someone who is authorized), but they don’t really present much protection for intellectual property in this case. Egress monitoring (often referred to as “DLP” solutions) is a great way to reduce the likelihood of intellectual property leaving the owner’s control in an unexpected/unapproved manner. Likewise, strong encryption is useful in the cloud to reduce the impact of theft either from leakage to other cloud tenants or from insider threats (such as malicious admins in the employ of the cloud provider). 

Finally, digital watermarks aid protection of intellectual property by proving original ownership, which is essential for enforcing intellectual property rights (in the case of software design, mainly copyright protections).

### Question # 4 - Alice is the CEO for a software company; she is considering migrating the operation from the current traditional on-premises environment into the cloud. What is probably the biggest factor in her decision?    
A. Network scalability    
B. Off-site backup capability    
C. Global accessibility    
D. Reduced overall cost due to outsourcing administration     
Answer: D.     

While all of these are traits of cloud computing and will likely benefit Alice’s company, from her position as senior manager of the organization she is likely to consider the financial benefit first and foremost.

### Question # 5 - In which of the following situations does the data owner have to administer the OS?    
A. IaaS    
B. PaaS    
C. Off-site archive     
D. SaaS    
Answer: A.     

With infrastructure as a service (IaaS), the customer (data owner) will administer the OS and applications. In PaaS, the provider will manage the underlying hardware and the OS. In an on-premises enterprise, the data owner is also the system owner and will be responsible for everything. 

In an SaaS environment, the cloud provider will handle all aspects of processing, except for adding and manipulating the production data.

### Question # 6 - You are setting up a cloud implementation for an online retailer who will accept credit card payments. According to the Payment Card Industry Data Security Standard (PCI DSS), what can you never store for any length of time?     
A. Personal data of consumers    
B. The credit card verification (CCV) number     
C. The credit card number    
D. Home address of the customer     
Answer: B.     

PCI DSS requires that the CCV (or, sometimes, “CVV” for “card verification value”) only be used in the transaction, not stored. The data described in all the other options may be stored after the transaction is complete.

### Question # 7 - The Payment Card Industry Data Security Standard (PCI DSS) distinguishes merchants by different tiers, based on ____________.    
A. Number of transactions per year   
B. Dollar value of transactions per year    
C. Geographic location     
D. Jurisdiction     
Answer: A.      

The four merchant levels in PCI are distinguished by the number of transactions that merchant conducts in a year. The dollar value of transactions per year, geographic location, and jurisdiction are not attributes that are evaluated for PCI DSS tier levels.

### Question # 8 - What is usually considered the difference between business continuity (BC) efforts and disaster recovery (DR) efforts?    
A. BC involves a recovery time objective (RTO), and DR involves a recovery point objective (RPO).    
B. BC is for events caused by humans (like arson or theft), whereas DR is for natural disasters.     
C. BC is about maintaining critical functions during a disruption of normal operations, and DR is about recovering to normal operations after a disruption.    
D. BC involves protecting human assets (personnel, staff, users), whereas DR is about protecting property (assets, data).    
Answer: C .       

Technically, BC efforts are meant to ensure that critical business functions can continue during a disruptive event, and DR efforts are supposed to support the return to normal operations. However, in practice, the efforts often coincide, use the same plans/personnel, and have many of the same procedures.
Option A is incorrect; both BC and DR use the RTO and RPO as metrics to determine success.
Option B is incorrect; BC and DR efforts are not specific to the cause of a disruptive event.
Option D is incorrect; health and human safety should be paramount in all security efforts, with very few exceptions.

### Question # 9 - For business continuity and disaster recovery (BC/DR) purposes, the contract between the primary cloud provider and customer should include all of the following except _______________.    
A. Which party will be responsible for initiating a BC/DR response activity.      
B. How a BC/DR response will be initiated.    
C. How soon the customer’s data can be ported to a new cloud provider in the event a disruptive event makes the current provider unable to continue service.    
D. How much a new cloud provider will charge the customer if data has to be ported from the current cloud provider because of a disruptive event      
Answer: D. 

The contract between the cloud customer and current cloud provider has no bearing on what the customer will have to pay to a new provider; that will be governed by the contract between the customer and the new provider.
All the other options are topics that should be addressed in the contract between the current cloud provider and the cloud customer in order to properly address BCDR needs.

### Question # 10 - When the cloud customer requests modifications to the current contract or service-level agreement (SLA) for business continuity/disaster recovery (BD/DR) purposes, who should absorb the cost of modification?     
A. The customer absorbs the cost.    
B. The provider absorbs the cost.    
C. The cost should be split equally.      
D. Modifications don’t cost anything.      
Answer: A.     

The customer will have to pay for the costs of modification requested by the customer, regardless of purpose.
All the other options are simply incorrect, especially option D, which is never true.

### Question # 11 - Which of the following is not a factor an organization might use in the cost–benefit analysis when deciding whether to migrate to a cloud environment?      
A. Pooled resources in the cloud     
B. Shifting from IT investment as capital expenditures to operational expenditures     
C. The time savings and efficiencies offered by the cloud service    
D. Branding associated with which cloud provider might be selected    
Answer:D.    

The brand associated with the cloud provider should not influence the cost–benefit analysis; the cloud provider’s brand (and even which cloud provider an organization uses) will most likely not even be known to the consumers who have a business relationship with the organization.
The provider does not absorb the cost when the customer’s requests a modification of the SLA. Though an even split of the cost between customer and provider may seem fair, the customer pays for all costs associated with modifications to the SLA by the customer. Finally, customer modifications to their SLA are chargeable expenses that will almost certainly be paid for by the customer.

### Question # 12 - Which of the following is the least important factor an organization might use in the cost–benefit analysis when deciding whether to migrate to a cloud environment?      
A. Depreciation of IT assets    
B. Shift in focus from IT dependencies to business process opportunities      
C. Whether the provider bills on a monthly or weekly basis    
D. Costs associated with utility consumption    
Answer: C.    

The timing of recurring payments to the provider will probably not be a significant factor in the cost–benefit analysis.
All the other options are topics that are more important to review when an organization is considering cloud migration.

### Question # 13 - Which of the following is an aspect of IT costs that will likely be reduced by moving from a traditional, on-premises IT environment into the cloud?    
A. Number of users     
B. Cost of software licensing     
C. Number of applications     
D. Number of clientele    
Answer: B.     

In a traditional environment, enterprise software costs can be exorbitant, and the price of licensing doesn’t even reflect the hidden costs associated with licensing, such as managing the license library. In a cloud arrangement, especially software as a service (SaaS), the customer pays only the contract fee to the cloud provider, and it is the provider’s responsibility to arrange for software licensing and to manage those licenses.
Option A is incorrect because the number of users should not be affected whether the organization is operating in the cloud or a legacy environment. The exception would be the reduced number of privileged users, because the cloud provider will be handling more administrative tasks in the environment; however, because “privileged” was not specified, option B is still a better answer.

Option C is incorrect because that may or may not be true of an organization’s migration to the cloud.

Option D is incorrect because the organization certainly hopes it is not going to lose clientele by moving to the cloud!

### Question # 14 - Which of the following is an aspect of IT costs that will likely be reduced by moving from a traditional, on-premises IT environment to the cloud?     
A. Utilities costs     
B. Security costs     
C. Landscaping costs    
D. Travel costs    
Answer: A. 

Cloud providers are purchasing utilities (power, water, Internet connectivity) at such a massive rate that they can realize per-unit cost savings that would far exceed any smaller organizations’ pricing for individual data centers. In this case, economies of scale are very much in favor of the larger entity.
Option B may or may not be true, depending on the degree of sensitivity and value of the organization’s data and what controls the organization will request/contract for in the cloud.

Options C and D are not influenced by cloud migration in any way and are wholly dependent on other factors within the organization.

### Question # 15 - Which of the following is an aspect of IT costs that will likely be reduced by moving from a traditional, on-premises IT environment to the cloud?     
A. Personnel training    
B. Personnel turnover    
C. Capital expenses for IT assets    
D. Loss due to an internal data breach   
Answer: C.    

Constant reinvestment in IT assets (which are almost always obsolete by the time they’re marketed, much less by the time they’re deployed in operational environments) is plagued with sunk costs; money spent on hardware devices or software licenses is unlikely to be recovered. Avoiding expenditures for IT systems by moving to the cloud means reducing these costs considerably.

Option A is incorrect; cloud migration should not affect the need for personnel training; employees will just need to be trained in a different manner.

Options B and D should not be affected by cloud migration in any way; whether your organization has a high personnel turnover rate or risk from internal threat is not based on whether the IT environment is owned or leased.

### Question # 16 - Although cloud migration might offer significant cost savings for an organization, which of the following factors might reduce the actual financial benefit the organization realizes in a cloud environment?    
A. Altitude of the cloud data center   
B. Security controls and countermeasures   
C. Loss of ownership of IT assets   
D. Costs of Internet connectivity for remote users   
Answer: B.   

Every security process, tool, and behavior entails a related cost, both financially and operationally. Although a “base price” cloud service might appear extremely affordable compared to the traditional environment, add-ons such as encryption, digital rights management (DRM), security incident/event management (SIM/SEM/SIEM), and intrusion detection/prevention systems (IDS/IPS) may all come with additional cost and may degrade performance, thus reducing the cost savings compared to the cost of operations prior to migration. This is extremely important for the organization to consider before migration, especially if the organization exists in a highly regulated industry.

Option A is incorrect because the altitude of the cloud data center does not translate into a reduction of the actual financial benefit the organization would realize in moving to the cloud environment.

Option C is wrong because it should be the opposite of the actual case: losing ownership of the IT assets, and paying only for the use of those assets, should lead directly to a savings over the costs of a traditional IT environment, if compared on a seat-to-seat basis.

Option D should not be true; the cost of connecting users to the Internet should not be significantly greater if the organization operates in the cloud or with an on-premises data center—if the cost is considerably greater, the organization should never have migrated in the first place.

### Question # 17 - What is the international standard that dictates creation of an organizational information security management system (ISMS)?    
A. NIST SP 800-53   
B. PCI DSS   
C. ISO 27001   
D. NIST SP 800-37    
Answer: C. 

ISO 27001 mandates an ISMS; organizations can be certified according to compliance with 27001.
National Institute of Standards and Technology (NIST) SP 800-53 is the list of security controls approved for use by U.S. government agencies and a means to map them to the Risk Management Framework.
The Payment Card Industry Data Security Standard (PCI DSS) is the payment card industry’s framework of compliance for all entities accepting or processing credit card payments.

NIST SP 800-37 is the Risk Management Framework.

### Question # 18 - ISO 27001 favors which type of technology?   
A. Open source    
B. PC    
C. Cloud-based    
D. None   
Answer: D. 

The ISO 27001 standard is designed to be product agnostic. The other answers suggest ISO 27001 favors a type of technology, and are therefore incorrect.

### Question # 19 - Why might an organization choose to comply with the ISO 27001 standard?     
A. Price    
B. Ease of implementation    
C. International acceptance    
D. Speed    
Answer: C. 

The ISO standards are almost universally accepted and recognized, and they’re even mandated for certain industries/locales.
They are not, however, cheap, fast, or easy to adopt, implement, and audit against, so all the other answers are incorrect.

### Question # 20 - Why might an organization choose to comply with NIST SP 800-series standards?    
A. Price     
B. Ease of implementation     
C. International acceptance    
D. Speed    
Answer: A. 

The NIST standards are not particularly easy or fast to implement (in fact, they require continual improvement), and they are not widely recognized or mandated outside of the U.S. government federal sector.
However, they are in the public domain, so an organization would not have to pay for the standards material if the organization chose to use NIST standards.

### Question # 21 - Which standard contains guidance for selecting, implementing, and managing information security controls mapped to an information security management system (ISMS) framework?    
A. ISO 27002     
B. Payment Card Industry Data Security Standard (PCI DSS)     
C. NIST SP 800-37   
D. Health Insurance Portability and Accountability Act (HIPAA)    
Answer: A.    

ISO 27002 is used for choosing security controls in order to comply with the ISMS, which is contained in ISO 27001.
PCI DSS is the payment card industry’s framework of compliance for all entities accepting or processing credit card payments.
NIST SP 800-37 is the Risk Management Framework.
HIPAA is the U.S. law regarding patient data privacy in the medical sector.

### Question # 22 - The current American Institute of Certified Public Accountants (AICPA) publishes the _______________ standard, from which the Service Organization Control (SOC) reports are derived.     
A. Sherwood Applied Business Security Architecture (SABSA)      
B. Statement on Standards for Attestation Engagements (SSAE) 18    
C. Biba   
D. NIST SP 800-53    
Answer: B. 

SSAE 18 is the current AICPA audit standard, as of 2018.
All the other options are distractors: SABSA is an IT architecture framework, Biba is an access control model, and NIST SP 800-53 contains guidance for selecting security controls in accordance with the Risk Management Framework.

### Question # 23 - Which U.S. federal law affects banking and insurance companies?     
A. NIST 800-53   
B. HIPAA    
C. Sarbanes-Oxley Act (SOX)    
D. Gramm-Leach-Bliley Act (GLBA)    
Answer: D. 

GLBA is a U.S. federal law pertaining to financial and insurance customer information.
NIST 800-53 is a standard, not a law, so option A is incorrect.
Health Insurance Portability and Accountability Act (HIPAA) is a U.S. federal law concerning medical information, so option B is incorrect.
SOX affects publicly traded corporations, making option C incorrect.

### Question # 24 - The Statement on Standards for Attestation Engagements 18 (SSAE 18) Service Organization Control (SOC) reports are audit tools promulgated by the American Institute of Certified Public Accountants (AICPA). What kind of entities were SOC reports designed to audit?     
A. U.S. federal government    
B. Privately held companies    
C. Companies that provide services    
D. Nonprofit organizations    
Answer: C.   

The SSAE 18 is an audit standard, and the SOC reports were specifically designed to report on the suitability of organizations that provide services. This is not to say that SOC reports are not used to assess other types of organizations—they are, but they were not designed for that purpose, so all the other answers are incorrect.

### Question # 25 - The Statement on Standards for Attestation Engagements (SSAE) 18 Service Organization Control (SOC) reports are audit tools promulgated by the American Institute of Certified Public Accountants (AICPA). As an IT security professional, when reviewing SOC reports for a cloud provider, which report would you most like to see?    
A. SOC 1   
B. SOC 2, Type 1   
C. SOC 2, Type 2    
D. SOC 3   
Answer: C.    

The SOC 2, Type 2 report will provide details on IT security controls used by the target and how well those controls function.

The SOC 1 report provides information about financial reporting mechanisms of the target only and is of little interest to the IT security professional, so option A is incorrect.

The SOC 2, Type 1 report describes IT security controls designed by the target only but not how effectively those controls function, so option B is incorrect.

The SOC 3 report is only an attestation that the target was audited and that it passed the audit, without detail, so option D is incorrect.

### Question # 26 - The Statement on Standards for Attestation Engagements (SSAE) 18 Service Organization Control (SOC) reports are audit tools promulgated by the American Institute of Certified Public Accountants (AICPA). As an investor, when reviewing SOC reports for a cloud provider, which report would you most like to see?    
A. SOC 1    
B. SOC 2, Type 1    
C. SOC 2, Type 2   
D. SOC 3    
Answer: A. 

The SOC 1 report provides information about financial reporting mechanisms of the target only. Although this information may be of little use to the IT security professional, it may be of great use to potential investors, if for nothing other than providing some assurance that reporting is valid and believable.
The SOC 2, Type 1 report describes IT security controls designed by the target only but not how effectively those controls function. While of some interest to the IT security professional, this is of little interest to the investor, so option B is incorrect.
The SOC 2, Type 2 report will provide details on IT security controls used by the target and how well those controls function. While of great interest to the IT security professional, this is of little interest to the investor, so option C is incorrect.
The SOC 3 report is only an attestation that the target was audited and that it passed the audit, without detail, so option D is incorrect.

### Question # 27 - The Statement on Standards for Attestation Engagements (SSAE) 18 Service Organization Control (SOC) reports are audit tools promulgated by the American Institute of Certified Public Accountants (AICPA). You are an IT security professional working for an organization that is considering migrating from your on-premises environment into the cloud. Assuming some have passed SSAE 18 audits and some haven’t, which SOC report might be best to use for your initial review of several different cloud providers in order to narrow down the field of potential services in a fast, easy way?     
A. SOC 1   
B. SOC 2, Type 1   
C. SOC 2, Type 2   
D. SOC 3    
Answer: D.   

The SOC 3 report is an attestation that the target was audited and that it passed the audit, without detail; you could use the SOC 3 reports to quickly narrow down the list of possible providers by eliminating the ones without SOC 3s.

The SOC 1 report provides information about financial reporting mechanisms of the target only. This information may be of little use to the IT security professional and won’t help you choose a cloud vendor, so option A is incorrect.

The SOC 2, Type 1 report describes IT security controls designed by the target only but not how effectively those controls function. While of some interest to the IT security professional, it is more comprehensive and detailed than a SOC 3 report, so it would take more time; option B is incorrect.

The SOC 2, Type 2 report will provide details on IT security controls used by the target and how well those controls function. While of great interest to the IT security professional, it is very detailed and comprehensive and wouldn’t be a speedy tool to narrow the field. Option C is incorrect.

### Question # 28 - Which of the following entities would not be covered by the Payment Card Industry Data Security Standard (PCI DSS)?      
A. A bank issuing credit cards    
B. A retailer accepting credit cards as payment    
C. A business that processes credit card payments on behalf of a retailer    
D. A company that offers credit card debt repayment counseling    
Answer: D.     

PCI DSS applies only to those entities that want to engage in the business of taking or processing credit card payments, which would include options A, B, and C. 

A counseling service is not engaged in commerce involving credit cards and therefore is under no obligation to adhere to the PCI DSS.

### Question # 29 - What sort of legal enforcement may the Payment Card Industry (PCI) Security Standards Council not bring to bear against organizations that fail to comply with the Payment Card Industry Data Security Standard (PCI DSS)?     
A. Fines    
B. Jail time    
C. Suspension of credit card processing privileges     
D. Subject to increased audit frequency and scope    
Answer: B.   

Because PCI DSS is strictly voluntary, and the PCI Council is not a government body but a consortium of private interests, they cannot detain or imprison anyone.

They can, however, assess fees, suspend processing privileges, and require more auditing, so the other answers are true and therefore incorrect.

### Question # 30 - The Payment Card Industry Data Security Standard (PCI DSS) merchant levels are based on _______________.    
A. Dollar value of transactions over the course of a year    
B. Number of transactions over the course of a year   
C. Location of the merchant or processor    
D. Dollar value and number of transactions over the course of a year    
Answer: B.     

The PCI merchant levels are based on how many transactions a compliant entity engages in over the course of a year.
All the other options are incorrect because the dollar value of transactions and location of the merchant or processor are not the criteria used for determining PCI DSS merchant levels. Only the transactions a compliant entity engages in over the course of a year is the correct answer.

### Question # 31 - In terms of greatest stringency and requirements for security validation, which is the highest merchant level in the Payment Card Industry (PCI) standard?    
A. 1    
B. 2    
C. 3    
D. 4   
Answer: A.   

Merchant level 1 is for the merchants that engage in the most transactions per year (six million or more). It carries with it the requirement for the most comprehensive, detailed, and repeated security validation actions.

It may be tempting to choose the highest number when choosing an answer for the highest merchant level. It may be counterintuitive to think that level 1 would be a higher level than a level 4. However, level 1 is the highest merchant level and is the correct answer to this question.

### Question # 32 - The Payment Card Industry Data Security Standard (PCI DSS) requires _______________ security requirements for entities involved in credit card payments and processing.     
A. Technical    
B. Nontechnical    
C. Technical and nontechnical    
D. Neither technical nor nontechnical    
Answer: C.    

The Payment Card Industry Data Security Standard (PCI DSS) requires multiple kinds of technical and nontechnical security requirements (including specific control types) for those entities that choose to subscribe to the standard.

Option A is partially correct and partially incorrect. While the security requirements are partially technical, some requirements are also nontechnical. Therefore, option A is incorrect.

Option B is also partially correct and partially incorrect. While the security requirements are partially nontechnical, some requirements are technical. Therefore, option B is incorrect.

Option C is incorrect because the requirements are technical and nontechnical, not neither technical nor nontechnical.

### Question # 33 - According to the Payment Card Industry Data Security Standard (PCI DSS), if a merchant is going to store credit cardholder information for any length of time, what type of security protection must be used?     
A. Tokenization or masking     
B. Obfuscation or tokenization    
C. Masking or obfuscation    
D. Tokenization or encryption     
Answer: D. 

The Payment Card Industry Data Security Standard (PCI DSS) allows for cardholder information at rest to be secured with either tokenization or encryption, but use of one is mandatory.

The other options are distractors and not dictated by PCI DSS. They can, however, be useful in fulfilling certain credit card support services, such as customer support, where the personnel engaged in the activity (customer support agents, for instance) may need access to a limited set of the cardholder’s account information (for instance, name, mailing address, and date of the payment) but do not have a need to know other elements of that data set (particularly, the full credit card number); masking and obfuscation can satisfy that business need without putting data unduly at risk.

### Question # 34 - What element of credit cardholder information may never be stored for any length of time, according to the Payment Card Industry Data Security Standard (PCI DSS)?    
A. The full credit card number    
B. The card verification value (CVV)     
C. The cardholder’s mailing address    
D. The cardholder’s full name    
Answer: B.     

The Payment Card Industry Data Security Standard (PCI DSS) disallows the storage of the CVV for any length of time; the CVV may only be used during the payment transaction, and not saved.
The other options may be stored for future transactions with the same merchant. However, unlike the CVV they may be stored by the merchant.

### Question # 35 - When reviewing IT security products that have been subjected to Common Criteria certification, what does the Evaluation Assurance Level (EAL) tell you?     
A. How secure the product is from an external attack    
B. How thoroughly the product has been tested    
C. The level of security the product delivers to an environment    
D. The level of trustworthiness you can have if you deploy the product    
Answer: B.    

The EAL is a measure of how thoroughly the security features the product vendor claims the product offers have been tested and reviewed, and by whom.
The EAL does not offer any true measure of how well those security features will work in a production environment so options A and C are incorrect. Whether those features are preferable to other features offered by competing products, or whether the product is “good.” Therefore, option D is incorrect.

### Question # 36 - Which Common Criteria Evaluation Assurance Level (EAL) is granted to those products that are functionally tested by their manufacturer/vendor?    
A. 1    
B. 3   
C. 5  
D. 7   
Answer: A.   

EAL 1 is for functionally tested products. Option B is incorrect because EAL 3 is for solutions that have been methodically tested and checked.

Option C, EAL 5 is incorrect because that is for solutions that have been semi-formally designed and tested.

Option D is incorrect because EAL 7 is for solutions that have been formally verified design and tested.

### Question # 37 - Which Common Criteria Evaluation Assurance Level (EAL) is granted to those products that are formally verified in terms of design and tested by an independent third party?     
A. 1    
B. 3    
C. 5   
D. 7   
Answer: D.    

EAL 7 is for those products that have undergone independent third-party testing and verification of security feature design. All other options are distractors and incorrect.

EAL 1 is for functionally tested products.

EAL 3 is for solutions that have been methodically tested and checked.

EAL 5 is for solutions that have been semi-formally designed and tested.

### Question # 38 - Who pays for the Common Criteria certification of an IT product?    
A. National Institute of Standards and Technology (NIST)     
B. The vendor/manufacturer    
C. The cloud customer    
D. The end user   
Answer: B.   

The vendor/manufacturer of a given product will pay to have it certified, with the premise that certification costs are offset by premium prices that certified products command and that customers won’t purchase uncertified products.
NIST does not certify products for Common Criteria. NIST is a U.S. government organization.

Option C is incorrect because the cloud customer does not pay to have IT products certified.

Option D is incorrect because the end user is an individual and individuals do not pay to have IT products certified.
(Note: Of course, the manufacturer/vendor is going to amortize the cost of the certification process across the price of the products they sell, so the customers who purchase the product will eventually “pay” for the certification, but that’s a very oblique and abstract way of reading the question.)

### Question # 39 - Who publishes the list of cryptographic modules validated according to the Federal Information Processing Standard (FIPS) 140-2?   
A. The U.S. Office of Management and Budget (OMB)    
B. The International Standards Organization (ISO)   
C. International Information System Security Certification Consortium, or (ISC)2   
D. The National Institute of Standards and Technology (NIST)   
Answer: D.    

NIST publishes the list of validated crypto modules. The other choices are government or non-government organizations that are not involved with publishing the list of cryptographic modules that meet FIPS 140-2 requirements.

### Question # 40 - Who performs the review process for hardware security modules (HSMs) in accordance with the Federal Information Processing Standard (FIPS) 140-2?    
A. The National Institute of Standards and Technology (NIST)    
B. The National Security Agency (NSA)   
C. Independent (private) laboratories   
D. The European Union Agency for Network and Information Security (ENISA)  
Answer: C.     

Vendors seeking HSM certification under FIPS 140-2 send their products to independent laboratories that have been validated as Cryptographic Module Testing Laboratories under the National Voluntary Laboratory Accreditation Program (the Accreditation Program is run by NIST, which approves the laboratories). As of this writing, 21 labs in the United States and Canada are accredited.

Option A is incorrect because NIST does not perform the review process. NIST approves the independent laboratories that perform the review process.

Option B is incorrect. Of all the activities that the NSA does perform, reviewing the process for Hardware Security Modules in accordance with FIPS 140-2 is certainly not one of them.

Option D is incorrect because the ENISA is a European Union organization that supports European Union institutions and stakeholders.

### Question # 41 - In terms of the number of security functions offered, which is the highest Federal Information Processing Standard (FIPS) 140-2 security level a cryptographic module can achieve in certification?    
A. 1  
B. 2  
C. 3  
D. 4  
Answer: D.   

The highest security level a product can reach is 4. Option A is incorrect because Level 1 is the lowest level of security. Option B is incorrect because Level 2 simply improves upon the physical security of Level 2. Option C is incorrect because Level 3 improves upon Level 2 certification and adds tamper-detection/response capabilities.

### Question # 42 - What distinguishes the Federal Information Processing Standard (FIPS) 140-2 security levels for cryptographic modules?    
A. The level of sensitivity of data they can be used to protect   
B. The amount of physical protection provided by the product, in terms of tamper resistance   
C. The size of the IT environment the product can be used to protect  
D. The geographic locations in which the product is allowed   
Answer: B. 

The security levels acknowledge different levels of physical protection offered by a crypto module, with 1 offering crypto functionality and no real physical protection and 4 offering tamper-resistant physical features and automatic zeroization of security parameters upon detection of tamper attempts.
The question asks what distinguishes the security levels for cryptographic modules. Option A focuses on the sensitivity of the data being protected. The sensitivity of the data that is being protected is important when it comes to the cryptographic module being used, but that is not the distinction between the security levels in FIPS 140-2.

Option C is incorrect because the size of the IT environment the cryptographic module is protecting is not what distinguishes the different levels.

Option D is not correct because whether the cryptographic module is or is not allowed in a certain geographic location has no bearing on whether or not it works. The cryptographic module either works or it does not, regardless of its location.

### Question # 43 - For U.S. government agencies, what level of data sensitivity/classification may be processed by cryptographic modules certified according to the Federal Information Processing Standard (FIPS) 140-2 criteria?     
A. Sensitive but unclassified (SBU)    
B. Secret   
C. Top Secret   
D. Sensitive Compartmentalized Information (SCI)    
Answer: A. 

FIPS 140-2 is only for SBU data. Options B, C, and D are incorrect because FIPS 140-2 certifies cryptographic modules for unclassified data. Secret, Top Secret, and Sensitive Compartmentalized Information all are categorized as classified information when it refers to their sensitivity level.

### Question # 44 - Who pays for cryptographic modules to be certified in accordance with Federal Information Processing Standard (FIPS) 140-2 criteria?    
A. The U.S. government    
B. Module vendors     
C. Certification laboratories     
D. Module users   
Answer: B. 

Vendors who want their products certified under FIPS 140-2 must pay the laboratory that performs the evaluation.

Option A is incorrect because the U.S. government is not in the business of paying for cryptographic module certifications. The U.S. government can require the use of cryptographic modules in certain situations.
Certification laboratories receive funds for certifying cryptographic modules. They do not pay to have them certified. Therefore, option C is incorrect.

Option D is incorrect. Users do not pay to have solutions certified.

### Question # 45 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. What is probably the single most important way of countering the highest number of items on the OWASP Top Ten (regardless of year)?     
A. Social engineering training   
B. Disciplined coding practices and processes   
C. White-box source code testing    
D. Physical controls at all locations at which the application is eventually used    
Answer: B.     

Most of the items on the Top Ten could be addressed with strong coding practices and by adhering to strict internal management processes (on the part of the organization involved in development). A good number of the items that continually appear on the list, such as injection, cross-site scripting, insecure direct object references, security misconfiguration, missing function-level access control, use of components with known vulnerabilities, and unvalidated redirects and forwards, can all be addressed by basic development practices, such as bounds checking/input validation, code validation/verification protocols, and informed oversight of the project.

Strangely, option A is not correct in this case. Social engineering is perhaps the aspect of information security that is least understood (by users) and easiest to exploit, and it is the attack tactic most likely to succeed. Social engineering training could probably reduce the greatest number of overall security threats in our field today. However, this specific question is all about application security, and the element of social engineering is negligible.

Option C is not correct because source code testing is only one aspect of code review and would not address as many items on the Top Ten as option B would.

Option D is not correct for much the same reason option A is incorrect; this question is specifically about application security, and the physical protection element is very minor.

### Question # 46 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list usually includes “injection.” In most cases, what is the attacker trying to do with an injection attack?    
A. Get the user to allow access for the attacker.     
B. Insert malware onto the system.     
C. Trick the application into running commands.    
D. Penetrate the facility hosting the software.    
Answer: C. 

In injection attacks (a large percentage of which are called SQL injection, for the prevalence with which attackers target databases with this attack), the attacker enters a string of command code into a user-facing field in an attempt to get the application to run the command. This results in a process that the attacker can leverage or puts the software into a fail state that might negate some of the security controls that are present in normal operation.

Option A is incorrect; this is a description of social engineering.

Option B is incorrect; SQL injection does not typically involve malware.
An attack that allows someone to penetrate a facility is a physical attack. The attacker has to physically be at the facility itself. Option D is incorrect.

### Question # 47 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list usually includes “injection.” In most cases, what is the method for reducing the risk of an injection attack?      
A. User training      
B. Hardening the OS      
C. Input validation/bounds checking      
D. Physical locks     
Answer: C. 

Attackers attempting injection put command code into a data entry field; if the application has suitable input validation (that is, refusing code strings and confirming that input conforms to field value types), it will block those attacks.
Injection attacks target applications, not users, so user training has little to do with preventing injection, making option A incorrect.
The OS usually has little to do with injection attacks, which usually target user-facing web apps that ride on the OS, so option B is not correct.
Injection attacks are logical, not physical, so locks won’t aid the security effort in this case, making option D incorrect.

### Question # 48 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “broken authentication and session management.” Which of the following is a good method for reducing the risk of broken authentication and session management?       
A. Do not use custom authentication schemes.    
B. Implement widespread training programs.    
C. Ensure that strong input validation is in place.     
D. Use X.400 protocol standards.     
Answer: A. 

This answer requires a bit of thought and knowledge of common practices. Throughout the IT industry, many developers attempt to design and implement their own authentication schema. According to OWASP, this approach is almost always a bad idea because of the many vulnerabilities such custom schemes may fail to address. Using approved, tested authentication implementations is a way to avoid this problem.

Authentication schema should be transparent to users, who will have little or (preferably) no control over that element of communication. Thus, training is not applicable in this case, making option B wrong.

Input validation is used to counter injection attacks and has no efficacy in authentication implementations, making option C incorrect.

The X.400 standards are for email communication and are not applicable to session authentication; thus, option D is wrong.

### Question # 49 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “broken authentication and session management.” Which of the following is not a practice/vulnerability that can lead to broken authentication and infringe on session management?     
A. Session identification exposed in URLs     
B. Unprotected stored credentials    
C. Lack of session timeout    
D. Failure to follow Health Insurance Portability and Accountability Act (HIPAA) guidance     
Answer: D. 

HIPAA is the U.S. federal law governing medical information; it has nothing to do with authentication or session management. Failure to follow HIPAA leads to regulatory noncompliance (for those covered by it).

All the other options are practices that can enhance an attacker’s ability to compromise authentication implementations and sessions.

### Question # 50 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “broken authentication and session management.” Which of the following is not a practice/vulnerability that can lead to broken authentication and infringe on session management?     
A. Failure to rotate session IDs after a successful login     
B. Easily guessed authentication credentials    
C. Weak physical entry points in the data center     
D. Credentials sent over unencrypted lines     
Answer: C. 

As breaking authentication and session management is a logical attack, lack of physical controls don’t affect such attacks.
All the other options are practices that can enhance an attacker’s ability to compromise authentication implementations and sessions.

### Question # 51 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list usually includes “cross-site scripting (XSS).” Which of the following is not a method for reducing the risk of XSS attacks?      
A. Put untrusted data in only allowed slots of HTML documents.    
B. HTML escape when including untrusted data in any HTML elements.     
C. Use the attribute escape when including untrusted data in attribute elements.    
D. Encrypt all HTML documents.     
Answer: D.      

In many cases, HTML documents are meant to be seen by the public or new users who do not yet have trust associations (accounts) with the organization, so encrypting every HTML document would be counter to the purpose. Moreover, total encryption of everything, even material that is not particularly sensitive or valuable, incurs an additional cost with no appreciable benefit.
The other options are all actions that OWASP recommends for reducing the risk of XSS attacks: www.owasp.org/index.php/XSS_(Cross_Site_Scripting)_Prevention_Cheat_Sheet.

### Question # 52 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list usually includes “cross-site scripting (XSS).” Which of the following is not a method for reducing the risk of XSS attacks?      
A. Use an auto-escaping template system.      
B. Use XML escape for all identity assertions.      
C. Sanitize HTML markup with a library designed for the purpose.      
D. HTML escape JSON values in an HTML context and read the data with JSON.parse.     
Answer: B.    

Option B is a incorrect because the answer narrows the risk for only the identity assertions and does not address XSS attack risks. All the other options are actions recommended by OWASP for reducing XSS attack risks.
This question is particularly difficult as it delves into a level of detail that may or may not appear on the actual exam; however, all source documents listed in the Candidate Information Bulletin, including the OWASP Top Ten, are fair game for the test, so it is best to have at least an understanding of these sources.   

### Question # 53 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “insecure direct object references.” Which of these is an example of an insecure direct object reference?     
A. www.sybex.com/authoraccounts/benmalisow    
B. 10 ? “sybex accounts”; 20 goto 10     
C. mysql -u [bmalisow] -p [database1];    
D. bmalisow@sybex.com    
Answer: A.    

The URL in option A reveals a location of specific data as well as the format for potential other data (such as other authors’ pages/accounts); this is a classic example of an insecure direct object reference.
Option B is a DoS program string; C is a SQL database command line (which wouldn’t reveal any information on its own; it would prompt for a password); and option D is just an email address.    

### Question # 54 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “insecure direct object references.” Which of these is a method to counter the risks of insecure direct object references?      
A. Perform user security training.      
B. Check access each time a direct object reference is called by an untrusted source.     
C. Install high-luminosity interior lighting throughout the facility.    
D. Append each object with sufficient metadata to properly categorize and classify based on asset value and sensitivity.     
Answer: B.    

Untrusted sources calling a direct reference should be authenticated to ensure that the source has authorization to access that object.
Option A will not aid in insecure direct object risks; this is not a user issue, usually, but a programming issue. Option C is for physical security, while insecure direct object references are logical attacks. Option D does not reduce the risk of insecure direct object references because classification and categorization are not protections themselves but need to be paired with proper control sets in order to provide protection.

### Question # 55 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “security misconfiguration.” Which of these is an example of a security misconfiguration?    
A. Not providing encryption keys to untrusted users     
B. Having a public-facing website     
C. Leaving default accounts unchanged     
D. Using turnstiles instead of mantraps    
Answer: C. 

Default accounts are a continual security problem in the InfoSec space, and one that is relatively easy to address. Any new systems should be checked for default accounts, which should be stripped out before deployment.
Untrusted users should not have encryption keys, so this is not a misconfiguration; therefore, option A is incorrect.
A public-facing website can be extremely useful for marketing purposes and is not necessarily a security issue in and of itself, so option B is incorrect.
Option D might or might not be true; both turnstiles and mantraps are physical security controls, and we can’t be sure whether one or the other is preferable in any given situation, so we don’t know if this is a misconfiguration or a proper configuration. Option C is therefore preferable.

### Question # 56 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “security misconfiguration.” Which of these is an example of a security misconfiguration?     
A. Having unpatched software in the production environment     
B. Leaving unprotected portable media in the workplace    
C. Letting data owners determine the classifications/categorizations of their data    
D. Preventing users from accessing untrusted networks   
Answer: A. 

Any software with out-of-date builds can be considered misconfigured.
Option B is bad security practice but not considered a misconfiguration.
Data owners are supposed to classify/categorize the data under their control, so option C is not a correct answer.
Preventing users from reaching untrusted resources may be a proper control in a given environment, so option D is not a misconfiguration, and not a correct answer.

### Question # 57 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “security misconfiguration.” Which of these is a technique to reduce the potential for a security misconfiguration?     
A. Enforce strong user access control processes.    
B. Have a repeatable hardening process for all systems/software.    
C. Use encryption for all remote access.    
D. Use encryption for all stored data.     
Answer: B.   

This question requires some thought. All the options are examples of good security practices and could therefore arguably be ways to reduce misconfiguration risks. However, option B is the best answer for this specific question: it is a method for reducing risks due to misconfiguration—a repeatable process for hardening systems/software that addresses other bad practices and is itself a good practice. This is the best answer.

### Question # 58 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list usually includes “security misconfiguration.” Which of these is a technique to reduce the potential for a security misconfiguration?     
A. Broad user training that includes initial, recurring, and refresher sessions       
B. Deeper personnel screening procedures for privileged users than is used for regular users      
C. A repeatable patching process that includes updating libraries as well as software     
D. Randomly auditing all user activity, with additional focus on privileged users    
Answer: C.     

All the options are examples of good security practices and could therefore arguably be ways to reduce misconfiguration risks. However, option C is the best answer for this specific question. The other three options are personnel/administrative/managerial controls, where the security misconfiguration is more a technical issue, which requires a technical solution.

### Question # 59 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list usually includes “security misconfiguration.” Which of these is a technique to reduce the potential for a security misconfiguration?      
A. Purchase only trusted devices/components.      
B. Follow a published, known industry standard for baseline configurations.      
C. Hire only screened, vetted candidates for all positions.      
D. Update policy on a regular basis, according to a proven process.      
Answer: B. 

All the options are examples of good security practices and could therefore arguably be ways to reduce misconfiguration risks. However, option B is the best answer for this specific question. The other three options are personnel/administrative/managerial controls, where the security misconfiguration is more a technical issue, which requires a technical solution.

### Question # 60 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list usually includes “security misconfiguration.” Which of these is a technique to reduce the potential for a security misconfiguration?      
A. Get regulatory approval for major configuration modifications.     
B. Update the business continuity and disaster recovery (BC/DR) plan on a timely basis.     
C. Train all users on proper security procedures.     
D. Perform periodic scans and audits of the environment.     
Answer: D.     

All of these are good security practices, but only option D is a method for detecting and addressing misconfigurations.

### Question # 61 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “sensitive data exposure.” Which of these is a technique to reduce the potential for a sensitive data exposure?     
A. Extensive user training on proper data handling techniques     
B. Advanced firewalls inspecting all inbound traffic, to include content-based screening      
C. Ensuring the use of utility backup power supplies     
D. Roving security guards     
Answer: A.    

Users are the most likely source of sensitive data exposure, particularly inadvertently. Ensuring that users know how to handle material properly is an excellent means for addressing the issue.

Option B is incorrect because firewalls that inspect inbound traffic only will not notice data exposed accidentally or maliciously as it travels outbound.

Option C is incorrect because it has nothing to do with data disclosure and is instead about business continuity and disaster recovery (BC/DR).

Option D is incorrect because it has nothing to do with data disclosure and is instead about physical security.

### Question # 62 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “sensitive data exposure.” All of the following are techniques for reducing the possibility of exposing sensitive data, except ____________.      
A. Destroying sensitive data as soon as possible      
B. Avoiding categorizing data as sensitive      
C. Using proper key management when encrypting sensitive data    
D. Disabling autocomplete on forms that collect sensitive data   
Answer: B.     

Data needs to be categorized according to its value/sensitivity; avoiding accurate categorization is just as troublesome, from a security perspective, as not categorizing the data or overcategorizing it (putting it in a higher category than it deserves).

All the other options are ways of reducing the risk of sensitive data disclosure. Option A reduces the possibility of disclosure by reducing the amount of data on hand (from the OWASP: “Data you don’t have can’t be stolen”). Option C reduces the chance of disclosing keys, which leads to disclosing the data. Option D reduces the possibility that the form will disclose sensitive data to someone filling it out by prompting with an entry that should be protected.

### Question # 63 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list sometimes includes “missing function level access control.” Which of these is a technique to reduce the potential for a missing function-level access control?
A. Set the default to deny all access to functions, and require authentication/authorization for each access request.    
B. HTML escape all HTML attributes.     
C. Restrict permissions based on an access control list (ACL).    
D. Refrain from including direct access information in URLs.    
Answer: A. 

Setting the default to denying access forces all resource requests to be verified, thus ensuring that no particular function may be run without explicitly ensuring that it was called by an authorized user.

Option B is used to deter cross-site scripting attacks, so it is incorrect.

Option C is correct but insufficient; option A includes a more restrictive mode, so is therefore a better choice.

Option D is used to deter the possibility of insecure direct object references, so it is incorrect.    

### Question # 64 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list sometimes includes “missing function level access control.” Which of these is a technique to reduce the potential for a missing function-level access control?    
A. Run a process as both user and privileged user, compare results, and determine similarity.    
B. Run automated monitoring and audit scripts.   
C. Include browser buttons/navigation elements to secure functions.    
D. Enhance user training to include management personnel.   
Answer: A. 

The method in option A will help you determine if there are functions that regular users should not have access to and thereby demonstrate that you are missing necessary controls.
According to the OWASP, “automated tools are unlikely to find these problems,” so option B is incorrect.

Option C is incorrect because it is the exact opposite of what you’re trying to accomplish; this is an example of what happens when function-level access controls are missing.

Option D in no way addresses the problem of missing function-level access controls, which is a technical problem, not a user issue.

### Question # 65 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “cross-site request forgery” (CSRF). Which of these is a technique to reduce the potential for a CSRF?     
A. Train users to detect forged HTTP requests.     
B. Have users remove all browsers from their devices.     
C. Don’t allow links to or from other websites.    
D. Include a CAPTCHA code as part of the user resource request process.     
Answer: D.     

Having the user authenticate the intentional request is a way to reduce the automated, forged requests attackers might submit as part of CSRF; CAPTCHA is a great way to reduce the likelihood of success for automated attacks.

Option A is incorrect because HTTP requests are usually made by the browser, without the user’s knowledge; the user has no perspective of such requests, so this wouldn’t be a useful mechanism in prevention.

Option B is incorrect because it’s unrealistic. Removing all browsers would decrease the utility of the systems to the point where productivity would be negligible.

Option C is incorrect for similar reasons; the danger from CSRF is not because of links to the target website but because of the browser behavior.

### Question # 66 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “cross-site request forgery” (CSRF). A CSRF attack might be used for all the following malicious actions except _______________.    
A. The attacker could have the user log into one of the user’s online accounts.    
B. The attacker could collect the user’s online account login credentials, to be used by the attacker later.     
C. The attacker could have the user perform an action in one of the user’s online accounts.    
D. The attacker could trick the user into calling a fraudulent customer service number hosted by the attacker and talk the user into disclosing personal information.    
Answer: D.     

This is a description of social engineering, not CSRF, which is a browser-based attack.
All the other options are possible exploits an attacker might try to accomplish with a CSRF attack.

### Question # 67 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “cross-site request forgery” (CSRF). Which of the following is a good way to deter CSRF attacks?    
A. Have your website refuse all HTTP resource requests.     
B. Ensure that all HTTP resource requests include a unique, unpredictable token.     
C. Don’t allow e-commerce on your website.   
D. Process all user requests with only one brand of browser, and refuse all resource requests from other browsers.    
Answer: B. 

This is the option OWASP recommends as the very least form of protection. Having a unique, unpredictable token for each session reduces the likelihood an attacker will be able to reuse tokens known by the browser or craft tokens that can be used in future attacks.

Option A is not optimal or sensible because it would inhibit all web traffic and remote access.

Option C is not optimal or sensible because it would severely limit your online capabilities.

Option D is not sensible because all browsers use stored tokens/cookies, and no browser is preferable for the purpose over others.

### Question # 68 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “using components with known vulnerabilities.” Which of the following is a good way to protect against this problem?     
A. Use only components your organization has written.    
B. Update to current versions of component libraries as soon as possible.    
C. Never use anyone else’s component library.    
D. Apply patches to old component libraries.    
Answer: B.    

This is not an easy question and requires an understanding of how component libraries are used in software design.

Option B is preferable to the others because, according to the OWASP, publishers of component libraries do not often patch old components but rather issue the fixed component(s) as a new version. This is also why option D is incorrect.

Options A and C are two ways of stating the same thing, and not optimal; trying to use this method would require every one of your software packages to be wholly written by your programmers, which is actually not more secure than using published component libraries because the risk of additional human error and lack of review is introduced to the process.

### Question # 69 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “using components with known vulnerabilities.” Why would an organization ever use components with known vulnerabilities to create software?    
A. The organization is insured.      
B. The particular vulnerabilities exist only in a context not being used by developers.      
C. Some vulnerabilities exist only in foreign countries.    
D. A component might have a hidden vulnerability.    
Answer: B. 

This is not an easy question and requires an understanding of how component libraries are used in software design.

Option B makes the most sense; some vulnerabilities are known to exist only when a component is used in a specific way or with specific services; if the programmers are not including that way of using the component or the risky service, then the vulnerability would not pose a threat to the software they are creating and may therefore be acceptable.

Option A is not correct because an underwriter would be unlikely to cover a claim resulting solely from negligence; using a component with a known vulnerability and putting the product/user at risk knowingly would probably invalidate any insurance policy.

Option C might conceivably be considered correct in a fashion; different countries have different legislation/regulations, and a vulnerability that could cause noncompliance in one country might not in another. However, this is a rather tortured reading of the question, requiring some convoluted reasoning, and this option is therefore not the best answer.

Option D is not correct because a hidden vulnerability, by definition, is not a known vulnerability.   

### Question # 70 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “using components with known vulnerabilities.” Which of the following is a good way to protect against this problem?    
A. Use only standard libraries.    
B. Review all updates/lists/notifications for components your organization uses.   
C. Be sure to HTML escape all attribute elements.    
D. Increase the user training budget.     
Answer: B.    

Staying current with published vulnerabilities for your component is crucial. This might not be simple as there are many versions of design components, and nomenclature is not always uniform.

Option A is incorrect because even standard libraries are subject to vulnerabilities, so you have to review notifications about those as well.

Option C is not correct; this is a method for reducing the risk of cross-site scripting (XSS) attacks.

Option D will not work as users have no influence or effect on which components are used in software design.

### Question # 71 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list sometimes includes “unvalidated redirects and forwards.” Which of the following is a good way to protect against this problem?     
A. HTML escape all HTML attributes.     
B. Train users to recognize invalidated links.      
C. Block all inbound resource requests.     
D. Implement audit logging.     
Answer: B.     

Oddly enough, this may be a good topic to explain during user training; when an attacker is trying to conduct an attack by exploiting unvalidated redirects and forwards, it is often in conjunction with a social engineering/phishing aspect. Users trained to recognize social engineering/phishing indicators might be able to avoid susceptibility to these attacks.

Option A is not correct; this is a method for reducing the risk of cross-site scripting (XSS) attacks.

Option C is not correct; it is ridiculous and would result in preventing all remote access.

Option D is not correct; audit logging would only track activity, not prevent a user from being directed/forwarded to an attack site.

### Question # 72 - The Open Web Application Security Project (OWASP) Top Ten is a list of web application security threats that is created by a member-driven OWASP committee of application development experts and published approximately every 24 months. The OWASP Top Ten list often includes “unvalidated redirects and forwards.” Which of the following is a good way to protect against this problem?     
A. Don’t use redirects/forwards in your applications.    
B. Refrain from storing credentials long term.    
C. Implement security incident/event monitoring (security information and event management [SIEM]/security information management [SIM]/security event management [SEM]) solutions.     
D. Implement digital rights management (DRM) solutions.    
Answer: A.    

Basic as it may seem, not including redirects and forwards within your software is an easy way to avoid the problem altogether, and redirects/forwards are not necessary for efficient usage.

Option B is a incorrect because this type of attack is not aimed at stored credentials.

Options C and D are both incorrect because neither of those types of solutions detect or prevent this type of attack.

### Question # 73 - You are the security subject matter expert (SME) for an organization considering a transition from a traditional IT enterprise environment into a hosted cloud provider’s data center. One of the challenges you’re facing is whether your current applications in the on-premises environment will function properly with the provider’s hosted systems and tools. This is a(n) _______________ issue.      
A. Interoperability    
B. Portability    
C. Stability    
D. Security   
Answer: A. 

This is the definition of cloud migration interoperability challenges. Portability is the measure of how difficult it might be to move the organization’s systems/data from a given cloud host to another cloud host. Stability has no specific meaning here and is just a distractor. Security might be an element of this challenge but is not the optimum answer; the question posed a concern about functionality, not disclosure or tainting the information.

### Question # 74 - You are the security subject matter expert (SME) for an organization considering a transition from a traditional IT enterprise environment into a hosted cloud provider’s data center. One of the challenges you’re facing is whether the provider will have undue control over your data once it is within the provider’s data center; will the provider be able to hold your organization hostage because they have your data? This is a(n) _______________ issue.    
A. Interoperability    
B. Portability   
C. Stability   
D. Security    
Answer: B.    

This is the definition of cloud migration portability, the measure of how difficult it might be to move the organization’s systems/data from a given cloud host to another cloud host. Interoperability issues involve whether the cloud customer’s legacy services/data will interface properly with the provider’s systems. Stability has no specific meaning here and is just a distractor. Security might be an element of this challenge, but it is not the optimum answer; the question posed a concern about functionality, not disclosure or tainting the information.

### Question # 75 - You are the security subject matter expert (SME) for an organization considering a transition from a traditional IT enterprise environment into a hosted cloud provider’s data center. One of the challenges you’re facing is whether the cloud provider will be able to comply with the existing legislative and contractual frameworks your organization is required to follow. This is a _______________ issue.    
A. Resiliency    
B. Privacy    
C. Performance   
D. Regulatory    
Answer: D. 

This is the definition of a regulatory issue. Option B might also be a factor in this kind of issue, but because the subject of privacy or any specific related topic (such as personally identifiable information [PII], the European Union General Data Protection Regulation) was not mentioned, option D is the better answer. Resiliency issues involve the provider’s ability to handle disruptive externalities, such as natural disasters, system failures, and utility outages. Performance issues address the ability of the provider to meet the customer’s IT needs.

### Question # 76 - You are the security subject matter expert (SME) for an organization considering a transition from a traditional IT enterprise environment into a hosted cloud provider’s data center. One of the challenges you’re facing is whether the cloud provider will be able to allow your organization to substantiate and determine with some assurance that all of the contract terms are being met. This is a(n) _______________ issue.    
A. Regulatory    
B. Privacy    
C. Resiliency    
D. Auditability     
Answer: D.    

This is not an easy question. In the context of the question, the cloud customer is trying to ascertain whether they are getting what they’re paying for; that is, a way for them to audit the cloud provider and the service as a whole. This is not a regulatory issue, as it concerns the contractual agreement between the provider and the customer, not a third party performing oversight. It is also not a privacy issue (primarily; privacy concerns might be part of the contract, but it’s not the prevailing aspect of the issue here). Resiliency issues involve the provider’s ability to handle disruptive externalities, such as natural disasters, system failures, or utility outages.

### Question # 77 - Encryption is an essential tool for affording security to cloud-based operations. While it is possible to encrypt every system, piece of data, and transaction that takes place on the cloud, why might that not be the optimum choice for an organization?     
A. Key length variances don’t provide any actual additional security.
B. It would cause additional processing overhead and time delay.     
C. It might result in vendor lockout.    
D. The data subjects might be upset by this.    
Answer: B.    

Encryption consumes processing power and time; as with all security controls, additional security means measurably less operational capability—there is always a trade-off between security and productivity. Option A is gibberish and only a distractor. Option C is incorrect because vendor lock-out does not result from encryption; it is what might happen if the cloud provider goes out of business while holding your data. Data subjects are the individuals whose personally identifiable information (PII) an organization holds; usually, they will not know or care if something is encrypted (unless there is a breach of that PII, and then investigators will want to determine how that PII was protected) and would probably welcome total encryption, even though that might mean a decrease in operational capability.

### Question # 78 - Encryption is an essential tool for affording security to cloud-based operations. While it is possible to encrypt every system, piece of data, and transaction that takes place on the cloud, why might that not be the optimum choice for an organization?     
A. It could increase the possibility of physical theft.    
B. Encryption won’t work throughout the environment.     
C. The protection might be disproportionate to the value of the asset(s).   
D. Users will be able to see everything within the organization.    
Answer: C.    

Security should be commensurate with asset value, as determined by management; putting extra security on everything in an environment is usually not cost effective. The other options don’t make sense. For example, encryption doesn’t affect the potential for physical theft, encryption can be implemented organization-wide, and access controls can be placed on encrypted information as well as unencrypted.

### Question # 79 - Which of the following is not an element of the identification component of identity and access management (IAM)?     
A. Provisioning    
B. Management   
C. Discretion    
D. Deprovisioning   
Answer: C.    

Discretion is not an element of identification and has no meaning in this context. All the other options are aspects of the identification portion of IAM.

### Question # 80 - Which of the following entities is most likely to play a vital role in the identity provisioning aspect of a user’s experience in an organization?      
A. The accounting department     
B. The human resources (HR) office    
C. The maintenance team    
D. The purchasing office    
Answer: B. 

Of these options, HR is most likely to participate in identity provisioning; HR will usually validate the user’s identity against some documentation (driver’s license, passport, etc.) as part of the user’s initial employment process and then pass confirmation of validation along to whatever entity issues system sign-on credentials. None of the other entities usually takes part in user identification.

### Question # 81 - Why is the deprovisioning element of the identification component of identity and access management (IAM) so important?      
A. Extra accounts cost so much extra money.     
B. Open but unassigned accounts are vulnerabilities.     
C. User tracking is essential to performance.    
D. Encryption has to be maintained.    
Answer: B.    

Unused accounts that remain open can serve as attack vectors. All the other options are not associated with identity and access management.

### Question # 82 - All of the following are reasons to perform review and maintenance actions on user accounts except _______________.     
A. To determine whether the user still needs the same access     
B. To determine whether the user is still with the organization     
C. To determine whether the data set is still applicable to the user’s role     
D. To determine whether the user is still performing well    
Answer: D. 

Job performance is not a germane aspect of account review and maintenance; that is a management concern, not an access control issue. All the other options are legitimate access control concerns.

### Question # 83 - Who should be involved in review and maintenance of user accounts/access?     
A. The user’s manager    
B. The security manager     
C. The accounting department    
D. The incident response team    
Answer: A. 

This is not an easy question. The best answer to the question does not appear on the list; that would be the data owner, because the data owner should be the ultimate arbiter of who has what access to the data under the owner’s control. However, of these options, A is the best; the user’s manager will have the greatest amount of insight into the role of the user within the organization and therefore will understand best which data the user needs to access. The security manager does not have this insight, and the task of reviewing all access for all users within the organization would be far too large an undertaking for that position. Accounting and incident response play no part in reviewing ongoing user account applicability.

### Question # 84 - Which of the following protocols is most applicable to the identification process aspect of identity and access management (IAM)?    
A. Secure Sockets Layer (SSL)     
B. Internet Protocol Security (IPSec)     
C. Lightweight Directory Access Protocol (LDAP)    
D. Amorphous ancillary data transmission (AADT)    
Answer: C. 

LDAP is used in constructing and maintaining centralized directory services, which are vital in all aspects of IAM. SSL and IPSec are used to create secure communication sessions—important, but not most applicable for IAM. AADT is a fictitious term used as a distractor.

### Question # 85 - Privileged user (administrators, managers, and so forth) accounts need to be reviewed more closely than basic user accounts. Why is this?
A. Privileged users have more encryption keys.    
B. Regular users are more trustworthy.    
C. There are extra controls on privileged user accounts.   
D. Privileged users can cause more damage to the organization.    
Answer: D. 

The additional capabilities of privileged users make their activities riskier to the organization, so these accounts bear extra review. The number of encryption keys a user has is meaningless out of context; the amount of risk is the issue, not the number of keys. The user’s type (regular versus privileged) is not an indicator, itself, of trustworthiness. Additional review activity for privileged users is an extra control we place on privileged users, not a reason for doing so.   

### Question # 86 - The additional review activities that might be performed for privileged user accounts could include all of the following except _______________.   
A. Deeper personnel background checks   
B. Review of personal financial accounts for privileged users   
C. More frequent reviews of the necessity for access   
D. Pat-down checks of privileged users to deter against physical theft   
Answer: D. 

The efficacy of frisking administrators and managers is doubtful, and the harm to morale and disparity of enforcement likely outweighs any security benefit. All the other options could and should be included in privileged account review.

### Question # 87 - If personal financial account reviews are performed as an additional review control for privileged users, which of the following characteristics is least likely to be a useful indicator for review purposes?   
A. Too much money in the account   
B. Too little money in the account   
C. The bank branch being used by the privileged user   
D. Specific senders/recipients    
Answer: C. 

Which bank branch a privileged user frequents is unlikely to be of consequence. Too much money can indicate that the privileged user is accepting payment from someone other than the employer, which can be an indicator of malfeasance or corruption. Too little money can indicate that the privileged user is subject to undue financial stress, which might be the result of behavior that makes the privileged user susceptible to subversion, such as a drug habit, family problems, or excess gambling. Specific senders and recipients of personal funds can indicate untoward activity on the part of the privileged user.

### Question # 88 - How often should the accounts of privileged users be reviewed?    
A. Annually   
B. Twice a year    
C. Monthly  
D. More often than regular user account reviews   
Answer: D. 

There is no specific rule for the timeliness of privileged user account reviews. However, as a matter of course, privileged user accounts should be reviewed more often than the accounts of regular users because privileged users can cause more damage and therefore entail more risk.

### Question # 89 - Privileged user account access should be _______________.    
A. Temporary  
B. Pervasive   
C. Thorough   
D. Granular   
Answer: A. 

Privileged users should have privileged access to specific systems/data only for the duration necessary to perform their administrative function; any longer incurs more risk than value. The other options are not associated with appropriate privilege access management.

### Question # 90 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA’s Notorious Nine list, data breaches can be _______________.     
A. Overt or covert      
B. International or subterranean     
C. From internal or external sources     
D. Voluminous or specific    
Answer: C. 

The CSA points out that data breaches come from a variety of sources, including both internal personnel and external actors. Although breaches might be overt or covert, or large or small, we don’t usually think of them in these terms, and the CSA doesn’t discuss them that way, so options A and D aren’t correct. 
Option B is just incorrect because subterranean is not associated with the CSA’s Notorious Nine list of common threats.

### Question # 91 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, an organization that operates in the cloud environment and suffers a data breach may be required to _______________.     
A. Notify affected users     
B. Reapply for cloud service     
C. Scrub all affected physical memory     
D. Change regulatory frameworks     
Answer: A.     

Data breach notification laws are plentiful; organizations operating in the cloud are almost sure to be subject to one or more such laws. Option B is incorrect because the CSA does not suggest that an organization that operates in the cloud environment and suffers a data breach may be required to reapply for cloud service. 

Option C is unlikely because most cloud customers won’t have physical access to/control of devices; moreover, a breach does not always entail sanitization. 

Option D does not make sense, either; regulations are imposed on organizations, as legal mandates, and an organization does not get to choose which regulations affect it.

### Question # 92 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, an organization that suffers a data breach might suffer all of the following negative effects except _______________.      
A. Cost of compliance with notification laws    
B. Loss of public perception/goodwill     
C. Loss of market share      
D. Cost of detection     
Answer: D. 

The cost of detection exists whether or not the organization suffers a breach. All other options are costs an organization will likely face as the result of a breach.

### Question # 93 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, in the event of a data breach, a cloud customer will likely need to comply with all the following data breach notification requirements except _______________.       
A. Multiple state laws      
B. Contractual notification requirements      
C. All standards-based notification schemes     
D. Any applicable federal regulations     
Answer: C. 

This question requires a bit of thought. Option C is correct because an organization is not required to subscribe to all standards but instead only the standards it selects (or are imposed on it through regulation). However, most cloud customers will have to comply with multiple state laws (at the very least, the laws of the states where the customer’s organization resides, where the data center resides, and where its end clientele reside); any contractual requirements (between the cloud customer and its consumers, vendors, or service providers, such as, for example, Payment Card Industry Data Security Standard [PCI DSS]); and any federal regulations that govern that cloud customer’s industry.

### Question # 94 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, data loss can be suffered as a result of _______________ activity.      
A. Malicious or inadvertent      
B. Casual or explicit     
C. Web-based or stand-alone     
D. Managed or independent     
Answer: A. 

Data loss can be the result of deliberate or accidental behavior. The other options are less correct than option A.

### Question # 95 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, all of the following activity can result in data loss except _______________.    
A. Misplaced crypto keys      
B. Improper policy     
C. Ineffectual backup procedures     
D. Accidental overwrite     
Answer: B. 

Bad policy won’t explicitly lead to data loss, but it might hinder efforts to counter data loss. However, misplaced crypto keys can result in a self-imposed denial of service, bad backup procedures can result in failure to retain data (a form of data loss), and accidental overwrites occur all the time—hence the need for proper backups.     

### Question # 96 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, service traffic hijacking can affect which portion of the CIA triad?        
A. Confidentiality      
B. Integrity        
C. Availability        
D. All of the triad     
Answer: D. 

All. Service traffic hijacking can affect all portions of the CIA triad. Through hijacking, an attacker could eavesdrop on legitimate communication (breaching confidentiality), insert inaccurate/incorrect data into legitimate communication (damaging integrity), and/or redirect legitimate users from valid services (making the legitimate sources unavailable). Although all of the answers are correct, option D is the most comprehensive and therefore the best answer.

### Question # 97 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. The CSA recommends the prohibition of _______________ in order to diminish the likelihood of account/service traffic hijacking.     
A. All user activity        
B. Sharing account credentials between users and services       
C. Multifactor authentication     
D. Interstate commerce     
Answer: B. 

Users sharing account credentials is a fairly common (although undesirable) practice and one that can lead to significant misuse of the organization’s resources and greatly increase risk to the organization. Although ending all user activity would make our IT environments so much more secure and defensible, it would also make them utterly useless from a productivity standpoint, so option A is incorrect. Option C is incorrect because the CSA recommends multifactor authentication as a means to reduce the risk of hijacking. Though not documented on the CSA’s website, the CSA most certainly does not recommend the prohibition of interstate commerce in order to diminish the likelihood of account/service traffic hijacking. Therefore, option D is an incorrect answer.

### Question # 98 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, which aspect of cloud computing makes it particularly susceptible to account/service traffic hijacking?    
A. Scalability    
B. Metered service     
C. Remote access    
D. Pooled resources     
Answer: C. 

Cloud computing users are especially susceptible to hijacking attacks because all of their use is contingent on remote access; users in a traditional internal environment are not passing as much traffic over untrusted infrastructure (the Internet), and the type of traffic is often different (where identity credentials are passed only to servers/systems that are locally, physically connected to the user’s device).

Scalability might be seen as an attribute of cloud computing that increases the potential for hijacking attacks because a proliferation of users means more attack surface. But even that aspect is contingent on the users accessing cloud resources remotely, so option C is still a better answer than A.
The metered service nature of cloud computing has nothing to do with a hijacking threat; metered service indicates that the customer pays only for those resources users consume.

Cloud customers pool resources might be of concern when considering hijacking attacks because poorly configured cloud environments could leave one cloud customer subject to attack by another tenant in that same environment. But, again, hijacking is predicated on attacking data in transit, so it is the remote access aspect that is the best answer for this question.

### Question # 99 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, what is one reason the threat of insecure interfaces and APIs is so prevalent in cloud computing?     
A. Most of the cloud customer’s interaction with resources will be performed through APIs.    
B. APIs are inherently insecure.    
C. Attackers have already published vulnerabilities for all known APIs.   
D. APIs are known carcinogens.    
Answer: A. 

Because a significant percentage of cloud customer interactions with the cloud environment will utilize APIs, the threat of insecure APIs is of great concern in cloud computing.

Option B is incorrect because APIs are not inherently insecure and it is unlikely that the CSA has stated that they are.

Option C is incorrect because it is predicated on the inaccurate notion that all APIs are inherently insecure and that the vulnerabilities of all known APIs have been published.

Lastly, option B is inaccurate because APIs are not known carcinogens. To be a carcinogen, the carcinogen needs to be a substance that causes cancer in living tissue. As far as we know, APIs do not cause cancer.

### Question # 100 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, what is one reason the threat of insecure interfaces and APIs is so prevalent in cloud computing?      
A. Cloud customers and third parties are continually enhancing and modifying APIs.   
B. APIs can have automated settings.      
C. It is impossible to uninstall APIs.        
D. APIs are a form of malware.     
Answer: A.      

The continuous modification of APIs issued/designed by cloud providers introduces the potential for vulnerabilities to be created in interfaces that were previously thought to be vetted and secure. Increased complexity necessarily means increased potential for vulnerability. And third-party modifications may lead to user credentials being unknowingly exposed to those third parties.
Automation is not inherently a source of threats/vulnerabilities, so option B is not correct.

Options C and D are not true.

### Question # 101 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, what is one reason the threat of insecure interfaces and APIs is so prevalent in cloud computing?     
A. APIs are always used for administrative access.     
B. Customers perform many high-value tasks via APIs.     
C. APIs are cursed.     
D. It is impossible to securely code APIs.     
Answer: B. 

APIs will be used for many tasks that could have a significant negative impact on the organization, so any vulnerabilities are of great concern.
Not all API interaction involves administrative access, so option A is wrong.
APIs may or may not be cursed.
Secure code practices can be used to design robust APIs, so option D is incorrect.

### Question # 102 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, why are denial of service (DoS) attacks such a significant threat to cloud operations?      
A. DoS attackers operate internationally.       
B. There are no laws against DoS attacks, so they are impossible to prosecute.     
C. Availability issues prevent productivity in the cloud.     
D. DoS attacks that can affect cloud providers are easy to launch.     
Answer: C.      

If users can’t access the cloud provider, then the operational environment is, for all intents and purposes, useless. DoS attacks that affect availability of cloud services are therefore a great concern.

A lot of attackers/criminals operate internationally; this has no bearing on whether an organization operates in the cloud or otherwise. Option A is incorrect.
There are laws prohibiting DoS attacks, so option B is incorrect.

The volume of DoS traffic necessary to disrupt modern cloud providers is rather significant, so these types of attacks are not simple. Option D is incorrect.

### Question # 103 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, what do we call denial of service (DoS) attacks staged from multiple machines against a specific target?      
A. Invasive denial of service (IDoS)      
B. Pervasive denial of service (PDoS)      
C. Massive denial of service (MDoS)     
D. Distributed denial of service (DDoS)     
Answer: D.     

Denial-of-service attacks staged from multiple machines against a specific target is the definition of a DDoS. All the other options are either fictitious or are not typically associated with the definition of DDoS.

### Question # 104 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, what aspect of managed cloud services makes the threat of malicious insiders so alarming?       
A. Scalability     
B. Multitenancy      
C. Metered service      
D. Flexibility    
Answer: B.     

In a managed cloud service context, one malicious cloud administrator could ostensibly victimize a great number of cloud customers, making the impact much greater than a sole insider in the legacy environment.
The other options are not applicable to the insider threat.

### Question # 105 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, what aspect of managed cloud services makes the threat of abuse of cloud services so alarming from a management perspective?    
A. Scalability      
B. Multitenancy      
C. Resiliency     
D. Broadband connections     
Answer: A.     

Because users in cloud customer organizations often do not pay directly for cloud services (and are often not even aware of the cost of use), scalability can be a significant management concern; individuals, offices, or departments within the organization can create dozens or even hundreds of new virtual systems in a cloud environment, for whatever purpose they need or desire, and the cost is realized only by the department in the organization that is charged with paying the bill. This type of abuse hinges on the immense scalability of cloud services and is frequently not associated with any malicious intent but is instead an inadvertent result of well-intentioned or careless behavior.
The other options are not applicable to the threat of abuse of cloud services.

### Question # 106 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. According to the CSA, which of the following is not an aspect of due diligence that the cloud customer should be concerned with when considering a migration to a cloud provider?       
A. Ensuring that any legacy applications are not dependent on internal security controls before moving them to the cloud environment      
B. Reviewing all contractual elements to appropriately define each party’s roles, responsibilities, and requirements      
C. Assessing the provider’s financial standing and soundness     
D. Vetting the cloud provider’s administrators and personnel to ensure the same level of trust as the legacy environment     
Answer: D.      

The cloud customer will not have any insight into the personnel security aspects of the cloud provider; when an organization contracts out a service, the organization loses that granular level of control.
It is imperative that the cloud customer determine whether any application dependencies exist in the legacy environment before migrating to the cloud.
Reviewing the contract between the cloud customer and provider is an essential element of due diligence.
Determining the long-term financial viability of a cloud provider is a way to avoid losing production capability/data in the cloud.

### Question # 107 - The Cloud Security Alliance (CSA) publishes the Notorious Nine, a list of common threats to organizations participating in cloud computing. A cloud customer that does not perform sufficient due diligence can suffer harm if the cloud provider they’ve selected goes out of business. What do we call this problem?      
A. Vendor lock-in     
B. Vendor lockout      
C. Vendor incapacity     
D. Unscaled    
Answer: B.     

This is the definition of vendor lockout.
Vendor lock-in is when data portability is limited, either through unfavorable contract language or technical limitations.
Vendor incapacity and unscaled are not meaningful terms in the context of cloud computing.

### Question # 108 - Which of the following is not a method for creating logical segmentation in a cloud data center?       
A. Virtual local area networks (VLANs)      
B. Network address translation (NAT)     
C. Bridging     
D. Hubs     
Answer: D.     

A hub is a (mostly archaic) network device that simply connects physical machines together; it cannot serve the purpose of network segmentation.
All the other options are segmentation methods/tools. Option C may be perceived as a viable answer because bridges connect network segments (allowing a segmented network, but not really creating segmentation), but option D is a better choice for this question.

### Question # 109 - According to (ISC)2, the lack/ambiguity of physical endpoints as individual network components in the cloud environment creates what kind of threat/concern?      
A. The lack of defined endpoints makes it difficult to uniformly define, manage, and protect IT assets.       
B. Without physical endpoints, it is impossible to apply security controls to an environment.      
C. Without physical endpoints, it is impossible to track user activity.     
D. The lack of physical endpoints increases the opportunity for physical theft/damage.     
Answer: A.     

Knowing exactly where and what your assets are, from an IT security professional’s perspective, allows you to better apply uniform and ubiquitous governance and controls across the environment. Without these clear demarcations, that task becomes more difficult.
Nothing is impossible; these tasks may become more challenging, but not impossible. So options B and C are incorrect.

Option D is not true because lack of physical endpoints may actually reduce the threat of physical theft/damage.

### Question # 110 - When should cloud providers allow platform as a service (PaaS) customers shell access to the servers running their instances?     
A. Never      
B. Weekly      
C. Only when the contract stipulates that requirement     
D. Always    
Answer: A.     

PaaS customers should never be given shell access to underlying infrastructure because any changes by one customer may negatively impact other customers in a multitenant environment.

All the other options are simply incorrect.

### Question # 111 - In a PaaS implementation, each instance should have its own user-level permissions; when instances share common policies/controls, the cloud security professional should be careful to reduce the possibility of _______________ and _______________ over time.      
A. Denial of service (DoS)/physical theft       
B. Authorization creep/inheritance     
C. Sprawl/hashing      
D. Intercession/side-channel attacks    
Answer: B.     

Mass permissions assigned to multiple instances may be susceptible to inadvertent authorization creep and permission inheritance over time as users shift roles and responsibilities and are assigned to new tasks and teams and as new users come into the existing, fluid environment.
All the other options are just wrong, with at least one nonsensical element in each.

### Question # 112 - In a platform as a service (PaaS) environment, user access management often requires that data about user activity be collected, analyzed, audited, and reported against rule-based criteria. These criteria are usually based on _______________.       
A. International standards      
B. Federal regulations       
C. Organizational policies      
D. Federation directives    
Answer: C.     

Organizational policies dictate rules for access entitlement.
International standards do not apply to every organization’s internal needs and individual user roles, so option A is incorrect.
Not all organizations are bound by all (or any) federal regulations, but all organizations should have policies regarding user access rules, so option B is incorrect.

Option D is a nod to Star Trek and also incorrect.

### Question # 113 - An essential element of access management, _______________ is the practice of confirming that an individual is who they claim to be.      
A. Authentication    
B. Authorization     
C. Nonrepudiation      
D. Regression      
Answer: A. 

Authentication is verifying that the user is who they claim to be and assigning them an identity assertion (usually a user ID) based on that identity.
Authorization is granting access based on permissions allocated to a particular user/valid identity assertion.
Nonrepudiation is the security concept of not allowing a participant in a transaction to deny that they participated.
Regression is a statistical concept not relevant to the question in any way.

### Question # 114 - An essential element of access management, _______________ is the practice of granting permissions based on validated identification.       
A. Authentication     
B. Authorization     
C. Nonrepudiation      
D. Regression     
Answer: B. 

This is the definition of authorization.
Authentication is verifying that the user is who they claim to be and assigning them an identity assertion (usually a user ID) based on that identity.
Nonrepudiation is the security concept of not allowing a participant in a transaction to deny that they participated.
Regression is a statistical concept not relevant to the question in any way.

### Question # 115 - What is the usual order of an access management process?      
A. Access-authorization-authentication    
B. Authentication-authorization-access     
C. Authorization-authentication-access    
D. Authentication-access-authorization    
Answer: B.    

In access management, the user is first authenticated (their identity verified and validated as correct), then authorized (permissions granted based on their valid identity), and given access.

### Question # 116 - Why are platform as a service (PaaS) environments at a higher likelihood of suffering backdoor vulnerabilities?       
A. They rely on virtualization.     
B. They are often used for software development.     
C. They have multitenancy.     
D. They are scalable.     
Answer: B.     

PaaS environments are attractive for software development because they allow testing of software on multiple operating systems that are administered by the cloud provider. Software developers routinely use backdoors as development and administrative tools in their products; these backdoors, if left in software when it ships, are significant vulnerabilities.
All cloud environments, including PaaS, rely on virtualization, have multitenancy, and are scalable, so those options are not correct.

### Question # 117 - Backdoors are sometimes left in software by developers _______________.     
A. In lieu of other security controls     
B. As a means to counter denial of service (DoS) attacks      
C. Inadvertently or on purpose     
D. As a way to distract attackers     
Answer: C. 

Backdoors that were used legitimately during the development process can sometimes be left in a production version of the delivered software accidentally, when developers forget to remove them. Sometimes, these products ship with backdoors purposefully placed there for administrative and customer service functions as well.

Option A is incorrect as backdoors are not a control.

Option B is incorrect because backdoors don’t serve as DoS protection in any way.
 
Option D is incorrect because backdoors are not distractions for attackers, but means for attack.

### Question # 118 - Alice is staging an attack against Bob’s website. She is able to introduce a string of command code into a database Bob is running, simply by entering the command string into a data field. This is an example of which type of attack?      
A. Insecure direct object reference      
B. Buffer overflow    
C. SQL injection     
D. Denial of service     
Answer: C. 

This is an example of typical SQL injection. All the other options are also attacks listed in the Open Web Application Security Project (OWASP) Top Ten, but they do not have the characteristics as the one contained in the question.

### Question # 119 - Bob is staging an attack against Alice’s website. He is able to embed a link on her site that will execute malicious code on a visitor’s machine if the visitor clicks on the link. This is an example of which type of attack?      
A. Cross-site scripting      
B. Broken authentication/session management      
C. Security misconfiguration     
D. Insecure cryptographic storage    
Answer: A.     

This is the definition of a cross-site scripting attack. Options B and C are also attacks listed in the Open Web Application Security Project (OWASP) Top Ten. Option D is not in the Top Ten and is made up as a fictitious option.

### Question # 120 - Alice is staging an attack against Bob’s website. She has discovered that Bob has been storing cryptographic keys on a server with a default admin password and is able to get access to those keys and violate confidentiality and access controls. This is an example of which type of attack?     
A. SQL injection      
B. Buffer overflow      
C. Using components with known vulnerabilities     
D. Security misconfiguration     
Answer: D. 

This is likely a security misconfiguration, as crypto keys must not be disclosed or the cryptosystem does not provide protection; most successful attacks on cryptosystems have been configuration/implementation attacks, not mathematical or statistical. The other options are all also in the Open Web Application Security Project (OWASP) Top Ten.

### Question # 121 - Which of the following is a management risk that organizations migrating to the cloud will have to address?     
A. Insider threat      
B. Virtual sprawl     
C. Distributed denial of service (DDoS) attacks     
D. Natural disasters     
Answer: B.     

In the cloud environment, it is very easy for a user to generate a new virtual instance; that is one of the advantages of the cloud. However, this can pose a problem for management, as users might generate many more instances than expected because the users don’t usually realize (or have to pay) the per-instance costs associated with doing so. However, the organization will have to pay the full price of many more instances at the end of each billing cycle, and exceeding the allotted amount dictated by the contract can be quite expensive. In the traditional environment, this would not pose a risk because the number of possible instances is limited by the resource capacity within the organization and additional instances don’t have attendant direct costs. All the other options are not cloud-specific risks; they also exist in the traditional environment.

### Question # 122 - Which kind of hypervisor is the preferred target of attackers, and why?     
A. Type 1, because it is more straightforward     
B. Type 1, because it has a greater attack surface     
C. Type 2, because it is less protected     
D. Type 2, because it has a greater attack surface     
Answer: D.     

A Type 2 hypervisor is run on top of an existing operating system, greatly increasing the potential attack surface.

Option A does not make logical sense; a Type 1 hypervisor is not more straightforward than other hypervisors. Option A is not the correct answer.

Option B is not true. A Type 1 hypervisor has a smaller attack surface, not a larger one.

Option C is not true in general. Type 2 hypervisors are not necessarily less protected than other hypervisors. Option C is not the correct answer.

### Question # 123 - Which of the following would make a good provision to include in the service-level agreement (SLA) between cloud customer and provider?     
A. Location of the data center     
B. Amount of data uploaded/downloaded during a pay period        
C. Type of personnel security controls for network administrators      
D. Physical security barriers on the perimeter of the data center campus      
Answer: B.      

Option B is the only element that lends itself well to a discrete, objective metric; the other options might be something the customer is interested in but will often have little control over; if the customer is insistent on those points, they should be included in the contract, not the SLA.

### Question # 124 - What is the most significant aspect of the service-level agreement (SLA) that incentivizes the cloud provider to perform?     
A. The thoroughness with which it details all aspects of cloud processing      
B. The financial penalty for not meeting service levels     
C. The legal liability for violating data breach notification requirements      
D. The risk exposure to the cloud provider      
Answer: B. 

Usually, when a provider does not meet the terms specific in the SLA, the provider will not be paid for a period of service; this is the strongest, most immediate tool at the customer’s disposal. The other options simply are not true.

### Question # 125 - From a customer perspective, all of the following are benefits of infrastructure as a service (IaaS) cloud services except _______________.    
A. Reduced cost of ownership     
B. Reduced energy costs      
C. Metered usage    
D. Reduced cost of administering the operating system (OS) in the cloud environment     
Answer: D. 
 
In an IaaS configuration, the customer still has to maintain the OS, so option D is the only answer that is not a direct benefit for the cloud customer.

### Question # 126 - From an academic perspective, what is the main distinction between an event and an incident?      
A. Incidents can last for extended periods (days or weeks), whereas an event is momentary.      
B. Incidents can happen at the network level, whereas events are restricted to the system level.       
C. Events are anything that can occur in the IT environment, whereas incidents are unscheduled events.     
D. Events occur only during processing, whereas incidents can occur at any time.    
Answer: C.     

This is the textbook definition of an incident versus event. However, this question is not easy, because many sources in the IT security field define incidents differently; it’s common to think of incidents as events that have an adverse impact, or incidents are something that require response. However, option C is the correct answer.

### Question # 127 - The cloud computing characteristic of elasticity promotes which aspect of the CIA triad?      
A. Confidentiality      
B. Integrity     
C. Availability    
D. None    
Answer: D.     

Elasticity is a beneficial characteristic in that it supports the management goal of matching resources to user needs, but it does not provide any security benefit.

### Question # 128 - A hosted cloud environment is great for an organization to use as _______________.      
A. Storage of physical assets      
B. A testbed/sandbox     
C. A platform for managing unsecured production data      
D. A cost-free service for meeting all user needs    
Answer: B.     

Cloud customers can test different hardware/software implementations in the cloud without affecting the production environment and use this information to make decisions before investing in particular solutions. Option A is not true because the cloud does not store physical assets. Option C is not accurate because production data in the cloud must still be secured. And option D is not true because cloud hosting is not free; there is some cost (even if that cost is less than it would be for comparable on-premises hosting).

### Question # 129 - What is the entity that created the Statement on Standards for Attestation Engagements (SSAE) auditing standard and certifies auditors for that standard?       
A. National Institute of Standards and Technology (NIST)      
B. European Network and Information Security Agency (ENISA)      
C. General Data Protection Regulation (GDPR)       
D. American Institute of Certified Public Accountants (AICPA)     
Answer: D. 

The American Institute of Certified Public Accountants publishes the SSAE 18 standard. NIST is a U.S. government entity that publishes many standards for federal agencies, so option A is incorrect. ENISA is a European Union (EU) standards body, so option B is incorrect. The GDPR is an EU law about privacy data, so option C is incorrect.

### Question # 130 - The current American Institute of Certified Public Accountants (AICPA) standard codifies certain audit reporting mechanisms. What are these called?      
A. Sarbanes-Oxley Act (SOX) reports      
B. Secure Sockets Layer (SSL) audits    
C. Sherwood Applied Business Structure Architecture (SABSA)     
D. System and Organization Controls (SOC) reports      
Answer: D.     

SOC reports are the audit reporting mechanisms dictated by SSAE 18. SOX is a federal law targeting publicly traded corporations in the United States. SSL is a way to conduct secure online transactions. SABSA is an architecture framework.

### Question # 131 - Which of the following is not a report used to assess the design and selection of security controls within an organization?     
A. Consensus Assessments Initiative Questionnaire (CAIQ)     
B. Cloud Security Alliance Cloud Controls Matrix (CSA CCM)    
C. SOC 1    
D. SOC 2 Type 1     
Answer: C.       

The SOC 1 audit report is not for security controls; it is for financial reporting controls. The AICPA SOC 2 Type 1 audit report reviews the controls an organization has selected and designed. Both the CAIQ and the CCM are tools created by the CSA to review an organization’s controls across several frameworks, regulations, and standards.

### Question # 132 - Which of the following is a report used to assess the implementation and effectiveness of security controls within an organization?      
A. SOC 1    
B. SOC 2 Type 1    
C. SOC 2 Type 2    
D. SOC 3    
Answer: C.      

The SOC 2 Type 2 reviews the implementation of security controls. The SOC 1 reviews financial reporting controls, not security controls. The SOC 2 Type 1 reviews the design and selection of security controls, not implementation. The SOC 3 is only an attestation of an audit, so option C is better.

### Question # 133 -  _______________ is an example of due care, and _______________ is an example of due diligence.     
A. Privacy data security policy; auditing the controls dictated by the privacy data security policy     
B. The European Union General Data Protection Regulation (GDPR); the Gramm-Leach-Bliley Act (GLBA)   
C. Locks on doors; turnstiles    
D. Perimeter defenses; internal defenses    
Answer: A. 

Due care is the minimal level of effort necessary to perform your duty to others; in cloud security, that is often the care that the cloud customer is required to demonstrate in order to protect the data it owns. Due diligence is any activity taken in support or furtherance of due care. This answer, then, is optimum: the due care is set out by the policy, and activities that support the policy (here, auditing the controls the policy requires) are a demonstration of due diligence.

The General Data Protection Regulation (GDPR) and GLBA are both legislative mandates; these might dictate a standard of due care, but they are not the due care or due diligence, specifically.

Door locks and turnstiles are physical security controls; they both might be examples of due care efforts, but neither demonstrates due diligence.

Due care and diligence can be demonstrated by either internal or external controls/

processes; there is no distinction to be made based on where the control is situated.

### Question # 134 - In a Lightweight Directory Access Protocol (LDAP) environment, each entry in a directory server is identified by a _______________.     
A. Domain name (DN)     
B. Distinguished name (DN)      
C. Directory name (DN)     
D. Default name (DN)     
Answer: B. 

The distinguished name (DN) is the nomenclature for all entries in an LDAP environment.

A domain name is used to identify one or more IP addresses. For instance, Microsoft.com and google.com are domain names. Option A is incorrect.

A directory name is typically associated with a file system structure and not something related to LDAP. Option C is incorrect.
“Default Name” is not a common term, and is made up. Option D is not the correct answer.

### Question # 135 - Each of the following is an element of the Identification phase of the identity and access management (IAM) process except _______________.    
A. Provisioning      
B. Inversion     
C. Management     
D. Deprovisioning     
Answer: B.      

Inversion is not part of the IAM process at all and has no meaning in this context. All the other options are elements of identification.

### Question # 136 - Which of the following is true about two-person integrity?      
A. It forces all employees to distrust one another.       
B. It requires two different identity and access management matrices (IAM).       
C. It forces collusion for unauthorized access.       
D. It enables more thieves to gain access to the facility.      
Answer: C.      

By creating a need for two identity assertions or authentication elements to access assets, two-person integrity prevents a single person from gaining unauthorized access and forces a would-be criminal to join up with at least one other person to conduct a crime. This reduces the possibility of the crime taking place.

All the other options are simply untrue and are therefore exceedingly poor choices for answers to CCSP test questions.

### Question # 137 - All of the following are statutory regulations except the _______________.       
A. Gramm-Leach-Bliley Act (GLBA)     
B. Health Information Portability and Accountability Act (HIPAA)     
C. Federal Information Systems Management Act (FISMA)     
D. Payment Card Industry Data Security Standard (PCI DSS)     
Answer: D.     

The PCI DSS is a voluntary standard, having only contractual obligation. All the other options are statutes, created by lawmaking bodies.

### Question # 138 - A cloud data encryption situation where the cloud customer retains control of the encryption keys and the cloud provider only processes and stores the data could be considered a _______________.      
A. Threat     
B. Risk      
C. Hybrid cloud deployment model      
D. Case of infringing on the rights of the provider     
Answer: C.      

Because the cloud customer will retain ownership of some elements of hardware, software, or both at the customer’s location (for instance, security hardware modules [HSMs]), client-side key management could be considered a hybrid cloud model.

Option A is incorrect because the scenario stated in the question does not identify a threat.

Option B is incorrect because the scenario stated in the question does not identify a risk. Allowing the customer to retain their own encryption keys is 
actually less risky than sharing their encryption keys with the provider.

Option D is incorrect because the provider does not have a right to the customer’s encryption keys, so, there cannot be an infringement on the provider’s rights.

### Question # 139 - Which of the following is one of the benefits of a private cloud deployment?     
A. Less cost       
B. Higher performance     
C. Retaining control of governance     
D. Reduction in need for maintenance capability on the customer side     
Answer: C.     

With a private cloud deployment, the customer gets to dictate governance requirements, which is a significant benefit for customers in highly regulated industries.

Private clouds typically cost more than public cloud deployments, so option A is incorrect.

Performance is not necessarily enhanced (or decreased) by any of the cloud deployment models, so option B is incorrect.

Retaining a higher degree of control over the cloud environment will necessarily require the cloud customer to have more maintenance capability, not less, so option D is incorrect.

### Question # 140 - What are the two general delivery modes for the software as a service (SaaS) model?     
A. Ranked and free      
B. Hosted application management and software on demand      
C. Intrinsic motivation complex and undulating perspective details    
D. Framed and modular   
Answer: B.      

In SaaS, the cloud provider might license and deliver commercially available software for the customer, via the cloud (hosted application management), or provide the customer access to the provider’s proprietary software (software on demand).

All the other options are incorrect. The options contain legitimate words put together to form gibberish.

### Question # 141 - Your organization has migrated into a platform as a service (PaaS) configuration. A network administrator within the cloud provider has accessed your data and sold a list of your users to a competitor. Who is required to make data breach notifications in accordance with all applicable laws?     
A. The network admin responsible      
B. The cloud provider       
C. The regulators overseeing your deployment      
D. Your organization     
Answer: D.    

The cloud customer is ultimately responsible for all legal repercussions involving data security and privacy; the cloud provider might be liable for financial costs related to these responsibilities, but those damages can only be recovered long after the notifications have been made by the cloud customer.
All the other options are incorrect because they do not correctly identify who is required to make data breach notifications in accordance with all applicable laws. That responsibility rests with the cloud customer.

### Question # 142 - If an organization wants to retain the most control of their assets in the cloud, which service and deployment model combination should they choose?      
A. Platform as a service (PaaS), community     
B. Infrastructure as a service (IaaS), hybrid     
C. Software as a service (SaaS), public    
D. Infrastructure as a service (IaaS), private    
Answer: D.     

An IaaS service model allows an organization to retain the most control of their IT assets in the cloud; the cloud customer is responsible for the operating system, the applications, and the data in the cloud. The private cloud model allows the organization to retain the greatest degree of governance control in the cloud; all the other deployment models would necessitate giving up governance control in an environment with pooled resources.

### Question # 143 - If an organization wants to realize the most cost savings by reducing administrative overhead, which service and deployment model combination should they choose?     
A. Platform as a service (PaaS), community     
B. Infrastructure as a service (IaaS), hybrid     
C. Software as a service (SaaS), public    
D. Infrastructure as a service (IaaS), private   
Answer: C. 

With SaaS, the cloud customer is responsible only for the data in the cloud; the cloud provider is responsible for the underlying IT infrastructure, the operating system, and the applications; maintenance for this service model will be minimal, compared to the others. A public cloud deployment will reduce costs even more, as it is the least expensive of the options—with the least amount of control for the cloud customer.

All the other options would include some degree of administration of the cloud resources on the part of the cloud customer and so are not as optimal as option C.

