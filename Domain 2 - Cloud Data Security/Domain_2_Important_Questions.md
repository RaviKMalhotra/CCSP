A. Transparent encryption
B. Symmetric-key encryption
C. Application-level encryption
D. Homomorphic encryption
C. In application-level encryption, the application will encrypt data before it is placed in the database. In transparent encryption, the entire database is encrypted. Symmetric-key encryption is a kind of encryption and not truly indicative of a strategy used in database encryption. Homomorphic encryption is an experimental, theoretical process that might allow processing encrypted information without the need to decrypt it first.
A. The solution should give you better analysis capability by automating a great deal of the associated tasks.
B. Dashboards produced by the tool are a flawless management benefit.
C. You will have to coordinate with the cloud provider to ensure that the tool is acceptable and functioning properly.
D. Senior management will be required to approve the acquisition and implementation of the tool.
C. Because the tool will require at least some installation and reporting capability within the cloud environment, it is essential to coordinate with the cloud provider to ensure that the solution you choose will function properly and is allowed by the provider. Option A is true, but not a major concern; that is a benefit of SIEM/SEM/SIM tools. Option B is not true because dashboards can often misconstrue pertinent reporting data when they are used to chase management goals instead of distilling raw data appropriately. Option D is not true because management should not be involved in such granular decisions.
A. Encrypt data with a particular encryption engine.
B. Encrypt first resulting keys with another encryption engine.
C. Save backup of second resulting keys.
D. Destroy original second resulting keys.
C. In crypto-shredding, the purpose is to make the data unrecoverable; saving a backup of the keys would attenuate that outcome because the keys would still exist for the purpose of recovering data. All other steps outline the crypto-shredding process.
A. Crypto-shredding
B. Degaussing
C. Physical destruction
D. Overwriting
A. Cloud customers are allowed to encrypt their own data and manage their own keys; crypto-shredding is therefore possible. Degaussing is not likely in the cloud because it requires physical access to the storage devices and because most cloud providers are using solid-state drives (SSDs) for storage, which are not magnetic. Physical destruction is not feasible because the cloud customer doesn’t own the hardware and therefore won’t be allowed to destroy it. Overwriting probably won’t work because finding all data in all aspects of the cloud is difficult and the data is constantly being backed up and securely stored, so a thorough process would be very tricky.
A. Crypto-shredding
B. Using standard data formats
C. Avoiding proprietary services
D. Favorable contract terms
A. Crypto-shredding is for secure sanitization, not portability. The other methods all enhance portability.
A. Users might be required to install a DRM agent on their local devices.
B. DRM solutions might have difficulty interfacing with multiple different operating systems and services.
C. DRM solutions might have difficulty interacting with virtualized instances.
D. Ownership of intellectual property might be difficult to ascertain.
D. The owner of intellectual property will not change whether the material is stored in the cloud or in a legacy environment. Moving into the cloud will probably result in more use of personal devices, requiring users to install local DRM agents, so option A is true, making it not a suitable answer to this question. Options B and C are also true, due to the nature of cloud computing, and are therefore also not suitable for this question.
A. With the cloud provider
B. Off the cloud, with the data owner
C. With a third-party provider, in key escrow
D. Anywhere but with the cloud provider
A. Option A creates a conflict of interest and does not enforce separation of duties.
A. Long-term storage of the related cryptographic keys
B. Format of the data
C. Media the data resides on
D. Underground depth of the storage facility
D. A long-term storage facility may or may not be located underground; the security of that facility (and the data contained therein) is not dependent on this aspect. Option A is a security concern because loss of the keys may result in losing the data (by losing access to the data), and keeping the keys with the data they protect increases risk. Both the format of the data and the media on which it resides (options B and C) are important to bear in mind, as either (or both) may be outmoded by the time the data might need to be retrieved from the archive; data and formats do not age well.
A. Business continuity and disaster recovery (BC/DR)
B. Redundant Array of Inexpensive Disks (RAID)
C. Software-defined networking (SDN)
D. Content delivery network (CDN)
B. Data dispersion is basically RAID in the cloud, with data elements parsed and stored over several areas/devices instead of stored as a unit in a single place. RAID (and data dispersion) does aid in BC/DR activities by increasing the robustness and resiliency of stored data, but BC/DR is a much more general discipline, so it is not the optimum answer for the question. SDN is used for abstracting network control commands away from production data, and CDN is usually used for ensuring quality of streaming media.
A. Chunking
B. Vaulting
C. Lumping
D. Grouping
A. Where RAID used data striping across multiple drives, with data dispersion this technique is referred to as “chunking,” or sometimes “sharding” when encryption is also used. The other options are not common data dispersion terms used in cloud computing and have no meaning in this context.
A. Smurfing
B. Snarfing
C. Erasure coding
D. Real-time bitlinking
C. Erasure coding is the practice of having sufficient data to replace a lost chunk in data dispersion, protecting against the possibility of a device failing while it holds a given chunk; parity bits serve the same purpose in a traditional RAID configuration. The other options are not common data dispersion terms used in cloud computing and have no meaning in this context.
A. Protecting confidentiality against external attack on the storage area
B. Loss of availability due to single-storage-device failure
C. Loss due to seizure by law enforcement in a multitenant environment
D. Protecting against loss due to user error
D. Data dispersion can’t aid in inadvertent loss caused by an errant user; if the user accidentally deletes/corrupts a file, that file will be deleted/corrupted across all the storage spaces where it is dispersed. The technique does, however, protect against the other risks. It enhances confidentiality because an attacker gaining illicit access to a single storage space will only get a chunk of the data, which is useless without the other chunks. This same aspect also protects loss when law enforcement seizes a specific storage device/space when they are investigating another tenant at the same cloud provider your organization uses. And loss of availability due to single device failure is probably the primary reason for having data dispersion (like RAID before it).
A. Object
B. Volume
C. Synthetic
D. Database
B. Volume storage allows all the functions described in the question. Object storage has data arranged in a file structure, and databases arrange data in tables and relational schemes; neither of these options offers the functions described in the question. Synthetic is not a cloud memory configuration option.
A. Object storage
B. Volume storage
C. Synthetic storage
D. Databases
A. Object storage is usually arranged in a file hierarchy. Volume storage has data with no defined structure (only memory space), and databases ar-range data in tables and relational schemes; neither of these options offers the functions described in the question. Synthetic is not a cloud memory con-figuration option.
A. Preventing distributed denial of service (DDoS) attacks
B. Inventorying data assets
C. Interviewing data owners
D. Protecting against natural disasters
B. Egress monitoring solutions (often referred to as DLP tools, where DLP stands for data loss protection or data leak prevention, or some combination of these terms) require the organization to appropriately inventory and classify data assets so the tool knows what to protect. DLP does not aid in protections for DDoS or natural disasters, which affect availability, not confidentiality (DLP only enhances confidentiality efforts). Option C is not a benefit of implementing an egress monitoring solution.
A. Arbitrates contract breaches
B. Performs personnel evaluation reviews
C. Discovers data assets according to classification/categorization
D. Applies another level of access control
C. Egress monitoring solutions (often referred to as DLP tools, where DLP stands for data loss protection or data leak prevention, or some combination of these terms) will often include a discovery function, which will locate data assets according to criteria defined by the organization. DLP solutions cannot arbitrate contract breaches or perform personnel evaluations. Usually, DLPs also do not apply additional access controls; that is typically a characteristic of a digital rights management (DRM) solution.
A. Uses biometrics to scan users
B. Inspects incoming packets
C. Resides on client machines
D. Uses stateful inspection
C. Egress monitoring solutions (often referred to as DLP tools, where DLP stands for data loss protection or data leak prevention, or some combination of these terms) will often include an agent that resides on client devices in order to inspect data being shared/sent by end users. DLP tools do not inspect incoming packets, with or without stateful inspection; this is the job of firewalls. DLP solutions do not typically use biometrics in any way.
A. Personally identifiable information (PII)
B. Intellectual property
C. Plans and policies
D. Marketing material
B. DRM is mainly designed to protect intellectual property. It can also sometimes be used for securing PII, but intellectual property is a better answer here. Plans and policies aren’t usually protected in this manner, and marketing material is usually meant to be disseminated, so it does not require protection.
A. Patents
B. Trademarks
C. Personally identifiable information (PII)
D. Copyright
D. DRM is often deployed to ensure that copyrighted material (frequently software) is only delivered to and used by licensed recipients. Patents are more complicated and not often distributed to a mass market, so DRM does not assist in that way. Trademarks are representations of a brand and meant to be distributed, so DRM does not protect them. PII is not typically a type of intellectual property.
A. Persistence
B. Influence
C. Resistance
D. Trepidation
A. Persistence is the trait that allows DRM protection to follow protected files wherever they might be stored/copied. The other options are not characteristics associated with DRM solutions.
A. Automatic expiration
B. Multilevel aggregation
C. Enhanced detail
D. Broad spectrum
A. Automatic expiration is the trait that allows DRM tools to prevent access to objects when a license expires or to remove protections when intellectual property moves into the public domain. The other options are not characteristics associated with DRM solutions.
A. Transparent encryption modification
B. Bilateral enhancement
C. Continuous audit trail
D. Encompassing flow
C. Continuous audit trail is the trait that allows DRM tools to log and exhibit all access to a given object. The other options are not characteristics associated with DRM solutions.
A. Mapping to existing access control lists (ACLs)
B. Delineating biometric catalogs
C. Preventing multifactor authentication
D. Prohibiting unauthorized transposition
A. Mapping to existing access control lists (ACLs) is the trait that allows DRM tools to provide additional access control protections for the organization’s assets. The other options are not characteristics associated with DRM solutions.
A. Store
B. Use
C. Deploy
D. Archive
A. The Cloud Secure Data Lifecycle phases are, in order, Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD).
A. Create
B. Destroy
C. Use
D. Encrypt
C. The Cloud Secure Data Lifecycle phases are, in order, Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD).
A. The term is not used only by (ISC)2.
B. Not all phases are secure.
C. Not all phases take place in the cloud.
D. It’s not actually a cycle.
D. The Cloud Secure Data Lifecycle phases are, in order, Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD). This is not truly a cycle because data does not continue after the destroy phase (that is to say, the same data or process does not go back to create after destroy).
A. Create
B. Store
C. Define
D. Use
A. The Cloud Secure Data Lifecycle phases are, in order, Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD). The best practice for categorizing/classifying data is to do so when it is first created/collected so that the proper security controls can be applied to it throughout the rest of the cycle.
A. Data dispersion
B. Crypto-shredding
C. Cryptoparsing
D. Cryptosporidium
B. The Cloud Secure Data Lifecycle phases are, in order, Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD). Crypto-shredding (also called cryptographic erasure) is the preferred method of data sanitization for a cloud environment; this should take place in the final phase of the cycle, destroy.
A. The first
B. The second
C. The fourth
D. The fifth
D. The Cloud Secure Data Lifecycle phases are, in order, Create, Store, Use, Share, Archive, Destroy (a good mnemonic might be CSU-SAD). Archiving (the fifth phase) is the process of moving data out of the production environment and into long-term storage.
A. Volume storage
B. Databases
C. Content delivery network (CDN)
D. Object storage
D. Object storage stores data as objects (hence the name), often arranged in a hierarchical structure.
A. Volume storage
B. Databases
C. Content delivery network (CDN)
D. Object storage
A. In volume storage, the user is assigned a logical drive space into which anything (such as raw data, objects, or applications) may be saved or installed, similar to a mounted drive on a traditional network.
A. Volume storage
B. Databases
C. Content delivery network (CDN)
D. Neutral storage
C. CDNs are often used to place large stores of multimedia data in a location geographically near to the end users who will consume that data; this approach is designed mostly to accomplish a reduction in data degradation due to distance between resource and user.
A. Ephemeral
B. Database
C. Long-term
D. Nefarious
B. The PaaS model allows the cloud customer to install and run applications in the cloud environment. With a database, the cloud customer can store data in a database administered by the cloud provider but can then tailor applications and services for reaching into and manipulating that database.
A. Infringing
B. Data dispersion
C. Voiding
D. Crypto-shredding
B. Data dispersion is the cloud version of using RAID arrays, protecting data by spreading it across multiple volumes/devices.
A. Deltas
B. Inversion
C. Parity bits
D. Transposition
C. Similar to parity bits in RAID, erasure coding is used in cloud data dispersion implementations to create a situation where data can still be recovered even if a segment or portion of the dispersed data is lost (due to drive failure, disaster, etc.).
A. Sensitive data that may leave the organization’s control
B. All data within the organization’s control
C. Data being processed by the organization’s users
D. Data that could be intercepted while out of the organization’s control
A. DLP, also referred to as egress monitoring, is used to detect and prevent sensitive data from leaving the organization’s control without proper approval.
A. Email content
B. FTP traffic
C. Material saved to portable media
D. Voice over Internet Protocol (VoIP) conversations
D. Commercial DLP products that monitor speech in real time and censor conversations are not yet widely available.
A. Pattern matching
B. Inference
C. Keyword identification
D. Metadata tags
B. Inference is an attack technique that derives sensitive material from an aggregation of innocuous data; DLP tools, thus far, do not have this capability.
A. If it’s hardware-based and your production environment is in an infrastructure as a service (IaaS) model
B. If you purchased it from a vendor other than the cloud provider
C. If it’s software-based and your production environment is in a platform as a service (PaaS) model
D. If it affects all guest instances on any given host device
C. A cloud customer can install applications on a PaaS environment, usually as they see fit and without prior coordination with the provider.
A. The additional risks of external attack associated with using the tool
B. The production impact it will have on the environment
C. What the price of the tool was
D. How the solution works
B. All security functions come with an attendant negative productivity effect: the most secure environment will be the least productive, and the most productive will be the least secure. Egress monitoring tools will have an overhead cost in terms of production impact and loss of efficiency and speed. This may affect the cost savings that were realized in a cloud migration from the legacy environment, and senior management needs to understand this trade-off.
A. Survey your company’s departments about the data under their control.
B. Reconstruct your firewalls.
C. Harden all your routers.
D. Adjust the hypervisors.
A. In order to “train” the egress monitoring solution properly, you’ll need to inform it as to which data in your organization is sensitive…and, in order to do that, you’ll need to determine what information your data owners deem sensitive; a survey is a way to do that.
A. Immediate decrease in lost data
B. A series of false-positive indications
C. Increase in morale across the organization
D. Increase in gross revenue
B. It will take a while for the tool to “learn” the particulars of your environment and to be conditioned properly. A significant number of false-positive indications will be expected in the near term, until you can hone the responses to properly meet your organization’s needs.
A. Sensitive data sent inadvertently in user emails
B. Sensitive data captured by screenshots
C. Sensitive data moved to external devices
D. Sensitive data in the contents of files sent via File Transfer Protocol (FTP)
B. It’s unlikely that any egress monitoring tools will be able to detect sensitive data captured, stored, and/or sent as graphic image files, which is the usual form of screenshots.
A. Getting signed user agreements from all users
B. Installation of the solution on all assets in the cloud data center
C. Adoption of the tool in all routers between your users and the cloud provider
D. Ensuring that all your customers install the tool
A. This is a tricky question. In the cloud environment, we know that all users will be entering the environment through remote access; in many cases, this will include the use of their personal devices. In order for egress monitoring solutions to function properly, all devices accessing the production environment must have local agents installed, and that requires signed user agreements.
A. Digital rights management (DRM) and security event and incident management (SIEM) tools
B. An investment in upgraded project management software
C. Digital insurance policies
D. The Uptime Institute’s Tier certification
A. Egress monitoring tools combined with DRM and SIEM enhance the security value of each because you create in-depth/layered defense.
A. Suspend user accounts and notify the security office when it detects possible sensitive data egress attempted by a user
B. Halt the transaction and notify the user’s supervisor when the user attempts to transfer sensitive data
C. Query the user as to whether they intend to send sensitive data upon detection of an attempted transfer
D. Sever remote connections upon detection of a possible sensitive data transfer
C. These are all possible settings for a modern egress monitoring solution. However, the best option, in light of the question, is to query the user as to their intent; this aids the user in understanding and knowing when sensitive data might be leaving the organization accidentally, through a mistake on the user’s part. The other options are more severe and restrictive; these will enhance security but reduce productivity and are management and technological controls instead of awareness tools, so they are incorrect answers for this question.
A. Data will not remain in one place or form in the cloud
B. The cloud environment will include redundant and resilient architecture
C. There will be a deleterious impact on production upon installing the tool
D. You might not have sufficient proper administrative rights in the cloud infrastructure
B. The fact that cloud data centers are designed with multiple redundancies of all systems and components won’t really have any bearing on your decision and implementation of your egress monitoring solution.
A. Access control
B. Data exfiltration
C. E-discovery/forensics
D. Data categorization/classification
A. Egress monitoring solutions do not facilitate access control efforts in any way.
A. Data at rest
B. Data in motion
C. Data in use
D. Data of relief
D. The term data of relief doesn’t really mean anything and is therefore the correct answer for this question.
A. The user
B. The data itself
C. The encryption engine
D. The encryption keys
A. The user is not really an aspect of an encryption deployment, although it may be argued that the user will need to refrain from disclosing their own key(s) to anyone else.
A. Physical loss or theft of a device
B. Disgruntled users
C. Malicious cloud administrators accessing the data
D. Virtual machine snapshots stolen from storage
B. An authorized user will still be able to access and decrypt the data for which they’ve been granted permissions, so encryption will not offer any protections for that threat.
A. File-level encryption
B. Digital rights management (DRM)
C. Application-level encryption
D. Transport Layer Security (TLS)
D. TLS is encryption used in a communication session, not a storage volume.
A. File-level encryption
B. Secure Sockets Layer (SSL)
C. Transparent encryption
D. Application-level encryption
B. SSL is encryption used in a communication session, not a storage volume.
A. In the application accessing the database
B. In the operating system on which the application is run
C. Within the database accessed by the application
D. In the volume where the database resides
A. The application contains the encryption engine used in application-level encryption.
A. File-level encryption
B. Transparent encryption
C. Application-level encryption
D. Object-level encryption
B. Encrypting specific tables within the database is one of the options of transparent encryption; this is not true of the other options, so they are incorrect.
A. File-level encryption
B. Transparent encryption
C. Application-level encryption
D. Volume encryption
C. Application-level encryption involves encrypting the data before it enters the fields of the database; it is much more difficult to search and review data that has been encrypted, so this reduces the functionality of the database.
A. With the cloud customer
B. With a third-party provider
C. At the cloud provider data center
D. Anywhere but with the cloud provider
D. Best practice is to not keep the encryption keys alongside the data they’ve been used to encrypt.
A. Legislation
B. Business needs
C. Average media longevity
D. Contracts
C. Data retention periods should be established in policy regardless of the projected lifetime of the media the data resides on. All the other options do/should influence data retention periods.
A. External hacking detection
B. Prediction of physical device theft
C. Data classification/categorization issues
D. Social engineering attacks
A. Event monitoring tools can help detect external hacking efforts by tracking and reporting on common hack-related activity, such as repeated failed login attempts and scanning. It is unlikely that these tools could predict physical device theft; they could, of course, report on a device that is no longer connected to the environment after it has been removed by noting a lack of event activity, but that’s not quite the same thing. Event monitoring tools don’t aid in data classification/categorization; egress monitoring and digital rights management tools might provide that function, though. Social engineering attacks are mostly transparent to the majority of logical tools (the exception being social engineering efforts combined with IT traffic, such as phishing, which might be detected by email filters and sophisticated firewalls).
A. Detecting untrained personnel
B. Predicting system outages
C. Sending alerts for conflicts of interest
D. Enforcing mandatory vacation
B. Event monitoring tools can be used to predict system outages by noting decreases in performance; repeated performance issues can be an indicator a device is failing. While an event monitoring tool might be able to detect a user who continually conducts unproductive activity or fails to complete certain functions, it is impossible to determine if the source of the problem is lack of training. These tools in no way serve to detect conflict of interest or enforce mandatory vacation, which are managerial/administrative controls.
A. Reducing workload for production personnel
B. Decreasing size of log files
C. Optimizing performance
D. Ensuring adequate lighting of workspaces
C. Event monitoring tools can detect repeated performance issues, which can be used by administrators and architects to enhance performance/productivity. These tools don’t aid in the managerial function of noting individual workload, nor do they reduce log file sizes (indeed, they might add to the size of log files) or have anything to do with lighting.
A. Detecting ambient heating, ventilation, and air-conditioning (HVAC) problems
B. Ensuring proper cloud migration
C. Deciding risk parameters
D. Protecting all physical entry points against the threat of fire
A. Event monitoring tools can detect repeated performance issues, which can be indicative of improper temperature settings in the data center; also, some system monitoring metrics, such as CPU temperature, can directly indicate inadequate HVAC performance. These tools do not aid in cloud migration (which is the task of architects and administrators) nor in risk decisions (which is the task of senior management); they also don’t provide any kind of assistance with fire.
A. Personnel safety
B. Vehicle tracking
C. Incident evidence
D. Acoustic dampening
C. Event logs are used to reconstruct a narrative of activity; they tell the story of what happened, how it happened, and so forth. This is crucial for evidentiary purposes. Event logging tools do not aid in any of the other options (especially acoustic dampening, which is gibberish in this context).
A. Greater physical security
B. Psychological deterrence
C. Cost savings
D. More logs can be reviewed, at faster speeds
D. The manual element of log review is tedious and necessarily slow because it requires a trained, knowledgeable person to perform the task; these tools can greatly increase the amount of log data that can be reviewed, in a much shorter amount of time. These tools do not, however, aid in any of the other options.
A. It is good practice to introduce pseudorandom numbers when generating keys.
B. Public keys should never be shared with anyone.
C. Losing the keys is equivalent to losing the data.
D. Symmetric keys should be passed out of band.
B. Public keys have to be shared in order for asymmetric cryptography to function properly; that is their purpose. Private keys, on the other hand, must remain secret, known only to the individuals to whom they are assigned.
A. The shipping department should get only a masked version of the customer’s
B. The customer service department should get only a masked version of the customer’s Social Security (SS) number.
C. The billing department should get only a masked version of the customer’s credit card number.
D. The Human Resources (HR) department should get only a masked version of the employee’s driver’s license number.
B. The customer service representative may need to see a partial version of the customer’s SS number to verify that the customer is who they claim to be, but that representative does not need to see the full number, which would create an unnecessary risk.
A. Random substitution
B. Algorithmic substitution
C. Deletion
D. Conflation
D. Conflation is not a masking technique and is meaningless in this context. All the others are suggested as possible masking techniques.
A. Random substitution
B. Shuffling
C. Deletion
D. Algorithmic substitution
C. While deletion is a very good way to avoid the possibility of inadvertently disclosing production data in a test environment, it also eliminates the usefulness of the data set as a plausible approximation of the production environment, greatly reducing the quality of the testing.
A. Creating a test environment for a new application
B. Allowing a customer service representative limited access to account data
C. Providing detailed reports to regulators
D. Notifying shareholders
A. Static masking involves modification of an entire data set, all at once. This would be a good method to create a sample data set for testing purposes.
A. Creating a test environment for a new application
B. Allowing a customer service representative limited access to account data
C. Sending incident response notifications
D. Implementing business continuity and disaster recovery (BC/DR)
B. Dynamically masking a user’s account information each time a customer service representative accesses that data is an efficient, secure means of masking data as necessary.
A. You could corrupt the production data.
B. The data could be subject to easy inadvertent disclosure.
C. Algorithms are two-way operations.
D. A null set has no test value.
C. Using an algorithm to mask data suggests that the same algorithm, if learned or reverse-engineered by an aggressor, could be used on the masked data to reveal the production data.
A. Username; password
B. User’s name; user’s age
C. User’s IP address; user’s media access control (MAC) address
D. Location; income level
B. The user’s name is a direct identifier, explicitly stating who that person is. The user’s age is not a direct identifier because it doesn’t specify a certain person, but it is a piece of demographic information that could be used to narrow down the user’s identity from a group of users of different ages, so it is an indirect identifier.
A. Access
B. Cryptographic keys
C. Numeric values
D. Identifying information
D. Anonymization is the process of removing identifiers from data sets so that data analysis tools and techniques cannot be used by malicious entities to divine personal or sensitive data from nonsensitive aggregated data sets.
A. Gramm-Leach-Bliley Act (GLBA)
B. Payment Card Industry (PCI)
C. Child Online Protection Act (COPA)
D. Sarbanes-Oxley Act (SOX)
B. PCI requires that credit card numbers and other cardholder data be obscured when stored for any length of time. Encryption is one approved method; tokenization is another.
A. One
B. Two
C. Three
D. Four
B. Tokenization will require, at a minimum, a database for the tokens and another for the stored sensitive data.
A. Regulatory or contractual compliance
B. Inference
C. Reduced cost of compliance
D. Mitigating risk from data lost to intrusion
B. Inference is an attack strategy, not a reason for implementing tokenization.
A. RAID
B. BIOS
C. DDoS
D. SYN-ACK
A. In the traditional environment, a RAID array is a set of disks/drives on which data
A. Removing all access to unauthorized parties
B. Ensuring that an unauthorized user only gets a useless fragment of data
C. Moving data across jurisdictional boundaries
D. Tracking all incoming access requests
B. Bit-splitting involves chopping data sets up into segments and storing those segments in multiple places/devices. An attacker getting access to one segment won’t be gaining anything of value because one segment of the data set would most likely make no sense out of context.
A. By making seizure of data by law enforcement more difficult
B. By hiding it from attackers in a specific jurisdiction
C. By ensuring that users can only accidentally disclose data to one geographic area
D. By restricting privilege user access
A. When law enforcement entities wish to seize assets (including data), they must cooperate with other law enforcement agencies in other jurisdictions if the data is not contained fully within their own. This may aid a data owner who is concerned about the risk of losing their data in a multitenant environment if another tenant conducts illicit activity and law enforcement seizes an entire data storage device as part of an investigation, accidentally collecting data belonging to innocent parties.
A. Less security
B. Greatest risk of unauthorized access
C. Significantly greater processing overhead
D. Violating regulatory compliance
C. Bit-splitting, as with many security methods/technologies, carries a significantly greater overhead than data sets that don’t use this method. Bit-splitting, in particular, takes an extensive amount of processing to perform.
A. It may require trust in additional third parties beyond the primary cloud service provider.
B. There may be cause for management concern that the technology will violate internal policy.
C. Users will have far greater difficulty understanding the implementation.
D. Limited vendors make acquisition and support challenging.
A. This is not a simple question and requires the reader to think through the situation suggested by each answer. Option A is correct because the data owner may opt to perform bit-splitting across multiple cloud services to enhance security (not all the “eggs” will be in one “basket”). When this is the case, the data owner will have additional dependencies: all the vendors involved in storing the various data elements.
A. Greater chance of physical theft of assets
B. Loss of public image
C. Some risk to availability, depending on the implementation
D. A small fire hazard
C. Ironically, data dispersion can lead to some additional risk of loss of availability, depending on the method/breadth of the dispersion. If the data is spread across multiple cloud providers, there is a possibility that an outage at one provider will make the data set unavailable to users, regardless of location. However, there are methods for attenuating this threat, and bit-splitting usually provides greater availability of data over traditional storage without dispersion.
A. Inverse postulation
B. Homomorphic encryption
C. Didactic alignment
D. Obverse reinstantiation
B. This is the definition of homomorphic encryption.
A. Big data
B. Real-time analytics
C. Agile analytics
D. Agile business intelligence
B. Real-time analytics allows for reactive and predictive operations (such as recommending other, related products) based on customers’ current and past shopping behavior.
A. Obverse polyglotism
B. Big data
C. Real-time analytics
D. Agile analytics/business intelligence
D. The Agile approach to data analysis offers greater insight and capabilities than previous generations of analytical technologies.
A. Metadata
B. Labels
C. Content analysis
D. Data hover
D. Data hover is a made up term which is not a data discovery technique. All the other answers are actual data discovery techniques.
A. Metadata
B. Labels
C. Content analysis
D. Data hover
A. This is the definition of metadata: data about data, usually created by systems (hardware and/or software) when the data is captured/collected.
A. The security office
B. Users
C. Data owners
D. Regulators
C. The data owners, presumably the personnel closest to and most familiar with the data, should be the ones labeling it.
A. During the risk assessment
B. As part of the business impact analysis (BIA)
C. At collection/creation
D. When the discovery tools are implemented
C. For the most efficient classification/categorization process, and to streamline the application of proper controls, data labeling should be performed when the data is first being collected/created.
A. Egress monitoring solutions
B. Digital rights management (DRM)
C. iSCSI
D. Fibre Channel over Ethernet (FCoE)
A. Egress monitoring tools (often referred to as DLP) are specifically designed to seek out and identify data sets based on content; this is part of how they operate. They can be used for or in conjunction with content-based data discovery efforts.
A. Keywords
B. Pattern matching
C. Frequency
D. Inheritance
D. Inheritance has nothing to do with content analysis; it is usually referring to object-oriented traits derived from originating objects.
A. Increased chance of external penetration
B. Flawed management decisions based on edited displays
C. Higher likelihood of inadvertent disclosure
D. Raised incidence of physical theft
B. Because dashboards are often used for management purposes (graphical representations of technical data), management pressures often result in skewed data dashboarding (“no red!”), which can lead to the “data” being used for fallacious decisions.
A. Bandwidth latency issues
B. Poor physical security of the data center
C. Severe statutory regulation
D. Inaccurate or incomplete data
D. A data discovery effort can only be as effective as the veracity and quality of the data it addresses. Bad data will result in ineffective data discovery.
A. Allowing sufficient access to large volumes of data
B. Preserving metadata tags
C. Assigning labels
D. Preserving and maintaining the data
C. Label assignment is a task of the data owner—the cloud customer, not the provider.
A. National Institute of Standards and Technology (NIST) Special Publication (SP)
B. Applicable laws and regulations
C. Payment Card Industry Data Security Standard (PCI DSS)
D. The managed services contract and SLA
D. The cloud customer will have to determine which levels of performance/responsibilities on the part of the provider will be necessary to meet the customer’s needs for data discovery. These should be codified in the contract/service-level agreement (SLA).
A. The cloud provider
B. National Institute of Standards and Technology (NIST)
C. Regulators
D. The cloud customer
D. This is a difficult question and requires insight on the practice of classifying data and a good understanding of the material. While the determination of what sorts of data need to be protected may come from external sources (laws, standards, regulations, etc.), the classification of data for each data owner/cloud customer will be specific to that entity. Therefore, the cloud customer will have to impose data classification schema on itself and its own data.
A. File size
B. Origin of the data
C. Sensitivity of the data
D. Whatever the data owner decides
D. This is a difficult, and somewhat tricky, question. Each organization has to decide, for itself, how to classify its own data. With that said, many factors bear on this determination: external regulations and drivers, the type of industry in which the organization operates, and so forth. But the kinds of data the organization uses, and how that data is sorted, will differ for every organization, and each must make its own determination on how to best sort that data.
A. Security
B. Labeling
C. Control
D. Markup
B. This is another difficult question. Classification of data is an element of labeling, insofar as labeling is the grouping of data into discrete categories and types. Labels must be affixed to objects and data sets in accordance with an overall policy that lists objective criteria to guide the data owner(s) in assigning the appropriate label; this is a form of classification.
A. Inverse or obverse
B. Automatic or manual
C. Correct or incorrect
D. Diurnal or nocturnal
B. An organization could implement an automated tool that assigns labels based on certain criteria (location of the source of the data, time, creator, content, etc.), much like metadata, or the organization could require that data creators/collectors assign labels when the data is first created/collected, according to a policy that includes discrete, objective classification guidance.
A. Color change
B. Time
C. Repurposing
D. Transfer of ownership
A. Color is unlikely to be a characteristic for which data is classified, much less reclassified. Although some exceptions might exist (motion picture production, satellite imagery, paint vendors, etc.), those would be far from the norm, and the other answers are much more general cases and would apply to many more organizations. Therefore, color is the correct answer (in the negative), and the rest are incorrect (because they are true).
A. Dollar values
B. Metadata
C. Security controls
D. Policies
C. The purposes of classifying/categorizing data is to create proper associated control sets for each data type and aid the efficiency and cost-effectiveness of applying those controls to that data.
A. Multitenancy
B. Virtualization
C. Remote access
D. Physical distance
B. Data transforming from raw objects to virtualized instances to snapshotted images back into virtualized instances and then back out to users in the form of raw data may affect the organization’s current classification methodology; classification techniques and tools that were suitable for the traditional IT environment might not withstand the standard cloud environment. This should be a factor of how the organization considers and perceives the risk of cloud migration.
A. The user
B. The subject
C. The cloud provider
D. The cloud customer
D. The cloud customer, as the PII data owner, is ultimately legally responsible for all losses of PII data. The customer may be able to recoup some of the costs of damages related to the breach by placing financial liability on the provider through the use of strong contract terms and conditions, but all legal responsibility falls on the customer, in all cases.
A. The cloud customer
B. The cloud provider
C. The regulator
D. The individual
D. The subject is the human being to whom the PII applies.
A. The cloud customer
B. The cloud provider
C. The regulator
D. The individual
B. In a PII context, the processor is any entity that processes data on behalf or at the behest of the data owner. In the case of most managed cloud service arrangements, that will be the cloud service provider. (The cloud customer may also process its own data, but the customer is the data owner/controller.)
A. The cloud customer
B. The cloud provider
C. The regulator
D. The individual
A. In a PII context, the controller is the entity that creates/collects, owns, or manages the data—that is, the data owner. In a managed cloud service arrangement, that would be the cloud customer.
A. Storing
B. Viewing
C. Destroying
D. Printing
B. This is not a simple question, and it requires a bit of insight into uses of data. The most suitable answer here is “viewing,” as it is entirely passive; the viewer is not performing any action on the data. “Processing,” in a PII context, is any manipulation of the data, to include securing or destroying it, in electronic or hard-copy form. In a “viewing” action, the processor would be displaying the data to the viewer, while the viewer is only receiving it, not storing it or using it. Note that the answer did not involve “using,” which definitely would be a processing action.
A. Argentina
B. The United States
C. Italy
D. Australia
B. The United States has some federal PII laws that apply to specific sectors (the government itself [Privacy Act], medical providers [Health Information Portability and Accountability Act], financial and insurance vendors [Gramm-Leach-Bliley Act], etc.), but not a single, overarching federal law that addresses PII in a uniform, nationwide manner.
A. Opt in
B. Opt out
C. Undergo screening
D. Provide a biometric template
A. Under HIPAA, the subject must opt in to information sharing—that is, the subject (the patient) must explicitly state, in writing and with a signature, who the vendor is allowed to share personal information with, such as family members, spouses, parents, and children. (Under HIPAA, this personal information is referred to as electronic private health information [ePHI].) The vendor is prohibited from sharing the patient’s data with anyone else.
A. Opt in
B. Opt out
C. Undergo screening
D. Provide a biometric template
B. Under GLBA, financial and insurance vendors are allowed to share account holders’ personal data with other entities (including other businesses owned by the same vendor) unless the account holder explicitly states, in writing, that the vendor is not allowed to do so. The vendor is required to provide a form for opting out of data sharing when the account holder creates the account and annually every subsequent year.
A. A passing fad
B. A human right
C. A legal obligation
D. A business expense
B. The EU is probably at the forefront of global efforts to sanctify and enshrine personal privacy; the current statutes and precedents based on court decisions have clearly denoted Europe’s intent to treat individual privacy as a human right.
A. Argentina
B. The United States
C. Japan
D. Israel
B. The EU regulations associated with personally identifiable information (PII) belonging to EU citizens prohibit that data to be utilized in any way in any country that does not have a national privacy law commensurate with the EU regulations. Of this list, only the United States has no such law. Indeed, the EU regulations might very well be taken to be aimed directly at the United States, and probably for good reason; the United States has not proven to be a good steward of or even recognize the importance of personal privacy.
A. Secure
B. Delivered
C. Forgotten
D. Protected
C. The right to be forgotten is the EU’s codification of an individual’s right to have any data store containing their own personal data purged of all personally identifiable information (PII). There are, of course, some obvious exceptions (such as law enforcement databases).
A. A PLA might limit the provider’s liability.
B. A PLA would force the provider to accept more liability.
C. A PLA is nonbinding.
D. A PLA is not enforceable.
B. Under current laws and regulations, ultimate liability for the security of privacy data rests on the data controller—that is, the cloud customer. A PLA would require the cloud provider to document expectations for the cloud customer’s data security, which would be an explicit admission of liability. There is little motivation for cloud providers to take on this additional liability (and the costs associated with it) with no mandate or market force pushing them to do so.
A. ISACA’s Control Objectives for Information and Related Technology (COBIT)
B. Payment Card Industry Data Security Standard (PCI DSS)
C. The Capability Maturity Model (CMM)
D. International Organization for Standardization (ISO) 27001
C. The CMM is not included in the CSA CCM and, indeed, is not even a security framework.
A. Health Information Portability and Accountability Act (HIPAA)
B. Family Education Rights and Privacy Act (FERPA)
C. Personal Information Protection and Electronic Documents Act (PIPEDA)
D. Digital Millennium Copyright Act (DMCA)
D. The DMCA deals with intellectual property and not specifically with personal privacy. It is not included in the CSA CCM.
A. A trusted device
B. Proprietary software
C. Medical records
D. Financial data
A. DRM solutions are mainly designed to protect intellectual property assets (and mainly those covered by copyright, hence the name), but they can also be used to provide enhanced protection to other electronic information. All the other options are forms of electronic information, while option A is a piece of hardware; DRM does not enhance hardware security, so this is the correct answer.
A. User consent and action
B. Enhanced security protocols
C. Use of the cloud
D. Newer, upgraded devices
A. Deploying DRM usually requires installing a local agent on each device intended for use in that environment; with BYOD, that means getting all users to agree and install that agent because they own the devices.
A. A uniform browser installation
B. Platform-agnostic solutions
C. Turnstiles
D. A secondary business continuity and disaster recovery (BC/DR) vendor
B. In a BYOD environment, users might bring any number of devices/operating systems to the network, and any DRM solution selected for the purpose must interact well with all of them.
A. Physical security
B. Infrastructure as a service (IaaS)
C. Application security
D. Business drivers
D. The CSA CCM does not deal with whether security controls are feasible or correct from a business perspective, only whether they are applicable to an organization under certain regulations.
A. A tracking device
B. An access policy
C. A hardware security module (HSM)
D. A biometric system
B. For DRM to work properly, each resource needs to be outfitted with an access policy so that only authorized entities may make use of that resource.
A. Roaming identity services (RIS)
B. Egress monitoring solutions (DLP)
C. Internal hardware settings (BIOS)
D. The TEMPEST program
B. DRM and DLP work well to address complementary security issues—namely, asset classification/categorization and discovery, along with access and dissemination of those assets.
A. Continuous audit trail
B. Limiting printing output
C. Persistence
D. Automatic expiration
C. Access rights following the object in whatever form or location it might be or move to is the definition of persistence, one of the required traits for a DRM solution of any quality.
A. Continuous audit trail
B. Limiting printing output
C. Persistence
D. Automatic expiration
A. Capturing all relevant system events is the definition of a continuous audit trail, one of the required traits for a DRM solution of any quality.
A. Integration with email filtering engines
B. Disabling screencap capabilities
C. Continuous audit trail
D. Dynamic policy control
D. The question describes dynamic policy control, one of the required traits for a DRM solution of any quality.
A. Persistence
B. Disabling screencap capabilities
C. Automatic expiration
D. Dynamic policy control
C. The question describes automatic expiration, one of the required traits for a DRM solution of any quality.
A. Persistence
B. Support for existing authentication security infrastructure
C. Continuous audit trail
D. Dynamic policy control
B. The question describes support for existing authentication security infrastructure, one of the required traits for a DRM solution of any quality.
A. Location of the data archive
B. Frequency of backups
C. Security controls in long-term storage
D. Data recovery procedures
D. This is not an easy question and requires some interpretation and abstract thought. All of the elements listed are extremely important aspects of the data retention policy. However, using proper data retrieval procedures is the one without which all the others may become superfluous. An organization can perform thorough backups in a timely manner and secure them properly at an excellent location, but if those backups can’t be used to restore the operational environment, they are pointless.
A. Deletion
B. Archiving
C. Crypto-shredding
D. Storing
B. The question states the definition of archiving.
A. The date on which the policy will expire
B. The assignment of an entity to review the applicability of the possibility occasionally
C. The assignment of an entity to monitor and maintain the process described in the policy
D. A list of the laws, regulations, practices, and/or standards that drove the creation of the policy
A. Not all policies are temporary or have expected durations; usually, policy is an enduring piece of governance that will continue until such time as it is revoked.
A. Removing data objects or files
B. Minimizing or eliminating data remanence
C. Removing pointers and metadata about specific files or objects
D. Creating a secure, archived copy for business continuity and disaster recovery (BC/DR) purposes
D. Secure sanitization is intended to ensure that there is no possible way for the data to be recovered; a backup copy would defeat the entire purpose.
A. Drives and disks must be demagnetized for true secure destruction.
B. Physical destruction is the only acceptable method of secure sanitization.
C. Deletion usually only removes pointers or indicators of file location.
D. Only administrators should be allowed to delete files or objects.
C. Deletion, using basic system assets (usually the operating system), mainly involves removing pointers to and addresses of the files or objects that are the targets of deletion. This leaves the raw data remaining on the storage resource, and it could be recovered later.
A. Cloud data doesn’t have substance
B. Regulations prevent it
C. The hardware belongs to the provider
D. Most of the data is subterranean
C. The preferred methods of secure sanitization require physical access to (and control of) the hardware on which the data is stored; in the cloud, this belongs to the cloud provider, and the cloud customer will not be allowed to perform destructive procedures.
A. Data in the cloud is constantly being replicated and backed up
B. Delete commands are prohibited in the cloud
C. Internet service providers (ISPs) will not allow destruction of data stored in the cloud
D. The end clients may prevent it
A. One of the benefits of using managed cloud services is that most providers are constantly performing backup and preservation activities in order to ensure that customers do not lose data. This can make it complicated for customers to even locate all their stored data, much less permanently destroy it.
A. Only law enforcement is permitted to destroy cloud data
B. The largest cloud vendors have prevented customers from destroying data
C. Cloud data renews itself automatically
D. The cloud is often a multitenant environment
D. Secure sanitization would affect storage resources where more than one customer stores their data; truly secure destructive measures would likely result in destroying data belonging to someone else.
A. Degaussing
B. Crypto-shredding
C. Physical destruction of resources that store the data
D. Legal order issued by the prevailing jurisdiction where the data is geographically situated
C. Destroying the drive, disk, and media where the data resides is the only true, complete method of data destruction.
A. All the data storage space in the cloud is already gaussed.
B. Cloud data storage may not be affected by degaussing.
C. Federal law prohibits it in the United States.
D. The blast radius is too wide.
B. Cloud data storage likely uses solid-state drives (or disks), which are not affected by degaussing because they don’t use magnetic properties to store data.
A. Yes, but only if you use multiple passes.
B. No, because you can’t get physical access to cloud storage resources.
C. Yes, but it requires a final pass with all zeros or ones.
D. No, because the logical location of the stored data is almost impossible to determine.
D. Overwriting is the practice of filling the entire storage of the target data with randomized characters (usually involving multiple passes and a final pass with a single, repeated character). In the cloud, this is untenable for many reasons, including the fact that cloud data is constantly moving from one storage resource to another and is not kept in a single, identifiable logical location for an extended period of time (which is actually a security benefit). Without you knowing which storage resources to overwrite, overwriting is impossible.
A. Overwriting an entire storage resource would affect other tenants’ data
B. Regulators usually frown on the practice
C. Locating the specific storage locations of cloud data is almost impossible
D. Data is being backed constantly in the cloud; before you finished overwriting an entire data set, it would have been replicated elsewhere
B. Regulators do not disapprove of secure sanitization; it is an acceptable form of secure data destruction if implemented properly.
A. The cloud provider also managing the organization’s keys
B. Lack of physical access to the environment
C. External attackers
D. Lack of user training and awareness
A. Crypto-shredding relies on the eventual destruction of the final keys; if keys are not under the management of the customer, they may be replicated or difficult to dispose of.
A. One
B. Two
C. Three
D. Four
B. The proper procedure for crypto-shredding requires two cryptosystems: one to encrypt the target data, the other to encrypt the resulting data encryption keys.
A. Ensuring profitability
B. Increasing performance
C. Motivating users
D. Correcting accidental errors
D. If users inadvertently erase or modify data, an archived backup copy could be useful for restoring the original, correct version.
A. Team building and morale
B. Forensic investigation
C. Choosing security controls
D. Enhancing quality
B. An archived data set could be useful for investigative purposes, especially if it covers a significant period of time and includes multiple copies. The archived versions may be used as a reference to determine when a certain malicious activity occurred, which is useful during an investigation.
A. Compliance/audit
B. Monitoring performance
C. Gathering investment
D. Enforcing policy
A. Archiving may be required by regulation, and archived versions of the environment or data may be used to create deliverables for auditors, especially if the archive included event logs.
A. The cloud customer
B. The cloud provider
C. The customer’s regulator
D. Depends on the contract
D. Many cloud providers will offer archiving services as a feature of the basic cloud service; realistically, most providers are already performing this function to avoid inadvertent loss of customer data, so marketing it is a logical step. However, because the customer is ultimately responsible for the data, the customer may elect to use another, or an additional, archive method. The contract will stipulate specific terms, such as archive size, duration, and so on.
A. How long the data must be kept before destruction
B. The depth of underground storage bunkers used for archiving
C. The names of specific personnel tasked with restoring data in the event of data loss in the operational environment
D. The name(s) of regulators approving the policy
A. The policy for data archiving and retention must include guidance on the length of time data is expected to remain stored.
A. Names of personnel allowed to receive backup media, if third-party off-site archiving services are used
B. Explicit statement of data formats and types of storage media
C. A list of personnel whose data will be archived on a regular basis
D. Which Internet service provider (ISP) should be used for backup procedures
B. It is important to indicate the data format and media type for long-term storage in order to ensure restoration capability; outdated or obsolete data formats and media may not be useful for restoration of data to the operational environment several years after it has been stored.
A. Applicable regulatory entities
B. Federal and local law enforcement
C. The originator or publisher of the governing policy
D. The cloud provider’s security response office
C. Once the policies have been published and put into force, the names and contact information of the people who crafted them are no longer useful or germane.
A. Definition of security events and incidents
B. The brand or vendor of the cloud provider’s audit or logging tool
C. Process for adding new audit or logging rules
D. Process for filtering out false positives by amending the rule set
B. This is a question that requires some thought. All the answers are processes or elements that should be included in the security operations’ procedures except for option B; the cloud customer will not get to select, or probably even know, what tools and devices the cloud provider has put into place, so this will not be included in the customer’s procedures.
A. Prohibiting certain parties from a private conversation
B. Ensuring that a transaction is completed before saving the results
C. Ensuring that someone cannot turn off auditing capabilities while performing a function
D. Preventing any party that participates in a transaction from claiming that it did not
D. Option D is the definition of nonrepudiation.