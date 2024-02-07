## Cybersecurity Incident Report: Network Traffic Analysis

### Part 1: Provide a summary of the problem found in the DNS and ICMP traffic log

<ins>The UDP protocol reveals that</ins>: a DNS resolution request was sent to the DNS server, but failed to reach its destination. 

<ins>This is based on the results of the network analysis, which show that the ICMP echo reply returned the error message</ins>: “destination port unreachable”. 

<ins>The port noted in the error message is used for</ins>: DNS queries over UDP on port 53. 

<ins>The most likely issue is</ins>: a firewall rule or network setting that is blocking the UDP traffic to port 53, preventing the DNS request from reaching the server to retrieve the required IP address.


### Part 2: Explain your analysis of the data and provide at least one cause of the incident

Customers started reporting inability to access the website www.yummyrecipesforme.com

The IT team became aware through customer reports that they were unable to access the website.

In response, the IT department employed the network analyzer tool tcpdump to capture packets during a website access attempt in order to analyze the network traffic.

Key findings: The analysis uncovered that the DNS resolution requests sent via UDP consistently encountered a "destination port unreachable" error, with the error messages indicating that UDP port 53, integral for DNS service, was inaccessible.

A likely cause of the incident: A probable cause appears to be a misconfiguration or blockage that is preventing the DNS requests from reaching the DNS server via the necessary UDP port 53.

