# Domain 2 Important Questions 3

### Question # 1 - An email is an example of what type of data?     
A.	Structured data.   
B.	Semi- structured data.   
C.	RFC- defined data.   
D.	Unstructured data.

Answer: D     

### Question # 2 - Nick wants to ensure that data is properly handled once it is classified. He knows that data labeling is important to the process and will help his data loss prevention tool in its job of preventing data leakage and exposure. [When should data be labeled in his data] lifecycle?       
A.	Creation.  
B.	Storage.  
C.	Use.  
D.	Destruction.  

Answer: A            

### Question # 3 - Jacinda is planning to deploy a data loss prevention (DLP) system in her cloud environment. Which of the following challenges is most likely to impact the ability of her DLP system to determine whether sensitive data is being [transmitted outside of her organization]? 
A.  Lack of data labeling.     
B.	Use of encryption for data in transit.  
C.	Improper data labeling.  
D.	Use of encryption for data at rest.  

Answer: B               

### Question # 4 - Susan wants to ensure that [super user access] in her cloud environment can be properly audited. Which of the following is [not a common item required] for auditing of privileged user access?    
A.	The remote IP address.  
B.	The account used.  
C.	The password used.  
D.	The local IP address.  

Answer: C      

### Question # 5 - 	Ben’s organization uses the [same data deletion procedure for their on-site systems and their third-party-provided, cloud-hosted systems]. Ben believes there is a problem with the process currently in use, which involves [performing a single-pass zero-wipe of the disks and volumes in use before they are reused]. What problem with this approach should Ben highlight for the cloud environment?   
A.	Crypto- shredding is a secure option for third- party- hosted cloud platforms.  
B.	Zero- wiping alone is not sufficient, and random patterns should also be used.  
C.	Zero- wiping requires multiple passes to ensure that there will be no remnant data.   
D.	Drives should be degaussed instead of wiped or crypto- shredded to ensure that data is fully destroyed at the physical level.   

Answer: A                	

### Question # 6 - Jason has been informed that [his organization needs to place a legal hold] on [information] related to pending litigation. What action should he take to place the hold?   
A.	Restore the files from backups so that they match the dates for the hold request.  
B.	Search for all files related to the litigation and provide them immediately to opposing counsel.   
C.	Delete all the files named in the legal hold to limit the scope of litigation.   
D.	**Identify scope files and preserve them until they need to be produced.**   

Answer: D             

### Question # 7 - Murali is reviewing a customer’s file inside of his organization’s customer relationship management tool and sees the customer’s Social Security number listed as XXX- XX- 8945. What [data obfuscation] technique has been used?   
A.	Anonymization.  
B. 	Masking.  
C.	Randomization.  
D.	Hashing.  

Answer: B      

Masking data involves **replacing data with alternate characters like X or** *. 
		This is typically done via controls in the software or database itself, as the underlying data remains intact in the database. 
**Anonymization or deidentification [removes data] that might allow individuals to be identified**. 
**Hashing is used to allow data to be referenced by a hash without displaying the actual data, but it causes properties of the data that may be needed for testing to be lost**. 
Randomization or shuffling data moves it around, disassociating the data but leaving real data in place to be tested.

### Question # 8 - 	An XML file is considered what type of data?    
A.	Unstructured data.  
B.	Restructured data.  
C.	Semi- structured data.  
D.	Structured data.  

Answer: C              

### Question # 9 - Lucca wants to [implement logging] in an infrastructure as a service cloud service provider’s environment for his Linux instances. He wants to capture events like creation and destruction of systems, as part of scaling requirements for performance. What logging tool or service should he use to have the most insight into these events?   
A.	Syslog from the Linux systems.  
B.	**The cloud service provider’s built- in logging function**.  
C.	Syslog- NG from the Linux systems.  
D.	Logs from both the local event log and application log from the Linux systems.  

Answer: B                 

### Question # 10 - Joanna’s company uses a load balancer to distribute traffic between multiple web servers. What data point is often lost when traffic passes through load balancers to local web servers in a cloud environment?    
A. The source IP address.      
B.	The destination port.  
C.	The query string.   
D.	The destination IP address.   

Answer: A                

### [important] Question # 11 - 	Isaac is using a hash function for both integrity checking and to allow address data to be referenced without the actual data being exposed. Which of the following attributes of the data will be [not be lost] when the data is hashed?   
A.	Its ability to be uniquely identified. 
B.	The length of the data.  
C.	The formatting of the data.  
D.	The ability to sort the data based on street number.  

Answer: A        

Hashing **converts variable length data to fixed- length outputs, meaning that the length, formatting, and the ability to perform operations on the data using strings or numbers will be lost**. 
Its ability to be uniquely identified won’t be lost— Isaac just needs to know the hash of a given address to continue to reference that data element.

### Question # 12 - Amanda’s operating procedures for [secure data storage require] her to ensure that she is using [data dispersion] techniques. What does Amanda need to do to be compliant with this requirement?    
A.	Delete all data not in secure storage.   
B.	Store data in more than one location or service.     
C.	Avoid storing data in intact form, requiring data from more than one location to use a data set.     
D.	Geographically separate data by at least 15 miles to ensure that a single natural disaster cannot destroy it.     

Answer: B       

### Question # 13 - 	Lisa runs [Windows] instances in her cloud- hosted environment. Each Windows instance is created [with a C: drive] that houses the operating system and application files. What type of storage best describes the C: drive for these Windows instances?    
A.	Long- term storage.  
B.	**Ephemeral storage**.    
C.	Raw storage.   
D.	Volume- based storage.   

Answer: B       

[important] **Storage** that is associated with an instance **that will be destroyed when the instance is shut down is ephemeral storage**. 
Raw storage is storage that you have direct access to **like a hard drive, or an SSD that has access to the underlying device**. 
**Long- term storage** is storage that is **intended to continue to exist, and is often used for logs or data storage**. 
**Volume- based** storage is storage **allocated as a virtual drive or device within the cloud**.

### [important] Question # 14 - Steve is working to classify data based on his organization’s data classification policies. Which of the following is [not] a common type of classification?    
A.	Size of the data.   
B.	Sensitivity of the data.  
C.	Jurisdiction covering the data.  
D.	Criticality of the data.   

Answer: A       


### [important] Question # 15 - Chris is reviewing his data lifecycle and wants to take actions in the data creation stage that can help his data loss prevention system be more effective. Which of the following actions should he take to improve the success rate of his DLP controls?    
A.	Data labeling.   
B.	Data classification.   
C.	Hashing.    
D.	Geolocation tagging.   

Answer: A       

[important] **Data labels can help DLP systems identify and manage data**, 
so Chris should ensure that data is labeled as part of its creation process to help his DLP identify and protect it. 
[important] **Classification is important, but without tags it won’t be useful to the DLP**. 
Hashing can be used to help a DLP identify specific files, but tends to be done by the DLP system itself if needed, and geolocation tagging is not a typical DLP protection.

### Question # 16 - Gary is gathering data to support a legal case on behalf of his company. Why might he digitally sign files as they are collected and preserve them along with the data in a documented, validated way?    
A.	To allow for data dispersion.   
B.	To ensure the files are not copied.	  
C.	To keep the files secure by encrypting them.   
D.	To support nonrepudiation.   

Answer: D       

### Question # 17 - Valerie is [performing a risk assessment] for her cloud environment and wants to [identify risks] to her [organization’s ephemeral volume- based storag]e used for system drives in a scalable, virtual machine–based environment. Which of the following is [not] a threat to ephemeral storage?      
A.	Inadvertent exposure.  
B.	Malicious access due to credential theft.   
C.	Poor performance due to its ephemeral nature.   
D.	Loss of forensic artifacts.   

Answer: C       

### [ critical and important ] Question # 18 - Which storage type is most likely to have remnant data issues in an environment in which the storage is reused for other customers after it is reallocated if it is not crypto- shredded when it is deallocated and instead is zero- wiped?    
A.	Ephemeral storage.   
B.	Raw storage.   
C.	Long-term storage.   
D.	Magneto- optical storage.  

Answer: B    

**Raw storage provides direct access to a disk, and without crypto- shredding is likely to have remnant data on the disk after it is used**. 
**Since long- term and ephemeral storage is typically abstracted, it is less likely to have remnant data in unallocated or reallocated sectors that would not be purged through typical wipe operations**

### Question # 19 - Kathleen wants to perform data discovery across a large data set and knows that some data types are more difficult to perform discovery on than others. Which of the following data types is the hardest to perform discovery actions on?    
A.	**Unstructured data**.  
B.	Semi- structured data.   
C.	Rigidly structured data.   
D.	Structured data.   

Answer: A       

### Question # 20 - Isaac wants to filter events based on the country of origin for authentications. What log information should he use to perform a best- effort match for logins?      
A.  userID.   
B.	IP address.   
C.	Geolocation.   
D.	MAC address.   

Answer: C       

### [important] Question # 21 - Charleen wants to use a [data obfuscation method] that [allows realistic data to be used without the data being actual data associated with specific users or individuals]. What data obfucation method should she use?    
A.	Hashing.  
B.	Shuffling.  
C.	Randomization.  
D.	Masking.  

Answer: B       

While there may be some concerns about real data being used, Charleen’s goal is to have actual data for testing, making shuffling her best option. Hashing, randomization, and masking all remove or modify data in meaningful ways, resulting in testing not being as accurate as it might be against real- world data

### Question # 22 - Michelle wants to [track deletion of files] in an object storage bucket. What potential issue should she be aware of if [her organization makes heavy use of object- based storage for storage of ephemeral files]?          
A.	The logging may not be accurate.    
B.	Logging may be automatically disabled if too many events occur.     
C.	Creation and deletion events cannot be logged in filesystems.     
D.	**The high volume of logging may increase operational costs**.    

Answer: D       

### Question # 23 - Diana is outlining the labeling scheme her organization will use for their data. Which of the following is not a common data label?     
A.	Creation date     
B.	**Data monetary value**     
C.	Date of scheduled destruction     
D.	Confidentiality level     

Answer: B       

### [important] Question # 24 - Susan wants to be prepared for [legal holds]. What [organizational policy] often accounts for legal holds?      
A.	Data classification policy     
B.	Retention policy     
C.	Acceptable use policy      
D.	Data breach response policy      

Answer: B       

**Retention policies often include language that addresses legal holds because holds can impact retention practices and requirements**. 
Data classification, acceptable use, and data breach response policies typically do not include legal hold language.

### Question # 25 - Henry wants to follow the OWASP guidelines for key storage. Which of the following is [not] a best practice for key storage?     
A.	Keys must be stored in plaintext to allow for access.     
B.	Keys must be protected in both volatile and persistent memory.     
C.	Keys stored in databases should be encrypted using key encryption keys.      
D.	Keys should be protected in storage to ensure that they are not modified or changed inadvertently.      

Answer: A       

### Question # 26 - Marco wants to implement an information rights management tool. What phase of the data lifecycle relies heavily on IRM to ensure the organization retains control of its data?     
A.	Create   
B.	Store   
C.	Share    
D.	Destroy    

Answer: C       

### [important] Question # 27 - JSON is an example of what type of data?      
A.	Structured data  
B.	Semi- structured data   
C.	Unstructured data     
D.	Labeled data     

Answer: B       

XML and JSON are both examples of semi- structured data. Other examples include CSV files, XML, NoSQL databases, and HTML files

### Question # 28 - 	Charleen wants to [perform data discovery] on her organization’s data, which is stored in [archival storage] hosted by her organization’s cloud service provider. What issue should she point out about this discovery plan?    
A.	**It may be slow and costly due to how archival storage is designed and priced**.    
B.	The data may not exist because it has been archived.     
C.	The discovery process cannot be run against archival storage because it is not online under normal circumstances.    
D.	The data will need to be decrypted before being scanned for discovery purposes.     

Answer: A       

### [important] Question # 29 - 	Ujama’s manager has asked him [to perform data mapping] to prepare for his next task. What will Ujama be doing?     
A.	Adding data labels to unstructured data     
B.	**Matching fields in one database to fields in another database**      
C.	Identifying the storage locations for files of specific types on system drives      
D.	Building a file and folder structure for data storage     

Answer: B       

### Question # 30 - Lin wants to ensure that her organization’s data labels remain with the data. How should she label her data to give it the best chance of retaining its labels?      
A. 	Embed the labels in the filename.      
B.	Add the labels to the file’s content at the beginning of the file.      
C.	Add labels to the file metadata.     
D.	Add the labels to the file’s content at the end of the file.     

Answer: C       

### [important] Question # 31 - 	Nina’s organization has lost the cryptographic keys associated with one of their cloud- based servers. What can Nina do to recover the data the keys were used to protect? 
A. Generate new keys to recover the data.   
B. Use the passphrase for the keys to recover the keys.      
C. Reverse the hash that was used to encrypt the data.      
D. The data is lost and Nina cannot recover it.    

Answer: D       

### Question # 32 - 	Madani is planning to perform data discovery on various data sets and files his organization has. On which type of data will discovery be most easily performed?      
A.	Unstructured data     
B.	Semi- structured data      
C.	Encrypted data     
D.	Structured data     

Answer: D       

### Question # 33 - Ashley tracks the handling of a forensic image, including recording who handles it, when it was collected and when each transfer occurs, and why the transfer occurred. What practice is Ashley performing?      
A.	**Documenting chain of custody**    
B.	Ensuring repudiation     
C.	A legal hold    
D.	Forensic accounting     

Answer: A       

### [tricky and important] Question # 34 - Which of the following is [not a common goal] of data classification [policies]?    
A.	Identifying classification levels     
B.	Assigning responsibilities     
C.	Defining roles     
D.	Mapping data      

Answer: D       

### Question # 35 - Hiroyuki wants to [optimize his organization’s data labeling process]. How and when should he implement data labeling to be most efficient and effective?     
A.	Manual labeling at the data creation stage    
B.	Automated labeling at the data creation stage    
C.	Automated labeling at the data use stage    
D.	Manual labeling at the data use stage     

Answer: B       

### [important] Question # 36 - Jen wants to ensure that keys used by individuals in her organization can be handled [properly]. Which of the following is [not] a best practice for [handling long- term keys] in use by humans?     
A.	Anonymize access using the key    
B.	Identify the key user    
C.	Identify when the key is used     
D.	Uniquely tag the keys     

Answer: A       

**Anonymizing access using a key removes the ability to provide accountability and works against organizational best practices**. 
Identifying the key, the user, and when and how it is used supports accountability for usage

### Question # 37 - Danielle wants to ensure that the data stored in her cloud- hosted datacenter is properly destroyed when it is no longer needed. Which of the following options should she choose?     
A.	Physical destruction of the media    
B.	Crypto- shredding    
C.	Degaussing    
D.	Overwriting    

Answer: B       

### [important] Question # 38 - 	Charles wants to use [tokenization] as a security practice for his organization’s data. What technical requirement will he have to meet to accomplish this?     
A.  He will need to encrypt his data.    
B.	**He will need two distinct database**s.     
C.	He will need to use a FIPS 140- 2 capable cryptographic engine to create tokens.     
D.	He will need to deidentify the data.    

Answer: B      

**Tokenization relies on two distinct databases, one with actual data and one with tokenized data**. 
Token servers then pull the data the token represents from the real data database when needed. 
This process does not require encryption, specify FIPS 140 requirements, or involve deidentification practices.

### [important] Question # 39 - Once Charles has his two databases ready, [what step comes next in the tokenization process]?     
A.	**Data discovery to identify sensitive data**     
B.	Tokenization of the index values     
C.	Hashing each item in the database      
D.	Randomization of data in the database to prepare for tokenization     

Answer: A       

### Question # 40 - 	Jack wants to understand how data is used in his organization. What tool is often used to help IT professionals understand where and how data is used and moved through an organization?      
A. 	Data classification    
B.	Data mapping     
C.	Dataflow diagrams     
D.	Data policies     

Answer: C       

### Question # 41 - Annie has a database with a field titled “chosen name” and she has another database with a field titled “name.” She knows that these fields are used for the same purpose in her organization and wants to use data from both databases. What process could she use to match these and other fields to allow her to do so more easily?     
A.	Data mapping     
B.	Column consolidation     
C.	Data labeling     
D.	Columnar aggregation      

Answer: A       

### Question # 42 - Which of the following items is [not] commonly included in dataflow diagrams?    
A.	Data types or fields    
B.	Services 
C. 	Systems    
D. 	**Data lifespan information**     

Answer: D       

### [tricky] Question # 43 - 	Jim’s organization wants to implement cryptographic erasure as their primary means of destroying data when they are done with it. What first step is required to support this through the data’s lifecycle?     
A.	Hash all of the data at creation.     
B.	Zero- wipe drives before they are used to ensure no previous data is resident.    
C.	Encrypt the drive or volume at creation.     
D.	All of the above.    

Answer: C       

### Question # 44 - 	Charles wants [to store data in a relational database], which uses columns and tables that describe the data. Which of the following types of data cannot be easily stored in a relational database other than as a text blob?    
A.	Structured data    
B.	Semi- structured data    
C.	Unstructured data    
D.	All of the above    

Answer: C       

### [important] Question # 45 - Olivia wants [to write a data retention policy] for her organization. Which list best describes common components of a retention policy?    
A.	Retention periods, regulatory compliance requirements, data classification, data deletion and lifespan, and archiving and retrieval procedures.     
B.	Retention periods, logging, data classification, data deletion processes, and compliance requirements.    
C.	Data classification requirements, regulatory compliance requirements, data creation and tagging requirements, and data retrieval procedures.    
D.	Regulatory and compliance requirements and mapping to retention periods for the organization, legal hold processes, and data deletion requirements.   

Answer: A       

### Question # 46 - Hui wants to revoke a certificate issued by her information rights management (IRM) system. How can she verify that the certificate has been revoked?     
A.	Issue a new certificate using the same information as the original certificate.    
B.	Attempt to access the data using her own certificate.     
C.	**Check the IRM’s certificate revocation list**.     
D.	Delete the private keys for the original certificate.    

Answer: C       

### [important] Question # 47 - 	Frank’s organization is preparing to adopt an information rights management tool. What IRM capability focuses on providing rights to individuals based on their roles to ensure appropriate data access?     
A.	Tagging.   
B.	Data labeling.   
C.	Encryption.  
D.	Provisioning.   

Answer: D       

The **provisioning capability of IRM systems** focuses on **providing rights to individuals based on roles and job functions**. 
Tagging and data labeling are used to ensure that data is handled appropriately based on rules. Encryption secures data at rest and in transit

### [important] Question # 48 - Randy is following his organization’s data classification policy and tags data that was identified in the organization’s business impact analysis. What type of classification is Randy performing?     
A. 	**Criticality**.   
B.	Jurisdiction.   
C.	Security.   
D.	Sensitivity.   

Answer: A       

Business impact analysis helps to determine what data is needed to continue the operations of the business. This is an assssment of the criticality of the data, and Randy knows that the data he flags may be necessary in the event of a disaster or other business continuity issue

### Question # 49 - Susan is concerned that her organization doesn’t understand how a critical application works in their cloud environment. Recent issues indicate that her organization’s developers and cloud architects have different ideas about how systems and services work together. What should Susan prepare to help document and explain how systems and services work together?    
A.	Data classification.   
B.	A business impact analysis.  
C.	A dataflow diagram.  
D.	Data mapping.  

Answer: C       

### [important and thinking] Question # 50 - Jane is considering [data dispersion as a security and availability strategy] for her organization. What risk should she highlight as the [most] significant potential problem if her organization does adopt a [multivendor approach to dispersion]?     
A.	Data dispersion makes it difficult to encrypt data.    
B.	Geographic dispersion may impact performance.    
C.	**An outage at a provider may result in data not being available**.  
D.	Most cloud vendors do not offer support for dispersion.   

Answer: C       

### Question # 51 - 	Selah is implementing an information rights management system. What requirement will she encounter if she wants to control files on workstations and laptops?   
A.	The need to deploy a cloud- native server.  
B.	The need to install an agent on endpoint devices.  
C.	The need to deploy an on- site server.  
D.	The need to install an agent on cloud- based systems.   

Answer: B       

### Question # 52 - 	Audio and video files are examples of what type of data?  
A.	**Unstructured data**. 
B.	Sensitive data. 
C.	Labeled data.   
D.	Structured data.    

Answer: A       

### Question # 53 -	Wayne wants to perform data discovery on a very large data set stored in a cloud service using a tool that is hosted in a different cloud service, which will require copying the data to the cloud where the tool resides. What is the primary cost concern he should consider when evaluating an option like this?    
A.	The cost of the storage tier the data is currently in    
B.	Ingress and egress fees for moving the data between cloud services    
C.	The cost of logs generated by the discovery process in the cloud where it is hosted    
D.	The cost of logs generated by the discovery process in the cloud where the data resides      

Answer: B       

### Question # 54 -	Amanda’s organization uses a [chain of custody process] for forensic data and has captured a drive image from a compromised system hosted in their cloud environment. Amanda wants to analyze the drive without causing issues that might result in repudiation of the drive image or an issue with the chain of custody of the image. What actions should she take to analyze the drive?        
A.	Analyze the drive while connected to a forensic write- protect device.       
B.	Analyze the drive using only approved forensic software.      
C.	Make a copy of the original image, validate it, and then analyze the copy.      
D.	Log all actions taken on the original copy of the drive to maintain a chain of custody.      

Answer: C       

### Question # 55 -	Which of the following is not a common information rights management tool control capability?       
A.	Preventing taking a screenshot or photo of the displayed text        
B.	Disabling copying of text     
C.	Preventing local copies from being saved     
D.	Disallowing printing      

Answer: A       

### Question # 56 -	Felix operates his organization’s cloud resources in multiple countries, including member states of the European Union. What is the most significant concern Felix should express about conducting data discovery across data sets contained in their cloud storage?      
A.	Costs may vary across difference regions, making it difficult to estimate the price for the discovery.       
B.	Regulatory requirements will vary across different locations and may make compliance difficult during discovery.      
C.	Structured data will be harder to process than unstructured data, making inter- region discovery challenging.    
D.	Encryption may not be allowed between regions, making the discovery less secure.     

Answer: B       

### Question # 57 -	Jason wants to [lower] the ongoing cost of using storage in his cloud infrastructure as a service environment for logs and other data that is infrequently accessed. What should he consider doing with the data?     
A.	Delete the data to save costs.    
B.	Archive the data to a lower cost storage tier.     
C.	Move the data to a third- party service provider to reduce costs.     
D.	Archive the data to a higher performance storage tier.      

Answer: B       

### [important] Question # 58 -	Frank knows that his organization adds data labels for data during its creation. What additional phase of the cloud data lifecycle often includes data labels as data is combined or modified?       
A. 	Store    
B.	**Use**      
C.	Sharing    
D.	Deletion     

Answer: B       

### Question # 59 -	Chris wants to send data from his web application to client systems securely. What encryption  protocol should he use?        
A.	SSL     
B.	MD5     
C.	SHA- 1      
D.	TLS     

Answer: D       

### Question # 60 -	Kathleen’s organization uses a technique known as [bit-splitting] that [breaks up encrypted information] across multiple cloud services to make it more difficult to acquire and recover the data. What cloud data concept best describes activities like this?      
A.	Data dispersion    
B.	Data mapping     
C.	Business continuity     
D.	Dataflows     

Answer: A       

technique known as [bit-splitting] that [breaks up encrypted information] across multiple cloud services to make it more difficult to acquire and recover the data

### Question # 61 -	Gurleen’s organization has preserved data due to a legal hold, but the data has hit the end of its retention timeframe due to statutory requirements. What should Gurleen do?     
A.	Contact the appropriate government agency about the statute to inquire about the legal hold.       
B.	Delete the data based on the statutory requirements.      
C.	Continue to preserve the data to meet the legal hold requirements.      
D.	Make a copy of the data for the legal hold and delete the original data.      

Answer: C       

### Question # 62 -	Quentin’s organization uses ephemeral storage that is attached to systems when they are instantiated in the organization’s cloud-hosted environment. What will happen when the instances are terminated?        
A.	The volume will be retained to be used with a future instance.      
B.	The volume will be wiped and reused for the next instance owned by Quentin’s organization that is instantiated.    
C.	The data will be moved to a long- term storage tier until it is manually deleted.     
D.	**The storage will be wiped and reclaimed by the provider to be allocated elsewhere**.     

Answer: D       

### [knowledge] Question # 63 -	Renee wants to [set a retention period for log files] in her data retention [policy] that minimizes the ongoing cost of retention. What retention period should she select for ephemeral logs that do not have a contractual or legal requirement for retention?     
A.	**45 days**    
B.	6 months    
C.	3 years    
D.	7 years     

Answer: A       

**Ephemeral data is often kept for shorter time periods like 45 days**, 
a time period sufficient to allow investigations without building up large volumes of data that will not be used and which can be expensive to store. 
Longer- term storage may be required by law or contracts or due to specific contractual requirements.
⚡ Exam Tip (CCSP/CISSP) - If question says "no legal or regulatory requirement" → **choose shortest retention** (cost-effective, lower risk).
If financial → 5 or 7 years (depending on law).
If healthcare → 6 years (HIPAA).
If tax/audit → 7 years (SOX/IRS).
If security logs → minimum 1 year (PCI DSS), often 3 years internally.

### Question # 64 -	Brian has been tasked with [performing a cryptographic erasure] process on an encrypted drive. What steps does he need to take to ensure that the data is securely destroyed?      
A. 	Destroy all copies of the encryption key.      
B.	Encrypt, then decrypt the drive.         
C.	Decrypt, then re- encrypt the drive with a new key.            
D.	Degauss the drive, then zero- wipe it.        

Answer: A       

### Question # 65 -	Lincoln wants to identify threats to the availability of data stored in a [long- term storage  service like Amazon’s Glacier]. Which of the following threats should he identify as impacting availability?     
A.	Service outages     
B.	Credential theft     
C.	Improper permissions     
D.	Lack of encryption     

Answer: A       

### [important] Question # 66 -	Theresa wants to identify endpoint systems rather than users for her information rights management system. What is typically used to identify a system to an IRM?       
A. A system name     
B.	An IP address    
C.	A user ID and password          
D.	**A certificate**     

Answer: D       

### Question # 67 -	Derek’s organization uses a cryptographic one- way function applied to data in a database to allow it to be referenced without using the actual data. What anonymization technique are they using? 
A. 	Anonymization     
B.	Masking         
C.	**Hashing**       
D.	Shuffling        

Answer: C       

### [important] Question # 68 -	Henry stores his cloud environment’s log files [in a filesystem designed for durability and performance for logs]. What type of storage is he using?      
A.	Long- term storage     
B.	Ephemeral storage    
C.	Raw storage    
D.	Volume- based storage    

Answer: A       

### [important] Question # 69 -	Alaina’s organization uses a secrets management service provided by their cloud service provider. Alaina knows that the secrets are critical to the operations of the service and wants to implement a [“break- glass”] emergency procedure in case the service is unavailable. Which of the following is not a common best practice for this type of secrets recovery capability?    
A. 	Build an automated backup system for secrets.     
B.	Test the restore process for secrets regularly.      
C.	Use a second instance in the original provider’s cloud for the backup system.     
D.	Encrypt backups and place them on secure storage.    

Answer: C       

### [important] Question # 70 -	Alaina wants to [implement secrets detection] to help identify issues with [secrets exposure]. Which of the following techniques will most easily help her organization detect poor practices in internal test environments without undue risk?     
A.	Use a secrets manager for development, test, and production to keep secrets secure.       
B.	**Use standard test secrets and search for them**.     
C.	Use multiple detection utilities to reduce the chance of missing a secret.     
D.	Use high entropy secrets to limit the possibility of guessed secrets.     

Answer: B       

### Question # 71 -	Angie wants to [move 100 terabyte]s of her organization’s data to archival class storage in her cloud provider’s environment. Which of the following decision points will be most impactful when deciding on cost of the new solution?        
A.	The amount of data to be archived      
B.	The type of data     
C.	The sensitivity of the data     
D.	Retrieval time    

Answer: D       

### Question # 72 -	What process is shown in the following figure?       

DB1     
Name     
Primary email     
Home phone    
	 	
DB2     
Firstnamelastname     
Preferred_email     
Cell phone    
Home phone    
Business phone    

A.	Field hashing     
B.	Table matching      
C.	String comparison     
D.	Data mapping     

Answer: D       

### [important] Question # 73 -	Wei’s organization is implementing an information rights management system. What IRM process ensures that users receive the rights and privileges they need to access files protected by the IRM?      
A.	Tagging     
B.	**Provisioning**     
C.	Labeling    
D.	Data mapping    

Answer: B       

### [important] Question # 74 -	Dana is preparing to [move her organization’s data to cloud archival storage]. Which of the following [is the most] important consideration related to [performance] for archival storage?     
A.	The cost of the storage    
B.	Data access patterns    
C.	The volume or amount of data    
D.	The amount of time the data will be stored for   

Answer: B       

### Question # 75 -	What [role] defined by a [data classification policy] holds the overall responsibility for data and is typically a member of senior management? 
A.	The data custodian      
B.	**The data owner**     
C.	The data processor     
D.	The data user     

Answer: B       

### [important] Question # 76 -	Elaine’s organization [has suffered a data breach], and [tokenized data has been exposed]. What concern should Elaine express about the tokenized data? 
A. 	It can be un- hashed to reveal the original data.      
B.	Tokenized data does not create a data breach concern.             
C.	**Tokenized data is only a concern if the database it is matched with is also exposed**.           
D.	Tokenized data could be decrypted if the encryption key for the tokens was also stolen.         

Answer: C       

### Question # 77 -	Asha wants to be able to [easily restore files] in her [cloud] service environment if a change is accidentally made. What feature could she use to allow easy restoration?      
A. 	Enable versioning.     
B.	Use a daily backup process.    
C.	Set up recurring snapshots.     
D.	Enable automatic archiving.     

Answer: A       

### Question # 78 -	Brian is reviewing his organization’s [secrets management policies and practices]. Which of the following is [not] a practice that they should use?     
A.	Reduce the number of people with administrative access to the secret store.     
B.	Regularly rotate secrets.     
C.	Maximize the rights of important secrets to reduce the total number of secrets required.     
D.	Enable logging and alerting on secrets access and usage.    

Answer: C       

### Question # 79 -	Chris wants to audit access to highly sensitive data stored in his cloud provider’s block storage service. What type of logging should he enable to monitor for use of privileged accounts to access specific buckets?      
A. 	Enable authentication logging.     
B.	Enable access logging.      
C.	Enable bandwidth monitoring.     
D.	Enable timestamps.     

Answer: B       

### Question # 80 -	Jaime is performing data discovery and wants to search for a specific term in the unstructured data she’s working with. What type of discovery is she performing?     
A. 	Label- based discovery      
B.	Metadata- based discovery     
C.	Content- based discovery     
D.	Structure- based discovery     

Answer: C       

### Question # 81 -	Mike has become aware of a certificate’s private key that has been exposed as part of an incident. What should Mike do first to limit the potential impact of the exposure?      
A. 	Immediately issue a new certificate and securely transmit it to the user.     
B.	Immediately revoke the certificate and add it to the certificate revocation list.     
C.	Search for all locations of the certificate to understand what impact its exposure may have.    
D.	Interview the user or owner to identify why the certificate was exposed.    

Answer: B       

### [important] Question # 82 -	Dan’s DLP deployment has been experiencing false positives when keying on pattern matching, resulting in extra work for his organization’s security team. What can he do to best improve the DLP’s performance if the DLP is currently relying on pattern matching as the primary means of identifying sensitive information? 
A. 	Tag data with its sensitivity level.     
B.	Apply a data lifecycle and delete unneeded data to reduce the data being monitored.       
C.	Classify data based on a classification scheme.    
D.	Use regular expressions to improve the pattern matching algorithm’s success rate.    

Answer: A       

### Question # 83 -	Olivia’s cloud environment uses ephemeral machines that are instantiated and shut down as utilization grows and shrinks. She is concerned about the ability to determine what system an event occurred on. What key data element should she ensure is recorded when each machine sends log data?      
A.	The system’s IP address     
B.	An administrative user associated with the system       
C.	A unique tag for each system instance    
D.	The system’s deletion time    

Answer: C       

### Question # 84 -	Valerie’s organization is legally allowed to dispose of specific operational data after 7 years and has an automated disposal process that removes the data based on lifecycle tags. Valerie has recently been informed that the data from one customer has been placed on a legal hold. What should she do?      
A.	Delete the data; the law allows disposal at 7 years, regardless of legal holds.          
B.	Preserve the data requested until the legal hold is over.     
C.	Retain the full data set until the legal hold is over.     
D.	Make a copy of all of the data, move it to alternate storage, and delete the original to meet both legal requirements.     

Answer: B       

### Question # 85 -	Heikki is preparing to deploy a data loss prevention system. He has []prioritized, categorized, and labeled his data]. What will he need to do to ensure that the system can help secure his organization’s data?     
A.	Establish DLP policies.     
B.	Perform data matching.     
C.	Define the data lifecycle.     
D.	Train users.     

Answer: A       

### Question # 86 -	Kara is performing data discovery on a large number of pictures and uses the data embedded in the photos, including the time it was taken, the camera, and similar data. What type of discovery is she performing?       
A. Metadata- based discovery     
B.	Content- based discovery     
C.	Tag- based discovery    
D.	Label- based discovery    

Answer: A       

### [important and tricky] Question # 87 -	Rick is informed that the development team for one of his organization’s applications is [using tokenized data for customer information]. What does Rick know based on this information?     
A. 	The actual customer information is stored in the tokenized database.      
B.	The customer data is secure because tokens cannot be breached.     
C.	A breach of the token database would result in a customer data breach.     
D.	The tokenized data can be looked up against a database that contains customer data.    

Answer: D       

### Question # 88 -	As part of an incident response process, Jack wants to validate the integrity of system instances running in his cloud environment. What can he do to quickly and efficiently check that the virtual machine images have not been modified?    
A.	Check the cloud provider’s logs for modifications to the machine.    
B.	Check hashes of machine instances against a hash of the original.     
C.	Check timestamps and dates for files on the machine against the original.    
D.	Rebuild the machine and manually compare it against the original.    

Answer: B       

### [important] Question # 89 -	Tara has backups for her cloud service stored in the long- term storage service her cloud  service provider provides and in a separate third- party long- term backup environment. What concept has Tara implemented?      
A.	Deduplication     
B.	Dispersion    
C.	Protected supply chain     
D.	Lifecycle management    

Answer: B       

### Question # 90 -	Christina’s organization operates branches in multiple countries but wants to archive its data in the organization’s primary cloud-hosting environment in North America. What is the most important concern she should raise about centralizing data in this scenario?     
A.	The need to ensure regulatory compliance     
B.	The potential for exposure as the data is moved     
C.	Transfer speeds from international locations    
D.	The fact that permissions may need to be remapped due to the move     

Answer: A       

### Question # 91 -	What cloud data lifecycle phase occurs at the question mark shown in the following figure?      
A.	Archive     
B.	Distribute    
C.	Encrypt    
D.	Use    

Answer: D       

### [tricky] Question # 92 -	Ben has used a hashing algorithm on a file. Which of the following is not something he will know about the output?     
A.	It will be of fixed length.   
B.	It will be nonreversible.    
C.	Identical files will generate identical output.    
D.	Two different files can be hashed to the same output.    

Answer: D       

### Question # 93 -	Jacinda wants to implement an information rights management solution. What phase of the cloud data lifecycle will rely heavily on the IRM to ensure that privileges are appropriately managed?        
A. 	Create     
B.	Store        
C.	Share        
D.	Destroy        

Answer: C       

### Question # 94 -	What cloud data lifecycle stage occurs at the question mark shown in the following image?      
A.	Storage     
B.	Encryption    
C.	Labeling   
D.	Provisioning   

Answer: A       

### [very important concept] Question # 95 -	Naomi’s organization has removed addresses, names, and phone numbers from data sets while retaining customer information like orders and website activity. What data obfuscation technique has she used?      
A.	Anonymization    
B.	Hashing    
C.	Shuffling    
D.	Tokenization    

Answer: A       

### Question # 96 -	Melissa is designing her organization’s data retention policy. Which of the following is not a common component of a data retention policy? 
A.	Retention periods     
B.	Data value     
C.	Regulatory compliance     
D.	Data classification     

Answer: B       

### Question # 97 -	Gary’s cloud provider gives him direct access to actual drives in servers as part of his  hosting plan. What type of storage is Gary using when he installs operating systems and applications on those drives?      
A.	Long- term storage     
B.	Ephemeral storage     
C.	Raw storage     
D.	Volume- based storage     

Answer: C       

### [important] Question # 98 -	Maria has implemented an information rights management tool for her cloud- hosted SharePoint site. What requirement will her organization’s SharePoint users need to meet to access controlled files?    
A.	They will need to access the files only via local fileshares.    
B.	They will need to use multifactor authentication for all file access.     
C.	They will need to open the files using tools that support IRM.     
D. They will need to request access to each file before opening it.       

Answer: C       

### [important] Question # 99 -	Angelo is implementing a [data discovery process]. Which of the following steps should he begin with to help [speed up the discovery process]?   
A. 	Map data to compliance requirements.    
B.	Extract and catalog metadata.    
C.	Scan for sensitive data.    
D.	Classify data.    

Answer: B       

### Question # 100 -	Bob has contracted with his cloud service provider to allow his organization to directly access SSDs in his environment due to specialized requirements and to certify that the drives have been physically destroyed after they are removed from use by his organization. What type of storage is Bob using?     
A.	Long- term    
B.	Raw storage    
C.	Ephemeral storage    
D.	Block storage   

Answer: B       


### Chapter 2: Domain 2: Architecture and Design

Question # 1.	D. Emails and other freeform text are examples of unstructured data. Structured data like the data found in databases is carefully defined, whereas semi- structured data like XML and JSON applies structure without being tightly controlled. While email itself is defined by an RFC, the term RFC-d efined data is not used in this context.

Question # 2.	A. Data labeling typically occurs during the Creation phase of the data lifecycle. Data labels may also be changed or added during use as data is modified.

Question # 3.	B. Jacinda is likely to face challenges using her DLP system due to the broad and consistent use of encryption for data in transit or data in motion in cloud environments. She will need to take particular care to design and architect her environment to allow the DLP system to have access to the traffic it needs. Data labeling can be a challenge, if it is lacking or if it  isn’t done properly, but DLP systems can use pattern matching and other techniques to 
 
identify data. Data at rest is typically not as much of a concern for a DLP system since preventing loss requires understanding when data is going somewhere, not when it is remaining in a location.

Question # 4.	C. Passwords are intentionally not captured or logged since creating an audit log that contains passwords would be a significant security issue. The source and destination IP address as well as the account used for privileged access are all common log data that can help when events need to be audited.

Question # 5.	A. Cryptographic erasure, or crypto- shredding, is the only way to ensure that drives and volumes hosted by third parties are securely cleared. Zero- wiping may result in remnant data, particularly where drives are dynamically allocated space in a hosted environment. Degaussing or other physical destruction is typically not possible with third- party- hosted systems without a special contract and dedicated hardware.

Question # 6.	D. Legal holds require organizations to identify and preserve data that meets the hold’s scope. Jason should identify the files and preserve them until they are required. Restoring files might erase important data, deleting files is completely contrary to the concept of the hold, and holds do not require immediate production— they are just what they sound like, a requirement to hold the data.

Question # 7.	B. Masking data involves replacing data with alternate characters like X or *. This is typically done via controls in the software or database itself, as the underlying data remains intact in the database. Anonymization or deidentification removes data that might allow individuals to be identified. Hashing is used to allow data to be referenced by a hash without displaying the actual data, but it causes properties of the data that may be needed for testing to be lost. Randomization or shuffling data moves it around, disassociating the data but leaving real data in place to be tested.

Question # 8.	C. XML and JSON are both examples of semi- structured data. Other examples include CSV files, XML, NoSQL databases, and HTML files.

Question # 9.	B. The provider’s own logging function is the best option. Information about systems being created and destroyed won’t exist on the local systems, and thus syslog, syslog- ng, and local logs won’t work. In addition, Linux typically doesn’t have an application log— both event and application logs are common for Windows systems.

Question # 10.	A. Original source IP addresses may not be visible in the local web server log. Fortunately, load-balancer logs can be used if they are available. The destination IP address will typically remain, as well as the destination port and the actual query.

Question # 11.	A. Hashing converts variable length data to fixed- length outputs, meaning that the length, formatting, and the ability to perform operations on the data using strings or numbers will be lost. Its ability to be uniquely identified won’t be lost— Isaac just needs to know the hash of a given address to continue to reference that data element.

Question # 12.	B. Data dispersion is the practice of ensuring that important data is stored in more than one location or service. It does not necessarily require specific distances or geographic limits, doesn’t require deletion of data not in secure storage, and doesn’t require you to use multiple data sets to access data.

Question # 13.	B. Storage that is associated with an instance that will be destroyed when the instance is shut down is ephemeral storage. Raw storage is storage that you have direct access to like a hard drive, or an SSD that has access to the underlying device. Long- term storage is storage that is intended to continue to exist, and is often used for logs or data storage. Volume- based storage is storage allocated as a virtual drive or device within the cloud.

Question # 14.	A. The size of the data or files is not typically a data classification type or field. Sensitivity, jurisdiction, and criticality are all commonly used to classify data.

Question # 15.	A. Data labels can help DLP systems identify and manage data, so Chris should ensure that data is labeled as part of its creation process to help his DLP identify and protect it. Classification is important, but without tags it won’t be useful to the DLP. Hashing can be used to help a DLP identify specific files, but tends to be done by the DLP system itself if needed, and geolocation tagging is not a typical DLP protection.

Question # 16.	D. Chain of custody documentation, often including actions like hashing files to ensure they are not changed from their original form, is commonly done to support nonrepudiation. Digitally signing files and data dispersion won’t prevent copying and does not encrypt them.

Question # 17.	C. Ephemeral storage will have the performance of its overall storage type, so low performance isn’t an expected issue. Inadvertent exposure, malicious access, and loss of forensic artifacts are all concerns for ephemeral storage.

Question # 18.	B. Raw storage provides direct access to a disk, and without crypto- shredding is likely to have remnant data on the disk after it is used. Since long- term and ephemeral storage is typically abstracted, it is less likely to have remnant data in unallocated or reallocated sectors that would not be purged through typical wipe operations.

Question # 19.	A. Unstructured data is the most difficult to perform discovery against because the data is unlabeled and requires discovery to be done using searches or other techniques that can handle arbitrary data. Rigidly structured data is not a common description of a type of data for the purposes of the CCSP exam.

Question # 20.	C. While it isn’t always perfectly accurate, geolocation (sometimes called geoIP) data attempts to identify the location of a given IP address. Isaac can use that data to attempt to match authentication events to logins, although VPNs and other tools may obscure the actual login location for users.

Question # 21.	B. While there may be some concerns about real data being used, Charleen’s goal is to have actual data for testing, making shuffling her best option. Hashing, randomization, and masking all remove or modify data in meaningful ways, resulting in testing not being as accurate as it might be against real- world data.

Question # 22.	D. Michelle should be aware that logging deletion events, like any other high- volume event, may incur additional costs for her organization. Since the question specifically mentions ephemeral files and heavy usage, this may be a more significant concern for her organization. Logs will show the relevant information, and there is nothing to indicate they would not be accurate, logging is enabled or disabled by the account holder or owner, and creation and deletion event logging is supported by object- based filesystems.

Question # 23.	B. Data’s confidentiality level is often contained in a label, but the monetary value is not a common data label. Creation and scheduled destruction date are also common data labels.

Question # 24.	B. Retention policies often include language that addresses legal holds because holds can impact retention practices and requirements. Data classification, acceptable use, and data breach response policies typically do not include legal hold language.

Question # 25.	A. Keys should never be stored in plaintext format and should instead be stored in a secure manner— typically encrypted in a hardware security module or other key vault.

Question # 26.	C. While IRMs are useful through many of the phases of the cloud data lifecycle, Marco knows that sharing data is when an IRM is most heavily used to ensure that data is not inadvertently exposed or misused.

Question # Question # 27.	B. JSON is an example of semi- structured data. Other examples include CSV files, XML, NoSQL databases, and HTML files.

Question # 28.	A. Cloud archival storage is typically designed primarily as a storage location with infrequent and smaller scale access, not for large- scale interactive access like a discovery process will use. It is likely to be a slow and potentially costly effort if the data is scanned while in the archival location. Charleen should validate if scanning the archived data makes sense, or if moving it to a different storage tier may fit the organization’s needs better. The data should exist as archival storage is used to preserve data; archival storage is online but may be slow; and no mention of encryption was made, so we cannot assume that it was encrypted.

Question # 29.	B. Data mapping is the process of matching fields in databases to allow them to be integrated or for purposes such as data migration.

Question # 30.	C. Adding labels as part of the file’s metadata is a common practice and is less likely to be changed than including them in the filename. Modifying the files themselves with data at the beginning or end of the file can cause issues with processing that may not be prepared to handle labeled data.

[important] Question # 31.	D. Key escrow and backup is incredibly important, and once a key is lost, it cannot be recovered and the data should be considered lost. 
Generating new keys will not decrypt the data, 
the passphrase isn’t sufficient to recover keys, and hashing is not a form of encryption and cannot be reversed.

Question # 32.	D. Madani knows that structured data is well-defined and organized, and will be the easiest to perform discovery actions on. It isn’t possible to perform discovery against encrypted data unless it is decrypted for the discovery process. Unstructured data is harder than semi- structured data discovery in most cases.

Question # 33.	A. Ashley is documenting the chain of custody for the image to ensure it can be used in court. Repudiation might occur if the chain of custody was not properly documented. A legal hold does not necessarily require chain of custody documentation, although organizations may choose to or be required to ensure it. Forensic accounting is a term used to describe financial investigations.

Question # 34.	D. Data mapping is a term used to describe matching fields in databases to allow data migration or integration. Data classification policies do identify classification levels, assign responsibilities, and define roles.

Question # 35.	B. Labeling data at creation ensures that it can be properly handled through the rest of its lifecycle. Automated labeling is preferable where possible to avoid human error and to accommodate the volume of data that most organizations create.

Question # 36.	A. Anonymizing access using a key removes the ability to provide accountability and works against organizational best practices. Identifying the key, the user, and when and how it is used supports accountability for usage.

Question # 37.	B. Crypto- shredding is the only viable option in environments controlled or managed by a third- party organization in most circumstances. Physical destruction is not permitted or supported by third- party providers, nor is degaussing, which will also not work on many modern drives. Overwriting may be appealing, but remnant data is an issue with SSDs and volumes that are dynamically allocated.

[important] Question # 38.	B. **Tokenization relies on two distinct databases, one with actual data and one with tokenized data**. 
Token servers then pull the data the token represents from the real data database when needed. 
This process does not require encryption, specify FIPS 140 requirements, or involve deidentification practices.

Question # 39.	A. **With the source database ready and a tokenization database prepared to be populated, the next step is to identify which data should be tokenized**. 
**Not all data is sensitive, and thus not all data needs to be tokenized**. 
Once you know what data will be tokenized, you can tokenize it— sometimes by hashing the data. 
Randomization is not part of this process.

Question # 40.	C. Dataflow diagrams are a critical part of organizational understanding of how data is created, moves, and is used throughout an organization. They often include details like ports, protocols, data elements and classification, and other details that can help you understand not only where data is, but how it gets there and what data is in use.

Question # 41.	A. Annie should map the data between the database fields and then use the mappings to help her sort and manage data as needed. Data labeling is used to tag data with important information like classification, creation date or time, or other elements. Column consolidation and columnar aggregation were made up for this question.

Question # 42.	D. Data lifespan is not a typical entry in a dataflow diagram since they focus on flows, not policies. Data types, fields or names, services, systems, ports, protocols, and security details are all commonly included in dataflow diagrams.

Question # 43.	C. Encrypting the drive or volume at creation ensures that any data written to the drive or volume through its lifespan will be encrypted and that destruction of the encryption key will result in secure destruction of the data.

Question # 44.	C. Unstructured data does not have the structure required to be easily stored in a database. Semi- structured and structured data is easier to store in a relational database since it has descriptors and elements that make it easier to map into fields.

Question # 45.	A. Retention policies often include retention periods, regulatory and compliance requirements, data classification impacts on retention, how and when data should be deleted, and archiving and retrieval processes. In addition, Olivia may want to include monitoring, maintenance, and enforcement.

Question # 46.	C. An IRM needs to maintain a 
certificate revocation list that allows users and applications to validate certificates, just like any other service that uses certificates. That means that Hui should be able to check to see if the revoked certificate is in the list to validate her actions. Issuing a new certificate using the same information, accessing the data using her own certificate, or deleting the private keys will not invalidate the existing certificate.

Question # 47.	D. **The provisioning capability of IRM systems focuses on providing rights to individuals based on roles and job functions. Tagging and data labeling are used to ensure that data is handled appropriately based on rules. Encryption secures data at rest and in transit**.

Question # 48.	A. Business impact analysis helps to determine what data is needed to continue the operations of the business. This is an assessment of the criticality of the data, and Randy knows that the data he flags may be necessary in the event of a disaster or other business continuity issue.

Question # 49.	C. Susan should prepare a dataflow diagram to share with her application developers and cloud architects to make sure that the application and service environment is correctly documented. Data mapping matches fields in databases, business impact analysis work assesses the importance of data to an organization’s work, and data classification describes data based on things like sensitivity, jurisdiction, or criticality.

Question # 50.	C. The most common risk, and thus the most impactful risk in this list, is the potential for a provider outage to result in the inability to access dispersed data.

Question # 51.	B. Installation of a local agent is typically required by IRM systems to ensure data is properly handled on endpoint systems. The question doesn’t specify the use of a server either in the cloud or locally, and the endpoints mentioned are not cloud- based.

Question # 52.	A. Unstructured data includes data like images, audio, video, word processing files, and other data that does not have a formally defined structure like structured data does. There’s no information that indicates that this is sensitive information, and there isn’t any mention of labeling in the question.

Question # 53.	B. Ingress and egress fees are often some of the highest expenses involved in this effort. Since the data is already contained in a storage tier, no new expenses should arise. Logs are textbased and can be stored efficiently, so it is unlikely that log files will be a major cost driver.

Question # 54.	C. Amanda knows that the original drive should be preserved, and actions should only be taken on a forensic copy. Working with the original, regardless of the process, is not a forensic best practice.

Question # 55.	A. While IRM systems can control actions on the system, taking a photo (or even a screenshot) of displayed text is typically outside of their capabilities. Preventing copying, printing, and making copies are all common IRM features.

Question # 56.	B. Regulatory compliance is important for organizations, and Felix needs to point out that discovery across multiple countries and regions may involve a complex set of regulations to comply with. Costs may vary in different regions, but that is not the primary concern Felix needs to raise. There isn’t any mention in the question of whether data is structured or not, and while encryption import and export may be covered by law, discovery can be conducted using local tools in each region if necessary.

Question # 57.	B. Archiving data to a lower- cost, and typically lower- performance storage tier, is a common strategy for cloud data retention. Examples like Amazon’s Glacier allow for long- term storage with infrequent or slow access and may come with additional costs for retrieval, but optimize costs when data is unlikely to be accessed. Deleting the data does not allow it to be used, moving to a third- party service provider is more complex, and moving to a higher- performance storage tier does not meet his cost needs.

Question # 58.	B. The Use phase of the data lifecycle often includes modification of data, and thus will require labels to change or be added.

Question # 59.	D. TLS, or Transport Layer Security, is the encryption protocol of choice for web application traffic. It replaced SSL. Both MD5 and SHA- 1 are hashing algorithms, not encryption.

Question # 60.	A. **Data dispersion best fits this description, and bit splitting is a form of data dispersion**, although it is one that is more frequently associated with malicious use to avoid forensic analysis and investigations.

Question # 61.	C. Legal holds normally take precedence over other deletion requirements. While Gurleen should check with her organization’s legal counsel, in general she should continue to preserve the data.

Question # 62.	D. Ephemeral storage that is associated with instances in most cloud provider’s infrastructure is wiped and reclaimed for reallocation when instances are terminated. If the instance were merely shut down, the storage would be retained for when the system was reactivated.

Question # 63.	A. **Ephemeral data is often kept for shorter time periods like 45 days**, 
a time period sufficient to allow investigations without building up large volumes of data that will not be used and which can be expensive to store. 
Longer- term storage may be required by law or contracts or due to specific contractual requirements.
⚡ Exam Tip (CCSP/CISSP) - If question says "no legal or regulatory requirement" → **choose shortest retention** (cost-effective, lower risk).
If financial → 5 or 7 years (depending on law).
If healthcare → 6 years (HIPAA).
If tax/audit → 7 years (SOX/IRS).
If security logs → minimum 1 year (PCI DSS), often 3 years internally.

Question # 64.	A. While it may seem quite simple, securely erasing all copies of the encryption key is all that it takes to complete the destruction process for crypto- shredding.

Question # 65.	A. Service outages are the only direct threat to availability on this list. Lincoln should review the service provider’s history of service outages and issues as he makes decisions about adopting the service.

Question # 66.	D. **Information rights management systems typically rely on [certificates] to identify systems. 
They can be [issued centrally] and managed, as well as used for [digital signatures and encryption]**.

Question # 67.	C. **Derek’s organization is using hashing, which uses a one- way cryptographic function to replace data with values that can be referenced without exposing the actual data. 
Anonymization focuses on removing data that can be associated with specific users or individuals, 
masking uses alternate characters to conceal data, and shuffling switches data around while retaining actual data for testing**.

Question # 68.	A. **[Long- term storage] is storage that is intended to continue to exist and is often used for logs or data storage. 
Storage that is associated with an instance that will be destroyed when the instance is shut down is ephemeral storage. 
Raw storage is storage that you have direct access to like a hard drive or an SSD that has access to the underlying device. 
Volume- based storage is storage allocated as a virtual drive or device within the cloud**.

Question # 69.	C. **[OWASPs Secrets Management Cheatsheet] describes [three] main requirements for “break- glass” secrets backup environments: 
	ensuring automated backups are in place and executed regularly based on the number of secrets and their lifecycle, 
 	frequently testing the restore procedures, and 
  	encrypting backups and placing them on secure, monitored storage**.

Question # 70.	B. Using standard test secrets makes them easier to detect if they are in an exposed location. Since Alaina specifically has an internal test environment, this is the right location to use standard secrets. Secrets managers should be used in all locations, but they won’t help with identifying issues with secrets exposure. Multiple utilities may be tempting, but they add overhead and additional work where a properly configured and tested utility will provide sufficient detection in most cases. High entropy secrets are useful, but secrets with a known and consistent format can more easily be detected and thus problems with exposure can be detected.

Question # 71.	D. **Retrieval time, the amount of time before data can be accessed, is a [primary driver] for the cost of archival storage in cloud environments**. The size of the data in the question is fixed, so Angie needs to figure out what other options she can control. 
The type and sensitivity of the data do not impact costs but may impact practices that Angie will put in place to secure and manage it.

Question # 72.	D. The figure shows a data mapping process between two database tables matching names, phone numbers, and email addresses. String comparison compares two strings to determine if they are the same. Field hashing and table matching were made up for this question.

Question # 73.	B. **Provisioning for IRM systems gives users the rights and permissions that they need to access files they have rights to**. 
Tagging and labeling help to mark files based on data classification guidelines, allowing the IRM to apply rules appropriately, and data mapping maps fields in databases to each other.

[very important] Question # 74.	B. **[Data access patterns] are one of the most important things to understand before selecting archival storage**. 
**Archival storage classes and services often focus on inexpensive, low frequency, slow access**, 
but other options can include more dynamic access capabilities— often at a higher cost since the storage needs to be capable of higher performance. 
The cost of the storage is just that— cost, not performance. 
The volume of the data, and the amount of time that the data will be stored for, also influence cost, not performance.

Question # 75.	B. Data owners are defined by data classification policies and hold overall responsibility for data that they own. Data custodians are responsible for the data, ensuring access control, proper storage, and other operational controls. Data processors are often third parties who process the data as part of a business process, and data users are end users who use the data for their job.

[important] Question # 76.	C. **Tokenized data is only a concern if the database with original data that it references is also exposed**. 
**Tokens are not encrypted, and while hashing is used in many tokenization processes, hashes are a one- way function and should have additional transformations performed to ensure that simply hashing data to get matches will not succeed**.

Question # 77.	**A. Versioning tools like those found in Amazon’s S3 environment allow you to revert to a previous version 
	if an inadvertent change occurs, 
 	if data is corrupted, or 
  	if the file is deleted**. 
**This can take up significant amounts of additional space** in some circumstances, so Asha should carefully consider where and when she enables versioning in her cloud environment. 
Daily backups, recurring snapshots, or archiving processes will take longer to restore from in most cases and may allow for multiple changes before backup, snapshot, or archiving occurs.

Question # 78.	C. The concept of least privilege is used for secrets too, and maximizing the number of rights a secret provides instead of minimizing it is a bad idea. Brian should instead seek to limit the rights a given secret provides to constrain the impact of a potential breach or misuse.

Question # 79.	B. Access logging will allow Chris to monitor for access to specific buckets by individuals, including privileged accounts. Authentication logging won’t show access, nor will bandwidth logging. Timestamps should be on by default for any log event.

Question # 80.	C. Jaime is performing content- based discovery by searching for specific terms in unstructured data. Label-b ased discovery would rely on data labels, metadata- based discovery uses metadata information, and structure- based discovery was made up for this question.

Question # 81.	B. Mike should immediately revoke the certificate so that any malicious use will be limited. 
He may then want to determine why the certificate was exposed and issue a new certificate to ensure that the user or owner can continue to perform their job.

[important] Question # 82.	A. **Tagging data will help the DLP manage it appropriately without having to rely on pattern matching**. 
Reducing the overall amount of data may help, but Dan’s first priority should be using more effective methods. 
Classifying data helps, but only if you tag it or otherwise help the DLP to easily manage it. 
Regular expressions are part of pattern matching. Refining them may help, but the underlying issue of relying on the most challenging matching mode will remain.

Question # 83.	C. Tags are an important tool when working with ephemeral systems. While IP addresses may be reused and administrative accounts are likely to be the same across systems, tags can be unique, allowing events to be tracked to an instance. The system’s deletion time should be logged, as should the time it is instantiated, but this obviously wouldn’t be in every log event created by the machine.

Question # 84.	B. **Legal holds typically override other agreements and lifecycles**. 
**Valerie should preserve only the data requested or covered by the legal hold**, and she should continue with normal practices for the remaining data.

Question # 85.	A. Heikki’s next step will be to set up policies that apply appropriate controls to the data that he has categorized and labeled. Once those policies are set, he can train users and run the DLP.

Question # 86.	A. Kara is performing metadata- based discovery using the metadata that already exists in most digital photos. Content-b ased discovery might compare the photos looking for specific subjects, and label- or tag- based discovery would leverage data labels.

[important] Question # 87.	D. **Rick knows that the tokenized data can be looked up against a database that contains the original customer data, allowing it to be accessed as needed**. 
**The actual customer data is stored in a separate database, meaning that a breach of the token database would not result in a customer data breach**. 
The customer data is more secure but could still be breached if attackers leveraged the tokens and their lookup capability.

Question # 88.	B. Hashes can be used to validate whether an image has been modified, but it is important to note that a running machine will have a different hash than the original. Jack may need to check specific file hashes instead. Cloud provider logs may not show changes to an instance, timestamps are time-consuming to check and may be modified when files are copied, and rebuilding the machine will typically result in differences.

[important] Question # 89.	B. **Dispersion is the concept of ensuring that data is in multiple locations so that a single failure, event, or loss cannot result in the destruction or loss of the data**. 
[important] **Deduplication involves removing duplicates from a data set**; 
protected supply chain and lifecycle management are how data is managed throughout its life and doesn’t specifically describe where data is stored for redundancy.

Question # 90.	A. When data is created and used in other countries, it may be subject to regulations specific to those countries. Christina should point out that regulatory compliance is critical and could prove complex in this scenario. Exposure issues should be accounted for through best practices like using encryption for all transfers. Transfer speeds for archival data are typically not as critical as for operational data, and permissions should be set to be appropriate for the data regardless of location.

Question # 91.	D. The Use stage occurs after Classification and before Transfer or Archiving.

[very important] Question # 92.	D. **Ben knows that hashes are one- way functions and cannot be reversed**. 
**They generate fixed- length output from variable- length input**, and **identical files will generate identical output**. 
**Two different files should never generate the same output— this is known as a collision and is not acceptable in a hashing algorithm**.

Question # 93.	C. IRM can be particularly useful during the sharing stage of the cloud data lifecycle since information rights management tools can ensure privileges and access to data are appropriately managed as data moves around the organization and potentially leaves it.

Question # 94.	A. Storage occurs after creation in the cloud data lifecycle. Labeling is typically done as part of the creation process. Provisioning may be done at any time but is often associated with use. Encryption is not a stage in the cycle.

Question # 95.	A. **Naomi has attempted to anonymize** the data b**y removing personally identifiable data**. 
**Hashes use a one- way cryptographic function** to reference data without having the data itself exposed or in use. 
**Shuffling moves data around so it is not associated with its original entries, but allows actual data to be used for testing**. 
Tokenization uses two databases with data mapped to reference items known as tokens, allowing tokens to be referenced and then data that those tokens refer to be accessed.

Question # 96.	B. Data value is typically not included in a data retention policy. Instead, retention periods, compliance requirements, and data classification are included as well as lifecycle requirements and archiving and retrieval procedures.

Question # 97.	C. **Raw storage is storage that you have direct access to like a hard drive or an SSD that has access to the underlying device**. 
**Long- term storage is storage that is intended to continue to exist** and is **often used for logs or data storage**. 
**Storage that is associated with an instance that will be destroyed when the instance is shut down is ephemeral storage**. 
Volume- based storage is storage allocated as a virtual drive or device within the cloud.

Question # 98.	C. **IRM tools require that client devices and applications support IRM or that they access files via web applications that can provide IRM controls**. 
Fortunately, SharePoint users tend to use Microsoft Office heavily, meaning that many, if not most, of the files will be opened using tools that natively support IRM.

Question # 99.	B. **Using existing metadata will help Angelo with his data discovery process, so he should start with that**. 
Once he has the metadata processed, he can use it to speed up other cataloging efforts like scanning for sensitive data, classifying data, and mapping the data to compliance requirements.

Question # 100.	B. This is an example of raw storage, which directly presents underlying hardware to users.
