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

![Screenshot 2024-04-10 082944](https://github.com/kanagavel7/Enumeration/assets/162578954/cb6bbffb-f8ca-45fe-8859-35d79d45132d)

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file

![Screenshot 2024-04-10 083014](https://github.com/kanagavel7/Enumeration/assets/162578954/28e4a6ed-5787-4d03-b4a6-dbc47b2273d1)
 in the domain yahoo.com




intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![Screenshot 2024-04-10 083056](https://github.com/kanagavel7/Enumeration/assets/162578954/10e83e1d-b751-48e2-bfbf-70f646f8ba7b)

inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

![Screenshot 2024-04-10 083245](https://github.com/kanagavel7/Enumeration/assets/162578954/e3de2476-f14e-46d6-a937-204d076f79f4)

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![Screenshot 2024-04-10 083343](https://github.com/kanagavel7/Enumeration/assets/162578954/ea919e0c-e35b-4f21-8d5a-458af597faf1)

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![Screenshot 2024-04-10 083445](https://github.com/kanagavel7/Enumeration/assets/162578954/17934e10-785d-49c6-bce1-3b9d834f3ba3)

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

 ![Screenshot 2024-04-10 083602](https://github.com/kanagavel7/Enumeration/assets/162578954/77a9b694-b709-4f4b-b1bb-4a5a2b5aeda5)

# DNS Enumeration


## DNS Recon

provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion

## OUTPUT:

![Screenshot 2024-04-10 084807](https://github.com/kanagavel7/Enumeration/assets/162578954/52d49c20-c23a-4837-b019-b77b58e934ff)

## dnsenum
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

![Screenshot 2024-04-10 085459](https://github.com/kanagavel7/Enumeration/assets/162578954/6bf30c9e-bc8e-4808-b9a5-a554ef0b2905)

![Screenshot 2024-04-10 085638](https://github.com/kanagavel7/Enumeration/assets/162578954/9083fcbe-aa2e-405c-9242-2c49fa1ae990)

## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![Screenshot 2024-04-10 090354](https://github.com/kanagavel7/Enumeration/assets/162578954/cf6d1829-97ae-4123-9b04-21b966d76bc8)

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  
  ![Screenshot 2024-04-10 091531](https://github.com/kanagavel7/Enumeration/assets/162578954/5372d63a-65c8-42de-9e95-883d2dc42299)


## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![Screenshot 2024-04-10 090743](https://github.com/kanagavel7/Enumeration/assets/162578954/e0a09bff-a73a-4d95-8221-6003fa8e8f96)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

