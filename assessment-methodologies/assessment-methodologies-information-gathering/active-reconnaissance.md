# Active Reconnaissance

### Active Reconnaissance

In this process, you will directly interact with the computer system to gain information. This information can be relevant and accurate. But there is a risk of getting detected if you are planning active reconnaissance without permission. If you are detected, then system admin can take severe action against you and trail your subsequent activities.\

Tools & Websites 

|  Tool & Website  |              Used for              |                                               usage                                               |
| :--------------: | :--------------------------------: | :-----------------------------------------------------------------------------------------------: |
|     **dig**     |         DNS Lookup utility         |                                          dig axfr @<dns server> <URL>                                            |
|  **fierce.txt**  |         DNS Lookup utility        |                                    fierce --domain zonetransfer.me
| **dnsenum** |   DNS Lookup utility |                                     ./dnsenum.sh \ [ -d ] <domain> [-f <file] [-n <dns server>] [-c]                                    |
|   **dnsenum**  |       DNS Lookup utility       |      dnsrecon \[ -d ] \<URL>      |
|  **dnsmap**  |       DNS Lookup utilty      |      dnsmap <targetDomain> \[ -w ] wordlist.txt \[ -r ] /tmp/results.txt
| **hosts file linux** | Linux File for Mapping Hostnames to IP Addresses | cat /etc/hosts |
| **hosts file windows** | Windows File for Mapping Hostnames to IP Addresses |  type c:\Windows\System32\drivers\etc\hosts |  
|  **nmap** | Port Scanning Tool & Host Discovery | sudo nmap \[ -sn ] ip/cidr \[ 192.168.1.0/24 ]
| arp-scan | Host Discovery | arp-scan \[ -l ] 

### DNS Zone Transfer

What is #DNS ( Domain Name System ) is a protocol that is used to resolve domain names/hostnames to IP addresses. \`\`

* DNS Server ( nameserver) is like a telephone directory that contains domain names and their corresponding IP addressees.
* DNS Records
* A - Resolves a hostname or domain to an IPv4 address.
* AAAA - Resolves a hostname or domain to an IPv6 address.
* NS - Reference to the domains nameserver
* MX - Resolves a domain to a mail server.
* CNAME - Used for domains aliases ( redirect domains to other domains)
* TXT - Text record
* HINFO - Host information
* SOA - Domain authority
* SRV - Service records.
* PTR - Resolves an IP Address to hostname

What is DNS Interrogation?

DNS Interrogation is the process of enumerating DNS records for specifc domain, this process is very important to fetch IP address of a domain, sub domains, mail server addresses, and more. DNS Lookup \
\
`https://mxtoolbox.com/DNSLookup.aspx`\
![](<../../.gitbook/assets/image (2) (1).png>)

What is Zone Transfer ?

* DNS Server admins may want to copy or transfer zone files from one DNS server to another. this process is known as a zone transfer
* if misconfigured and left unsecured, this functionality can be abused by attackers to copy the zone file from the primary DNS Server to another DNS server
* A DNS Server Zone transfer can provide penetration testers with a hostility view of an organinzation network layout, and maybe some time internal network addresses.

## Network Discovery 

 What is Nmap used for?

Nmap **allows you to scan your network and discover not only everything connected to it, but also a wide variety of information about what's connected, what services each host is operating, and so on**. It allows a large number of scanning techniques, such as UDP, TCP connect (), TCP SYN (half-open), and FTP.



 What is arp command in windows ?

arp -a: This command is used to **display the ARP table for a particular IP address**. It also shows all the entries of the ARP cache or table. arp -g: This command works the same as the arp -a command. arp -d: This command is used when you want to delete an entry from the ARP table for a particular interface.

 What is netdiscover?

 Netdiscover is **an active/passive address reconnaissance tool**, mainly developed for those wireless networks without dhcp server, when you are wardriving. It can be also used on hub/switched networks.




