# 🔗 eJPTv2-notes

<figure><img src=".gitbook/assets/ejpt.png" alt=""><figcaption></figcaption></figure>

It's my eJPTv2 personal note-taking, based on INE PTSv2 course, and some resources I used to gain extra information to fully understand the subject and the technology behind it!



\#smb ports : 135 - 139 - 445 https://sevrosecurity.com/checklists/service-enumeration/ shodan ips with open smb ports

!\[\[Pasted image 20230507194437.png]]

### Windows Recon : SMB Discover And Mount

* nmap
  * `nmap -sV -sC ( default version and script enumeration)`
  * `nmap -o ( Operation System Enumeration )`
* Windows Command line for smb
* net use
  * `net use * /delete ( remove all connections)`
  * `net use < drive D: - Z: whatever > \\<ip address>\<share folder> <password> /user:<username>`
* net view

#### Nmap scan clues for smb for windows

* NetBios
* DNS\_Domain\_Name
* Port 3389 (MS WBT Server )
* Port 49152-163 ( MSRPC )
* Smb-os-discovery script

### SMB: Nmap scripts

SMB Version per OS :

!\[\[Pasted image 20230508025955.png]]

!\[\[Pasted image 20230507194016.png]]

> #### nmap scripts

cd /usr/share/nmap/scripts; ls |  grep smb

!\[\[Pasted image 20230507193807.png]]

Nmap scans :

```bash
 - nmap -p445 --script smb-protocols <ip> ( SMB Version )
 - nmap -p445 --script smb-security-mode <ip> (Message_signing : disabled - authentication_level : )
 - nmap -p445 --script smb-enum-sessions <ip> ( USERS LOGGED IN : )
 - nmap -p445 --script smb-enum-sessions --script-args smbusername=<username> smbpassword=<password> <ip> ( User logged in : and Active SMB Sessions )
 - nmap -p445 --script smb-enum-shares <ip> 
 - nmap -p445 --script smb-enum-shares --script-args smbusername=<username> smbpassword=<password> <ip> 
 -  nmap -p445 --script smb-enum-users --script-args smbusername=<username> smbpassword=<password> <ip> 
 -   nmap -p445 --script smb-enum-domains --script-args smbusername=<username> smbpassword=<password> <ip> 
 -  nmap -p445 --script smb-enum-shares, smb-ls --script-args smbusername=<username> smbpassword=<password> <ip> 
 -   nmap -p445 --script smb-enum-protocols <ip> 
```

### SMB: SMB Map

````bash
┌──(root💀kali)-[~]
└─# wafw00f zonetransfer.me

                ______
               /      \                                                                          
              (  W00f! )                                                                         
               \  ____/                                                                          
               ,,    __            404 Hack Not Found                                            
           |`-.__   / /                      __     __                                           
           /"  _/  /_/                       \ \   / /                                           
          *===*    /                          \ \_/ /  405 Not Allowed                           
         /     )__//                           \   /                                             
    /|  /     /---`                        403 Forbidden                                         
    \\/`   \ |                                 / _ \                                             
    `\    /_\\_              502 Bad Gateway  / / \ \  500 Internal Error                        
      `_____``-`                             /_/   \_\                                           
                                                                                                 
                        ~ WAFW00F : v2.1.0 ~                                                     
        The Web Application Firewall Fingerprinting Toolkit                    ```
````
