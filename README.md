# TCPDump_Project
### Objective
Learning about packet sniffing and identifying the activities on a virtualised Kali Linux.

### Disecting TCPDump Command Lines

    tcpdump -i eth0 -v dst [IP Address/Website]

**tcpdump:** This is the name of the command-line tool used for capturing network traffic. It allows you to intercept and display the packets flowing through a network interface.

**-i eth0:** This option specifies the network interface to capture traffic from. In this case, eth0 is the network interface being monitored. eth0 is a common name for the first Ethernet network interface card in a Linux system.

**-v:** This option stands for "verbose" mode. When used, it provides more detailed information about the captured packets, such as protocol headers and other packet details.

**dst [IP Address/Website]:** This part of the command specifies the filter for capturing packets based on their destination. In this case, it's filtering packets where the destination IP address matches the specified IP address or website. Replace [IP Address/Website] with the actual IP address or website URL you want to monitor traffic for.

### Steps for IP Packet Sniffing 

|    | Commands                            | Comments                            |
|----|-------------------------------------|-------------------------------------|
|  1 | ifconfig                            | Check for your ip adress if needed  |
|  2 | tcpdump -i eth0 -v dst [IP]         | It will produce a 'listening status |
|  3 | wait for activites                  | Doing a refresh on a page will generate results|
|  4 | identifying activity                | In this experient we have looked through data and found 'www.youtube.com' the page we have refreshed |

This implies that the target IP is using the website. 

### Steps for Website Sniffing 

Similarly, it will be the same steps, but instead of checking for IP address, we will have to check for a web address. 

### Video Demostration 

https://github.com/JolynNgSC/TCPDump_Project/assets/164031233/c2a07e2d-67ab-48ac-bb22-237252f98fa2

