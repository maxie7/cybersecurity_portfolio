# Incident handler's journal

| Date: April 01, 2024 | Entry #01 |
| -------------------- | --------- |
| Description          | Documenting a cybersecurity incident <br><br> This incident occurred in the two phases: <ol><li>**Detection and Analysis:** The scenario outlines how the organization first detected the ransomware incident. For the analysis step, the organization contacted several organizations for technical assistance</li> <li>**Containment, Eradication, and Recovery:** The scenario details some steps that the organization took to contain the incident. For example, the company shut down their computer systems. However, since they could not work to eradicate and recover from the incident alone, they contacted several other organizations for assistance.</li></ol> |
| Tool(s) used | None |
| The 5 W's | <ul><li>**Who:** An organized group of unethical hackers</li><li>**What:** A ransomware security incident</li><li>**Where:** At a health care company</li><li>**When:** Tuesday 9:00 a.m.</li><li>**Why:** The incident happened because unethical hackers were able to access the company's systems using a phishing attack. After gaining access, the attackers launched their ransomware on the company's systems, encrypting critical files. The attackers' motivation appears to be financial because the ransom note they left demanded a large sum of money in exchange for the decryption key.</li></ul> |
| Additional notes | <ol><li>How could the health care company prevent an incident like this from occurring again?</li><li>Should the company pay the ransom to retrieve the decryption key?</li></ol> |

| Date: April 02, 2024 | Entry #02 |
| -------------------- | --------- |
| Description          | Analyzing a packet capture file |
| Tool(s) used | For this activity, I used Wireshark to analyze a packet capture file. Wireshark is a network protocol analyzer that uses a graphical user interface. The value of Wireshark in cybersecurity is that it allows security analysts to capture and analyze network traffic. This can help in detecting and investigating malicious activity. |
| The 5 W's | <ul><li>**Who:** N/A</li><li>**What:** N/A</li><li>**Where:** N/A</li><li>**When:** N/A</li><li>**Why:** N/A</li></ul> |
| Additional notes | I've never used Wireshark before, so I was excited to begin this exercise and analyze a packet capture file. At first glance, the interface was very overwhelming. I can see why it's such a powerful tool for understanding network traffic. |

| Date: April 02, 2024 | Entry #03 |
| -------------------- | --------- |
| Description          | Capturing the first packet |
| Tool(s) used | For this activity, I used tcpdump to capture and analyze network traffic. Tcpdump is a network protocol analyzer that's accessed using the command-line interface. Similar to Wireshark, the value of tcpdump in cybersecurity is that it allows security analysts to capture, filter, and analyze network traffic. |
| The 5 W's | <ul><li>**Who:** N/A</li><li>**What:** N/A</li><li>**Where:** N/A</li><li>**When:** N/A</li><li>**Why:** N/A</li></ul> |
| Additional notes | After carefully following the instructions and redoing some steps, I was able to get through this activity and capture network traffic. |

| Date: April 02, 2024 | Entry #04 |
| -------------------- | --------- |
| Description          | Investigate a suspicious file hash |
| Tool(s) used | For this activity, I used VirusTotal, which is an investigative tool that analyzes files and URLs for malicious content such as viruses, worms, trojans, and more.  It's a very helpful tool to use if you want to quickly check if an indicator of compromise like a website or file has been reported as malicious by others in the cybersecurity community. For this activity, I used VirusTotal to analyze a file hash, which was reported as malicious. <br><br>This incident occurred in the **Detection and Analysis** phase. The scenario put me in the place of a security analyst at a SOC investigating a suspicious file hash. After the suspicious file was detected by the security systems in place, I had to perform deeper analysis and investigation to determine if the alert signified a real threat. |
| The 5 W's | <ul><li>**Who:** An unknown malicious actor</li><li>**What:** An email sent to an employee contained a malicious file attachment with the SHA-256 file hash of 54e6ea47eb04634d3e87fd7787e2136ccfbcc80ade34f246a12cf93bab527f6b</li><li>**Where:** An employee's computer at a financial services company</li><li>**When:** At 1:20 p.m., an alert was sent to the organization's SOC after the intrusion detection system detected the file</li><li>**Why:** An employee was able to download and execute a malicious file attachment via e-mail.</li></ul> |
| Additional notes | How can this incident be prevented in the future? Should we consider improving security awareness training so that employees are careful with what they click on? |

