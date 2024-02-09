## Cybersecurity Incident Report: Network Attacks Analysis

### Section 1: Identify the type of attack that may have caused this network interruption

One potential explanation for the website's connection timeout error message is: The logs show a surge of TCP SYN requests coming from a single unfamiliar IP address. These are requests to open connections, without completing them.
This event could be an attempted denial-of-service attack. The incomplete connections could be flooding and overwhelming the server resources. This blocks the server from being able to handle valid user connection requests.

### Section 2: Explain how the attack is causing the website to malfunction

When website visitors try to establish a connection with the web server, a three-way handshake occurs using the TCP protocol. Explain the three steps of the handshake:

1. The client sends a SYN (synchronize) packet to the server requesting a connection.

2. The server responds with a SYN-ACK (synchronize-acknowledge) packet, confirming receipt of the SYN and requesting acknowledgement.

3. The client sends an ACK (acknowledge) packet to complete the three-way handshake.

Explain what happens when a malicious actor sends a large number of SYN packets all at once:

A malicious actor can exploit this process by sending a flood of SYN packets without completing the three-way handshake.

Explain what the logs indicate and how that affects the server:

The logs showed a spike of incomplete SYN requests from an unfamiliar IP address. This indicates an attempted SYN flood attack. The attack overwhelms the server with unfulfilled requests, using up resources and preventing legitimate connections.
