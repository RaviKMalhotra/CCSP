Chapter 5: Domain 5—Cloud Security Operations
Domain 5 in the Certified Cloud Security Professional (CCSP) Exam Outline both introduces some significant new concepts, such as the physical design of a data center and the attendant standards and guidelines, and restates some material covered in earlier domains, such as multitenancy, resource pooling, and the like.

### Question # 1 - What is the primary incident response goal?     
A. Remediating the incident                  
B. Reverting to the last known good state        
C. Determining the scope of the possible loss       
D. Outcomes dictated by business requirements       
Answer:  D. 

This is not an easy question; different industries and different organizations will have differing goals. Each organization will determine for itself what the primary goal of incident response will be, and this may even differ from incident to incident, depending on the nature of the incident itself (in other words, a given organization may set priorities such that the primary goal of incident response in a disaster is continuity of operations, while the goal in responding to unauthorized access may be halting data disclosure).

### Question # 2 - You are in charge of building a cloud data center. Which raised floor level is sufficient to meet standard requirements?     
A. 10 inches      
B. 8 inches        
C. 18 inches        
D. 2 feet      
Answer: D. 

The minimum recommended height of a raised floor in a data center is 24 inches. All other options are incorrect.

### Question # 3 - You are in charge of building a cloud data center. What purposes does the raised floor serve?          
A. Allows airflow and increases structural soundness for holding large components       
B. Cold air feed and a place to run wires for the machines                               
C. Additional storage for critical components and a dedicated access to a landline           
D. Fire suppression systems and personnel safety                 
Answer: B. 

The raised floor in a data center will serve as an air plenum (usually for cold air) and a wiring chase. All the other options are incorrect.

### Question # 4 - You are in charge of building a cloud data center. Which of the following is a useful rack configuration for regulating airflow?         
A. Exhaust fans on racks facing the inlet vents of other racks           
B. Inlet fans on racks facing exhaust fans of other racks           
C. All racks perpendicular to each other                       
D. Exhaust fans on racks facing exhaust fans on other racks                 
Answer: D. 

The preferred method is cold aisle containment (hot aisle containment, where the inlets on racks face each other, is all right too). Options A and B are the same incorrect answer, just worded differently; if the exhaust fans on one rack face into the inlet vents on another rack, you would end up blowing warm air into the components, defeating the purpose of airflow management. Perpendicular racks will not optimize your airflow.

### Question # 5 - An event is something that can be measured within the environment. An incident is a(n) _______________ event.          
A. Deleterious         
B. Negative           
C. Unscheduled            
D. Major            
Answer: C.          

All activity in the environment can be considered events. Any event that was not planned or known is an incident. In the security industry, we often ascribe negative effects to the term incident, but incidents are not always malicious; they are only unscheduled.

All the other options are incorrect.

### Question # 6 - Which of the following factors would probably most affect the design of a cloud data center?            
A. Geographic location              
B. Functional purpose              
C. Cost                 
D. Aesthetic intent           
Answer: A. 

This is a difficult, nuanced question. Options A–C are true; each element would affect the design of a cloud data center (D is not something that should be included in data center design). But the physical location of the data center would include legal constraints (based on jurisdiction), geological/natural constraints (based on altitude, proximity to water formations/flooding, climate, natural disaster, etc.), price, and other variables. Therefore, location would most likely have the greatest impact on the design of the facility.

### Question # 7 - All of the following elements must be considered in the design of a cloud data center except _______________.                
A. External standards, such as ITIL or ISO 27001            
B. Physical environment           
C. Types of services offered                         
D. Native language of the majority of customers              
Answer: D. 

Language of the customers is irrelevant, assuming they can pay. All the other options are factors that must be considered in data center design.

### Question # 8 - In designing a data center to meet their own needs and provide optimum revenue/profit, the cloud provider will most likely aim to enhance _______________.          
A. Functionality               
B. Automation of services          
C. Aesthetic value          
D. Inherent value           
Answer: B.        

This is not an easy question. All the options are correct except C. Option B is the most correct because it will lead to maximizing performance, value, and profitability.

### Question # 9 - You are the security officer for a small cloud provider offering public cloud infrastructure as a service (IaaS); your clients are predominantly from the education sector, located in North America. Of the following technology architecture traits, which is probably the one your organization would most likely want to focus on?          
A. Reducing mean time to repair (MTTR)          
B. Reducing mean time between failure (MTBF)          
C. Reducing the recovery time objective (RTO)            
D. Automating service enablement          
Answer: D.           

The goal of automating service enablement is probably paramount for any cloud service provider (of the qualities listed), because it allows for the most scalability and offers the most significant reduction in costs (which mainly come from personnel) and therefore the most profitability. The details of “public cloud,” “IaaS,” and “North America” are distractors in this context as they are irrelevant—this answer would be true for any cloud provider offering any type of services.

Options A and B are not true because most cloud providers of any appreciable size are purchasing hardware on a scale that makes the per-unit failure rate fairly irrelevant; the bulk nature of IT purchases by cloud providers makes differences in MTTR and MTBF between vendors and products statistically insignificant.

Option C is incorrect because RTO is a quality involving business continuity and disaster recovery (BC/DR) planning, not IT architecture.

### Question # 10 - What is perhaps the main way in which software-defined networking (SDN) solutions facilitate security in the cloud environment?          
A. Monitoring outbound traffic          
B. Monitoring inbound traffic          
C. Segmenting networks                
D. Preventing distributed denial of service (DDoS) attacks               
Answer: C. 

Network segmentation allows providers to create zones of trust within the cloud environment, tailoring the available services to meet the needs of a variety of clients and markets.

SDN does not really involve monitoring outbound traffic (that is done by egress monitoring solutions) or inbound traffic (that is usually performed by firewalls and routers), nor does it really prevent DDoS attacks (nothing can prevent such attacks, and risk reduction is usually done by routers), so all the other options are incorrect.

### Question # 11 - The logical design of a cloud environment can enhance the security offered in that environment. For instance, in a software as a service (SaaS) cloud, the provider can incorporate _______________ capabilities into the application itself.           
A. High-speed processing          
B. Logging                  
C. Performance-enhancing          
D. Cross-platform functionality           
Answer: B. 

The ability to log activity is useful for many security purposes (such as monitoring and forensics); having that purposefully included in SaaS applications reduces the need to have a different tool added to the environment to achieve that same goal and reduces the possibility that any additional interface won’t perform optimally.

The other options are all about enhancing the customer’s ability to perform business function or meeting the customer’s business needs. Although this is paramount from the customer’s perspective and may tangentially fulfill some security purpose (increased processing capacity may, for instance, allow the use of additional encryption, where the overhead may otherwise deter the use of that tool), these are not direct security purposes and therefore are not correct answers to this specific question.

### Question # 12 - You are tasked with managing a cloud data center in Los Angeles; your customers are mostly from the entertainment industry, and you are offering both platform as a service (PaaS) and software as a service (SaaS) capabilities. From a physical design standpoint, you are probably going to be most concerned with _______________.           
A Offering digital rights management (DRM) capabilities          
B. Insuring against seasonal floods               
C. Preventing all malware infection potential            
D. Ensuring that the racks and utilities can endure an earthquake          
Answer: D. 

California is known for suffering massive destruction from earthquakes, and physical design is the means with which this risk is addressed.
All the other options either involve a nonphysical risk (DRM will be necessary, because the entertainment industry relies heavily on copyrighted material) or a method other than physical design to address a risk (floods are 

physical threats, but insurance is an administrative control for risk transfer), so D is the best choice of these options.

### Question # 13 - You are the security manager for a small retail business involved mainly in direct e-commerce transactions with individual customers (members of the public). The bulk of your market is in Asia, but you do fulfill orders globally. Your company has its own data center located within its headquarters building in Hong Kong, but it also uses a public cloud environment for contingency backup and archiving purposes. Your cloud provider is changing its business model at the end of your contract term, and you have to find a new provider. In choosing providers, which tier of the Uptime Institute rating system should you be looking for, if minimizing cost is your ultimate goal?           
A. 1           
B. 3             
C. 4            
D. 8        
Answer: A. 

For the purposes described in the question, a Tier 1 data center should suffice; it is the cheapest, and you need it only for occasional backup purposes (as opposed to constant access). The details of location and market are irrelevant.

Tiers 3 and 4 would be much more expensive, and they are not necessary for your business purposes; options B and C are thus incorrect.

There is no Tier 8 in the Uptime Institute system.

### Question # 14 - You are the security manager for a small retail business involved mainly in direct e-commerce transactions with individual customers (members of the public). The bulk of your market is in Asia, but you do fulfill orders globally. Your company has its own data center located within its headquarters building in Hong Kong, but it also uses a public cloud environment for contingency backup and archiving purposes. Your cloud provider is changing its business model at the end of your contract term, and you have to find a new provider. In choosing providers, which of the following functionalities will you consider absolutely essential?         
A. Distributed denial of service (DDoS) protections          
B. Constant data mirroring            
C. Encryption              
D. Hashing          
Answer: C.           

If your company is involved in e-commerce, you are most likely using credit cards for online transactions; if you’re using credit cards, you are almost certainly constrained by the Payment Card Industry Data Security Standard (PCI DSS) or one of the other contractual standards like it. Because of this, you will be required to encrypt or tokenize all stored cardholder data, and for long-term storage, encryption is the cheaper, more durable process.
DDoS and mirroring are availability protections, and availability is not your company’s main concern for cloud services from the question description; long-term storage is not focused on availability. Options A and B are thus incorrect.

Hashing is an integrity protection, and though hashes may be useful in this case (to determine whether stored data is accurate), they won’t be as important as compliance with credit card standards. Option C is the preferable answer compared to D.

### Question # 15 - You are the security manager for a small retail business involved mainly in direct e-commerce transactions with individual customers (members of the public). The bulk of your market is in Asia, but you do fulfill orders globally. Your company has its own data center located within its headquarters building in Hong Kong, but it also uses a public cloud environment for contingency backup and archiving purposes. Which of the following standards are you most likely to adopt?                  
A. National Institute of Standards and Technology (NIST) 800-37        
B. General Data Protection Regulation (GDPR)          
C. ISO 27001                     
D. Sarbanes–Oxley Act (SOX)            
Answer: C. 

ISO is the only truly international standard on this list of choices; all the rest are either American laws or standards (options A and D) or European (option B).

### Question # 16 - You are the security manager for a small retail business involved mainly in direct e-commerce transactions with individual customers (members of the public). The bulk of your market is in Asia, but you do fulfill orders globally. Your company has its own data center located within its headquarters building in Hong Kong, but it also uses a public cloud environment for contingency backup and archiving purposes. Your company has decided to expand its business to include selling and monitoring life-support equipment for medical providers. What characteristic do you need to ensure is offered by your cloud provider?         
A. Full automation of security controls within the cloud data center          
B. Tier 4 of the Uptime Institute certifications           
C. Global remote access                 
D. Prevention of ransomware infections              
Answer: B. 

The changing nature of your business will require a much more stringent set of operating standards, to include an increase in Uptime Institute tier levels; because you’re no longer just using the cloud for backup and long-term storage and are now using it in direct support of health and human safety, Tier 4 is required.

Fully automated security controls are useful from the provider’s perspective (allowing more profitability and scalability), but this is not a major concern of the customer. Option A is incorrect.
Global remote access and reducing the risk of malware infections (to include ransomware) are basic functions of almost all cloud providers; these functions aren’t useful discriminators when choosing cloud providers because all cloud providers have them. Options C and D are thus incorrect.

### Question # 17 - When designing a cloud data center, which of the following aspects is not necessary to ensure continuity of operations during contingency operations?          
A. Access to clean water           
B. Broadband data connection        
C. Extended battery backup                  
D. Physical access to the data center             
Answer: C. 

Backup power does not have to be delivered by batteries; it can be fed to the data center through redundant utility lines or from a generator.
All the other elements are necessary for safe and secure data center operations, for both the personnel and the equipment within the data center.

### Question # 18 - You are the security manager for a small surgical center. Your organization is reviewing upgrade options for its current, on-premises data center. In order to best meet your needs, which one of the following options would you recommend to senior management?           
A. Building a completely new data center                            
B. Leasing a data center that is currently owned by another firm          
C. Renting private cloud space in a Tier 2 data center            
D. Staying with the current data center                
Answer: A. 

This answer is mostly arrived at through a process of elimination.

Option B is not optimum because of the potential for vendor lock-in, restrictions on buildout, and privacy concerns.

Option C is not optimum because Tier 2 is not sufficient for medical uses.

Option D is not optimum because there was obviously a reason to consider a new option.

We are therefore left with option A, which is the most expensive of the choices but allows the greatest amount of control and security.

### Question # 19 - When building a new data center within an urban environment, which of the following is probably the most restrictive aspect?          
A. The size of the plot          
B. Utility availability          
C. Staffing              
D. Municipal codes           
Answer: D. 

In any large metropolitan area, government restrictions on development and construction can severely limit how you use your property; this can be a significant limiting factor in building a data center.
The size of the plot may or may not matter, depending on if you are allowed to build up or dig down to make use of additional space—these options will be limited by municipal building codes, so option D is preferable to option A.
Utilities and personnel are usually easy to acquire in an urban setting, so options B and C are incorrect.

### Question # 20 - When you are building a new data center in a rural setting, which of the following is probably the most restrictive aspect?           
A. Natural disasters          
B. Staffing                               
C. Availability of emergency services          
D. Municipal codes          
Answer: C.           

In a rural location, the positioning and depth of first responders (fire, law enforcement, paramedics, etc.) may be severely limited in comparison to an urban setting.
Natural disasters affect all locations, rural or urban, so a rural setting is not any more or less limiting in planning accordingly; option A is incorrect.
Oddly enough, because of the very limited need for personnel within modern data centers with significant automation, recruiting and placing the number of people necessary to serve the purpose should not be too difficult; option 

B is not correct.

One of the appeals of a rural setting is that building codes are often rudimentary or nonexistent. Option D is incorrect.
### Question # 21 - All tiers of the Uptime Institute standards for data centers require _______________ hours of on-site generator fuel.                
A. 6           
B. 10             
C. 12          
D. 15        
Answer: C. 

All the other options are incorrect.

### Question # 22 - The American Society of Heating, Refrigeration, and Air Conditioning Engineers (ASHRAE) guidelines for internal environmental conditions within a data center suggest that a temperature setting of _______________ degrees (F) would be too high.                 
A. 93            
B. 80              
C. 72             
D. 32             
Answer: A.              

The range suggested by the ASHRAE Technical Committee 9.9 is 64 to 81 degrees Fahrenheit. All the other options are distractors (although D is particularly distracting, because it is lower than the recommended range, but that is not what the question is asking).

### Question # 23 - Internal data center conditions that exceed the American Society of Heating, Refrigeration, and Air Conditioning Engineers (ASHRAE) guidelines for humidity could lead to an increase of the potential for all of the following except _______________.              
A. Biological intrusion                
B. Electrical shorting                    
C. Corrosion/oxidation                   
D. Social engineering                  
Answer: D.                

Being damp does not make people more susceptible to trickery.
Moisture in the air can, however, create mold/mildew, short circuits, and rust, so all the other options are incorrect.

### Question # 24 - Setting thermostat controls by measuring the _______________ temperature will result in the highest energy costs.              
A. Server inlet               
B. Return air              
C. Under-floor                
D. External ambient              
Answer: B.            

The return air temperature will be slightly higher than anywhere else inside the data center because the air has been warmed by passing through the equipment (thus cooling the equipment but warming the air). Using this as a temperature set point will result in much cooler air feeding the server inlets, which takes more energy, which will be more expensive.

Options A and C are incorrect because that air is already cold; using these locations as set points will not consume as much energy and may result in somewhat warmer air entering the servers. This will be less expensive than option B.

Option D is an outlying distractor; if you set your heating, ventilation, and air conditioning (HVAC) controls to respond to the temperature outside the data center, your HVAC units are responding to temperatures that have nothing to do with the internal environment. In effect, you’d be trying to adjust the temperature of the outside world, which is ridiculous.

### Question # 25 - Heating, ventilation, and air conditioning (HVAC) systems cool the data center by pushing warm air into _______________.            
A. The server inlets            
B. Underfloor plenums           
C. HVAC intakes              
D. The outside world             
Answer: D.              

The HVAC system is a heat exchange, swapping warm internal air from the data center to the outside world and drawing fresh air through the HVAC chillers to feed the internal environment.
All the other options are incorrect because they will have the opposite effect by pushing warm air into those areas that cools air is supposed to be.

### Question # 26 - It is important to include _______________ in the design of underfloor plenums if they are also used for wiring.              
A. Mantraps                  
B. Sequestered channels             
C. Heat sinks             
D. Tight gaskets                    
Answer: D. 

When cables come up through a raised floor used as a cold air feed, we don’t want cold air bleeding around the cables in an unplanned manner; this can cause inefficiencies in airflow control. Gaskets are required at all points where cable comes through the floor, to restrict airflow and reduce the possibility of cold air escaping.
All the other options are incorrect because we want to minimize obstructions in underfloor plenums we use for airflow. Options A, B, and C do not accomplish this.

### Question # 27 - Cable management includes all of the following except _______________.           
A. Tagging cables                   
B. Removing unused/obsolete cables            
C. Banding and bundling cables              
D. Removing unused machines             
Answer: D.              

While minimizing equipment in the operational environment can aid in many efforts, including cable management, it is not strictly an aspect of cable management, so this is the best choice from those available. All the other options are definitely aspects of cable management.

### Question # 28 - How often should cable management efforts take place?               
A. Annually              
B. Continually              
C. Quarterly               
D. Weekly               
Answer: B.                

Cable management is an ongoing process. All the other options are incorrect because they are time based intervals rather than continuous.

### Question # 29 - You are designing a private cloud data center for an insurance underwriter, to be located in a major metropolitan area. Which of the following airflow management schemes is preferable?                 
A. Hot aisle          
B. Cold aisle                    
C. Either hot aisle or cold aisle             
D. Free flow                
Answer: C.                   

It shouldn’t matter which design you use as long as airflow is managed. Neither hot nor cold aisle containment is preferable to the other, so options A and B are incorrect. Airflow does need to be managed, though, so option D is incorrect as well.

### Question # 30 - Which of the following factors will probably have the most impact on the cost of running your heating, ventilation, and air conditioning (HVAC) systems?            
A. Whether you choose hot or cold aisle containment               
B. The external ambient environment               
C. The initial cost of the HVAC systems               
D. Proper cable maintenance               
Answer: B.              

This is a difficult question because almost all of the options are true—they will all have an effect on the cost of running HVAC systems.
Because HVAC operates as a heat exchange, the outside environment will dictate how much power is needed to force warm air out of the data center. The warmer the climate in the location of the data center, the more energy it will take to exchange the heat, and the more costly the HVAC operation. This is the most significant factor.

Option A is incorrect and it is the only choice that does not affect energy costs; hot and cold aisle containment should be equivalent in terms of operational costs.
The initial cost of the HVAC units themselves will probably have an effect on operational costs because better equipment will cost more money, but it will also be more efficient and therefore less expensive to operate than 

cheaper alternatives. However, the effect still won’t be as significant as the external climate, so option C is still not as good as option B.
Good cable management will make airflow more efficient and therefore make HVAC less expensive, but this will not be as dramatic in impact on operating costs as the external environment. Once again, option B is preferable to option D.

### Question # 31 - You are designing a Tier 4 data center for a large hospital. In order to plan for the possibility of losing utility power, in addition to having sufficient generators, you should plan to locate the data center _______________.             
A. In an urban setting           
B. In a rural environment             
C. Near a coast           
D. At the border of different counties, regions, or states           
Answer: D.          

Usually, different political regions are served by different utility providers; placing your data center on such a boundary may make it feasible to have redundant, overlapping power providers.
Municipalities typically limit selection of power providers by granting an artificial monopoly to a single provider; option A is incorrect.
Rural settings are often only served by a single provider because the demand is not sufficient to support competition; option B is incorrect.
Coasts do not affect the availability of multiple power providers; option C is a distractor.

### Question # 32 - Because most cloud environments rely heavily on virtualization, it is important to lock down or harden the virtualization software, or any software involved in virtualization. Which of the following is not an element of hardening software?          
A. Removing unused services and libraries          
B. Maintaining a strict license catalog             
C. Patching and updating as necessary                 
D. Removing default accounts              
Answer: B.            

While maintaining a library of software licenses is important, it is not part of the practice we ordinarily consider “hardening.”
The other options are all aspects of software hardening.

### Question # 33 - Which of the following is not an aspect of host hardening?            
A. Removing all unnecessary software and services              
B. Patching and updating as needed                              
C. Performing more frequent and thorough audits on the host                     
D. Installing a host-based firewall and an intrusion detection system (IDS)              
Answer: C. 

Audits usually aren’t considered an element of hardening. Hardening is the process of provisioning a specific element (in this case, a host) against attack. Audits don’t protect against attack; they only detect and direct response to attacks.
All the other options are aspects of host hardening.

### Question # 34 - Which of the following is not an element of ongoing configuration maintenance?              
A. Penetration tests of guest OSs and hosts              
B. Social engineering tests of all users                       
C. Patch management of guest OSs, hosts, and applications                
D. Vulnerability scans of guest OSs and hosts                   
Answer: B. 

Users are not an aspect of configuration management.
All the other options are elements of secure configuration management.

### Question # 35 - Storage controllers will be used in conjunction with all the following protocols except _______________.       
A. HTTPS                                               
B. Internet Small Computer Systems Interface (iSCSI)              
C. Fibre Channel                  
D. Fibre Channel over Ethernet               
Answer: A.                 

HTTPS is not a storage protocol. All the other options are.

### Question # 36 - Which of these characteristics of a virtualized network adds risks to the cloud environment?            
A. Redundancy           
B. Scalability              
C. Pay-per-use            
D. Self-service                
Answer: B.          

Virtual switches are widely used in virtualized networks. Unlike physical switches, which only lose one connection if a connecting cable is lost, virtual switches can be connected to multiple virtual machines via a single cable; if a cable is lost in a virtualized network, that can affect tens or dozens of devices. In this context, the benefits offered by scalability come with attendant risks.
The other options are characteristics that don’t cause additional risk to the environment; in fact, redundancy reduces risk.

### Question # 37 - Security best practices in a virtualized network environment would include which of the following?                                      
A. Using distinct ports and port groups for various virtual local area networks (VLANs) on a virtual switch rather than running them through the same port                    
B. Running Internet Small Computer Systems Interface (iSCSI) traffic unencrypted in order to have it observed and monitored by a network intrusion detection system (NIDS)             
C. Adding a host-based intrusion detection system (HIDS) to all virtual guests             
D. Hardening all outward-facing firewalls in order to make them resistant to attack             
Answer: A.          

It is possible to route multiple VLANs through a switch port (physical or virtual) with proper frame tagging. However, to optimize isolation of subnets and processes in a virtual network environment, it is better to use different ports instead.
iSCSI traffic should be encrypted as another layer of defense within the environment; option B is wrong.
HIDSs may or may not be cost-effective, depending on the value and sensitivity of the data on each guest; the additional overhead may not justify their use. Option C is incorrect.
Firewalls should be hardened regardless of the nature of the network whether virtual or physical.

### Question # 38 - In order to enhance virtual environment isolation and security, a best practice is to _______________.           
A. Ensure that all virtual switches are not connected to the physical network                                     
B. Ensure that management systems are connected to a different physical network than the production systems              
C. Never connect a virtual switch to a physical host            
D. Connect physical devices only with virtual switches                  
Answer: B.                

The management systems control the entirety of the virtual environment and are therefore extremely valuable and need to be protected accordingly. When possible, isolating those management systems, both physically and virtually, is optimum.
All the other options are incorrect because they imply that virtual and physical cannot coexist when in fact they need to coexist to work correctly.
 
### Question # 39 - Which of the following is a risk that stems from a virtualized environment?                      
A. Live virtual machines in the production environment are moved from one host to another in the clear.                    
B. Cloud data centers can become a single point of failure.                                                           
C. It is difficult to find and contract with multiple utility providers of the same type (electric, water, etc.).                 
D. Modern service level-agreement (SLA) demands are stringent and very hard to meet.                     
Answer: A. 

When an active virtual machine is moved from a given host to another (for instance, when the host is going into maintenance state), it is passed along the network without encryption. Theoretically, an insider threat observing the line along which the virtual machine is moving could capture/copy it in its entirety.
All the other options are not risks specific to a virtualized environment and are therefore incorrect.

### Question # 40 - Which of the following is a risk that stems from a pooled-resources environment?                                  
A. Loss of data to widespread phishing attacks                                                            
B. Loss of availability due to widespread distributed denial of service (DDoS) attacks                      
C. Loss of data to widespread insider threat                                         
D. Loss of data to law enforcement seizure of neighboring assets                     
Answer: D. 

In a pooled environment, law enforcement may acquire physical or logical assets (drives, data stores, etc.) that include your organization’s data, even if your organization was not the target of the investigation.

All the other options are not risks due to pooled resources; they exist in all environments. These options are not correct.

### Question # 41 - Modern managed cloud service providers will often use secure keyboard/video/mouse (KVM) devices within their data centers. These devices are extremely expensive compared to their non-secured counterparts. Which of the following is one of the reasons cloud service providers do this?                       
A. They have plenty of revenue and can afford it.                                
B. They have invested heavily in the secure KVM market.           
C. Cloud data centers need very few of these devices.          
D. Managed cloud providers often manufacture their own devices as well.                    
Answer: C. 

The cost of each device is spread across many machines in the data center; unlike a desktop-based environment, where every user and every machine need their own KVM setup, just a few devices can serve an entire data center.
While the cloud provider may generate a great deal of revenue, no company likes to throw away money unnecessarily; option A is incorrect.
Cloud providers are not typically invested in KVM vendors. Option B is incorrect.

Option D is simply incorrect.

### Question # 42 - The American Society of Heating, Refrigeration, and Air Conditioning Engineers (ASHRAE) guidelines for internal environmental conditions within a data center suggest that a temperature setting of _______________ degrees (F) would be too low.                              
A. 93               
B. 80             
C. 72               
D. 32          
Answer: D.              

The range suggested by the ASHRAE Technical Committee 9.9 is 64 to 81 degrees Fahrenheit. All the other options are incorrect (although A is particularly distracting, because it is higher than the recommended range, but that is not what the question is asking).

### Question # 43 - Modern managed cloud service providers will often use secure keyboard/video/mouse (KVM) devices within their data centers. These devices are extremely expensive compared to their non-secured counterparts. Which of the following is one of the reasons cloud service providers do this?                    
A. The risk of transferring data from one customer to another is significant.          
B. The risk of devices leaving the cloud data center is significant.             
C. It makes physical inventories much easier to maintain.            
D. Audit purposes         
Answer: A.           

Secure KVMs support drastically isolated operations; they cut down on the possibility of data being inadvertently shared from one customer to another.

Option B is incorrect because devices will not leave the cloud data center simply because they are not managed by secure KVMs.

Option C is incorrect because using secure KVMs will not have an effect on physical inventories.

Option D does contain enough information to be the correct answer. “Audit purposes” is ambiguous.

### Question # 44 - A truly air-gapped machine selector will _______________.           
A. Terminate a connection before creating a new connection           
B. Be made of composites and not metal           
C. Have total Faraday properties           
D. Not be portable           
Answer: A.           

Referred to as “break before make,” these devices often take the form of manual pushbutton controls; as the button is pushed, the current connection is forced to physically separate, and when the button is fully engaged, the new connection is made.

Options B and C have more to do with risks of electromagnetic emanations than with air-gapped selectivity; even air-gapped devices can leak data through emanations.

Option D is incorrect because portability is not a property we seek in device selectors.

### Question # 45 - Which of the following cloud data center functions do not have to be performed on isolated networks?          
A. Customer access provision       
B. Management system control interface        
C. Storage controller access            
D. Customer production activities      
Answer: D.       

The production activities will make full use of pooled resources, so they will not be isolated (unless the customer is paying for that specific characteristic of service).
All the other options are functions that should take place on isolated networks/segments.

### Question # 46 - Which of the following is not a characteristic of a virtual local area network (VLAN)?                          
A. Broadcast packets sent by a machine inside the VLAN will reach all other machines in that VLAN.            
B. Broadcast packets sent from outside the VLAN will not reach other machines outside the VLAN.            
C. Broadcast packets sent from a machine outside the VLAN will not reach machines inside the VLAN.              
D. Broadcast packets sent by a machine inside the VLAN will not reach machines outside the VLAN.                
Answer: B. 

Broadcast packets sent by machines outside the VLAN will reach machines outside the VLAN that are on the same network/segment.
All the other options are characteristics of a VLAN.

### Question # 47 - In order for communications from inside a virtual local area network (VLAN) to reach endpoints outside the VLAN, _______________.                     
A. The communications must go through a gateway             
B. The traffic must be encrypted           
C. A repeater must be used                        
D. The external endpoint must be in receive mode               
Answer: A.           

Gateway devices enforce the VLAN rules and can allow or deny outbound traffic.

Communications traffic from a VLAN may or may not be encrypted; option B is incorrect.

Repeaters are used to enhance signals along a line over a certain distance; they have nothing to do with VLANs. Option C is incorrect.

Option D makes no sense in this context.

### Question # 48 - Transport Layer Security (TLS) uses _______________ to authenticate a connection and create a shared secret for the duration of the session.                         
A. Security Assertion Markup Language (SAML) 2.0         
B. X.509 certificates          
C. 802.11X                        
D. The Diffie-Hellman process          
Answer: B. 

TLS uses X.509 certificates to establish a connection and create a symmetric key that lasts for only one session.

SAML is used for federation authentication/identification; option A is incorrect.

802.11 is the suite of wireless standards; option C is incorrect.

Diffie-Hellman uses asymmetric key pairs to create a symmetric key; option D is incorrect.

### Question # 49 - Halon is now illegal to use for data center fire suppression. What is the reason it was outlawed?             
A. It poses a threat to health and human safety when deployed.            
B. It can harm the environment.                
C. It does not adequately suppress fires.           
D. It causes undue damage to electronic systems.              
Answer: B. 

This question is an outlier because it is one of the few such questions where the answer is not that it poses a threat to health and human safety (although, in fact, it does; option A is true, but incorrect). Halon was not prohibited because of this property. Halon was outlawed because it, like other CFCs (chlorofluorocarbons), was blamed for depleting the earth’s ozone layer. Halon is still allowed in some very specialized cases (such as fire-suppression systems on aircraft), but this is an exception.
Options C and D are incorrect and untrue.

### Question # 50 - When cloud computing professionals use the term ping, power, pipe, which of the following characteristics is not being described?           
A. Logical connectivity          
B. Human interaction           
C. Electricity                
D. Heating, ventilation, and air conditioning (HVAC)              
Answer: B.             
User interaction with the cloud is not described in this term. All the other options are characteristics of cloud computing mentioned in ping, power, pipe.

### Question # 51 - Which of the following is not a goal of a site survey?             
A. Threat definition              
B. Target identification           
C. Penetration testing            
D. Facility characteristics            
Answer: C.                

The penetration test is not part of the site survey, which is one of the initial steps in securing/auditing a facility. The penetration test will, however, probably make use of the site survey information later.

All the other options are goals of the site survey.

### Question # 52 - Designing system redundancy into a cloud data center allows all the following capabilities except _______________.              
A. Incorporating additional hardware into the production environment         
B. Preventing any chance of service interruption            
C. Load-sharing/balancing                                           
D. Planned, controlled failover during contingency operations             
Answer: B. 

There is no such thing as zero risk; there will always be some chance of service interruption, no matter how minimized.

All the other options are capabilities allowed by redundancy.

### Question # 53 - Gaseous fire suppression systems that function by displacing oxygen need to be installed in conjunction with _______________.        
A. Water cooling         
B. Filters                
C. Occupant training                         
D. Failsafe or “last person out” switches           
Answer: D. 

Before flooding an enclosed space with a gas that will displace oxygen, it is important to ensure that all personnel are out of the area. While this requires personnel training, such training is ineffective without a system to support this capability. Option C is true, but not as accurate as option D.

Options A and B are incorrect because they do not make senses given the question is about a system that displaces oxygen in the facility.

### Question # 54 - What aspect of data center planning occurs first?                          
A. Logical design            
B. Physical design             
C. Audit              
D. Policy revision            
Answer: A. 

The logical design should come before the physical design; function dictates form. Audit and revision come after creation.

### Question # 55 - Which of the following are not examples of personnel controls?           
A. Background checks         
B. Reference checks                    
C. Strict access control mechanisms            
D. Continuous security training          
Answer: C. 

While physical controls that inhibit movement affect personnel, they are not regarded as personnel controls. All the other options are examples of personnel controls.

### Question # 56 - Updating virtual machine management tools will require _______________.               
A. An infusion of capital               
B. An alternate data center               
C. Sufficient redundancy             
D. Peer review               
Answer: C. 

Because updating the virtualization toolset may require server downtime, it is essential to have a sufficient amount of redundant machines to roll out the update over the environment without significant disruption of operations.

Option A assumes that there isn’t already enough of whatever the infusion of capital will purchase. Option A is incorrect.

Thankfully, option B is incorrect. It would be costly to obtain an alternate data center each time the virtual machine management tools are updated.

Peer review is not required when updating virtual machine management tools. Option D is incorrect.

### Question # 57 - Access control to virtualization management tools should be _______________.           
A. Rule-based           
B. Role-based          
C. User-based          
D. Discretionary       
Answer: B. 

It is important to limit access to the virtualization toolset to those administrators, engineers, and architects who are vital for supporting the virtualized environment and nobody else.

The other options are incorrect because they do not restrict access to the virtualization management tool set as specifically as role-based access control does. If someone’s role changes and they no longer require access, then their access should be terminated.

### Question # 58 - Before deploying a specific brand of virtualization toolset, it is important to configure it according to _______________.                
A. Industry standards                       
B. Prevailing law of that jurisdiction           
C. Vendor guidance            
D. Expert opinion          
Answer: C.         

Toolset vendors will specify secure configurations of their products; these must be followed in order to fulfill due care requirements.
Standards and laws don’t usually specify builds for products or brands, so options A and B are incorrect.
Expert opinion, while useful, is not sufficient to demonstrate due care in many cases; option D is not the best response.

### Question # 59 - Which of the following is essential for getting full security value from your system baseline?          
A. Personnel training           
B. Documentation            
C. Host-based intrusion detection system (HIDS)            
D. Encryption               
Answer: B. 

In order to understand, optimize, and re-create your secure baseline, proper and full documentation is absolutely essential.

Personnel training is important for secure system use, but it is not an element of baselining. Option A is incorrect.

A secure baseline for a given system may include HIDS and/or encryption, but they are not essential elements, so options C and D are incorrect.

### Question # 60 - Which of the following is essential for getting full security value from your system baseline?           
A. Capturing and storing an image of the baseline                        
B. Keeping a copy of upcoming suggested modifications to the baseline            
C. Having the baseline vetted by an objective third party                                     
D. Using a baseline from another industry member so as not to engage in repetitious efforts            
Answer: A. 

An image of the baseline should be stored securely, preferably in more than one location (to include the archive, the disaster kit, and any alternate site, to name a few). It is essential to have a copy on hand for reconstructing the environment during contingency operations, and it is also useful for audit/review purposes.

Option B is incorrect because planned modifications are not yet part of the actual baseline.

Option C may be a good answer in some situations; however, it is not essential, and option A is still a better answer.

Option D is incorrect because every environment (and, therefore, the baseline used in that environment) should be exclusively tailored for the organization using that environment.

### Question # 61 - Patching can be viewed as a configuration modification and therefore subject to the organization’s configuration management program and methods. What may also be an aspect of patching in terms of configuration management?                 
A. Patching doesn’t need to be performed as a distinct effort; patching can go through the normal change request process like all other modifications.                      
B. Any patches suggested or required by vendors to maintain compliance with service contracts must be made immediately, regardless of internal process restrictions.                     
C. Any patches suggested by third parties should not be considered as they may invalidate service contracts or warranties and negatively affect the organization’s security posture.           
D. The configuration or change management committee or board may grant blanket approval for patches (at a certain impact level) without the need to go through the formal change process.         
Answer: D. 

In order to ensure timely application of patches, patching may receive blanket approval and only be reviewed by the committee or board after the fact for final approval.

Requiring normalized processing for patching may delay patching and expose the organization to undue risk; option A is thus incorrect.

Patching still needs to involve testing and confirmation to avoid interoperability and additional security problems, making option B incorrect.

Third parties can identify security problems as well as vendors; external patches need to be considered as well as vendor patches. Option C is thus incorrect.

### Question # 62 - Clustering hosts allows you to do all the following except _______________.          
A. Meet high-availability demands                 
B. Optimize performance with load balancing            
C. Enhance scalability                                                 
D. Apply updates, patches, or configuration modifications instantly            
Answer: D.           

Clustering does not preclude the time and diligence necessary to perform patching or updates.
All the other options are attributes provided by host clustering.

### Question # 63 - Which of the following is not a way to apportion resources in a pooled environment?        
A. Reservations          
B. Limits           
C. Tokens            
D. Shares      
Answer: C.      

Tokenization is a method for obscuring or protecting data using two distinct databases, not a resource allocation method.
All the other options are methods for allocating shared resources.

### Question # 64 - A loosely coupled storage cluster will have performance and capacity limitations based on the _______________.        
A. Physical backplane connecting it            
B. Total number of nodes in the cluster         
C. Amount of usage demanded                     
D. The performance and capacity in each node          
Answer: D. 

In a loosely coupled storage cluster, each node acts as an independent data store that can be added or removed from the cluster without affecting other nodes. This, however, means that the overall cluster’s performance/capacity depends on each node’s own maximum performance/capacity.

The physical backplane can be a limiting factor in a tightly coupled architecture but has less effect in a loosely coupled cluster; option A is incorrect.

Because each node in a loosely coupled cluster has its own limitations, the number of nodes will not affect overall performance. Option B is incorrect.

Option C is incorrect because “usage demanded” is not a factor in performance and capacity of a loosely coupled storage cluster.

### Question # 65 - When putting a system into maintenance mode, it’s important to do all of the following except _______________.       
A. Transfer any live virtual guests off the host          
B. Turn off logging                                    
C. Lock out the system from accepting any new guests          
D. Notify customers if there are any interruptions               
Answer: B. 

Auditing is probably even more important during maintenance mode than normal operation because administrator activity is almost always involved.

All the other options are necessary measures for maintenance mode.

### Question # 66 - Typically, a cloud customer seeking stand-alone hosting will expect all of the following except _______________.           
A. More control over governance of the environment           
B. Greater administrative control of the environment          
C. Higher overall security of the environment             
D. Lower costs for the environment             
Answer: D.         

Almost invariably, stand-alone hosting will cost more than pooled resources and multitenancy.

All the other options are characteristics of stand-alone hosting.

### Question # 67 - Methods for achieving “high availability” cloud environments include all of the following except _______________.              
A. Extreme redundancy                             
B. Multiple system vendors for the same services                                                                                   
C. Explicitly documented business continuity and disaster recovery (BC/DR) functions in the service-level agreement (SLA) or contract                 
D. Failover capability back to the customer’s on-premises environment                
Answer: D.               

In many cases, the customer will no longer have an on-premises environment after a cloud migration.
All the other options are methods cloud providers use to achieve “high availability” environments.

### Question # 68 - You are in charge of a cloud migration for your organization. You anticipate attack traffic from various sources, each using a variety of both automated and manual intrusion techniques. In order to deter novel attacks used only against your organization, you would be wise to employ firewalls that use _______________ to detect threats.                  
A. Attack signatures                      
B. Behavioral outliers                
C. Content filters                
D. Biometric templates                 
Answer: B.          

Behavioral detection looks for activity beyond the norm of the organization’s usual traffic. Unique attacks would most likely fall into this category.

Unique attacks would not be detected by signature matching because no signatures exist for unique attacks; option A is incorrect.

Content filtering is less a means of detection and more a means of controlling traffic that users/systems are exposed to; while it may be useful for mitigating the possibility of malware infection, it’s 

less suited to the purpose posed in the question. Option C is incorrect.

Firewalls don’t work with biometrics; option D is a distractor.

### Question # 69 - Firewalls can be included in all the following aspects of a cloud environment except _______________.                
A. The guest OS                              
B. The cloud data center IT architecture               
C. Bandwidth providers used to connect to the cloud              
D. Applications used to manipulate data in the cloud                
Answer: C.       

Internet service providers don’t usually offer firewall services.
All the other options are locations/ways to implement firewalls.

### Question # 70 - A honeypot can be used for all the following purposes except _______________.                 
A. Gathering threat intelligence              
B. Luring attackers                   
C. Distracting attackers                    
D. Delaying attackers                 
Answer: B.                 

It is very important to distinguish the purpose of the honeypot. It is not for luring in attackers; a lure is an invitation, and inviting an attack decreases the organization’s ability to have the attacker prosecuted or conduct successful litigation against the attacker.
All the other options are purposes of a honeypot.

### Question # 71 - Which of the following should honeypots contain?                  
A. Inward-facing connections                
B. Network schematics                    
C. Production data                     
D. Detection systems                     
Answer: D. 

The honeypot is used to gather information about the attacker, the attacker’s tools, and the attacker’s techniques.
The honeypot should not contain anything of value; all the other options are incorrect.

### Question # 72 - Because all cloud access is remote access, contact between users and the environment should include all of the following except _______________.                  
A. Encryption                               
B. Secure login with complex passwords                    
C. Once in-all in                
D. Logging and audits                    
Answer: C.             

It’s preferable to have compartmentalized zones of trust within the production environment and not allow total access with one set of credentials.
All the other options are aspects that should be used in cloud access.

### Question # 73 - Most attacks that overcome encryption protections exploit _______________.                 
A. Mathematical principles                
B. Misconfigurations                 
C. Supercomputers                   
D. Statistical probabilities                 
Answer: B.                

Historically, when encryption had been used as a security mechanism, it was not defeated by attacking the encryption directly but rather by subverting the encryption implementation.
All the other options are actual methods for breaking encryption but are not the best answer for this question.

### Question # 74 - Administrators and engineers who work for cloud service providers will have a significant amount of control over multiple customer environments and therefore pose a severe risk. Which of the following is not a technique used to mitigate this level of increased risk from privileged users in the cloud data center?              
A. Two-person control             
B. Enhanced logging of administrative activity                    
 C. Granting privileged access only on a temporary basis             
D. Assigning permanent administrators to select customer accounts             
Answer: D.                   

Cloud vendors do not typically assign individual administrators permanently to specific accounts. All the other options (A–C) are methods used to reduce risks associated with privileged accounts.

### Question # 75 - Which of these is a vital action to determine whether the business continuity and disaster recovery (BC/DR) effort has a chance of being successful?                
A. Perform an integrity check on archived data to ensure that the backup process is not corrupting the data.              
B. Encrypt all archived data to ensure that it can’t be exposed while at rest in the long term.               
C. Periodically restore from backups.                                                          
D. Train all personnel on BC/DR actions they should take to preserve health and human safety.            
Answer: C.               

All the options are useful for enhancing the security and efficacy of the BC/DR effort, but only option C ensures that the BC/DR has a likely chance of success.

### Question # 76 - Patches do all the following except _______________.               
A. Address newly discovered vulnerabilities               
B. Solve cloud interoperability problems               
C. Add new features and capabilities to existing systems                
D. Address performance issues                
Answer: B.                     

Patches can, and often do, create interoperability problems.
All the other options are functions offered by patching.

### Question # 77 - When applying patches, it is necessary to do all of the following except _______________.                  
A. Test the patch in a sandbox that simulates the production environment                 
B. Put the patch through the formal change management process                 
C. Be prepared to roll back to the last known good build                
D. Inform users of any impact or interruptions                 
Answer: B.                 

In many cases, patches are released to deal with an imminent vulnerability/risk. Some organizations will give blanket preapproval for applying these patches and having the formal change management process approve the patch after the fact.

All the other options are activities that should take place with patching.

### Question # 78 - Which of the following is a risk associated with automated patching?           
A. Users can be leveraged by intruders.                    
B. A patch may not be applicable to a given environment.          
C. Patches can come loaded with malware, in a Trojan horse attack.              
D. Automated patching is slow and inefficient.         
Answer: B.             

Not all patches are necessary for all environments. Automated patching won’t always account for variations in organizations and could cause interoperability problems in some.

Users don’t usually apply patches and aren’t involved in automatic patching; option A is incorrect.

It is rare that an automated patch tool will be exploited to install malware; option C is incorrect.

Automated patching is faster and more efficient than manual patching; option D is incorrect.

### Question # 79 - Which of the following is a risk associated with automated patching, especially in the cloud?                    
A. Snapshot/saved virtual machine (VM) images won’t take a patch.                  
B. Remote access disallows patching.                         
C. Cloud service providers aren’t responsible for patching.              
D. Patches aren’t applied among all cloud data centers.              
Answer: A.                  

When a VM instance is inactive, it is saved as a snapshot image in a file; patches can’t be applied until the instance is running. Automated patching set to a certain scheduled time may miss inactive VMs.

Patches can be applied remotely or locally; option B is not true or correct.

Patching may be the responsibility of the cloud customer or provider, depending on the service model, type, and contract. Option C is incorrect.

Cloud service providers should apply patches ubiquitously throughout their service environment; option D is incorrect.

### Question # 80 - Which of the following is a risk associated with automated patching, especially in the cloud?                 
A. Patches may interfere with some tenants’ production environments.             
B. Patches don’t work with software as a service (SaaS) service models.                  
C. Patches don’t work with private cloud builds.                     
D. Vendors don’t issue patches to cloud providers.                
Answer: A.                     

Because a multitenant environment may have a variety of different configurations for various customers, a given patch might interfere with a certain number of customers due to interoperability problems.

Option B is untrue. Patches do work with SaaS models. Option B is incorrect.

Option C is untrue. Patches do work with private cloud builds. Option C is incorrect.

On the contrary, vendors do issue patches to cloud providers. Option D is incorrect.

### Question # 81 - Which of the following is a risk associated with manual patching, especially in the cloud?                 
A. It can happen too quickly.                                                        
B. Vendors release patches that work only with their proprietary automated tools.                       
C. It’s not scalable.                                                    
D. Users can be tricked into installing malware that looks like a patch.                       
Answer: C.                          

Manual patching requires a significant degree of effort and time and is simply not feasible in a large enterprise, much less in the vast environment of the cloud.

Manual patching is slower than automated patching. Option A is incorrect.

Option B is incorrect; this is true in both traditional and cloud environments.

Option D is incorrect; users should not be performing patching.

### Question # 82 - Which of the following is a risk associated with manual patching especially in the cloud?                    
A. No notice before the impact is realized                  
B. There is a lack of applicability to the environment.                              
C. Patches may or may not address the vulnerability they were designed to fix.                
D. The possibility for human error exists.                    
Answer: D.                    

Patching is a mundane, repetitive process, and people have trouble focusing on such tasks, especially for the number of times necessary to patch a cloud environment. Automation can aid in addressing this aspect of patching.

With human involvement in patching, there is an opportunity to be aware of imminent patch impacts and to determine applicability of the patch before it is applied; options A and B are incorrect.
Option C is a risk involved with all patching and not limited to manual patching; option D is preferable as it is specific to the question.

### Question # 83 - You are the security manager for an organization that uses the cloud for its production environment. According to your contract with the cloud provider, your organization is responsible for patching. A new patch is issued by one of your vendors. You decide not to apply it immediately for fear of interoperability problems. What additional risk are you accepting?                    
A. The cloud provider will suspend your access for violating its terms of service.                 
B. The cloud provider may sue your organization for breach of contract.                     
C. Your organization is subject to the vulnerability the patch addresses.                              
D. Your end clients will no longer trust your organization, and this will hurt your revenue flow.                   
Answer: C.                          

It is perfectly reasonable to not want to use the first version of a patch as there may be interoperability problems or even additional vulnerabilities contingent with its implementation. However, for as long as your environment remains unpatched, you are subject to attack through that new vulnerability.

All the other options are untrue.

The cloud provider will not suspend your access or sue your organization if you delay patching because of concerns about interoperability afterwards. Options A and B are incorrect.
Option D is incorrect. The opposite may actually be true. Your end clients may appreciate that you delay or test the patch before installing it on production systems.

### Question # 84 - You are the security manager for an organization that uses the cloud for its production environment. According to your contract with the cloud provider, your organization is responsible for patching. A new patch is issued by one of your vendors. You decide not to apply it immediately for fear of interoperability problems. Who may impose penalties on your organization for this decision if the vulnerability is exploited?                
A. The cloud provider            
B. Regulators               
C. Your end clients                        
D. Your Internet service provider (ISP)            
Answer: B.                     

If your organization doesn’t apply a patch for a known vulnerability, regulators may claim the organization was not performing adequate due diligence and penalize it accordingly.

None of the other entities listed in the other options can assess penalties, so they are incorrect. (End clients may try to recover damages realized from an attack through a known vulnerability, but those penalties will be imposed by a court if the end clients conduct successful litigation.)

### Question # 85 - Which of the following aspects of a cloud environment is most likely to add risk to the patch management process?                  
A. Variations in user training and familiarity with the cloud                                                    
B. A cloud services contract that specifies which parties are responsible for which aspects of patching                  
C. VMs located physically in one location but operating in different time zones                 
D. The prevalence of attacker activity at the time the patch is applied                                          
Answer: C. 

If patches are rolled out across an environment where users are operating virtual machines (VMs) at different times, there is a possibility that VMs will not be patched uniformly, which could lead to data disruption.

Option A is incorrect. Users should not be performing patching.

Option B is incorrect; a contract specifying who is responsible for specific patching activities actually reduces risk by enhancing the probability of proper patch application.

Option D is incorrect; attacker activity should be irrelevant to the patch process.

### Question # 86 - Which type of web application monitoring most closely measures actual activity?                    
A. Synthetic performance monitoring                
B. Real-user monitoring (RUM)                         
C. Security information and event management (SIEM)              
D. Database application monitor (DAM)                   
Answer: B.                               

RUM harvests information from actual user activity, making it the most realistic depiction of user behavior.

Synthetic monitoring approximates user activity but is not as exact as RUM; option A is incorrect.

SIEM monitors more than web applications, so option C is not ideal for this question.

DAM is an OSI Layer 7 tool for monitoring database activity, specifically, so it is not the ideal answer for this question.

### Question # 87 - When using real-user monitoring (RUM) for web application activity analysis, which of the following do you need to take into account?                  
A. False positives                       
B. Attacker baseline actions                    
C. Privacy concerns                          
D. Sandboxed environments                            
Answer: C.                          

Depending on the jurisdiction, RUM may entail unlawful surveillance, so the practitioner must take this into account and plan accordingly.

Option A is incorrect. False positives are typical for real-user monitoring systems.

Option B has no relevance in this context. Option B is incorrect.

Sandboxed environments are not a concern when using real-user monitoring for web application activity analysis. Option D is incorrect.

### Question # 88 - Synthetic performance monitoring may be preferable to real-user monitoring (RUM) because _______________.                     
A. It costs less                                         
B. It is a more accurate depiction of user behavior                      
C. It is more comprehensive                          
D. It can take place in the cloud                         
Answer: C.                           

Synthetic agents can simulate user activity in a much faster, broader manner and perform these actions 24/7 without rest.
All the other options are incorrect; synthetic agents may cost more than RUM, are less accurate than actual user activity, and both can take place on the cloud.

### Question # 89 - You are the security manager for an organization with a cloud-based production environment. You are tasked with setting up the event monitoring and logging systems. In your jurisdiction, private entities are allowed to monitor all activity involving their systems, without exception. Which of the following best describes a logging scheme you would recommend?                      
A. Logging every event, at all levels of granularity, including continual screen shots, keystroke logging, and browser history                            
B. Sufficient logging to reconstruct a narrative of events at some later date                       
C. Logging only data related to incidents after they have occurred                             
D. Logging specific data sets recommended by industry standards and guidelines                              
Answer: B. 

Logging should suffice for the purpose of reconstructing the pertinent information (who, what, where, when, etc.) necessary to form a narrative of what transpired. This will be different for every organization and environment (so option D is incorrect). You will have to make this determination for your organization.

Logging everything would result in log storage that exceeds the amount of data in the production environment and would actually make it more difficult to locate pertinent information. Option A is incorrect.

Option C is incorrect. Logging data after the fact is impossible.

### Question # 90 - Who should be performing log review?                                                         
A. Only certified, trained log review professionals with a great deal of experience with the logging tool                      
B. The internal audit body                     
C. External audit providers                                              
D. Someone with knowledge of the operation and a security background                       
Answer: D. 

It is important for the log review to be performed by someone who understands the normal operations of the organization so that they can discern between regular activity and anomalous behavior. This person also needs a security background so they can recognize common attack patterns/activity.

Option A sounds great, but the better answer is option D. A person with knowledge of the operation is a better fit than someone who is trained to review logs.

Options B and C are incorrect. Auditors are not the ones who should be reviewing logs for an organization.

### Question # 91 - Which of these subsystems is probably most important for acquiring useful log information?             
A. Fan             
B. RAM                
C. Clock                             
D. Uninterruptible power supply (UPS)                          
Answer: C.                           

The clock needs to be synched throughout the environment so that all activity can be contextualized and mapped and a true narrative of events can be reconstructed later.
All the other options are incorrect because they are simply IT terms. When it comes to useful logs, having the correct time relevant to all logged activity is vital.

### Question # 92 - A SIEM (security information and event management) system does not eliminate the need for human participation in _______________.                  
A. Log collection              
B. Responding to alerts                        
C. Mathematical normalization of different logs                         
D. Detecting and alerts                   
Answer: B.              

Response to anomalous activity detected by the SIEM tool will still require human involvement.

All the other options are functions that the SIEM system can perform on its own as automated tasks.

### Question # 93 - Log data should be protected _______________.                          
A. One level below the sensitivity level of the systems from which it was collected             
B. At least at the same sensitivity level as the systems from which it was collected              
C. With encryption in transit, at rest, and in use                                 
D. According to National Institute of Standards and Technology (NIST) guidelines                 
Answer: B.                     

Because the logs are essential to reconstructing a record of what occurred within the environment, they are a valuable target for attackers. They therefore need a sufficient level of protection commensurate with the data/systems they are about.

We don’t want to have less protection on the logs than on the systems they monitor; the controls on those systems were chosen according to what threats and risks they may be exposed to—the level of security provided by those controls are, at a minimum, required for the log data. Option A is incorrect.

Encryption may or may not be used for securing log data, depending on the level of sensitivity of the systems/data they are protecting; option C is too specific and thus incorrect.
NIST guidelines are not suitable for all organizations and uses; option D is too broad and incorrect.

### Question # 94 - Risk is usually viewed with consideration for all the following elements except _______________.                 
A. Impact that could occur if a given circumstance is realized                       
B. The likelihood or probability a circumstance will occur                  
C. In the context of specific threats to an organization                                  
D. According to risks recently realized by other organizations in the same industry                        
Answer: D.                      

While historical information, especially that specific to the organization’s industry, can be useful in assessing threats, risk must be considered independently from other occurrences; whether something has occurred elsewhere does not necessarily directly affect the likelihood it will or will not occur for a certain target.

All the other options are elements typically considered in the risk context.

### Question # 95 - Risk management entails evaluating all of the following except _______________.                    
A. Threats                 
B. Vulnerabilities                          
C. Countermeasures                                   
D. Customers                               
Answer: D.                                 

We usually do not evaluate our customer base as an aspect of risk management. All the other options are aspects of common risk management practices.

### Question # 96 - Impact resulting from risk being realized is often measured in terms of _______________.                 
A. Amount of data lost                        
B. Money                            
C. Amount of property lost                   
D. Number of people affected                        
Answer: B. 

While all the options are somewhat true, because all of that information can be used to provide the most comprehensive risk picture, the best answer among those listed is money; it is a discrete, numeric metric that can be used both for comparison to countermeasure/control cost and for recompense efforts (insurance claims, lawsuits, etc.).

### Question # 97 - You are the security officer for a small nonprofit organization. You are tasked with performing a risk assessment for your organization; you have one month to complete it. The IT personnel you work with have been with the organization for many years and have built the systems and infrastructure from the ground up. They have little training and experience in the field of risk. Which type of risk assessment would you choose to conduct?                     
A. Quantitative                      
B. Qualitative                            
C. Pro forma                            
D. Informal                                 
Answer: B.                            

Qualitative risk assessments are preferable in situations where the organization has personnel who understand the IT environment but may not have a lot of experience with risk functions and where the organization does not have a great deal of time or money to spend on the project.

A quantitative risk assessment requires a significant budget of time and money as well as well-trained, experience personnel familiar with risk; option A is not correct.
Options C and D 
E. are incorrect; these are not types of risk assessments.

### Question # 98 - Which of the following is most useful in determining the single loss expectancy (SLE) of an asset?                    
A. The frequency with which you expect that type of loss to occur                      
B. The dollar value of the asset                          
C. The sensitivity of the asset                           
D. The size and scope of the asset                               
Answer: B.                            

The monetary value of the asset is the most objective, discrete metric possible and the most accurate for the purposes of SLE determination.
The other options are factors that may bear on how you determine the dollar value of the asset but are not as useful as option B.

### Question # 99 - Which of the following will likely best help you predict the annualized rate of occurrence (ARO) of a specific loss?                 
A. Threat intelligence data                
B. Historical data                
C. Vulnerability scans                    
D. Aggregation analysis                      
Answer: B.                       

While previous activity is not a great predictor of future outcomes (especially in the field of IT security), it is the best source we have.

Threat intelligence information is useful but not as good as historical data in predicting ARO; option A is not as good as option B.

Vulnerability scans and aggregation do not really aid in predicting rate of occurrence at all; options C and D are incorrect.

### Question # 100 - Which of the following has the most effect on exposure factor (EF)?                  
A. The type of threat vector                 
B. The source location of the attack                         
C. The target of the attack                              
D. The jurisdiction where the attack takes place                                
Answer: A.                          

The threat vector is the multiplier involved in determining exposure factor; of the options listed, this is the best answer (and, other than C, the only one that actually has bearing on EF).

### Question # 101 - You are a consultant, performing an external security review on a large manufacturing firm. You determine that its newest assembly plant, which cost $24 million, could be completely destroyed by a fire but that a fire suppression system could effectively protect the plant. The fire suppression system costs $15 million. An insurance policy that would cover the full replacement cost of the plant costs $1 million per month. What is the annual rate of occurrence (ARO) in this scenario?                    
A. 12                
B. $24 million                   
C. 1                   
D. $10 million                 
Answer: C.                     

Absent any other information about a total physical loss, we can consider the rate of occurrence as 1: We would not expect the plant to burn down more than once in a year. In fact, we would expect that unless the plant was involved in some particularly flammable activity, the ARO would be less than 1 (that is, a fire is not expected every year) due to controls involved in the planning and building process of the plant (location of flammable material, fire-resistant construction techniques, etc.).

Options B and D are incorrect. The ARO is a number, not a dollar amount.

It is unlikely that the plant would burn down 12 times a year or every month. Option A is incorrect.

### Question # 102 - You are a consultant performing an external security review on a large manufacturing firm. You determine that its newest assembly plant, which cost $24 million, could be completely destroyed by a fire but that a fire suppression system could effectively protect the plant. The fire suppression system costs $15 million. An insurance policy that would cover the full replacement cost of the plant costs $1 million per month. What would you recommend?                  
A. Accept the risk of fire, and save money by not spending anything on controls/countermeasures.                       
B. Get the fire suppression system.                       
C. Get the insurance policy.                            
D. It is impossible to decide from this information.                      
Answer: D.                    

What we can’t determine from the available information is the actual annualized loss expectancy (ALE); the cost of the physical plant itself is not the actual value of the asset, so it’s impossible to determine the ALE and therefore impossible to compare the ALE against the cost of possible controls and countermeasures.

All the other options are incorrect; we can’t make a suitable choice from the available information.

### Question # 103 - You are a consultant performing an external security review on a large manufacturing firm. You determine that its newest assembly plant, which cost $24 million, could be completely destroyed by a fire but that a fire suppression system could effectively protect the plant. The fire suppression system costs $15 million. An insurance policy that would cover the full replacement cost of the plant costs $1 million per month. In order to establish the true annualized loss expectancy (ALE), you would need all of the following information except _______________.                    
A. The amount of revenue generated by the plant                  
B. The rate at which the plant generates revenue                   
C. The length of time it would take to rebuild the plant                        
D. The amount of product the plant creates                 
Answer: D.                 

Unless this number is being used to determine the measures of options A or B, or we’re trying to better estimate the cost of the impact of the first occurrence (i.e., including the value of lost product in the single loss expectancy [SLE]), the amount of product the plant creates is not as important as the attendant revenue that amount generates for the company.

All the other options are factors we need to know: The amount of revenue and the pace at which it is generated by the plant and the duration of downtime for the plant in the event of fire (so as to calculate possible lost revenue) will help us arrive at the annualized loss expectancy (ALE). In fact, additional information would also be useful, such as potential loss of market share if product was not delivered for the duration of the downtime, etc.

### Question # 104 - You are a consultant performing an external security review on a large manufacturing firm. You determine that its newest assembly plant, which cost $24 million, could be completely destroyed by a fire but that a fire suppression system could effectively protect the plant. The fire suppression system costs $15 million. An insurance policy that would cover the full replacement cost of the plant costs $1 million per month. The plant generates $2 million of revenue each month. The time to rebuild the plant at the current location is six months. What should you recommend?                       
A. Accept the risk of fire, and save money by not spending anything on controls and countermeasures.                       
B. Get the fire suppression system.                       
C. Get the insurance policy.                                 
D. It is impossible to decide from this information.                     
Answer: B.                         

The fire suppression system is the most cost-effective, reasonable means of dealing with the risk, if we use the formula for determining annualized loss expectancy (ALE).
First, we need to determine the single loss expectancy (SLE) and annualized rate of occurrence (ARO). ARO can be assumed to be 1; absent any other information about the plant, we don’t expect more than one fire per year (and perhaps less, but we don’t have that information, either). The SLE is $36 million ($24 million for the cost of rebuilding the plant, assuming no increase in costs over the previous construction, plus $2 million per month of lost revenue, for the six months it will take to rebuild).
Therefore, the ALE is $36 million (36 [SLE] × 1 [ARO]).

Either the fire suppression system or the insurance policy would be appealing, from a strictly financial standpoint, if we only compared the ALE to the annualized cost of the countermeasure ($15 million for the suppression system, $12 million for the insurance policy).

However, other factors have a bearing on this consideration too. For instance, fire poses a threat to health and human safety; obviating such risks should be a paramount concern to senior management. An insurance policy doesn’t truly protect people, it only offsets the damages people experience through loss. Also, the insurance policy would be a recurring, continual cost; it costs less than the fire suppression system in the first year of the plant’s operation ($12 million for insurance versus $15 million for the system), but once the system is purchased, though it may need upkeep and maintenance, we can assume it won’t cost the same amount in future years, and it probably won’t cost anywhere near as much as the continual costs of the insurance.
All the other options are not as good as B.

### Question # 105 - Risk mitiga tion must always also entail which other method of addressing risk?                      
A. Risk acceptance                   
B. Risk avoidance                               
C. Risk transfer                                   
D. Risk attenuation                                            
Answer: A. 

Because risk can never be mitigated to zero (there is no such thing as “no risk” or “perfect security”), there will always be some residual risk after risk mitigation; this residual risk must be accepted.
Risk mitigation does not always involve risk transfer, or risk avoidance. “Risk attenuation” is not an industry-standard term associated with risk management Options B, C, and D are incorrect.

### Question # 106 - Which of the following poses a secondary risk?                       
A. Fire exit signs                        
B. Oxygen-displacing fire suppression                             
C. Automated fire detection systems                    
D. Fail-safe fire egress paths                     
Answer: B.                             

Secondary risk is any risk resulting from enacting a control/countermeasure to the original risk. In this case, a fire suppression system that displaces oxygen is a means to mitigate the original risk (fire) but adds a new risk (suffocating people).
All the other options are not causes of secondary risk (except if we draw out unreasonable conclusions from the most extreme, ridiculous cases, for example, “the secondary risk is the risk that the control doesn’t work”).

### Question # 107 - Which of the following is not true about risk mitigation?                          
A. A given control/countermeasure should never cost more than the impact of the risk it mitigates.             
B. Risk cannot be reduced to zero.                                    
C. The end state of risk mitigation is risk at a tolerable level.                  
D. Risk mitigation is always the best means to address risk.                    
Answer: D. 

The best means to address risk is completely dependent on the business needs of the specific entity and process. Mitigation may or may not be the optimum choice.
All the other options are true statements about risk mitigation.

### Question # 108 - Which of the following is not true about risk mitigation?                        
A. The cost of the control/countermeasure per year is simple: the overall cost (of acquisition, implementation, and maintenance) divided by life span, in years.                    
B. Ignoring risk is not risk mitigation; ignoring risk is risk acceptance.                                                        
C. The cost of mitigation can be compared against the cost of a control/countermeasure to determine the optimum course of action.                       
D. Risk is fluid, so all risk assessments are pointless.                              
Answer: D.                     

A risk assessment may, indeed, be an estimate of a moving target, but it is invaluable in terms of measuring risk at any given point in time.

### Question # 109 - Which comes first?                   
A. Accreditation                     
B. Operation                         
C. Maintenance                             
D. Certification                            
Answer: D.                               

In the certification/accreditation model of system approval, certification is the fundamental step.
All other options are incorrect because certification comes first in the certification/accreditation model of system approval.

### Question # 110 - The National Institute of Standards and Technology (NIST) Risk Management Framework (RMF) is required for federal agencies in the United States. Which of the following is not a characteristic of the RMF?                     
A. Automation of controls wherever possible                             
B. Focuses on continual improvement and near real-time risk management                  
C. Is based on cost metrics and perceived threats                                          
D. Links risk management at the process level to risk management at the managerial level                           
Answer: C. 

The RMF is based on perceived risk as opposed to threats (threats may factor into risk assessment but are not the driver for the RMF).
All the other options are true regarding the RMF.

### Question # 111 - Symmetric encryption involves _______________.                    
A. Two key pairs, mathematically related                
B. Unknown parties, sharing information                     
C. Signed certificates                         
D. A shared secret                           
Answer: D.                                

In symmetric encryption, a single key is used to both encrypt and decrypt a message. This is often referred to as a shared secret.
Two key pairs are not used in symmetric encryption; option A is incorrect.
Parties most often must be known to each other using symmetric encryption; option B is incorrect.
Certificates require public-private key pairs, which is not an element of symmetric encryption; option C is incorrect.

### Question # 112 - Symmetric encryption involves _______________.                     
A. The Diffie-Hellman key exchange                      
B. Passing keys out of band                            
C. Mathematically related key pairs                                  
D. A one-way mathematical algorithm for validating messages                             
Answer: B. 

In symmetric encryption, the key must usually be passed through a different medium than will be used for sending and receiving the encrypted messages.

DH is usually used for asymmetric encryption, to establish a temporary symmetric key; option A is incorrect.

Option C describes asymmetric encryption and is therefore incorrect.

Option D describes hashing and is therefore incorrect.
