Chapter 2: Domain 2—Cloud Data Security
In Domain 2, the exam outline focuses on the data owned by the cloud customer, hosted in the cloud. The domain discusses methods for securing the data, including specific tools and techniques.

### Question # 1 - In which of these options does the encryption engine reside within the application accessing the database?    
A. Transparent encryption    
B. Symmetric-key encryption    
C. Application-level encryption     
D. Homomorphic encryption      
Answer: C. 

In application-level encryption, the application will encrypt data before it is placed in the database. 
In transparent encryption, the entire database is encrypted. 
Symmetric-key encryption is a kind of encryption and not truly indicative of a strategy used in database encryption. 
[important] **Homomorphic encryption is an experimental, theoretical process that might allow processing encrypted information without the need to decrypt it first**.

### Question # 2 - You are the security team leader for an organization that has an infrastructure as a service (IaaS) production environment hosted by a cloud provider. You want to implement an event monitoring (security information and event management [SIEM]/security information management [SIM]/security event management [SEM]) solution in your production environment in order to acquire better data for security defenses and decisions. Which of the following is probably your most significant concern about implementing this solution in the cloud?     
A. The solution should give you better analysis capability by automating a great deal of the associated tasks.    
B. Dashboards produced by the tool are a flawless management benefit.     
C. You will have to coordinate with the cloud provider to ensure that the tool is acceptable and functioning properly.     
D. Senior management will be required to approve the acquisition and implementation of the tool.     
Answer:  

Because the tool will require at least some installation and reporting capability within the cloud environment, it is essential to coordinate with the cloud provider to ensure that the solution you choose will function properly and is allowed by the provider. 
Option A is true, but not a major concern; that is a benefit of SIEM/SEM/SIM tools. 
Option B is not true because dashboards can often misconstrue pertinent reporting data when they are used to chase management goals instead of distilling raw data appropriately. 
Option D is not true because management should not be involved in such granular decisions.

### Question # 3 - Which of the following is not a step in the crypto-shredding process?     
A. Encrypt data with a particular encryption engine.     
B. Encrypt first resulting keys with another encryption engine.     
C. Save backup of second resulting keys.     
D. Destroy original second resulting keys.     
Answer: C.      

**In crypto-shredding, the purpose is to make the data unrecoverable; saving a backup of the keys would attenuate that outcome because the keys would still exist for the purpose of recovering data**. 
All other steps outline the crypto-shredding process.

### Question # 4 - Which of the following sanitization methods is feasible for use in the cloud?     
A. Crypto-shredding     
B. Degaussing     
C. Physical destruction     
D. Overwriting     
Answer: A.      

**Cloud customers are allowed to encrypt their own data and manage their own keys; crypto-shredding is therefore possible.** 
**Degaussing** is not likely in the cloud **because it requires physical access** to the storage devices and because most cloud providers are using solid-state drives (SSDs) for storage, which are not magnetic. 
Physical destruction is not feasible because the cloud customer doesn’t own the hardware and therefore won’t be allowed to destroy it. 
Overwriting probably won’t work because finding all data in all aspects of the cloud is difficult and the data is constantly being backed up and securely stored, so a thorough process would be very tricky.

### Question # 5 - Which of the following is not a method for enhancing data portability?     
A. Crypto-shredding     
B. Using standard data formats     
C. Avoiding proprietary services     
D. Favorable contract terms      
Answer: A.      

**Crypto-shredding is for secure sanitization**, not portability. The other methods all enhance portability.

### Question # 6 - When implementing a digital rights management (DRM) solution in a cloud environment, which of the following does not pose an additional challenge for the cloud customer?     
A. Users might be required to install a DRM agent on their local devices.     
B. DRM solutions might have difficulty interfacing with multiple different operating systems and services.     
C. DRM solutions might have difficulty interacting with virtualized instances.     
D. Ownership of intellectual property might be difficult to ascertain.      
Answer: D.       

**The owner of intellectual property will not change whether the material is stored in the cloud or in a legacy environment**. 
Moving into the cloud will probably result in more use of personal devices, requiring users to install local DRM agents, so option A is true, making it not a suitable answer to this question. 
Options B and C are also true, due to the nature of cloud computing, and are therefore also not suitable for this question.

### Question # 6.1 - Which of the following BEST describes Digital Rights Management (DRM) in a cloud environment?       
A. Controlling where data is stored and encrypted across multiple providers                    
B. Restricting how digital assets (documents, media, data) can be used, copied, or shared          
C. Enforcing firewall rules for cloud-hosted applications           
D. Tracking user activity for regulatory compliance          
Answer: B

**DRM focuses on usage control of data (view, print, copy, forward), not just storage or firewalls**.

### Question # 6.2 - Which of the following is NOT a common function of DRM/IRM solutions?
A. Preventing unauthorized copying of data
B. Controlling printing or screenshotting of files
C. Encrypting content with persistent protection
D. Optimizing data compression for cloud storage efficiency
Answer: D

**👉 Compression has nothing to do with DRM.**

### Question # 6.3 - What is the main difference between DRM and traditional encryption?
A. DRM protects data only when in transit, encryption protects at rest.
B. Encryption prevents access without a key, DRM enforces usage restrictions even after decryption.
C. DRM requires asymmetric keys, encryption only uses symmetric keys.
D. Encryption protects against malware, DRM protects against hackers.
Answer: B

**DRM ensures persistent control even after a file is decrypted (e.g., no printing, no forwarding).**

### Question # 6.4 - An organization shares a sensitive report with a partner. They want to allow reading but block downloading or printing. Which control is most appropriate?
A. Access Control List (ACL)
B. Digital Rights Management (DRM)
C. File Integrity Monitoring (FIM)
D. Public Key Infrastructure (PKI)
Answer: B

**DRM enforces usage policies beyond access control.**

### Question # 6.5 - Which of the following could weaken DRM protections in a cloud setting?
A. Users accessing files via secured viewers only
B. Screenshots or screen-recording tools bypassing controls
C. Applying persistent encryption with keys stored externally
D. Using identity-based access enforcement
Answer: B

**👉 Screenshots and side-channel methods are known DRM bypass challenges.**

### Question # 6.6 - In a cloud DRM/IRM solution, the policy server is responsible for:
A. Deciding where encrypted data is physically stored
B. Defining and enforcing access and usage policies for digital content
C. Conducting vulnerability scans on hosted applications
D. Monitoring system availability and uptime
Answer: B

**👉 Policy servers decide who can do what with the file.**

### Question # 6.7 - Which of the following industries is most regulated and heavily reliant on DRM/IRM solutions for sensitive data handling?
A. Media and entertainment
B. Financial services
C. Healthcare
D. All of the above
Answer: D

👉 Media uses DRM for piracy, finance for compliance, healthcare for HIPAA/PHI protection.

### Question # 6.8 - Which is a limitation of DRM in enterprise use?
A. Can’t protect against unauthorized use after decryption
B. May cause usability issues and impact collaboration
C. Doesn’t integrate with access controls
D. Provides no encryption support
Answer: B

**👉 DRM can frustrate users and reduce productivity if policies are too strict**.

### Question # 6.9 - In the cloud, DRM is often integrated with:
A. Identity and Access Management (IAM)
B. Key Management Systems (KMS)
C. Cloud Access Security Brokers (CASB)
D. All of the above
Answer: D

**👉 DRM works hand-in-hand with IAM, KMS, and CASB for holistic cloud data security.**

### [important] Question # 6.10 - Which of the following best describes persistent protection in DRM?
A. Protecting data while at rest
B. Protecting data only during transmission
C. Ensuring policies remain enforced regardless of where data travels
D. Ensuring files are deleted after use
Answer: C

**👉 DRM travels with the file — so policies are enforced even after it leaves the enterprise boundary**.

### Question # 7 - When implementing cryptography in a cloud environment, where is the worst place to store the keys?      
A. With the cloud provider     
B. Off the cloud, with the data owner     
C. With a third-party provider, in key escrow      
D. Anywhere but with the cloud provider       
Answer: A.       

Option A creates a conflict of interest and does not enforce separation of duties.
The best practice is to not store cryptographic keys with the data they encrypt, to avoid a potential conflict of interest and to enforce separation of duties. 
Each of the other choices is a reasonable choice and therefore not the answer to this question.

### Question # 8 - Which of the following is not a security concern related to archiving data for long-term storage?     
A. Long-term storage of the related cryptographic keys     
B. Format of the data     
C. Media the data resides on      
D. Underground depth of the storage facility      
Answer: D.     

A long-term storage facility may or may not be located underground; the security of that facility (and the data contained therein) is not dependent on this aspect. 
**Option A is a security concern because loss of the keys may result in losing the data (by losing access to the data), and keeping the keys with the data they protect increases risk**. 
Both the format of the data and the media on which it resides (options B and C) are important to bear in mind, as either (or both) may be outmoded by the time the data might need to be retrieved from the archive; data and formats do not age well.

### [important] Question # 9 - Data dispersion is a cloud data security technique that is most similar to which legacy implementation?      
A. Business continuity and disaster recovery (BC/DR)    
B. Redundant Array of Inexpensive Disks (RAID)     
C. Software-defined networking (SDN)     
D. Content delivery network (CDN)    
Answer: B.      

**Data dispersion is basically RAID in the cloud**, 
with data elements parsed and stored over several areas/devices instead of stored as a unit in a single place. 
RAID (and data dispersion) does aid in BC/DR activities by increasing the robustness and resiliency of stored data, but BC/DR is a much more general discipline, so it is not the optimum answer for the question. SDN is used for abstracting network control commands away from production data, and CDN is usually used for ensuring quality of streaming media.

### [important] Question # 10 - Data dispersion uses _______________, where the traditional implementation is called “striping.”      
A. Chunking     
B. Vaulting     
C. Lumping     
D. Grouping     
Answer: A. 

[important] **Where RAID used data striping across multiple drives, with data dispersion this technique is referred to as “chunking,” or sometimes “sharding” when encryption is also used**. 
The other options are not common data dispersion terms used in cloud computing and have no meaning in this context.

### [important] Question # 11 - Data dispersion uses _______________, where the traditional implementation is called “parity bits.”       
A. Smurfing   
B. Snarfing   
C. Erasure coding    
D. Real-time bitlinking     
Answer: C.     

[important] **Erasure coding is the practice of having sufficient data to replace a lost chunk in data dispersion, protecting against the possibility of a device failing while it holds a given chunk**; 
**parity bits serve the same purpose in a traditional RAID configuration**. 
The other options are not common data dispersion terms used in cloud computing and have no meaning in this context.

### Question # 12 - Data dispersion provides protection for all the following security aspects except _______________.    
A. Protecting confidentiality against external attack on the storage area   
B. Loss of availability due to single-storage-device failure    
C. Loss due to seizure by law enforcement in a multitenant environment   
D. Protecting against loss due to user error    
Answer: D.     

Data dispersion can’t aid in inadvertent loss caused by an errant user; if the user accidentally deletes/corrupts a file, that file will be deleted/corrupted across all the storage spaces where it is dispersed. 
The technique does, however, protect against the other risks. 
It enhances confidentiality because an attacker gaining illicit access to a single storage space will only get a chunk of the data, which is useless without the other chunks. This same aspect also protects loss when law enforcement seizes a specific storage device/space when they are investigating another tenant at the same cloud provider your organization uses. And loss of availability due to single device failure is probably the primary reason for having data dispersion (like RAID before it).

### Question # 13 - Your organization is migrating the production environment to an infrastructure as a service (IaaS) cloud implementation. Your users will need to be able to get access to their data, install programs, and partition memory space for their own purposes. You should configure the cloud memory as _______________.    
A. Object   
B. Volume   
C. Synthetic   
D. Database   
Answer: B.    

Volume storage allows all the functions described in the question. 
**Object storage has data arranged in a file structure,** 
and **databases arrange data in tables and relational schemes**; 
neither of these options offers the functions described in the question. 
Synthetic is not a cloud memory configuration option.

### Question # 14 - Your organization is migrating the production environment to an infrastructure as a service (IaaS) cloud implementation. Your users will need to be able to get access to their data and share data with other users in a defined way, according to a hierarchy. You should configure the cloud memory as _______________.    
A. Object storage   
B. Volume storage   
C. Synthetic storage   
D. Databases   
Answer: A.    

Object storage is usually arranged in a file hierarchy. 
Volume storage has data with no defined structure (only memory space), and databases ar-range data in tables and relational schemes; neither of these options offers the functions described in the question. Synthetic is not a cloud memory con-figuration option.

### Question # 15 - What is one of the benefits of implementing an egress monitoring solution?    
A. Preventing distributed denial of service (DDoS) attacks    
B. Inventorying data assets    
C. Interviewing data owners    
D. Protecting against natural disasters    
Answer: B.     

Egress monitoring solutions (often referred to as DLP tools, where DLP stands for data loss protection or data leak prevention, or some combination of these terms) require the organization to appropriately inventory and classify data assets so the tool knows what to protect. 
DLP does not aid in protections for DDoS or natural disasters, which affect availability, not confidentiality (DLP only enhances confidentiality efforts). 
Option C is not a benefit of implementing an egress monitoring solution.

### Question # 16 - Egress monitoring solutions usually include a function that _______________.    
A. Arbitrates contract breaches    
B. Performs personnel evaluation reviews    
C. Discovers data assets according to classification/categorization     
D. Applies another level of access control     
Answer: C. 

Egress monitoring solutions (often referred to as DLP tools, where DLP stands for data loss protection or data leak prevention, or some combination of these terms) will often include a discovery function, which will locate data assets according to criteria defined by the organization. 
DLP solutions cannot arbitrate contract breaches or perform personnel evaluations. 
Usually, DLPs also do not apply additional access controls; that is typically a characteristic of a digital rights management (DRM) solution.

### [important] Question # 17 - Egress monitoring solutions usually include a function that _______________.     
A. Uses biometrics to scan users     
B. Inspects incoming packets   
C. Resides on client machines     
D. Uses stateful inspection     
Answer: C. 

Egress monitoring solutions (often referred to as DLP tools, where DLP stands for data loss protection or data leak prevention, or some combination of these terms) **will often include an agent that resides on client devices in order to inspect data being shared/sent by end users**. 
DLP tools do not inspect incoming packets, with or without stateful inspection; this is the job of firewalls. 
DLP solutions do not typically use biometrics in any way.

### Question # 18 - Digital rights management (DRM) solutions (sometimes referred to as information rights management, or IRM) can be used to protect all sorts of sensitive data but are usually particularly designed to secure ____________.     
A. Personally identifiable information (PII)    
B. Intellectual property     
C. Plans and policies    
D. Marketing material     
Answer: B. 
  
**DRM is mainly designed to protect intellectual property**. 
**It can also sometimes be used for securing PII**, but intellectual property is a better answer here. 
Plans and policies aren’t usually protected in this manner, and marketing material is usually meant to be disseminated, so it does not require protection.

### [important] Question # 19 - Digital rights management (DRM) solutions (sometimes referred to as information rights management, or IRM) often protect unauthorized distribution of what type of intellectual property?     
A. Patents     
B. Trademarks     
C. Personally identifiable information (PII)      
D. Copyright      
Answer: D. 

DRM is often deployed to **ensure that copyrighted material (frequently software) is only delivered to and used by licensed recipients**. 
**Patents are more complicated and not often distributed to a mass market, so DRM does not assist in that way**. 
**Trademarks are representations of a brand and meant to be distributed, so DRM does not protect them**. 
[important] **PII is not typically a type of intellectual property**.

### Question # 20 - Which of the following characteristics is associated with digital rights management (DRM) solutions (sometimes referred to as information rights management, or IRM)?      
A. Persistence     
B. Influence     
C. Resistance     
D. Trepidation    
Answer:A.      

**Persistence is the trait that allows DRM protection to follow protected files wherever they might be stored/copied**. 
The other options are not characteristics associated with DRM solutions.

### [important] Question # 21 - Which of the following characteristics is associated with digital rights management (DRM) solutions (sometimes referred to as information rights management, or IRM)?     
A. Automatic expiration    
B. Multilevel aggregation    
C. Enhanced detail    
D. Broad spectrum    
Answer: A.     

Automatic expiration is the trait that allows DRM tools to prevent access to objects when a license expires or to remove protections when intellectual property moves into the public domain. 
The other options are not characteristics associated with DRM solutions.

### [important] Question # 22 - Which of the following characteristics is associated with digital rights management (DRM) solutions (sometimes referred to as information rights management, or IRM)?    
A. Transparent encryption modification    
B. Bilateral enhancement    
C. Continuous audit trail     
D. Encompassing flow    
Answer: C.     

**Continuous audit trail is the trait that allows DRM tools to log and exhibit all access to a given object.** 
The other options are not characteristics associated with DRM solutions.

### Question # 23 - Which of the following characteristics is associated with digital rights management (DRM) solutions (sometimes referred to as information rights management, or IRM)?    
A. Mapping to existing access control lists (ACLs)   
B. Delineating biometric catalogs   
C. Preventing multifactor authentication    
D. Prohibiting unauthorized transposition    
Answer: A.     

**Mapping to existing access control lists (ACLs) is the trait that allows DRM tools to provide additional access control protections for the organization’s assets**. 
The other options are not characteristics associated with DRM solutions.

### Question # 24 - According to the (ISC)2 Cloud Secure Data Lifecycle, which phase comes soon after (or at the same time as) the Create phase?     
A. Store   
B. Use   
C. Deploy   
D. Archive   
Answer: A.    

The Cloud Secure Data Lifecycle phases are, in order, **Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD)**.
Options B and D are phases of CSU-SAD but do not immediately follow Create.
Option C is not a phase of CSU-SAD.

### Question # 25 - According to the (ISC)2 Cloud Secure Data Lifecycle, which phase comes immediately before the Share phase?    
A. Create   
B. Destroy   
C. Use   
D. Encrypt    
Answer: C.     

The Cloud Secure Data Lifecycle phases are, in order, **Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD)**.
Options A and B are phases of CSU-SAD but do not immediately precede Share.
Option D is not a phase of CSU-SAD.

### [important] Question # 26 - Why is the term (ISC)2 Cloud Secure Data Lifecycle actually somewhat inaccurate?    
A. The term is not used only by (ISC)2.   
B. Not all phases are secure.   
C. Not all phases take place in the cloud.    
D. It’s not actually a cycle.     
Answer: D. 

The Cloud Secure Data Lifecycle phases are, in order, Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD). 
This is not truly a cycle **because data does not continue after the destroy phase** (that is to say, the same data or process does not go back to create after destroy).
Option A might be considered true because the CSU-SAD cycle is not unique to (ISC)2, but this is not the best answer; option D is preferable because it is not truly a cycle.
Options B and C are incorrect because activity in each of the phases involves security aspects and all phases relate to how data is involved in the cloud.

### Question # 27 - According to the (ISC)2 Cloud Secure Data Lifecycle, in which phase should the process of categorization/classification of data occur?    
A. Create   
B. Store   
C. Define  
D. Use   
Answer: A.     

The Cloud Secure Data Lifecycle phases are, in order, Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD). The best practice for categorizing/classifying data is to do so when it is first created/collected so that the proper security controls can be applied to it throughout the rest of the cycle.
Options B and D are phases of the CSU-SAD but are not the proper times to be applying classification/categorization; that would be too late in the cycle.
Option C is not a phase of CSU-SAD.

### [important] Question # 28 - Which of the following should occur during the final phase of the Cloud Secure Data Lifecycle?    
A. Data dispersion   
B. Crypto-shredding   
C. Cryptoparsing   
D. Cryptosporidium  
Answer: B. 

**The Cloud Secure Data Lifecycle phases are, in order, Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD). Crypto-shredding (also called cryptographic erasure) is the preferred method of data sanitization for a cloud environment; this should take place in the final phase of the cycle, destroy**.

Option A is incorrect because data dispersion is a means of making data more resilient and secure; in the final phase of the cycle, we want to get rid of the data, not make it resistant to loss.

Option C is incorrect because cryptoparsing is a made-up term and used here as a distractor.
Option D is incorrect because cryptosporidium is a microorganism and is not associated with InfoSec.

### Question # 29 - At what phase of the Cloud Secure Data Lifecycle does data enter long-term storage?    
A. The first    
B. The second    
C. The fourth    
D. The fifth   
Answer: D.     

The Cloud Secure Data Lifecycle phases are, in order, Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD). Archiving (the fifth phase) is the process of moving data out of the production environment and into long-term storage.
The other phases in the options are create, store, and share and are therefore incorrect.

### Question # 30 - What is a form of cloud storage where data is stored as objects, arranged in a hierarchal structure, like a file tree?    
A. Volume storage    
B. Databases   
C. Content delivery network (CDN)    
D. Object storage    
Answer: D.     

Object storage stores data as objects (hence the name), often arranged in a hierarchical structure.
Volume storage is not a hierarchal cloud storage structure and is therefore an incorrect answer for this question.
Option B is incorrect because databases are applications in both traditional and cloud computing.
A CDN is a geographically distributed network of proxy servers and their data centers. Option C is incorrect because it is not a form of cloud storage.

### Question # 31 - What is a form of cloud storage where data is stored in a logical storage area assigned to the user but not necessarily physically attached or even geographically proximate to the compute node the user is utilizing?    
A. Volume storage    
B. Databases    
C. Content delivery network (CDN)    
D. Object storage     
Answer: A. 

In volume storage, the user is assigned a logical drive space into which anything (such as raw data, objects, or applications) may be saved or installed, similar to a mounted drive on a traditional network.
Databases store data in an arrangement of characteristics and values, not in an unstructured drive space, so option B is incorrect.
CDNs are for distributing data with less chance of quality loss, so option C is incorrect.
Object storage arranges data as objects in a structured hierarchy, so option D is incorrect.

### Question # 32 - What is a form of cloud storage often used for streaming multimedia data to users?     
A. Volume storage    
B. Databases    
C. Content delivery network (CDN)    
D. Neutral storage    
Answer: C.       

**CDNs are often used to place large stores of multimedia data in a location geographically near to the end users who will consume that data; this approach is designed mostly to accomplish a reduction in data degradation due to distance between resource and user**.
Volume storage assigns a logical, unstructured drive space to the user, so option A is incorrect.
Databases store data in an arrangement of characteristics and values, so option B is incorrect.
Neutral storage is not a form of cloud storage, so option D is incorrect.

### [tricky & important] Question # 33 - What type of data storage is often used in platform as a service (PaaS) arrangements?    
A. Ephemeral    
B. Database    
C. Long-term   
D. Nefarious    
Answer: B.     

**The PaaS model allows the cloud customer to install and run applications in the cloud environment**. 
**With a database, the cloud customer can store data in a database administered by the cloud provider but can then tailor applications and services for reaching into and manipulating that database**.
Ephemeral and long-term storage take place in the software as a service (SaaS) model, and there is no such thing as “nefarious data storage,” so the other options are incorrect.

### Question # 34 - What is a form of cloud data protection where data is spread across multiple storage devices/locations, similar to RAID in the legacy environment?    
A. Infringing    
B. Data dispersion    
C. Voiding    
D. Crypto-shredding     
Answer: B. 

**Data dispersion is the cloud version of using RAID arrays, protecting data by spreading it across multiple volumes/devices**.
Options A and C are terms that have no meaning in this context.
Crypto-shredding is a form of device/media sanitization utilizing cryptography and has nothing to do with RAID, so option D is incorrect.

### Question # 35 - Erasure coding, in the cloud, is similar to what element of RAID implementations in a traditional IT environment?    
A. Deltas    
B. Inversion    
C. Parity bits     
D. Transposition     
Answer: C.      

**Similar to parity bits in RAID, erasure coding is used in cloud data dispersion implementations to create a situation where data can still be recovered even if a segment or portion of the dispersed data is lost (due to drive failure, disaster, etc.)**.
Options A and B have no meaning in this context.
Transposition is a cryptographic technique and does not relate to RAID in any way, so option D is also incorrect.

### Question # 36 - DLP (data loss prevention or data leak protection) solutions are implemented in the hopes of securing _______________.     
A. Sensitive data that may leave the organization’s control    
B. All data within the organization’s control   
C. Data being processed by the organization’s users    
D. Data that could be intercepted while out of the organization’s control    
Answer: A. 

**DLP, also referred to as egress monitoring, is used to detect and prevent sensitive data from leaving the organization’s control without proper approval**.
Because it is designed to prevent the egress of only certain data sets, options B and C are not correct.
Controlling data outside the reach of the organization is difficult at best. While there are some mechanisms that might accomplish this, DLP is not specifically designed for that purpose, so option D is incorrect.

### [important] Question # 37 - Which of the following will DLP (data loss prevention or data leak protection) solutions most likely not inspect?     
A. Email content   
B. FTP traffic   
C. Material saved to portable media    
D. Voice over Internet Protocol (VoIP) conversations      
Answer: D. 

Commercial DLP products that monitor speech in real time and censor conversations are not yet widely available.
A proper DLP solution will monitor all the technologies in the other options, so those are incorrect.

### [important] Question # 38 - DLP (data loss prevention or data leak protection) solutions may use all of the following techniques to identify sensitive data except _______________.      
A. Pattern matching     
B. Inference    
C. Keyword identification    
D. Metadata tags    
Answer: B.      

**Inference is an attack technique that derives sensitive material from an aggregation of innocuous data; DLP tools, thus far, do not have this capability**.
All the other techniques listed may be used by DLP solutions to detect sensitive data before it leaves the control of the owner.

### [very important] Question # 39 - You are the security manager of a small firm that has just purchased an egress monitoring solution to implement in your cloud-based production environment. In which of the following cases would you not have to get permission from the cloud provider to install and implement the tool?     
A. If it’s hardware-based and your production environment is in an infrastructure as a service (IaaS) model   
B. If you purchased it from a vendor other than the cloud provider    
C. If it’s software-based and your production environment is in a platform as a service (PaaS) model     
D. If it affects all guest instances on any given host device     
Answer: C. 

[very important] **A cloud customer can install applications on a PaaS environment, usually as they see fit and without prior coordination with the provider.**
If you are introducing hardware into the cloud environment, you will need permission from your cloud provider, regardless of the deployment model you use. Therefore, option A is incorrect (and unlikely to occur, as permission is probably not going to be granted).
Although the provider may offer an egress monitoring function as an add-on service, which would be permissible for you to use, the use of an outside vendor’s product may have to be reviewed by the provider before implementation, based on a number of other variables (such as the other possible answers). Option C is preferable, so option B is incorrect.
Affecting all images on a host may impact other customers in a multitenant environment, so option D is not the correct answer.

### Question # 40 - You are the security manager of a small firm that has just purchased an egress monitoring solution to implement in your cloud-based production environment. Before implementing the solution, what should you explain to senior management?    
A. The additional risks of external attack associated with using the tool     
B. The production impact it will have on the environment     
C. What the price of the tool was      
D. How the solution works      
Answer: B.      

[important] **All security functions come with an attendant negative productivity effect: 
the most secure environment will be the least productive, and the most productive will be the least secure. 
Egress monitoring tools will have an overhead cost in terms of production impact and loss of efficiency and speed**. 
This may affect the cost savings that were realized in a cloud migration from the legacy environment, and senior management needs to understand this trade-off.
Implementing an egress monitoring solution should not incur any additional risks of external attack, so option A is incorrect.
Because the tool has already been purchased, explaining the purchase price is irrelevant at this point, so option C is incorrect.
If it was germane (and it was likely not), you should have explained how the tool works before purchasing it; explaining at this point might be interesting but is not as important as option B, so option D is incorrect.

### Question # 41 - You are the security manager of a small firm that has just purchased an egress monitoring solution to implement in your cloud-based production environment. Which of these activities should you perform before deploying the tool?    
A. Survey your company’s departments about the data under their control.     
B. Reconstruct your firewalls.     
C. Harden all your routers.      
D. Adjust the hypervisors.     
Answer: A.      

In order to “train” the egress monitoring solution properly, you’ll need to inform it as to which data in your organization is sensitive…and, in order to do that, you’ll need to determine what information your data owners deem sensitive; a survey is a way to do that.
A proper egress monitoring solution should not affect or be affected by the firewalls, routers, or hypervisors, so options B, C, and D are incorrect.

### [important] Question # 42 - You are the security manager of a small firm that has just purchased an egress monitoring solution to implement in your cloud-based production environment. What should you expect immediately following the implementation of the tool?    
A. Immediate decrease in lost data    
B. A series of false-positive indications    
C. Increase in morale across the organization     
D. Increase in gross revenue     
Answer: B.     

**It will take a while for the tool to “learn” the particulars of your environment and to be conditioned properly.** 
A significant number of false-positive indications will be expected in the near term, until you can hone the responses to properly meet your organization’s needs.
The tool will not work optimally immediately upon implementation, so option A is incorrect.
Egress monitoring tools do not affect morale or revenues, so options C and D are incorrect.

### Question # 43 - You are the security manager of a small firm that has just purchased an egress monitoring solution to implement in your cloud-based production environment. What should you not expect the tool to address?     
A. Sensitive data sent inadvertently in user emails     
B. Sensitive data captured by screenshots    
C. Sensitive data moved to external devices    
D. Sensitive data in the contents of files sent via File Transfer Protocol (FTP)      
Answer: B. 

It’s unlikely that any egress monitoring tools will be able to detect sensitive data captured, stored, and/or sent as graphic image files, which is the usual form of screenshots.
A proper egress monitoring tool should be able to detect all the other types of activity, so the other options are incorrect.

### [tricky and important] Question # 44 - You are the security manager of a small firm that has just purchased an egress monitoring solution to implement in your cloud-based production environment. In order to get truly holistic coverage of your environment, you should be sure to include ____________ as a step in the deployment process.     
A. Getting signed user agreements from all users    
B. Installation of the solution on all assets in the cloud data center    
C. Adoption of the tool in all routers between your users and the cloud provider     
D. Ensuring that all your customers install the tool     
Answer: A.      

This is a tricky question. In the cloud environment, we know that all users will be entering the environment through remote access; in many cases, this will include the use of their personal devices. 
In order for egress monitoring solutions to function properly, all devices accessing the production environment must have local agents installed, and that requires signed user agreements.

It would be unnecessary (and intrusive, and cumbersome) to install agents on all assets in the cloud data center, which includes not only your organization’s assets but also those of all the other cloud tenants in that data center. This might even be illegal. Option B is incorrect.
Assuming you could install (or even know) all the routers between your users and the cloud data center is ridiculous; option C is incorrect.
Getting your customer to install an egress monitoring client would be nice, in theory…but also pointless. Your customers don’t work for you; they are outside your organization. Egress monitoring tools are used to prevent sensitive data from leaving your environment; by the time it has reached a customer, sensitive information is far outside your control and the egress monitoring tool would be of no use. Option D is therefore incorrect.

### Question # 45 - You are the security manager of a small firm that has just purchased an egress monitoring solution to implement in your cloud-based production environment. In order to increase the security value of the tool, you should consider combining it with _______________.     
A. Digital rights management (DRM) and security event and incident management (SIEM) tools     
B. An investment in upgraded project management software      
C. Digital insurance policies     
D. The Uptime Institute’s Tier certification     
Answer: A. 

**Egress monitoring tools combined with DRM and SIEM enhance the security value of each because you create in-depth/layered defense**.    
Project management software does not really have anything to do with security, so option B is incorrect.      
Insurance is a risk transfer mechanism and does not aid in risk mitigation efforts; egress monitoring is for risk mitigation, so option C is incorrect.      
The Tier certification program is for the cloud provider and is not used by the cloud customer, so option D is incorrect.      

### [important] Question # 46 - You are the security manager of a small firm that has just purchased an egress monitoring solution to implement in your cloud-based production environment. You are interested in fielding the solution as an awareness tool to optimize security for your organization through conditioning user behavior. You decide to set the solution to _______________.         
A. Suspend user accounts and notify the security office when it detects possible sensitive data egress attempted by a user          
B. Halt the transaction and notify the user’s supervisor when the user attempts to transfer sensitive data     
C. Query the user as to whether they intend to send sensitive data upon detection of an attempted transfer     
D. Sever remote connections upon detection of a possible sensitive data transfer     
Answer: C. 

These are all possible settings for a modern egress monitoring solution. However, the best option, in light of the question, is to query the user as to their intent; this aids the user in understanding and knowing when sensitive data might be leaving the organization accidentally, through a mistake on the user’s part. The other options are more severe and restrictive; these will enhance security but reduce productivity and are management and technological controls instead of awareness tools, so they are incorrect answers for this question.

### [important] Question # 47 - You are the security manager of a small firm that has just purchased an egress monitoring solution to implement in your cloud-based production environment. You understand that all of the following aspects of cloud computing may make proper deployment of the tool difficult or costly except _______________.    
A. Data will not remain in one place or form in the cloud     
B. The cloud environment will include redundant and resilient architecture    
C. There will be a deleterious impact on production upon installing the tool   
D. You might not have sufficient proper administrative rights in the cloud infrastructure    
Answer: B.       

The fact that cloud data centers are designed with multiple redundancies of all systems and components won’t really have any bearing on your decision and implementation of your egress monitoring solution.
Because data will move across nodes in the data center and will take different forms (such as live data in a virtualized instance or snapshotted data saved in a file store when a virtual machine is not being used at a specific moment), you will have to determine how the tool will function in that environment, and whether it was designed for cloud usage. Option A is incorrect.
Option C is true for any environment, not just the cloud; all security functions necessarily negatively impact operations and production. Option B is a better answer.
Option D is also correct; without administrative privileges to the underlying hardware (which customers should not have), the customer may not be able to install monitoring agents everywhere necessary for those tools to work properly.

### Question # 48 - Egress monitoring solutions can aid all of the following security-related efforts except _______________.    
A. Access control    
B. Data exfiltration     
C. E-discovery/forensics     
D. Data categorization/classification      
Answer: A.     

Egress monitoring solutions do not facilitate access control efforts in any way.
Egress monitoring tools do, however, provide all the functions listed in the other options, so those are incorrect.

### Question # 49 - The cloud security professional should be aware that encryption would most likely be necessary in all the following aspects of a cloud deployment except _______________.     
A. Data at rest    
B. Data in motion    
C. Data in use     
D. Data of relief    
Answer: D.     

The term data of relief doesn’t really mean anything and is therefore the correct answer for this question.
Encryption is used in all other aspects of cloud data.

### Question # 50 - As with the traditional IT environment, cloud data encryption includes all the following elements except _______________.     
A. The user     
B. The data itself     
C. The encryption engine       
D. The encryption keys    
Answer: A.      

The user is not really an aspect of an encryption deployment, although it may be argued that the user will need to refrain from disclosing their own key(s) to anyone else.
The other three options are the components of an encryption deployment.

### Question # 51 - Volume storage encryption in an infrastructure as a service (IaaS) arrangement will protect against data loss due to all of the following activities except _______________.     
A. Physical loss or theft of a device     
B. Disgruntled users     
C. Malicious cloud administrators accessing the data     
D. Virtual machine snapshots stolen from storage     
Answer: B.      

An authorized user will still be able to access and decrypt the data for which they’ve been granted permissions, so encryption will not offer any protections for that threat.
Volume storage encryption will, however, protect against all the other threats, because any outsider (that is, a person who does not have access to the volume operating system) will be able to steal only encrypted data, which they should not be able to decrypt in a timely fashion. Therefore, all the other options are incorrect.

### Question # 52 - In an infrastructure as a service (IaaS) arrangement, all of the following are examples of object storage encryption except _______________.     
A. File-level encryption    
B. Digital rights management (DRM)     
C. Application-level encryption     
D. Transport Layer Security (TLS)       
Answer: D. 

**TLS is encryption used in a communication session, not a storage volume.**
All the other options are examples of object storage encryption options, so they are incorrect.

### Question # 53 - All of the following are database encryption options that could be used in a platform as a service (PaaS) implementation except _______________.      
A. File-level encryption     
B. Secure Sockets Layer (SSL)      
C. Transparent encryption    
D. Application-level encryption    
Answer: B.     

**SSL is encryption used in a communication session, not a storage volume.**
All the other options are examples of database encryption options, so they are incorrect.

### [important] Question # 54 - In application-level encryption, where does the encryption engine reside?    
A. In the application accessing the database   
B. In the operating system on which the application is run    
C. Within the database accessed by the application    
D. In the volume where the database resides    
Answer: A. 

**The application contains the encryption engine used in application-level encryption.**
The operating system is responsible for providing the resources an application needs and for running the applications. The operating system does not do application-level encryption, so option B is incorrect.
Option C is incorrect because application-level encryption is performed by the application that interfaces with the database.
The application-level encryption engine may or may not reside in the same volume as the database engine, so option D is incorrect.

### [important] Question # 55 - Which of the following database encryption techniques can be used to encrypt specific tables within the database?    
A. File-level encryption    
B. Transparent encryption    
C. Application-level encryption     
D. Object-level encryption     
Answer: B. 

**Encrypting specific tables within the database is one of the options of transparent encryption;** this is not true of the other options, so they are incorrect.

### [important] Question # 56 - Which of the following database encryption techniques makes it difficult to perform database functions (searches, indexing, etc.)?     
A. File-level encryption    
B. Transparent encryption    
C. Application-level encryption     
D. Volume encryption      
Answer: C. 

[important] **Application-level encryption involves encrypting the data before it enters the fields of the database; it is much more difficult to search and review data that has been encrypted, so this reduces the functionality of the database**.
All the other options are incorrect because they are not database encryption techniques.

### [important] Question # 57 - According to (ISC)2, where should the cloud customer’s encryption keys be stored?     
A. With the cloud customer    
B. With a third-party provider     
C. At the cloud provider data center     
D. Anywhere but with the cloud provider       
Answer: D.      

Best practice is to not keep the encryption keys alongside the data they’ve been used to encrypt.
Options A and B are both viable but not as good as option D, which is more general and includes them both.
Option C is clearly incorrect because it is counter to the best practice advice offered by (ISC)2.

### Question # 58 - Which of the following is not used to determine data retention requirements?       
A. Legislation      
B. Business needs     
C. Average media longevity                  
D. Contracts     
Answer: C. 

Data retention periods should be established in policy regardless of the projected lifetime of the media the data resides on. 
All the other options do/should influence data retention periods.

### Question # 59 - Event monitoring tools (security information and event management [SIEM]/security information management [SIM]/security event management [SEM]) can aid in which of the following efforts?        
A. External hacking detection     
B. Prediction of physical device theft     
C. Data classification/categorization issues      
D. Social engineering attacks      
Answer: A. 

Event monitoring tools can help detect external hacking efforts by tracking and reporting on common hack-related activity, such as repeated failed login attempts and scanning. 

It is unlikely that these tools could predict physical device theft; they could, of course, report on a device that is no longer connected to the environment after it has been removed by noting a lack of event activity, but that’s not quite the same thing. Event monitoring tools don’t aid in data classification/categorization; egress monitoring and digital rights management tools might provide that function, though. Social engineering attacks are mostly transparent to the majority of logical tools (the exception being social engineering efforts combined with IT traffic, such as phishing, which might be detected by email filters and sophisticated firewalls).

### [important] Question # 60 - Event monitoring tools (security information and event management [SIEM]/security information management [SIM]/security event management [SEM]) can aid in which of the following efforts?     
A. Detecting untrained personnel    
B. Predicting system outages    
C. Sending alerts for conflicts of interest       
D. Enforcing mandatory vacation         
Answer: B.           

[important] **Event monitoring tools can be used to predict system outages by noting decreases in performance; repeated performance issues can be an indicator a device is failing**. 
While an event monitoring tool might be able to detect a user who continually conducts unproductive activity or fails to complete certain functions, it is impossible to determine if the source of the problem is lack of training. 
These tools in no way serve to detect conflict of interest or enforce mandatory vacation, which are managerial/administrative controls.

### Question # 61 - Event monitoring tools (security information and event management [SIEM]/security information management [SIM]/security event management [SEM]) can aid in which of the following efforts?    
A. Reducing workload for production personnel     
B. Decreasing size of log files     
C. Optimizing performance     
D. Ensuring adequate lighting of workspaces     
Answer: C. 

Event monitoring tools can detect repeated performance issues, which can be used by administrators and architects to enhance performance/productivity. These tools don’t aid in the managerial function of noting individual workload, nor do they reduce log file sizes (indeed, they might add to the size of log files) or have anything to do with lighting.

### Question # 62 - Event monitoring tools (security information and event management [SIEM]/security information management [SIM]/security event management [SEM]) can aid in which of the following efforts?     
A. Detecting ambient heating, ventilation, and air-conditioning (HVAC) problems           
B. Ensuring proper cloud migration     
C. Deciding risk parameters     
D. Protecting all physical entry points against the threat of fire       
Answer: A. 

Event monitoring tools can detect repeated performance issues, which can be indicative of improper temperature settings in the data center; also, some system monitoring metrics, such as CPU temperature, can directly indicate inadequate HVAC performance. These tools do not aid in cloud migration (which is the task of architects and administrators) nor in risk decisions (which is the task of senior management); they also don’t provide any kind of assistance with fire.

### Question # 63 - In addition to predictive capabilities, event monitoring tools (security information and event management [SIEM]/security information management [SIM]/security event management [SEM]) are instrumental in what other security function?      
A. Personnel safety    
B. Vehicle tracking    
C. Incident evidence     
D. Acoustic dampening      
Answer: C. 

Event logs are used to reconstruct a narrative of activity; they tell the story of what happened, how it happened, and so forth. This is crucial for evidentiary purposes. Event logging tools do not aid in any of the other options (especially acoustic dampening, which is gibberish in this context).

### Question # 64 - Which of the following is one of the benefits of event monitoring tools (security information and event management [SIEM]/security information management [SIM]/security event management [SEM])?      
A. Greater physical security    
B. Psychological deterrence     
C. Cost savings     
D. More logs can be reviewed, at faster speeds         
Answer: D. 

The manual element of log review is tedious and necessarily slow because it requires a trained, knowledgeable person to perform the task; these tools can greatly increase the amount of log data that can be reviewed, in a much shorter amount of time. These tools do not, however, aid in any of the other options.

### Question # 65 - As in a traditional IT environment, proper key management is crucial in the cloud. Which of the following principles is not true regarding key management?     
A. It is good practice to introduce pseudorandom numbers when generating keys.     
B. Public keys should never be shared with anyone.     
C. Losing the keys is equivalent to losing the data.     
D. Symmetric keys should be passed out of band.     
Answer: B. 

Public keys have to be shared in order for asymmetric cryptography to function properly; that is their purpose. Private keys, on the other hand, must remain secret, known only to the individuals to whom they are assigned.
Seeding key generation processes with pseudorandom numbers makes decryption that much more difficult and is a desired practice, so option A is incorrect.
Losing keys to encrypted data means that the data stays encrypted, which is a way of applying a denial-of-service attack on yourself, so option C is incorrect.
Symmetric keys, known as shared secrets, ought to be transmitted to recipients over a different medium than the mode of communication intended for the encrypted traffic. If the users intend to use encrypted email, for instance, they should pass the keys via telephone. Option D is therefore incorrect.

### Question # 66 - Which of the following is a good business case for the use of data masking?     
A. The shipping department should get only a masked version of the customer’s address.     
B. The customer service department should get only a masked version of the customer’s Social Security (SS) number.     
C. The billing department should get only a masked version of the customer’s credit card number.     
D. The Human Resources (HR) department should get only a masked version of the employee’s driver’s license number.       
Answer: B. 

The customer service representative may need to see a partial version of the customer’s SS number to verify that the customer is who they claim to be, but that representative does not need to see the full number, which would create an unnecessary risk.
The shipping department definitely needs the customer’s address in order to send things to the customer, so option A is not correct.
The billing department needs the customer’s full credit card number to process payments, so option C is incorrect.
HR needs the employee’s full license number in order to verify and validate the employee’s identity, so option D is not correct.

### Question # 67 - All of the following are methods of data masking suggested by (ISC)2 except _______________.     
A. Random substitution    
B. Algorithmic substitution     
C. Deletion     
D. Conflation     
Answer: D. Conflation is not a masking technique and is meaningless in this context. All the others are suggested as possible masking techniques.

### Question # 68 - If data masking is being performed for software testing purposes, which of the following is not a good masking technique to use?     
A. Random substitution    
B. Shuffling     
C. Deletion     
D. Algorithmic substitution       
Answer: C.       

While deletion is a very good way to avoid the possibility of inadvertently disclosing production data in a test environment, it also eliminates the usefulness of the data set as a plausible approximation of the production environment, greatly reducing the quality of the testing.
The other options modify the raw production data into something that approximates the real environment without disclosing real data, to a greater or lesser extent; some are better than the others, but they are all better than deletion for testing purposes.

### Question # 69 - For which use case would it probably be best to use static masking?     
A. Creating a test environment for a new application     
B. Allowing a customer service representative limited access to account data     
C. Providing detailed reports to regulators      
D. Notifying shareholders        
Answer: A. 

Static masking involves modification of an entire data set, all at once. This would be a good method to create a sample data set for testing purposes.
Static testing for customer service use would be overkill; replicating all the customer accounts at once so that the fraction of customers who contact customer service may receive assistance is inefficient and cumbersome, and customer account information is likely to change between static updates, making it less useful. Therefore, option B is incorrect.
Neither regulators nor shareholders need to see masked data, so both options C and D are incorrect.

### Question # 70 - For which use case would it probably be best to use dynamic masking?     
A. Creating a test environment for a new application      
B. Allowing a customer service representative limited access to account data     
C. Sending incident response notifications      
D. Implementing business continuity and disaster recovery (BC/DR)       
Answer: B.     

Dynamically masking a user’s account information each time a customer service representative accesses that data is an efficient, secure means of masking data as necessary.
Trying to mask each data element as it is called by an application in a test environment would be unwieldy and not likely to provide accurate test data, so option A is incorrect.
Neither incident response nor BC/DR purposes need masked data, so both options C and D are incorrect.

### Question # 71 - What is one possible risk associated with the use of algorithmic masking for obscuring a data set?      
A. You could corrupt the production data.     
B. The data could be subject to easy inadvertent disclosure.     
C. Algorithms are two-way operations.       
D. A null set has no test value.       
Answer: C. 

Using an algorithm to mask data suggests that the same algorithm, if learned or reverse-engineered by an aggressor, could be used on the masked data to reveal the production data.
Algorithmic masking causes no more risk to production data than the other masking methods, so option A is incorrect.
Accidental disclosure might be interpreted as the same thing as determining the original data from the masked set, so option B might be considered accurate, but option C is a better way of stating the risk, so B is incorrect.
Option D is about the use of the deletion technique for masking, not algorithmic, so it is incorrect.
This is not an easy question, and it involves some abstract thought to arrive at the correct answer.

### Question # 72 - ____________ is a direct identifier, and ____________ is an indirect identifier.      
A. Username; password      
B. User’s name; user’s age      
C. User’s IP address; user’s media access control (MAC) address        
D. Location; income level         
Answer: B. 

The user’s name is a direct identifier, explicitly stating who that person is. The user’s age is not a direct identifier because it doesn’t specify a certain person, but it is a piece of demographic information that could be used to narrow down the user’s identity from a group of users of different ages, so it is an indirect identifier.
Username and password are identity assertions and authentication credentials, not identifiers. The username might be a direct identifier, but the password is neither a direct nor an indirect identifier (especially if it is kept secret, as it should be). Option A is thus incorrect.
Option C is incorrect because both elements could be considered direct identifiers (depending on the jurisdiction) if the user’s machine is considered a legal representation of the user.
Option D is incorrect because both elements are indirect identifiers.

### Question # 73 - Anonymization is the process of removing ____________ from data sets.       
A. Access     
B. Cryptographic keys       
C. Numeric values      
D. Identifying information       
Answer: D. 

Anonymization is the process of removing identifiers from data sets so that data analysis tools and techniques cannot be used by malicious entities to divine personal or sensitive data from nonsensitive aggregated data sets.
All the other answers are incorrect because they are not part of the anonymization process.

### Question # 74 - Tokenization is a method of obscuring data that, other than encryption, can be used to comply with ____________ standards.      
A. Gramm-Leach-Bliley Act (GLBA)    
B. Payment Card Industry (PCI)     
C. Child Online Protection Act (COPA)     
D. Sarbanes-Oxley Act (SOX)      
Answer: B. 

PCI requires that credit card numbers and other cardholder data be obscured when stored for any length of time. Encryption is one approved method; tokenization is another.
GLBA, COPA, and SOX do not specifically require obscuring stored data, so those options are incorrect.

### Question # 75 - Tokenization requires at least ____ database(s).     
A. One    
B. Two    
C. Three    
D. Four    
Answer: B.     

Tokenization will require, at a minimum, a database for the tokens and another for the stored sensitive data.
One database will not suffice; a single database holding both the tokens and the sensitive data they represent would not be in compliance with any standard requiring data to be obscured. Option A is thus incorrect.
Option C might be an answer some readers choose; it is easy to overthink this question. You might consider that the data requires two databases (one for tokens, one for sensitive data), and that access control would require a third database (for authentication credentials); however, the tokenization methodology does not strictly require that access be controlled through an authentication server. Option C is therefore incorrect. Be sure not to read more into the question than appears at face value.
Option D is incorrect; that’s just too many databases.

### Question # 76 - Data owners might consider using tokenization for all of the following reasons except _______________.      
A. Regulatory or contractual compliance     
B. Inference    
C. Reduced cost of compliance     
D. Mitigating risk from data lost to intrusion       
Answer: B. 

Inference is an attack strategy, not a reason for implementing tokenization.
All the other options are good reasons to implement tokenization, and they are therefore not correct.

### Question # 77 - Bit-splitting, also known as data dispersion, might be thought of as ____________ in the cloud.      
A. RAID    
B. BIOS    
C. DDoS    
D. SYN-ACK     
Answer: A. 

In the traditional environment, a RAID array is a set of disks/drives on which data 
is spread to enhance the availability, security, and resiliency of the data. In the cloud, 
bit-splitting/data dispersion performs this same function in much the same way.
All the other options have nothing to do with spreading data across multiple storage areas.

### Question # 78 - Bit-splitting also provides security against data breaches by _______________.       
A. Removing all access to unauthorized parties     
B. Ensuring that an unauthorized user only gets a useless fragment of data     
C. Moving data across jurisdictional boundaries     
D. Tracking all incoming access requests    
Answer: B.     

Bit-splitting involves chopping data sets up into segments and storing those segments in multiple places/devices. An attacker getting access to one segment won’t be gaining anything of value because one segment of the data set would most likely make no sense out of context.

Bit-splitting may or may not function as an access control method; option B is preferable to A.

Bit-splitting may or may not move data across jurisdictions, which may or may not be useful to the data owner; option B is preferable to C.

Bit-splitting does not, in itself, provide access logs; option D is incorrect.

### Question # 79 - If bit-splitting is used to store data sets across multiple jurisdictions, how may this enhance security?     
A. By making seizure of data by law enforcement more difficult     
B. By hiding it from attackers in a specific jurisdiction     
C. By ensuring that users can only accidentally disclose data to one geographic area     
D. By restricting privilege user access      
Answer: A.      

When law enforcement entities wish to seize assets (including data), they must cooperate with other law enforcement agencies in other jurisdictions if the data is not contained fully within their own. This may aid a data owner who is concerned about the risk of losing their data in a multitenant environment if another tenant conducts illicit activity and law enforcement seizes an entire data storage device as part of an investigation, accidentally collecting data belonging to innocent parties.
Attackers are jurisdiction-agnostic; they don’t care where data is stored or what laws apply. Option B is thus incorrect.
Authorized users can access bit-split data regardless of the location and can disclose information worldwide; option C is incorrect.
Bit-splitting does not pertain to types of access roles; option D is incorrect.

### Question # 80 - Which of the following is a possible negative aspect of bit-splitting?     
A. Less security    
B. Greatest risk of unauthorized access    
C. Significantly greater processing overhead      
D. Violating regulatory compliance      
Answer: C.      

Bit-splitting, as with many security methods/technologies, carries a significantly greater overhead than data sets that don’t use this method. Bit-splitting, in particular, takes an extensive amount of processing to perform.
Bit-splitting should make a data set more secure and decrease the chance of unauthorized access, so options A and B are incorrect.
It is unlikely that bit-splitting would violate regulatory standards; even if that were to be the case, it is always true that bit-splitting carries greater overhead, so option C is preferable to D.

### Question # 81 - Which of the following is a possible negative aspect of bit-splitting?     
A. It may require trust in additional third parties beyond the primary cloud service provider.    
B. There may be cause for management concern that the technology will violate internal policy.    
C. Users will have far greater difficulty understanding the implementation.    
D. Limited vendors make acquisition and support challenging.     
Answer: A. 

This is not a simple question and requires the reader to think through the situation suggested by each answer. Option A is correct because the data owner may opt to perform bit-splitting across multiple cloud services to enhance security (not all the “eggs” will be in one “basket”). When this is the case, the data owner will have additional dependencies: all the vendors involved in storing the various data elements.
There should be no additional management concern; if bit-splitting is not compliant with the data owner’s policy, it won’t be adopted. Option B is incorrect.
Bit-splitting implementations should be transparent to users; option C is incorrect.
There are plenty of vendors offering bit-splitting solutions; option D is incorrect.

### Question # 82 - Which of the following is a possible negative aspect of bit-splitting?     
A. Greater chance of physical theft of assets    
B. Loss of public image     
C. Some risk to availability, depending on the implementation     
D. A small fire hazard      
Answer: C. 

Ironically, data dispersion can lead to some additional risk of loss of availability, depending on the method/breadth of the dispersion. If the data is spread across multiple cloud providers, there is a possibility that an outage at one provider will make the data set unavailable to users, regardless of location. However, there are methods for attenuating this threat, and bit-splitting usually provides greater availability of data over traditional storage without dispersion.
Data dispersion should have no effect on physical theft risks and would actually serve to minimize the opportunity for an attacker to acquire useful sensitive data as the data would be on several geographically disparate devices. Option A is incorrect.
Bit-splitting should have no effect on public image whatsoever; option B is incorrect.
Bit-splitting does not have an attendant fire risk; option D is incorrect.

### Question # 83 - Which of the following is a theoretical technology that is intended to allow encrypted material to be processed and manipulated without decrypting it first?     
A. Inverse postulation    
B. Homomorphic encryption     
C. Didactic alignment     
D. Obverse reinstantiation      
Answer: B. 

This is the definition of homomorphic encryption.
All the other answers are incorrect.

### Question # 84 - Which of the following is a data discovery approach used by e-commerce retailers to discern and predict shoppers’ needs?     
A. Big data   
B. Real-time analytics     
C. Agile analytics    
D. Agile business intelligence      
Answer: B. 

Real-time analytics allows for reactive and predictive operations (such as recommending other, related products) based on customers’ current and past shopping behavior.
All the other answers are data discovery approaches but not used for this particular application (options C and D are two names for the same thing).

### Question # 85 - Which of the following is a data discovery approach that offers insight to trends of trends, using both historical and predictive approaches?     
A. Obverse polyglotism    
B. Big data     
C. Real-time analytics      
D. Agile analytics/business intelligence      
Answer: D.       

The Agile approach to data analysis offers greater insight and capabilities than previous generations of analytical technologies.
Options B and C are other data discovery technologies, but neither is the correct answer.
Option A is incorrect because obverse polyglotism is just a made up term that does not have any relevance as an answer to the question.

### Question # 86 - Which of the following is not a data discovery technique?      
A. Metadata    
B. Labels    
C. Content analysis    
D. Data hover      
Answer: D.      
  
Data hover is a made up term which is not a data discovery technique. All the other answers are actual data discovery techniques.

### Question # 87 - Which of the following data discovery techniques involves using extra information automatically appended/included with the intended data when the data is created?        
A. Metadata    
B. Labels     
C. Content analysis     
D. Data hover      
Answer: A.      

This is the definition of metadata: data about data, usually created by systems (hardware and/or software) when the data is captured/collected.
Options B and C are also data discovery techniques, but not involving metadata.
Data hover is a made up term and is therefore, not a data discovery technique, so option D is incorrect.

### Question # 88 - When labeling is used as a data discovery technique, who should be applying the labels?    
A. The security office   
B. Users   
C. Data owners     
D. Regulators     
Answer: C.      

The data owners, presumably the personnel closest to and most familiar with the data, should be the ones labeling it.
The other answers are incorrect because they are not the data owners.

### Question # 89 - When data labels are being used in an environment (for discovery and other purposes), when should the labels be applied?     
A. During the risk assessment     
B. As part of the business impact analysis (BIA)     
C. At collection/creation     
D. When the discovery tools are implemented      
Answer: C.      

For the most efficient classification/categorization process, and to streamline the application of proper controls, data labeling should be performed when the data is first being collected/created.
Options A and B are incorrect because they are not part of a data labeling process.
Option D is incorrect because the discovery tools need to have the data labeled to work properly.

### Question # 90 - Which of the following tools might be useful in data discovery efforts that are based on content analysis?     
A. Egress monitoring solutions    
B. Digital rights management (DRM)    
C. iSCSI    
D. Fibre Channel over Ethernet (FCoE)    
Answer: A.     

Egress monitoring tools (often referred to as DLP) are specifically designed to seek out and identify data sets based on content; this is part of how they operate. They can be used for or in conjunction with content-based data discovery efforts.
Digital rights management (DRM) is an additional access control solution for objects, so option B is incorrect.
Internet Small Computer System Interface (iSCSI) allows storage controller commands to be sent over a Transmission Control Protocol (TCP) network and has nothing to do with data discovery; thus, option C is incorrect.
Fibre Channel over Ethernet (FCoE) is a standard for approaching fiber-media speeds of data transfer on an Ethernet network; it has nothing to do with data discovery, so option D is incorrect.

### Question # 91 - All of the following might be used as data discovery characteristics in a content-analysis-based data discovery effort except _______________.       
A. Keywords     
B. Pattern matching     
C. Frequency     
D. Inheritance     
Answer: D.      

Inheritance has nothing to do with content analysis; it is usually referring to object-oriented traits derived from originating objects.
All the other answers are characteristics of content that can be used in content-analysis methods of data discovery.

### Question # 92 - What is the risk to the organization posed by dashboards that display data discovery results?     
A. Increased chance of external penetration     
B. Flawed management decisions based on edited displays     
C. Higher likelihood of inadvertent disclosure      
D. Raised incidence of physical theft      
Answer: B.       

Because dashboards are often used for management purposes (graphical representations of technical data), management pressures often result in skewed data dashboarding (“no red!”), which can lead to the “data” being used for fallacious decisions.
All the other answers are not affected by dashboarding at all and are incorrect.

### Question # 93 - Which of these is most likely to have the greatest negative impact on data discovery effort?     
A. Bandwidth latency issues    
B. Poor physical security of the data center     
C. Severe statutory regulation     
D. Inaccurate or incomplete data     
Answer: D.       

A data discovery effort can only be as effective as the veracity and quality of the data it addresses. Bad data will result in ineffective data discovery.
All the other answers do not impact data discovery efforts and are only distractors. (Poor bandwidth might slow down data discovery, but it won’t have true negative impact, so option D is still better.)

### Question # 94 - Cloud customers performing data discovery efforts will have to ensure that the cloud provider attends to all of the following requirements except _______________.     
A. Allowing sufficient access to large volumes of data     
B. Preserving metadata tags     
C. Assigning labels      
D. Preserving and maintaining the data      
Answer: C. 

Label assignment is a task of the data owner—the cloud customer, not the provider.
All the other answers are requirements for the cloud provider to meet the data discovery needs of the customer and should be negotiated before migration.

### Question # 95 - Where should the cloud provider’s data discovery requirements be listed?    
A. National Institute of Standards and Technology (NIST) Special Publication (SP) 800-53    
B. Applicable laws and regulations    
C. Payment Card Industry Data Security Standard (PCI DSS)     
D. The managed services contract and SLA     
Answer: D.      

The cloud customer will have to determine which levels of performance/responsibilities on the part of the provider will be necessary to meet the customer’s needs for data discovery. These should be codified in the contract/service-level agreement (SLA).
The other answers are general regulations and standards; they will not contain specific guidance for every customer’s needs and are only distractors.

### Question # 96 - Who will determine data classifications for the cloud customer?     
A. The cloud provider     
B. National Institute of Standards and Technology (NIST)    
C. Regulators     
D. The cloud customer     
Answer: D.      

This is a difficult question and requires insight on the practice of classifying data and a good understanding of the material. While the determination of what sorts of data need to be protected may come from external sources (laws, standards, regulations, etc.), the classification of data for each data owner/cloud customer will be specific to that entity. Therefore, the cloud customer will have to impose data classification schema on itself and its own data.
The other answers represent external entities, some of whom might require that certain information be handled with a certain duty or care (such as Payment Card Industry [PCI] mandates for cardholder information). However, these entities will not impose a classification scheme on the data owner or cloud customer; that responsibility falls on the data owner or cloud customer to do for itself and the data under its control.

### Question # 97 - An organization’s data classification scheme must include which of the following categories?     
A. File size    
B. Origin of the data     
C. Sensitivity of the data      
D. Whatever the data owner decides     
Answer: D.      

This is a difficult, and somewhat tricky, question. Each organization has to decide, for itself, how to classify its own data. With that said, many factors bear on this determination: external regulations and drivers, the type of industry in which the organization operates, and so forth. But the kinds of data the organization uses, and how that data is sorted, will differ for every organization, and each must make its own determination on how to best sort that data.
All the other answers are factors that an organization might consider when creating a classification scheme, but they are not mandatory for every organization. Option D is still the best answer for this question.

### Question # 98 - Classification is usually considered a facet of data ____________.     
A. Security    
B. Labeling    
C. Control    
D. Markup   
Answer: B.    

This is another difficult question. Classification of data is an element of labeling, insofar as labeling is the grouping of data into discrete categories and types. Labels must be affixed to objects and data sets in accordance with an overall policy that lists objective criteria to guide the data owner(s) in assigning the appropriate label; this is a form of classification.
Option A might be considered apt, as labeling and classification fall generally under the auspices of “security,” but option B is more specific and therefore correct.
Classification is not considered a facet of data control or data markup. Therefore, options C and D are incorrect.

### Question # 99 - Data classification can be ____________ or ____________.      
A. Inverse or obverse     
B. Automatic or manual     
C. Correct or incorrect     
D. Diurnal or nocturnal    
Answer: B.      

An organization could implement an automated tool that assigns labels based on certain criteria (location of the source of the data, time, creator, content, etc.), much like metadata, or the organization could require that data creators/collectors assign labels when the data is first created/collected, according to a policy that includes discrete, objective classification guidance.
Option A is incorrect because even though the word pair may seem pretty technical, together they are meaningless with respect to data classification.
It may be true that data classification can be correct or incorrect, however, option C is not as good of an answer as option B. The goal for the data owner is to correctly classify the data and not to incorrectly classify the data. So, option C is incorrect.
It is difficult to imagine data classification that only takes place at a certain time of day. Therefore, it is not likely to be the correct answer and certainly option D is not as good an answer as option B.

### Question # 100 - Data may need to be reclassified for all the following reasons except _______________.       
A. Color change      
B. Time     
C. Repurposing     
D. Transfer of ownership     
Answer: A. 

Color is unlikely to be a characteristic for which data is classified, much less reclassified. Although some exceptions might exist (motion picture production, satellite imagery, paint vendors, etc.), those would be far from the norm, and the other answers are much more general cases and would apply to many more organizations. Therefore, color is the correct answer (in the negative), and the rest are incorrect (because they are true).

### Question # 101 - Proper __________ need(s) to be assigned to each data classification/category.     
A. Dollar values     
B. Metadata     
C. Security controls      
D. Policies      
Answer: C. 

The purposes of classifying/categorizing data is to create proper associated control sets for each data type and aid the efficiency and cost-effectiveness of applying those controls to that data.
While dollar value may be a good metric for assessing data type in many organizations, it is not the only such trait, and not for all organizations; option C is still a better answer, so A is wrong.
Metadata may or may not be used in a classification/categorization scheme; option B is incorrect.
Policies are not assigned to data types; a policy will dictate how data classifications/categories are assigned to data. Option D is incorrect.

### Question # 102 - Data transformation in a cloud environment should be of great concern to organizations considering cloud migration because ____________ could affect data classification processes and implementations.      
A. Multitenancy     
B. Virtualization      
C. Remote access      
D. Physical distance      
Answer: B. 

Data transforming from raw objects to virtualized instances to snapshotted images back into virtualized instances and then back out to users in the form of raw data may affect the organization’s current classification methodology; classification techniques and tools that were suitable for the traditional IT environment might not withstand the standard cloud environment. This should be a factor of how the organization considers and perceives the risk of cloud migration.
Multitenancy should be a consideration of cloud migration for the potential risks of data leakage and disclosure but not because of data transformation. Option A is not correct.
Remote access and physical distance should not include aspects of data transformation that are not already considered in the traditional IT environment, so options C and D are incorrect.

### Question # 103 - Who is ultimately responsible for a data breach that includes personally identifiable information (PII), in the event of negligence on the part of the cloud provider?     
A. The user     
B. The subject    
C. The cloud provider     
D. The cloud customer      
Answer: D.     

The cloud customer, as the PII data owner, is ultimately legally responsible for all losses of PII data. The customer may be able to recoup some of the costs of damages related to the breach by placing financial liability on the provider through the use of strong contract terms and conditions, but all legal responsibility falls on the customer, in all cases.
The other options are parties that may have some partial or contributory responsibility for the breach (especially, in this case, the provider, who was negligent), but the ultimate responsibility lies with the customer.

### Question # 104 - In a personally identifiable information (PII) context, who is the subject?      
A. The cloud customer    
B. The cloud provider     
C. The regulator     
D. The individual    
Answer: D.      

The subject is the human being to whom the PII applies.
The other answers are not data subjects, and are therefore incorrect.

### Question # 105 - In a personally identifiable information (PII) context, who is the processor?     
A. The cloud customer    
B. The cloud provider    
C. The regulator     
D. The individual      
Answer: B. 

In a PII context, the processor is any entity that processes data on behalf or at the behest of the data owner. In the case of most managed cloud service arrangements, that will be the cloud service provider. (The cloud customer may also process its own data, but the customer is the data owner/controller.)
Options A, C, and D are all incorrect. The cloud customer provides the subject’s PII to the cloud provider for processing. The regulator ensures that the PII is protected properly and the individual is the data subject. So, options A, C, and D are incorrect answers.

### Question # 106 - In a personally identifiable information (PII) context, who is the controller?     
A. The cloud customer    
B. The cloud provider     
C. The regulator      
D. The individual       
Answer: A. 

In a PII context, the controller is the entity that creates/collects, owns, or manages the data—that is, the data owner. In a managed cloud service arrangement, that would be the cloud customer.
Options B, C, and D are all incorrect. The cloud provider is the entity that processes the PII data. The regulator ensures that the PII is protected properly and the individual is the data subject.

### Question # 105 - In a personally identifiable information (PII) context, which of the following is not normally considered “processing”?      
A. Storing     
B. Viewing     
C. Destroying   
D. Printing   
Answer: B. 

This is not a simple question, and it requires a bit of insight into uses of data. The most suitable answer here is “viewing,” as it is entirely passive; the viewer is not performing any action on the data. “Processing,” in a PII context, is any manipulation of the data, to include securing or destroying it, in electronic or hard-copy form. In a “viewing” action, the processor would be displaying the data to the viewer, while the viewer is only receiving it, not storing it or using it. Note that the answer did not involve “using,” which definitely would be a processing action.
All the other answers are examples of processing and therefore not correct.

### Question # 106 - Which of the following countries does not have a national privacy law that concerns personally identifiable information (PII) and applies to all entities?      
A. Argentina      
B. The United States      
C. Italy      
D. Australia     
Answer: B.     

The United States has some federal PII laws that apply to specific sectors (the government itself [Privacy Act], medical providers [Health Information Portability and Accountability Act], financial and insurance vendors [Gramm-Leach-Bliley Act], etc.), but not a single, overarching federal law that addresses PII in a uniform, nationwide manner.
All the other options list countries that have such laws, and those options are therefore incorrect.

### Question # 107 - In protections afforded to personally identifiable information (PII) under the U.S. Health Information Portability and Accountability Act (HIPAA), the subject must __________ in order to allow the vendor to share their personal data.    
A. Opt in    
B. Opt out      
C. Undergo screening      
D. Provide a biometric template        
Answer: A.      

Under HIPAA, the subject must opt in to information sharing—that is, the subject (the patient) must explicitly state, in writing and with a signature, who the vendor is allowed to share personal information with, such as family members, spouses, parents, and children. (Under HIPAA, this personal information is referred to as electronic private health information [ePHI].) The vendor is prohibited from sharing the patient’s data with anyone else.

Under HIPAA, the patient does not have to opt out of information sharing; the default situation is to not share patient data. Option B is incorrect.

HIPAA does not require any kind of screening or template, so Options C and D are incorrect.

### Question # 108 - In protections afforded to personally identifiable information (PII) under the U.S. Gramm-Leach-Bliley Act (GLBA), the subject must __________ in order to prevent the vendor from sharing their personal data.       
A. Opt in    
B. Opt out     
C. Undergo screening             
D. Provide a biometric template     
Answer: B. 

Under GLBA, financial and insurance vendors are allowed to share account holders’ personal data with other entities (including other businesses owned by the same vendor) unless the account holder explicitly states, in writing, that the vendor is not allowed to do so. The vendor is required to provide a form for opting out of data sharing when the account holder creates the account and annually every subsequent year.

Option A is incorrect; under GLBA, the default situation allows banks and insurance providers (owned by the same entity) to share customer data—the customer must opt out of this arrangement if the customer doesn’t want information shared.
Options C and D are incorrect because they do not relate to the sharing of PII data by a bank or insurer.

### Question # 109 - The European Union (EU), with its implementation of privacy directives and regulations, treats individual privacy as ____________.     
A. A passing fad      
B. A human right     
C. A legal obligation      
D. A business expense     
Answer: B. 

The EU is probably at the forefront of global efforts to sanctify and enshrine personal privacy; the current statutes and precedents based on court decisions have clearly denoted Europe’s intent to treat individual privacy as a human right.
Options A and D are simply incorrect.

It is very possible to consider option C as correct because European businesses are held to strict standards regarding the privacy data under their control. However, option B has more significance and is more general, so it is the proper selection among this list.

### Question # 110 - If your organization collects/creates privacy data associated with European Union (EU) citizens and you operate in the cloud, you must prevent your provider from storing/moving/processing that data where?     
A. Argentina     
B. The United States     
C. Japan     
D. Israel     
Answer: B.     

The EU regulations associated with personally identifiable information (PII) belonging to EU citizens prohibit that data to be utilized in any way in any country that does not have a national privacy law commensurate with the EU regulations. Of this list, only the United States has no such law. Indeed, the EU regulations might very well be taken to be aimed directly at the United States, and probably for good reason; the United States has not proven to be a good steward of or even recognize the importance of personal privacy.

### Question # 111 - European Union (EU) personal privacy protections include the right to be _______________.     
A. Secure    
B. Delivered     
C. Forgotten     
D. Protected       
Answer: C.       

The right to be forgotten is the EU’s codification of an individual’s right to have any data store containing their own personal data purged of all personally identifiable information (PII). There are, of course, some obvious exceptions (such as law enforcement databases).
The other answers are not as accurate; “the right to be forgotten” is a very well-known and important aspect of the GDPR.

### Question # 112 - The Cloud Security Alliance (CSA) has developed a model for cloud privacy frameworks called the Privacy Level Agreement (PLA). Why might a cloud service provider be reluctant to issue or adhere to a PLA?         
A. A PLA might limit the provider’s liability.      
B. A PLA would force the provider to accept more liability.      
C. A PLA is nonbinding.      
D. A PLA is not enforceable.       
Answer: B. 

Under current laws and regulations, ultimate liability for the security of privacy data rests on the data controller—that is, the cloud customer. A PLA would require the cloud provider to document expectations for the cloud customer’s data security, which would be an explicit admission of liability. There is little motivation for cloud providers to take on this additional liability (and the costs associated with it) with no mandate or market force pushing them to do so.

Option A is wrong because the provider’s liability is already limited under current legal schemes; the PLA would not enhance that limitation.
Options C and D are wrong because agreements (as contracts) are both binding and enforceable, and even if they were not, those are not reasons.

### Question # 113 - The Cloud Security Alliance Cloud Controls Matrix (CSA CCM) lists security controls from all the following frameworks except _______________.     
A. ISACA’s Control Objectives for Information and Related Technology (COBIT)     
B. Payment Card Industry Data Security Standard (PCI DSS)     
C. The Capability Maturity Model (CMM)     
D. International Organization for Standardization (ISO) 27001      
Answer: C. 

The CMM is not included in the CSA CCM and, indeed, is not even a security framework.
All the other options are included in the CSA CCM and are therefore not correct answers for this question.
 
### Question # 114 - The Cloud Security Alliance Cloud Controls Matrix (CSA CCM) lists security controls from all the following laws except _______________.     
A. Health Information Portability and Accountability Act (HIPAA)    
B. Family Education Rights and Privacy Act (FERPA)     
C. Personal Information Protection and Electronic Documents Act (PIPEDA)     
D. Digital Millennium Copyright Act (DMCA)    
Answer: D. 

The DMCA deals with intellectual property and not specifically with personal privacy. It is not included in the CSA CCM.
All the other answers are laws that are included in the CSA CCM and are therefore not correct answers for this question.

### Question # 115 - Digital rights management (DRM) tools might be used to protect all the following assets except _______________.     
A. A trusted device    
B. Proprietary software     
C. Medical records     
D. Financial data      
Answer: A.       

DRM solutions are mainly designed to protect intellectual property assets (and mainly those covered by copyright, hence the name), but they can also be used to provide enhanced protection to other electronic information. All the other options are forms of electronic information, while option A is a piece of hardware; DRM does not enhance hardware security, so this is the correct answer.

### Question # 116 - Deploying digital rights management (DRM) tools in a bring-your-own-device (BYOD) environment will require _______________.      
A. User consent and action      
B. Enhanced security protocols      
C. Use of the cloud      
D. Newer, upgraded devices       
Answer: A. 

Deploying DRM usually requires installing a local agent on each device intended for use in that environment; with BYOD, that means getting all users to agree and install that agent because they own the devices.
DRM is an enhanced security protocol, so option B is incorrect.
The cloud is not specifically necessary for DRM implementations, even in BYOD environments, so option C is incorrect.
Any DRM solution involving a BYOD environment must be suitable for all devices, not just a certain selection, because the organization can’t easily mandate which devices are used (otherwise, it’s not BYOD). Option D is incorrect.

### Question # 117 - Deploying digital rights management (DRM) tools in a bring-your-own-device (BYOD) environment will require _______________.      
A. A uniform browser installation   
B. Platform-agnostic solutions    
C. Turnstiles    
D. A secondary business continuity and disaster recovery (BC/DR) vendor     
Answer: B. 

In a BYOD environment, users might bring any number of devices/operating systems to the network, and any DRM solution selected for the purpose must interact well with all of them.
The organization cannot dictate specific packages in a BYOD environment—otherwise it is not BYOD—so option A is incorrect.
Turnstiles are for physical access control and have no bearing on BYOD or DRM, so option C is incorrect.
BYOD and DRM should have no effect on BC/DR vendors (or the numbers thereof), and vice versa, so option D is incorrect.

### Question # 118 - The Cloud Security Alliance Cloud Controls Matrix (CSA CCM) addresses all the following security architecture elements except _______________.     
A. Physical security    
B. Infrastructure as a service (IaaS)     
C. Application security     
D. Business drivers     
Answer: D. 

The CSA CCM does not deal with whether security controls are feasible or correct from a business perspective, only whether they are applicable to an organization under certain regulations.
All the other answers are incorrect because they are too specific and not required by any regulation/legislation. Therefore, options A, C, and D are poor choices and also incorrect answers.

### Question # 119 - DRM requires that every data resource be provisioned with __________.      
A. A tracking device     
B. An access policy     
C. A hardware security module (HSM)      
D. A biometric system     
Answer: B. 

For DRM to work properly, each resource needs to be outfitted with an access policy so that only authorized entities may make use of that resource.
All the other answers are distractors.

### Question # 120 - Digital rights management (DRM) tools can be combined with __________ to enhance security capabilities.     
A. Roaming identity services (RIS)    
B. Egress monitoring solutions (DLP)     
C. Internal hardware settings (BIOS)     
D. The TEMPEST program     
Answer: B. 

DRM and DLP work well to address complementary security issues—namely, asset classification/categorization and discovery, along with access and dissemination of those assets.
RIS is a made-up term, so option A is not correct.

Adjusting BIOS settings is not particularly relevant to DRM in any way, so option C is incorrect.
TEMPEST is a program for harvesting data from electromagnetic emanations, so option D is not correct.

### Question # 121 - Digital rights management (DRM) tools should enforce __________, which is the characteristic of access rights following the object, in whatever form or location it might be or move to.     
A. Continuous audit trail   
B. Limiting printing output   
C. Persistence   
D. Automatic expiration     
Answer: C. 

Access rights following the object in whatever form or location it might be or move to is the definition of persistence, one of the required traits for a DRM solution of any quality.
All the other answers are traits that should be included in DRM solutions but do not match the definition in the question, so they are incorrect.

### Question # 122 - Digital rights management (DRM) tools should enforce __________, which is the practice of capturing all relevant system events.      
A. Continuous audit trail     
B. Limiting printing output     
C. Persistence     
D. Automatic expiration     
Answer: A. 

Capturing all relevant system events is the definition of a continuous audit trail, one of the required traits for a DRM solution of any quality.
All the other answers are traits that should be included in DRM solutions but do not match the definition in the question, so they are incorrect.

### Question # 123 - Digital rights management (DRM) tools should enforce __________, which is the capability to revoke access based on the decision of the object owner or an administrator action.    
A. Integration with email filtering engines    
B. Disabling screencap capabilities    
C. Continuous audit trail     
D. Dynamic policy control     
Answer: D.     

The question describes dynamic policy control, one of the required traits for a DRM solution of any quality.
All the other answers are traits that should be included in DRM solutions but do not match the definition in the question, so they are incorrect.

### Question # 124 - Digital rights management (DRM) tools should enforce __________, which is the revocation of access based on time.     
A. Persistence     
B. Disabling screencap capabilities      
C. Automatic expiration    
D. Dynamic policy control    
Answer: C. 

The question describes automatic expiration, one of the required traits for a DRM solution of any quality.
All the other answers are traits that should be included in DRM solutions but do not match the definition in the question, so they are incorrect.

### Question # 125 - Digital rights management (DRM) tools should enforce __________, which is interoperability with the organization’s other access control activities.     
A. Persistence    
B. Support for existing authentication security infrastructure     
C. Continuous audit trail     
D. Dynamic policy control     
Answer: B. 

The question describes support for existing authentication security infrastructure, one of the required traits for a DRM solution of any quality.
All the other answers are traits that should be included in DRM solutions but do not match the definition in the question, so they are incorrect.

### Question # 126 - In a data retention policy, what is perhaps the most crucial element?          
A. Location of the data archive     
B. Frequency of backups     
C. Security controls in long-term storage     
D. Data recovery procedures    
Answer: D.     

This is not an easy question and requires some interpretation and abstract thought. All of the elements listed are extremely important aspects of the data retention policy. However, using proper data retrieval procedures is the one without which all the others may become superfluous. An organization can perform thorough backups in a timely manner and secure them properly at an excellent location, but if those backups can’t be used to restore the operational environment, they are pointless.
All the other options are important, but option D is probably the most important.

### Question # 127 - __________ is the practice of taking data out of the production environment and putting it into long-term storage.     
A. Deletion    
B. Archiving     
C. Crypto-shredding      
D. Storing      
Answer: B.     

The question states the definition of archiving.
Deletion involves using the operating system or an application to obscure the location of an object or file, so option A is wrong.
Crypto-shredding is a secure sanitization technique using cryptographic techniques, so option C is wrong.
Storing is a general term covering all retention of data, so option B is a better answer than option D.

### Question # 128 - In general, all policies within an organization should include each of the following elements except _______________.      
A. The date on which the policy will expire      
B. The assignment of an entity to review the applicability of the possibility occasionally     
C. The assignment of an entity to monitor and maintain the process described in the policy       
D. A list of the laws, regulations, practices, and/or standards that drove the creation of the policy       
Answer: A. 

Not all policies are temporary or have expected durations; usually, policy is an enduring piece of governance that will continue until such time as it is revoked.
All the other options are elements that should usually be included in policies.

### Question # 129 - The goals of secure sanitization (or “data destruction”) include all of the following except _______________.     
A. Removing data objects or files     
B. Minimizing or eliminating data remanence      
C. Removing pointers and metadata about specific files or objects       
D. Creating a secure, archived copy for business continuity and disaster recovery (BC/DR) purposes         
Answer: D. 

Secure sanitization is intended to ensure that there is no possible way for the data to be recovered; a backup copy would defeat the entire purpose.
All the other answers are goals of secure sanitization.

### Question # 130 - Why is deleting a file or object insufficient for secure sanitization purposes?       
A. Drives and disks must be demagnetized for true secure destruction.     
B. Physical destruction is the only acceptable method of secure sanitization.     
C. Deletion usually only removes pointers or indicators of file location.    
D. Only administrators should be allowed to delete files or objects.      
Answer: C.      

Deletion, using basic system assets (usually the operating system), mainly involves removing pointers to and addresses of the files or objects that are the targets of deletion. This leaves the raw data remaining on the storage resource, and it could be recovered later.

Options A and B both include secure destruction methods, but they are not exclusive (obviously, because there are two of them), so therefore they are untrue and also incorrect.

Option D does not make practical sense; if users could not delete files/objects, common workplace activity would become burdensome and difficult.

### Question # 131 - Data destruction in the cloud is difficult because ____________.     
A. Cloud data doesn’t have substance     
B. Regulations prevent it    
C. The hardware belongs to the provider     
D. Most of the data is subterranean     
Answer: C. 

The preferred methods of secure sanitization require physical access to (and control of) the hardware on which the data is stored; in the cloud, this belongs to the cloud provider, and the cloud customer will not be allowed to perform destructive procedures.
Options A, B, and D are incorrect because the question is about the difficulty of performing data destruction in the cloud computing environment. Often, the only reliable form of data destruction is to destroy the hardware where it is stored. None of these options address that question the way that option C does.

### Question # 132 - Data destruction in the cloud is difficult because ____________.      
A. Data in the cloud is constantly being replicated and backed up     
B. Delete commands are prohibited in the cloud     
C. Internet service providers (ISPs) will not allow destruction of data stored in the cloud      
D. The end clients may prevent it           
Answer: A. 

One of the benefits of using managed cloud services is that most providers are constantly performing backup and preservation activities in order to ensure that customers do not lose data. This can make it complicated for customers to even locate all their stored data, much less permanently destroy it.
Delete commands are certainly allowed in the cloud. Otherwise, cloud providers would eventually run out of storage space. Option B is incorrect.

Option C is incorrect because ISPs do not have the authority to prohibit the destruction of data by data owners.
It may be unclear who the “end client” is in option D. If the end client is the individual, then it does not make sense that the individual would prohibit the destruction of data by the cloud provider, given that the cloud provider owns the hardware itself.

### Question # 133 - Data destruction in the cloud is difficult because ____________.      
A. Only law enforcement is permitted to destroy cloud data      
B. The largest cloud vendors have prevented customers from destroying data     
C. Cloud data renews itself automatically      
D. The cloud is often a multitenant environment      
Answer: D. 

Secure sanitization would affect storage resources where more than one customer stores their data; truly secure destructive measures would likely result in destroying data belonging to someone else.
Law enforcement can destroy their own data, however, law enforcement is not permitted to destroy data that belongs to other individuals. Option A is therefore incorrect.
Option B is incorrect because data destruction is required from time to time in the cloud as part of system maintenance.
Fortunately, option C is incorrect. If data renewed itself automatically in the cloud then cloud providers would eventually run out of storage space.

### Question # 134 - Which of the following is the best and only completely secure method of data destruction?      
A. Degaussing     
B. Crypto-shredding     
C. Physical destruction of resources that store the data      
D. Legal order issued by the prevailing jurisdiction where the data is geographically situated     
Answer: C. 

Destroying the drive, disk, and media where the data resides is the only true, complete method of data destruction.
Options A and B are also good methods for data destruction, but neither is the best method.
Option D is incorrect because a legal order is not a secure method of data destruction and therefore it cannot be the correct answer.

### Question # 135 - Aside from the fact that the cloud customer probably cannot reach the physical storage assets of the cloud provider and that wiping an entire storage space would impact other customers, why would degaussing probably not be an effective means of secure sanitization in the cloud?       
A. All the data storage space in the cloud is already gaussed.      
B. Cloud data storage may not be affected by degaussing.      
C. Federal law prohibits it in the United States.       
D. The blast radius is too wide.        
Answer: B. 

Cloud data storage likely uses solid-state drives (or disks), which are not affected by degaussing because they don’t use magnetic properties to store data.
Option A is incorrect because it is untrue. A gauss is a unit of magnetism. Not all data storage devices in the cloud are magnetic. Some storage space does not require magnetism to work. Solid State Drives (SSDs) are an example of a type of storage space that does not rely on magnetism to store data.
Federal law does not prohibit degaussing of magnetic media in the United States so option C is incorrect.
Option D is incorrect because process of degaussing magnetic media does not produce a blast and therefore it does not produce a blast radius.

### Question # 136 - Is overwriting a feasible secure sanitization method in the cloud?     
A. Yes, but only if you use multiple passes.    
B. No, because you can’t get physical access to cloud storage resources.        
C. Yes, but it requires a final pass with all zeros or ones.         
D. No, because the logical location of the stored data is almost impossible to determine.       
Answer: D.       

Overwriting is the practice of filling the entire storage of the target data with randomized characters (usually involving multiple passes and a final pass with a single, repeated character). In the cloud, this is untenable for many reasons, including the fact that cloud data is constantly moving from one storage resource to another and is not kept in a single, identifiable logical location for an extended period of time (which is actually a security benefit). Without you knowing which storage resources to overwrite, overwriting is impossible.

All the other options are only distractors. Options A and C describe elements of the overwriting process but not reasons why it’s challenging in the cloud. Option B is true, but overwriting does not require physical access, so the option is incorrect.

### Question # 137 - All of the following are reasons overwriting is not a viable secure sanitization method for data stored in the cloud except _______________.      
A. Overwriting an entire storage resource would affect other tenants’ data          
B. Regulators usually frown on the practice        
C. Locating the specific storage locations of cloud data is almost impossible       
D. Data is being backed constantly in the cloud; before you finished overwriting an entire data set, it would have been replicated elsewhere      
Answer: B. 

Regulators do not disapprove of secure sanitization; it is an acceptable form of secure data destruction if implemented properly.
All the other answers are actual reasons overwriting is not a viable secure sanitization method in the cloud.
  
### Question # 138 - Which of the following might make crypto-shredding difficult or useless?      
A. The cloud provider also managing the organization’s keys     
B. Lack of physical access to the environment     
C. External attackers      
D. Lack of user training and awareness      
Answer: A. 

Crypto-shredding relies on the eventual destruction of the final keys; if keys are not under the management of the customer, they may be replicated or difficult to dispose of.
The lack of physical access to the cloud environment should not affect the crypto-shredding process, so option B is incorrect.
External attackers should not affect the crypto-shredding process, so option C is incorrect.
Crypto-shredding should not require input or activity from users, so option D is incorrect.

### Question # 139 - Crypto-shredding requires at least ____ cryptosystem(s).     
A. One     
B. Two     
C. Three     
D. Four     
Answer: B.    

The proper procedure for crypto-shredding requires two cryptosystems: one to encrypt the target data, the other to encrypt the resulting data encryption keys.
All the other answers are wrong and just distractors.

### Question # 140 - In addition to having it for business continuity and disaster recovery (BC/DR) purposes, data archiving might also be useful for _______________.     
A. Ensuring profitability     
B. Increasing performance      
C. Motivating users      
D. Correcting accidental errors      
Answer: D. 

If users inadvertently erase or modify data, an archived backup copy could be useful for restoring the original, correct version.
All the other answers are incorrect; archiving does none of those things.

### Question # 141 - In addition to having it for business continuity and disaster recovery (BC/DR) purposes, data archiving might also be useful for _______________.       
A. Team building and morale    
B. Forensic investigation     
C. Choosing security controls     
D. Enhancing quality       
Answer: B.    

An archived data set could be useful for investigative purposes, especially if it covers a significant period of time and includes multiple copies. The archived versions may be used as a reference to determine when a certain malicious activity occurred, which is useful during an investigation.
All the other answers are incorrect; archiving does not aid in these functions.

### Question # 142 - In addition to having it for business continuity and disaster recovery (BC/DR) purposes, data archiving might also be useful for _______________.     
A. Compliance/audit    
B. Monitoring performance     
C. Gathering investment      
D. Enforcing policy    
Answer: A.       

Archiving may be required by regulation, and archived versions of the environment or data may be used to create deliverables for auditors, especially if the archive included event logs.
Archived data is not an optimum gauge of performance because it is not “live” data—that is, the archived data is no longer in the operational environment and so is not a useful indicator of how well that environment currently operates. Option B is therefore incorrect.
Archiving has nothing to do with investment; option C is incorrect.
Archiving may occur as the result of policy but is not an enforcement tool; thus, option D is incorrect.

### Question # 143 -  Who is responsible for performing archiving activities in a managed cloud environment?    
A. The cloud customer     
B. The cloud provider    
C. The customer’s regulator     
D. Depends on the contract      
Answer: D. 

Many cloud providers will offer archiving services as a feature of the basic cloud service; realistically, most providers are already performing this function to avoid inadvertent loss of customer data, so marketing it is a logical step. However, because the customer is ultimately responsible for the data, the customer may elect to use another, or an additional, archive method. The contract will stipulate specific terms, such as archive size, duration, and so on.
Either the cloud customer or provider (or both) may perform archiving, depending on the contract terms, so options A and B are incorrect.
Regulators do not perform archiving; option C is incorrect.

### Question # 144 -  Data archiving and retention policies should include __________.     
A. How long the data must be kept before destruction     
B. The depth of underground storage bunkers used for archiving     
C. The names of specific personnel tasked with restoring data in the event of data loss in the operational environment      
D. The name(s) of regulators approving the policy     
Answer: A. 

The policy for data archiving and retention must include guidance on the length of time data is expected to remain stored.
Describing or prescribing the physical specifications of a secure archive facility is probably beyond the responsibility or requirements of a data owner (and belowground storage is not a requirement for archiving and retention), so option B is incorrect.
Although it is important to task and train personnel to take part in data restoration from archived data, naming the specific personnel in the policy is not an optimum or useful practice, so option C is incorrect.
Although management is responsible for publishing and promulgating policy and governance, the name of the specific manager is not the essential element (but their office or position is). Regulators don’t personally approve internal policies of the organizations they oversee, so option D is incorrect.

### Question # 145 -  What should data archiving and retention policies include?     
A. Names of personnel allowed to receive backup media, if third-party off-site archiving services are used     
B. Explicit statement of data formats and types of storage media     
C. A list of personnel whose data will be archived on a regular basis         
D. Which Internet service provider (ISP) should be used for backup procedures      
Answer: B.       

It is important to indicate the data format and media type for long-term storage in order to ensure restoration capability; outdated or obsolete data formats and media may not be useful for restoration of data to the operational environment several years after it has been stored.

Options A and C are not correct because specific names don’t belong at the policy level of governance; the specific names (or identification credentials) of allowed third-party recipients should be included at the process/procedure level of governance, and a list of offices or departments whose data will be archived can be included in the policy.

Option D is not correct because the particular ISP should not have any bearing on the archiving policy.

### Question # 146 -  If the organization operates in a cloud environment, security operations procedures should include specific contact information for all of the following except _______________.    
A. Applicable regulatory entities    
B. Federal and local law enforcement     
C. The originator or publisher of the governing policy    
D. The cloud provider’s security response office     
Answer: C.      

Once the policies have been published and put into force, the names and contact information of the people who crafted them are no longer useful or germane.
All the other options represent entities that the organization may want to contact in the event of a security incident or breach and so should be included in security procedure documentation.

### Question # 147 -  If the organization operates in a cloud environment, security operations procedures should include guidance for all of the following audit or logging processes except _______________.     
A. Definition of security events and incidents     
B. The brand or vendor of the cloud provider’s audit or logging tool     
C. Process for adding new audit or logging rules    
D. Process for filtering out false positives by amending the rule set     
Answer: B.     

This is a question that requires some thought. All the answers are processes or elements that should be included in the security operations’ procedures except for option B; the cloud customer will not get to select, or probably even know, what tools and devices the cloud provider has put into place, so this will not be included in the customer’s procedures.

### Question # 148 -  What does nonrepudiation mean?     
A. Prohibiting certain parties from a private conversation     
B. Ensuring that a transaction is completed before saving the results     
C. Ensuring that someone cannot turn off auditing capabilities while performing a function     
D. Preventing any party that participates in a transaction from claiming that it did not    
Answer: D. 

Option D is the definition of nonrepudiation.

Option A is a description of confidentiality.

Option B is an element of the Atomicity, Consistency, Isolation, Durability (ACID) test to enhance the utility and security of a database.

Option C is a technique to reduce the likelihood of nonrepudiation but not the definition of the term.
