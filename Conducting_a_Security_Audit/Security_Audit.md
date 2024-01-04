## Controls assessment

To review control categories, types, and the purposes of each, read the control categories document.

### Current assets

Assets managed by the IT Department include: 

-	On-premises equipment for in-office business needs  
-	Employee equipment: end-user devices (desktops/laptops, smartphones), remote workstations, headsets, cables, keyboards, mice, docking stations, surveillance cameras, etc.
-	Management of systems, software, and services: accounting, telecommunication, database, security, ecommerce, and inventory management
-	Internet access
-	Internal network
-	Vendor access management
-	Data center hosting services  
-	Data retention and storage
-	Badge readers
-	Legacy system maintenance: end-of-life systems that require human monitoring 

### Administrative Controls

| Control Name | Control type and explanation | Needs to be implemented | Priority |
| ------------ | ---------------------------- | ----------------------- | -------- |
| Least Privilege | Preventative; reduces risk by making sure vendors and non-authorized staff only have access to the assets/data they need to do their jobs | Yes | High |
| Disaster recovery plans | Corrective; business continuity to ensure systems are able to run in the event of an incident/there is limited to no loss of productivity downtime/impact to system components, including: computer room environment (air conditioning, power supply, etc.); hardware (servers, employee equipment); connectivity (internal network, wireless); applications (email, electronic data); data and restoration | Yes | High |
| Password policies | Preventative; establish password strength rules to improve security/reduce likelihood of account compromise through brute force or dictionary attack techniques | Yes | High |
| Access control policies | Preventative; increase confidentiality and integrity of data | Yes | High |
| Account management policies | Preventative; reduce attack surface and limit overall impact from disgruntled/former employees | Yes | High |
| Separation of duties | Preventative; ensure no one has so much access that they can abuse the system for personal gain | Yes | High |

### Technical Controls
| Control Name | Control type and explanation | Needs to be implemented | Priority |
| ------------ | ---------------------------- | ----------------------- | -------- |
| Firewall     | Preventative; firewalls are already in place to filter unwanted/malicious traffic from entering internal network | No | N/A |
| Intrusion Detection System (IDS) | Detective; allows IT team to identify possible intrusions (e.g., anomalous traffic) quickly | Yes | High |
| Encryption | Deterrent; makes confidential information/data more secure (e.g., website payment transactions) | Yes | High |
| Backups | Corrective; supports ongoing productivity in the case of an event; aligns to the disaster recovery plan | Yes | High |
| Password management system | Corrective; password recovery, reset, lock out notifications | Yes | High |
| Antivirus software | Corrective; detect and quarantine known threats | Yes | High |
| Manual monitoring, maintenance, and intervention | Preventative/corrective; required for legacy systems to identify and mitigate potential threats, risks, and vulnerabilities | Yes | High |

### Physical Controls
| Control Name | Control type and explanation | Needs to be implemented | Priority |
| ------------ | ---------------------------- | ----------------------- | -------- |
| Time-controlled safe | Deterrent; reduce attack surface/impact of physical threats | Yes | Medium/Low |
| Adequate lighting | Deterrent; limit “hiding” places to deter threats | Yes | Medium/Low |
| Closed-circuit television (CCTV) surveillance | Preventative/detective; can reduce risk of certain events; can be used after event for investigation | Yes | High/Medium |
| Locking cabinets (for network gear) | Preventative; increase integrity by preventing unauthorized personnel/individuals from physically accessing/modifying network infrastructure gear | Yes | High/Medium |
| Signage indicating alarm service provider | Deterrent; makes the likelihood of a successful attack seem low | Yes | Low |
| Locks | Preventative; physical and digital assets are more secure | Yes | High |
| Fire detection and prevention (fire alarm, sprinkler system, etc.) | Detective/Preventative; detect fire in the toy store’s physical location to prevent damage to inventory, servers, etc. | Yes | Medium |


## Compliance checklist exemplar

### The Federal Energy Regulatory Commission - North American Electric Reliability Corporation (FERC-NERC)

The FERC-NERC regulation applies to organizations that work with electricity or that are involved with the U.S. and North American power grid. Organizations have an obligation to prepare for, mitigate, and report any potential security incident that can negatively affect the power grid. Organizations are legally required to adhere to the Critical Infrastructure Protection Reliability Standards (CIP) defined by the FERC. 

**Explanation**: N/A

### General Data Protection Regulation (GDPR)

GDPR is a European Union (E.U.) general data regulation that protects the processing of E.U. citizens’ data and their right to privacy in and out of E.U. territory. Additionally, if a breach occurs and a E.U. citizen’s data is compromised, they must be informed within 72 hours of the incident.

**Explanation**: Botium Toys needs to adhere to GDPR because they conduct business and collect personal information from people worldwide, including the E.U.

### Payment Card Industry Data Security Standard (PCI DSS)

PCI DSS is an international security standard meant to ensure that organizations storing, accepting, processing, and transmitting credit card information do so in a secure environment. 

**Explanation**: Botium Toys needs to adhere to PCI DSS because they store, accept, process, and transmit credit card information in person and online.
	
### The Health Insurance Portability and Accountability Act (HIPAA)

HIPAA is a federal law established in 1996 to protect U.S. patients' health information. This law prohibits patient information from being shared without their consent. Organizations have a legal obligation to inform patients of a breach. 

**Explanation**: N/A
	
### System and Organizations Controls (SOC type 1, SOC type 2)

The SOC1 and SOC2 are a series of reports that focus on an organization's user access policies at different organizational levels. They are used to assess an organization’s financial compliance and levels of risk. They also cover confidentiality, privacy, integrity, availability, security, and overall data safety. Control failures in these areas can lead to fraud.

**Explanation**: Botium Toys needs to establish and enforce appropriate user access for internal and external (third-party vendor) personnel to mitigate risk and ensure data safety.
