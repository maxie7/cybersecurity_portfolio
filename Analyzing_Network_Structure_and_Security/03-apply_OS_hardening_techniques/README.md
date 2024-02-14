## Tasks

In this activity, I will take on the role of a cybersecurity analyst working for a company that hosts the cooking website, yummyrecipesforme.com. Visitors to the website experience a security issue when loading the main webpage. My job is to investigate, identify, document, and recommend a solution to the security problem.

When investigating the security event, I will review a tcpdump log. I will need to identify the network protocols used to establish the connection between the user and the website. Network protocols are the communication rules and standards networked devices use to transmit data. Unfortunately, malicious actors can also use network protocols to invade and attack private networks. Knowing how to identify the protocols commonly used in attacks will help protect my organization’s network against these types of security events.

To complete the assignment, I will also need to document what occurred during the security incident. Then, I will recommend one security measure to implement to prevent similar security problems in the future.

---

## Scenario

You are a cybersecurity analyst for yummyrecipesforme.com, a website that sells recipes and cookbooks. A disgruntled baker has decided to publish the website’s best-selling recipes for the public to access for free.

The baker executed a brute force attack to gain access to the web host. They repeatedly entered several known default passwords for the administrative account until they correctly guessed the right one. After they obtained the login credentials, they were able to access the admin panel and change the website’s source code. They embedded a javascript function in the source code that prompted visitors to download and run a file upon visiting the website. After running the downloaded file, the customers are redirected to a fake version of the website where the seller’s recipes are now available for free.

Several hours after the attack, multiple customers emailed yummyrecipesforme’s helpdesk. They complained that the company’s website had prompted them to download a file to update their browsers. The customers claimed that, after running the file, the address of the website changed and their personal computers began running more slowly.

In response to this incident, the website owner tries to log in to the admin panel but is unable to, so they reach out to the website hosting provider. You and other cybersecurity analysts are tasked with investigating this security event.

To address the incident, you create a sandbox environment to observe the suspicious website behavior. You run the network protocol analyzer tcpdump, then type in the URL for the website, yummyrecipesforme.com. As soon as the website loads, you are prompted to download an executable file to update your browser. You accept the download and allow the file to run. You then observe that your browser redirects you to a different URL, greatrecipesforme.com, which is designed to look like the original site. However, the recipes your company sells are now posted for free on the new website.

The logs show the following process:

1. The browser requests a DNS resolution of the yummyrecipesforme.com URL.

2. The DNS replies with the correct IP address.

3. The browser initiates an HTTP request for the webpage.

4. The browser initiates the download of the malware.

5. The browser requests another DNS resolution for greatrecipesforme.com.

6. The DNS server responds with the new IP address.

7. The browser initiates an HTTP request to the new IP address.

A senior analyst confirms that the website was compromised. The analyst checks the source code for the website. They notice that javascript code had been added to prompt website visitors to download an executable file. Analysis of the downloaded file found a script that redirects the visitors’ browsers from yummyrecipesforme.com to greatrecipesforme.com.

The cybersecurity team reports that the web server was impacted by a brute force attack. The disgruntled baker was able to guess the password easily because the admin password was still set to the default password. Additionally, there were no controls in place to prevent a brute force attack.

Your job is to document the incident in detail, including identifying the network protocols used to establish the connection between the user and the website.  You should also recommend a security action to take to prevent brute force attacks in the future.

## Resources for more information

- [An introduction to using tcpdump at the Linux command line](https://opensource.com/article/18/10/introduction-tcpdump): Lists several tcpdump commands with example output. The article describes the data in the output and explains why it is useful.
- [tcpdump Cheat Sheet](https://www.comparitech.com/net-admin/tcpdump-cheat-sheet/): Lists tcpdump commands, packet capturing options, output options, protocol codes, and filter options
- [What is a computer port? | Ports in networking](https://www.cloudflare.com/learning/network-layer/what-is-a-computer-port): Provides a short list of the most common ports for network traffic and their associated protocols. The article also provides information about ports in general and using firewalls to block ports.
- [Service Name and Transport Protocol Port Number Registry](https://www.iana.org/assignments/service-names-port-numbers/service-names-port-numbers.xhtml): Provides a database of port numbers with their service names, transport protocols, and descriptions
- [How to Capture and Analyze Network Traffic with tcpdump?](https://geekflare.com/tcpdump-examples/): Provides several tcpdump commands with example output. Then, the article describes each data element in examples of tcpdump output.
- [Masterclass – Tcpdump – Interpreting Output](https://packetpushers.net/blog/masterclass-tcpdump-interpreting-output): Provides a color-coded reference guide to tcpdump output 
