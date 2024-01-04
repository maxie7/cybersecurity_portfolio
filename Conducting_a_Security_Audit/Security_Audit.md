# Controls assessment

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


# Compliance checklist exemplar

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


# Stakeholder memorandum

Complete each section of the stakeholder memorandum template to communicate your audit results and recommendations to stakeholders:
-	Scope
-	Goals
-	Critical findings (must be addressed immediately)
-	Findings (should be addressed, but no immediate need)
-	Summary/Recommendations

Use information from the following documents:
-	Botium Toys: Audit scope and goals
-	Controls assessment (completed in “Conduct a security audit, part 1”)
-	Compliance checklist (completed in “Conduct a security audit, part 1”)

## Memorandum

**TO**: IT Manager, Stakeholders

**FROM**: Maksym Kosenko

**DATE**: January 4, 2024

**SUBJECT**: Internal IT Audit Findings and Recommendations

Dear Colleagues,

I hope this memo finds you well. I would like to bring to your attention the results of the recent internal audit conducted on Botium Toys' IT assets and management systems. The audit aimed to evaluate the current state of our IT infrastructure and identify areas that require attention and improvement.

**Scope**:

The audit encompassed a comprehensive assessment of the company's IT assets and services, including but not limited to:

-	On-premises equipment catering to in-office business requirements.
-	Employee equipment, consisting of end-user devices such as desktops, laptops, smartphones, along with accessories like headsets, cables, keyboards, mice, and docking stations.
-	Management of various systems, software, and services encompassing accounting, telecommunication, database, security, ecommerce, and inventory management.
-	Oversight of internet access and the internal network.
-	Vendor access management to ensure secure collaborations.
-	Data center hosting services for critical applications and services.
-	Data retention and storage solutions to manage information effectively.
-	Badge readers for access control.
-	Maintenance of legacy systems that are nearing end-of-life and necessitate human supervision.

**Goals**:

The primary objectives of the audit were to assess the efficiency, security, and reliability of our IT assets and services. By doing so, we aimed to identify vulnerabilities, streamline operations, and enhance overall system performance.

**Critical Findings** (Must be addressed immediately):

During the audit, we identified several critical findings that demand immediate attention to ensure the security and stability of our IT environment:

1.	Security Vulnerabilities in Legacy Systems: Our end-of-life legacy systems have shown significant security vulnerabilities that expose our network to potential breaches. Immediate action is required to secure these systems or plan for their replacement.

2.	Access Control Weaknesses: Inconsistent badge reader implementation and vendor access management could lead to unauthorized access. It is crucial to strengthen access controls to safeguard sensitive areas and data.

**Findings** (Should be addressed, but no immediate need):

While the following findings do not pose an immediate threat, addressing them will contribute to overall operational improvement:

1.	Software Update Management: Some systems and software require more regular updates to ensure optimal performance and security. A more structured approach to update management is recommended.

2.	End-User Equipment Monitoring: Monitoring and managing end-user devices more proactively can prolong their lifespan and prevent unexpected downtime.

### Summary/Recommendations:

In summary, this audit has provided valuable insights into the state of our IT assets and management systems. To address the critical findings, I recommend the following actions:

1.	Legacy System Mitigation: Engage a team to assess and apply security patches to the end-of-life legacy systems or expedite plans for their replacement.

2.	Access Control Enhancement: Review and enhance our badge reader implementation and vendor access management protocols to prevent unauthorized entry.

3.	Update Management Protocol: Develop a comprehensive software update management protocol to ensure all systems and software are regularly updated to minimize security risks.

4.	End-User Device Management: Implement a proactive device monitoring strategy to extend the lifespan of end-user equipment and reduce unexpected disruptions.

Your commitment to addressing these issues promptly will reinforce the security and efficiency of our IT operations. Kindly review these recommendations and collaborate with the relevant teams to implement the necessary actions.
