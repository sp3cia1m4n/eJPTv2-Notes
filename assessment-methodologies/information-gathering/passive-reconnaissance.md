# Passive Reconnaissance

### Passive Reconnaissance

In this process, you will not be directly connected to a computer system. This process is used to gather essential information without ever interacting with the target systems.\


#### Website Recon & Footprinting

all commands are here, if you want more explanation regarding the tools and website,&#x20;

> Commands :

* host - Kali tool DNS lookup utility&#x20;
* robots.txt - Search Engine Crawl
* sitemaps.xml - Listing website content
* builtwith - addons to identify different web technologies&#x20;
* wappalyzer - addons to identify different web technologies&#x20;
* whatweb - kali tool that is used to identify different web technologies&#x20;
* httrack - website copier
* Reverse DNS - reverse IP address to DNS
* Whois - Kali and website tool is used to identifies who owns a domain and collect information about them like emails, addresses, especially if there don't activate the privacy protection \
  Netcraft -  is tool to scan websites. \
  DNSdumpster -&#x20;

***

***

#### Website Footprinting With Netcraft

> **Netcraft** - Netcraft provides internet security services for a large number of use cases, including cybercrime detection and disruption, application testing and PCI scanning.
>
> > ![](<../../.gitbook/assets/Pasted image 20230415162847.png>)

***

#### Website Footprinting

> DNSdumpster:  is an online passive scanning tool to obtain information about domains, block addresses, emails, and all kind of information DNS related.
>
> >

***

> DNSDumpster ( website )

![](<../../.gitbook/assets/Pasted image 20230415200917.png>)

***

#### WAF With wafw00f

> wafw00f

* Check firewall behind the website! it can detect mulitple firewall, very useful before using any scanning or footprinting tool
* wafw00f \<url>
* \-a or --findall  #  Find all WAFs which match the signatures, do not stop testing on the first one|\
  \
  ![](<../../.gitbook/assets/Pasted image 20230415174242.png>)

***

#### Subdomain Enumeration

* SubFinder
* Sublist3r

***

#### Google Dorks

> > Search Operators and Commands

* site:ine.com # specfic a domain
* inurl:admin # search specfic keyword in url
* site:\*.ine.com # search for subdomains
* intitle: admin # search intitle "index of" < show index files
* filetype:pdf # search by filetype
* Hacking with Google Dorks https://www.exploit-db.com/google-hacking-database

***

> **WayBackMachine**:  what is the Wayback Machine? The Internet Archive Wayback Machine is a service that allows people to visit archived versions of Web sites
>
> >

***

#### Email Harvesting

> **theHarvester** : a tool for gathering subdomain names, e-mail addresses, virtual hosts, open ports/ banners, and employee names from different public sources
>
> >

***

> **Spyse**_:_ is a search engine which can be used to identify internet assets and perform external reconnaissance easily.\
> \
> ![](<../../.gitbook/assets/image (1).png>)

***

#### Leaked Password Databases

> haveibeenpwned?  :  allows you to search across multiple data breaches to see if your email address or phone number has been compromised.
>
> > ![](<../../.gitbook/assets/Pasted image 20230415202549.png>)

>
>
> DeHashed : is a hacked-database search-engine created for Security Analysts, Journalists, Security Companies, and everyday people to help secure accounts and provide insight on database breaches and account leaks. Protect yourself before it's too late, don't wait until you're hacked.
>
> **What can I search for?**
>
> Anything! Our advanced systems allow you to search for I.P. Addresses, Emails, Usernames, Names, Phone Numbers, VIN Numbers, Addresses; and what makes us even more unique, we allow you to reverse search Passwords, Hashes, and more!
>
> **How can I protect myself or remove my data?**
>
> Simply contact us and we will remove your data. However, removing your data from our search engine will not remove it from others. Your data will still be public, So you must change your passwords!
>
> > ![](<../../.gitbook/assets/Pasted image 20230415204314 (1).png>)
