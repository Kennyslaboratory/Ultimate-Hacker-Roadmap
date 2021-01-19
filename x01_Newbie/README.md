# The Newbie's Curriculum - Level 1
So you've looked over the laundry list of technological concepts in the **[x00_Clueless](https://github.com/Kennyslaboratory/Ultimate-Hacker-Roadmap/tree/main/x00_Clueless)** level and said, _"Yeah! I know all of this stuff."_  

Odds are you are probably working in a Technical Support role already and making upwards around $40,000 / year.  Your current job is boring the crap out of you and you were always super interested in Penetration Testing but have no idea how to get a job without a Computer Science Degree, etc.

Great!  I'm here to finally level up your skills and get you out of that boring IT Support role--no longer are you forced to deal with angry old men over the phone who can't access their email.  But, don't quit your day job just yet.  Breaking the barrier between IT Support Specialist and Penetration Tester took me nearly 5 years to accomplish.  I went through a lot of ups and downs personally.  However, I didn't have a curated list of topics that I needed to master beforehand.  So hopefully, I can get you up to speed quickly!

-------
## What you should focus on:
If you want to become an Associate Penetration Tester then you should put 80% of your effort into **Web Application Hacking**.  Right now, the majority of work that security firms are contracted to test are Web Applications.  Esspecually applications that are deployed to the cloud, such as AWS, GCP, and Azure.  You'll need to have very indepth knowledge of these technologies if you expect to claw your way into an Associate position at a security firm that hires penetration testers.

## The Framework of Understanding a Vulnerability
`IMPORTANT!!!` Before you can move on to learning another vulnerability, you must be able to answer these 4 questions about the vulnerability you are currently researching:
 * **Find**
   * How do you Enumerate the vulnerability?
 * **Exploit**
   * How do you Exploit the vulnerability?
 * **Fix**
   * What are the modern and recommended fixes for the vulnerability?
 * **Bypass**
   * What protections don't work, and how can you bypass weak mitigations that lazy developers implement?
 
 -------
# Table of Contents

## Popular Penetration Testing Tools
 * **Popular Penetration Testing Distros**
    * Kali Linux
    * Parrot
    * BackBox
    * BlackArch
 * **Web Applications Tools**
   * BurpSuite
   * Nikto
   * Directory Busters
     * Dirb
     * Dirbuster
   * SQLmap
   * WPscan
   * CMSmap
   * w3af
   * CeWL
   * testssl.sh
      * **Less-Used Web App Tools...*
         * Aquatone
         * EyeWitness
         * Hydra
 * **Network-Based Tools**
   * nmap
   * Netcat
   * Wireshark
   * curl
      * **DNS Tools**
        * dig
        * dnsenum
        * dnsrecon
 * **Password Cracking Tools**
   * Hashcat
   * John the Ripper
 * **WiFi Hacking Tools**
   * airmon-ng
   * airodump-ng
   * aircrack-ng
   * naive-hashcat
 * **Reverse Engineering Tools**
   * **Linux-Based:**
     * gdb
     * Radare2
     * Hopper _($)_
     * file
     * strings
     * strace
     * ltrace
     * objdump
   * **Windows-Based:**
     * OllyDBG
     * WinDGB
     * IAP Pro _($)_
     * Windows SysInternals
       * ListDLLs
       * Procmon
       * Portmon
       * ProcDump
     * API Monitor
 * **Programming Tools**
   * Visual Studio
   * Visual Studio Code
   * Pycharm
   * Git
   * Git BASH
 * **Misc Tools**
   * MetaSploit Framework
   * **Top Browser Extensions**
      * Wappalyzer
      * Link Redirect Trace
      * JWT Debugger
      * JSONView
      * Retire.js
      * Builtwith
   

## Web Application Fundamentals
  * **HTML**
    * MetaTags
    * Forms
    * Attributes
    * iFrames
  * **CSS**
    * **CSS Frameworks:**
      * Bootstrap
      * Google Material
      * Purple
    * Stylesheet Subresource Integrity
  * **XML**
    * SVG Images
    * SAML _(Basic Familiarity)_
  * **JavaScript**
    * JavaScript Syntax Fundamentals
      * Function Prototyping
      * XMLHttpRequest()
      * JSON _(Data Serialization)_
    * jQuery _(Basic Familiarity)_
    * JavaScript Frameworks _(Basic Familiarity)_
      * Angular
      * Angular2
      * React
      * Vue
    * JavaScript Subresource Integrity
  * **Same-Origin Policy _(SOP)_**
  * **CORS**
    * Preflight Requests
  * **Content Deliver Networks _(CDNs)_**
  * **MVC Design Pattern**
    * Models
    * Views
    * Controllers
  * **HTTP Headers**
    * User-Agent
    * Host
    * Cookie
    * Authorization
    * Content-Type _(MIME Types)_
    * Transfer-Encoding
    * Accept-Encoding
    * Upgrade
    * **CORS Headers**
      * Origin
      * Access-Control-Allow-Origin
      * Access-Control-Allow-Credentials
      * Access-Control-Request-Method
      * Access-Control-Request-Headers
    * **HTTP Security Headers**
      * Strict-Transport-Security
      * Content-Security-Policy
      * X-XSS-Protection
      * X-Frame-Options
      * X-Content-Type-Options
    * X-Csrf-Token
  * **HTTP Requests**
    * GET
    * POST
    * PUT
    * DELETE
    * OPTIONS
  * **Session Management**
    * **Cookies**
      * Cookie Flags / Cookie Prefixes
        * HttpOnly
        * HostOnly
        * Secure
        * Same-Site
        * Expires
    * **JSON Web Tokens _(JWT)_**
      * JWS vs. JWE
        * JWT Header
          * alg:
          * typ:
        * JWT Payload
        * JWT Signature
      * Claims
 * **Database Essentials**
   * **SQL:**
     * **SQL DBMS:** _(Basic Familiarity)_
       * MySQL
       * SQLite
       * Microsoft SQL
       * PostgreSQL
       * Oracle DB
     * **SQL Syntax Basics:**
       * USE
       * SELECT
         * WHERE
         * LIKE
       * INSERT
       * UPDATE
       * DROP
       * DELETE
   * **NoSQL:**
     * **NoSQL DBMS:** _(Basic Familiarity)_
       * Redis
       * MongoDB
       * Apache CouchDB
        * Cloud Variants
          * AWS DynomoDB
          * GCP DataStore
          * Azure CosmosDB
     * **NoSQL Syntax Basics:**
        * $where
        * $eq
        * $ne
        * $gt
   * **Content Management Systems** _(CMS)_
      * WordPress
      * Drupal
      * Joomla
      * Django

## Web Application Reconnaissance
  * **Top 10 To-Do List**
      * Spidering with BurpSuite
        * Take notes of any attack vectors
          * Forms, File Uploads, etc.
      * Check robots.txt
      * nikto
      * Check Security Headers
        * https://securityheaders.com/
      * Google Dorks
      * Checking HTTP Responses for sensitive information
      * Forced Browsing
        * Authorization bugs, etc.
      * Enumerate subdomains
      * Check for HTML Comments
      * View custom JavaScript
        * DOM-XSS, (sources / sinks?)
        * APIs endpoints?
      * Enumerate Frameworks and Versions
        * BuiltWith, WApplzyer, Comments, etc.
        * Research for unpatched CVEs?
      * Session Management Configurations
        * Review OAuth2 Implementations
        * JSON Web Token Implementations
        * SAML Misconfigurations
        * Cookie Prefixes
  * **More Checks**
      * Testing SSL
        * testsssl.sh
        * ssllabs.com scan
      * Vhost Bruteforcing _(eh...)_
        * Accessing unresolved DNS via Host Header
      * CMS Scanners
        * wpscan
      * /.well-known/security.txt
      * Testing for CGI-Bin Vulnerabilities
      
      
## Web Application Vulnerabilities
  * **OWASP Top 10:**
    * **Injection**
      * **SQL Injection:**
        * Error-Based
        * UNION-Based
        * Blind
        * Second-Order SQL Injection
      * **NoSQL Injection**
        * JavaScript Injection
      * **CMD Injection**
      * **LDAP Injection**
    * **Broken Authentication**
    * **Sensitive Data Exposure**
    * **XXE**
      * Document Type Definitions
      * Entities
      * File Upload XXEs
      * XXE-OOB
        * Burp Collaborator
        
    * **Broken Access Controls**
      * Insecure Direct Object Reference
      * Forced Browsing
    * **Security Misconfigurations**
      * Default Passwords
      * Liberal File Permissions
      * Unecrypted backups
      * CORS Misconfigurations, etc.
    * **XSS**
      * Reflected
      * Stored
      * DOM-XSS
    * **Insecure Deserialization**
      * Java
      * PHP
      * .NET
    * **Using Components with Known Vulnerabilities**
    * **Insufficient Logging & Monitoring**
  * **Modern Application Attacks:**
    * HTTP Response Splitting
    * HTTP Request Smuggling
    * Cache Posioning
    * CORS Misconfigurations
    * Server-Side Template Injection 
    * OAuth2 Attacks
      * Open Redirect Token Theft
    * JSON Web Token CVEs
      * [CVE-2015-2951] - alg=none
      * [CVE-2016-10555] - RS/HS256 Key Mismatch
      * [CVE-2018-0114] - Key injection
    * Web Sockets
    * Prototype Pollution
  * **Other Attacks:**
    * CSRF
    * Directory Traversal
    * Local File Inclusion
      * Log Poisoning


## Advanced Networking Essentials
  * SYN Scanning
  * SSL/TLS In-Depth Understanding
    * Let's Encrypt
    * HSTS
    * x509
    * Digital Signatures
      * Certificate Authorities
        * Root CA
        * Intermediate CA
        * Server Certificates
        * Chain of Trust
    * Diffie-Hellman Key Exchange
  * Active Directory Services
    * LDAP
    * Single-Sign-On _(SSO)_
    * Kerberos
  * RADIUS
  * Linux iptables
    * ipTable Chains:
      * Input
      * Forward
      * Output
    * ipTable Connection Responses:
      * Accept
      * Drop
      * Reject
    
## Common Cryptography Algorithms
  * **Hashing Algorithms**
    * HMAC
    * MD5
    * SHA1, SHA2
    * Argon2
    * bCrypt
  * **Encryption Algorithms**
    * EC
    * RSA
    * AES
    * Deffie-Hellman Key Exchange
## Fundamental Network-Based Vulnerabilities
  * Man-In-The-Middle Attack
    * ARP Poisoning
    * Promiscuous Mode
  * WiFi Hacking / Security
    * Pre-Shared Keys
    * EAP
    * Promiscuous Detection
    * Cracking WEP
    * Cracking WPA/WPA2
        * 4-Way Handshakes
          * Pre-Wise Master Keys
          * Authenticator Nonce
          * Supplicant Nonce
        * DeAuth
    * WPA Enterprise
    * Bruteforcing WPS
    * Evil Twin Attack
    * Windows Active Directory Attacks
      * DCSync
      * Single-Sign-On Attacks
        * NTLM Hashes
        * Pass-The-Hash
      * Kerberos Attacks:
        * Pass-The-Ticket Attack
        * Golden Ticket Attack
        * Silver Ticket Attack

## Linux Essentials
  * Linux Distributions:
    * Debian vs. RedHat
    * Debian-Based Distros
      * Ubuntu
      * Kali Linux
      * ParrotOS
    * RedHat
      * RHEL _($)_
      * CentOS
      * Fedora
  * Linux CLI Essentials
    * System Management
    * Installing Software
      * apt _(Debian)_
        * .deb
        * dpkg
      * yum _(RedHat)_
        * .rpm
      * /usr/bin
      * /opt/
    * Networking
      * nmcli
      * nmtui
      * /etc/sysconfig/network-scripts/
    * Inspecting Logs
      * journelctl
      * /var/log
    * Environment Variables
      * env
  * Linux Data Exfilration _(Post exploitation)_
    * /tmp
    * /home
    * /var/log
    * ~/.bash_history
    * Check Environment Variables
      * env
      * printenv
    * /etc/passwd
    * /etc/shadow
    * ~/.ssh/id_rsa
    * /etc/cron.d
    * /var/www
    
## Memory / Binary Fundamentals
  * **Binary**
    * Bit vs. Nyble vs. Byte
    * 8-Bit Binary Translation
    * Base8 vs. Base10
    * Hexadecimal _(Base16)_
  * **The Kernel**
    * Physical Memory vs. Virtual Memory
    * SYSCALLs
    * System Interrupts
    * Modules

## BASH Scripting [to-do]
... ... ... ...

## Local Privilage Exculation
 * Windows
 * Linux
    * LinPEAS
    * Leveraging running processes running as root
        * ps -ef
        * ps -aux
    * Searching for outdated vulnerable software
        * dpkg -l _(Debian)_
        * rpm -qa _(CentOS)_


## Python Essentials
  * Understanding the Basics / coding fundamentals...
    * Loops, If/Else, Variables, Functions, etc
  * Reading / Writing Files
    * open()
      * Read, Write, Append
  * **Requests Module**
    * requests.get()
    * requests.post()
      * auth=(user, pass)
  * **Regular Expressions**
    * [Top 15 Commonly Used RegEx](https://digitalfortress.tech/tricks/top-15-commonly-used-regex/)
    * Parsing for Phone Numbers
    * Parsing for Emails
    * Parsing for Form Values


## Popular CVEs _(Stuff you should probably know about)_
  * Eternal Blue
  * DirtyCow
  * ShellShock
  * MeltDown
    * Spectre
  * HeartBleed
  * MS14-068: Kerberos Elevation of Privilege Vulnerability


## Recommended Certifications
 * CompTIA PenTest+
 * CompTIA Linux+
 * CCNA
 * CEH
 * AWS Certified Solutions Architect - Associate

---------------------------------------------
