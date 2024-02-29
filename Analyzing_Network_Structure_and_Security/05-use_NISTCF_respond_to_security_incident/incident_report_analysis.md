## Incident report analysis

### Applying the NIST framework

| Summary  | <div align="left">An ongoing investigation suggests a likely cyberattack vector after an intern received an authentic-looking phishing email this morning. The message directed her to an external site that prompted entry of internal network credentials, later revealed to be a decoy harvesting login information. Shortly thereafter, the intern found her own account suddenly disabled due to anomalous activity logs showing unauthorized customer database access. Further inquiry uncovered other suspicious account behavior as well as customer records either deleted entirely or modified with falsified data. While attack scope remains under review, these initial findings point to a coordinated attempt by malicious actor(s) to steal network access to view sensitive customer information and sow data disruption. The phishing-enabled intrusion demonstrates need for better systemic protections against credential theft alongside more widespread security awareness training to recognize social engineering risks. Appropriate external authorities have been alerted about the active breach as internal teams work urgently to determine damage, restore compromised data, and prevent future vulnerability by shoring up related policy and software defenses company-wide.</div> |
|----------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Identify | An internal investigation revealed that a recent security breach resulted from compromised login credentials belonging to an intern. It appears an attacker obtained the intern's username and password and used them to illegally access and delete customer data from our database. The incident management team is currently reviewing systems, devices, and access policies to fully assess the damage and determine precisely how the attacker gained entry in order to prevent future intrusions. Though the investigation remains ongoing, the initial audit found gaps in security around intern access permissions and password protocols which likely enabled the incident.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               | 
| Protect  | In response to the recent data breach, several new security measures are being enacted to bolster defenses against potential attacks. Employees will be required to use multi-factor authentication when logging into systems, allowing only three login attempts before accounts are locked, and will receive mandatory training on safeguarding login credentials. On the technology side, upgrades are underway to install an intrusion prevention system that can detect malicious network activity in real-time. Additionally, the team is reconfiguring firewall settings across the company's infrastructure to further limit external access to sensitive systems and data. Together, these changes signify a comprehensive commitment to securing vulnerabilities that permitted unlawful data access and theft during the previous incident. Regular audits will ensure these expanded authentication protocols, cybersecurity systems, and access policies provide ongoing protection.                                                                                                                                                                                                                                                                                                                   |
| Detect   | To bolster monitoring capabilities against potential cyber threats, new detection systems are being implemented for company networks. Firewall logs will be sent to a central security tool to analyze traffic patterns and identify abnormal or malicious activity attempting to penetrate systems. Additionally, an intrusion detection system (IDS) will run intrusion and anomaly detection checks in real-time across the entire network infrastructure to spot policy violations and known attack signatures. With layered insight into inbound connections from the internet, the security team aims to swiftly identify any unauthorized access attempts and respond appropriately to prevent incidents like the recent data breach. Ongoing tuning and threat intelligence updates will ensure these systems remain effective as the modern attack landscape evolves.                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Respond  | In the immediate aftermath, the security team disabled the compromised intern's account to prevent further access. Additionally, mandatory training has been rolled out company-wide to reinforce best practices around safeguarding login credentials and detecting social engineering attempts. Per incident response policy, upper management was briefed on the breach, including specifics on the type of customer data impacted. They are now in the process of disclosing the incident to affected individuals and applicable regulatory authorities in accordance with data breach notification laws. Law enforcement has also been informed to fully support any investigations, as they attempt to identify the perpetrator behind this criminal cyber attack. Across teams, we remain committed to transparent communication and taking all necessary steps to earn back customer trust after this violation of their privacy and our responsibility to protect sensitive information.                                                                                                                                                                                                                                                                                                                   |
| Recover  | To recover the compromised data, our technical teams are working to fully restore the customer database from a daily backup taken last night at midnight. This will return the deleted information, though changes entered since the backup will be lost. Employees have been notified that any new or altered customer records from this morning onwards will have to be manually re-ingested. After the rollback is complete, staff should re-enter recent data modifications to ensure information is current while bringing the system to a last-known good state prior to unauthorized tampering. Meanwhile, work continues to identify the root cause behind the breach to prevent further attacks. We will provide updates directly to customers as progress is made to retrieve and protect accurate records through improved defenses.                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

---