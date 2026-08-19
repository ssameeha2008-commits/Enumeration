# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
### Output:
<img width="1033" height="610" alt="image" src="https://github.com/user-attachments/assets/aeaa54aa-e350-4a4f-9971-3e708779d8ce" />


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
### Output:
<img width="1026" height="618" alt="image" src="https://github.com/user-attachments/assets/01ac89ed-0e36-4b9f-bddc-d1ec2e38ee46" />


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
### Output:
<img width="1034" height="620" alt="image" src="https://github.com/user-attachments/assets/4660aff0-6996-4649-9289-b9baad16abc1" />



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
### Output:
<img width="1037" height="712" alt="image" src="https://github.com/user-attachments/assets/a1ddbfad-9544-4e11-8e00-45758faf0cc0" />


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
### Output:
<img width="1035" height="767" alt="image" src="https://github.com/user-attachments/assets/f2cb6331-43ec-4db7-853d-a0f8db43088d" />


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
### Output:
<img width="1027" height="748" alt="image" src="https://github.com/user-attachments/assets/b66dd642-10cb-41ef-8817-72112558f034" />


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
### Output:
<img width="1027" height="591" alt="image" src="https://github.com/user-attachments/assets/d33417ad-79a5-496a-9c97-6563c1c4db1f" />


 
### DNS Enumeration


### DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
<img width="872" height="780" alt="image" src="https://github.com/user-attachments/assets/d22ed9cc-6532-4e2d-9cb7-de6e4dae5b74" />







### dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
### Output:
<img width="884" height="818" alt="image" src="https://github.com/user-attachments/assets/efab49e0-96f0-47aa-990d-c47a7367e95b" />



### smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
### Output:
<img width="929" height="433" alt="image" src="https://github.com/user-attachments/assets/37241827-d0d4-42ca-88c5-3f039b4193d5" />



### Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ### Output:
 <img width="720" height="99" alt="image" src="https://github.com/user-attachments/assets/55c6737b-06b1-4797-9046-e058268fbda9" />

  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
<img width="828" height="213" alt="image" src="https://github.com/user-attachments/assets/c02f6cfb-c5d5-4142-9da5-26b23fed820f" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

