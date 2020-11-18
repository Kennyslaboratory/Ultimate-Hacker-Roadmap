# The Newbie's Handbook - Level 2
So you've looked over the laundry list of technological concepts in my Skiddie's Handbook and said, _"Yeah! I know all of this stuff."_  

Odds are you are probably already working in a Technical Support role already and making upwards around $40,000 / year.  Your current job is boring the crap out of you and you were always super interested in Penetration Testing but have no idea how to get a job without a Computer Science Degree, etc.

Great!  I'm here to finally level up your skills and get you out that boring IT Support role--no longer are you forced to deal with angry old men over the phone who can't access their email.  But, don't quit your day job just yet.  Breaking the barrier between IT Support Specialist and Penetration Tester took me nearly 5 years to accomplish.  I went through a lot of ups and downs personally.  However, I didn't have a curated list of topics that I needed to master beforehand.  So hopefully, I can get you up to speed quickly!

-------
## What you should focus on:
If you want to become an Acossicate Penetration Tester then you should put 80% of your effort into **Web Application Hacking**.  Right now, the majority of work that security firms are contracted to test are Web Applications.  Esspecually applications that are deployed to the cloud, such as AWS, GCP, and Azure.  You'll need to have very indepth knowledge of these technologies if you expect to claw your way into an Associate position at a security firm that hires penetration testers.

## The Framework of Understanding a Vulnerability
IMPORTANT!!! Before you can move on to learning another vulnerability, you must be able to answer these 4 questions about the vulnerability you are currently researching:
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
 * Web Applications Tools
   * BurpSuite
   * WPscan
   * Nikto
   * Directory Busters
     * Dirb
     * Dirbuster
   * SQLmap
   * CeWL
   * Hydra
   * testssl.sh
 * Network-Based Tools
   * nmap
   * Netcat
   * Wireshark
   * curl
 * Password Cracking Tools
   * Hashcat
   * John the Ripper
 *
   

## Web Application Fundamentals
  * HTML
    * MetaTags
    * Forms
    * Attributes
    * iFrames
  * CSS
    * Stylesheet Subresource Integrity
  * JavaScript
    * JavaScript Syntax Fundamentals
    * XMLHttpRequest()
    * jQuery _(Basic Familiarity)_
    * JavaScript Frameworks _(Basic Familiarity)_
      * Angular
      * Angular2
      * React
      * Vue
    * JavaScript Subresource Integrity
  * Same-Origin Policy _(SOP)_
  * CORS
    * Preflight Requests
  * Content Deliver Netowrks _(CDNs)_
  * MVC Design Pattern
    * Models
    * Views
    * Controllers
  * HTTP Headers
    * Most Important HTTP Headers
      * User-Agent
      * Host
      * Cookie
      * Authorization
      * Content-Type _(MIME Types)_
      * Transfer-Encoding
      * Accept-Encoding
      * Upgrade
      * CORS Headers
        * Origin
        * Access-Control-Allow-Origin
        * Access-Control-Allow-Credentials
        * Access-Control-Request-Method
        * Access-Control-Request-Headers
      * X-Csrf-Token
  * HTTP Requests
    * GET
    * POST
    * PUT
    * DELETE
    * OPTIONS
  * Session Management
    * Cookies
      * Cookie Flags / Cookie Prefixes
        * HttpOnly
        * HostOnly
        * Secure
        * Same-Site
        * Expires
    * 
 * Database Essentials
   * SQL
     * SQL DBMS _(Basic Familiarity)_
       * MySQL
       * SQLite
       * Microsoft SQL
       * PostgreSQL
       * Oracle DB
     * SQL Syntax Basics
       * USE
       * SELECT
         * WHERE
         * LIKE
       * INSERT
       * UPDATE
       * DROP
       * DELETE
   * NoSQL
     * NoSQL DBMS _(Basic Familiarity)_
       * Redis
       * MongoDB
       * Apache CouchDB
        * Cloud Variants
          * AWS DynomoDB
          * GCP DataStore
          * Azure CosmosDB
     * NoSQL Syntax Basics
      * 

## Web Application Vulnerabilities
  * OWASP Top 10


## Advanced Networking Essentials
  * iptables
  * SSL/TLS In-Depth Understanding
    * HSTS
    * x509
    

## Network-Based Vulnerabilities
  * Man-In-The-Middle Attack
    * ARP Poisoning
  * WiFi Hacking / Security
    * Pre-Shared Keys
    * EAP
    * Promiscuous Mode
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

## Linux Essentials
  * Linux Distributions
    * Debian vs. RedHat
    * Popular Penetration Testing Distros
  * Linux CLI Essentials
    * System Management
    * Installing Software
    * Networking
    * Inspecting Logs
  * Linux Data Exfilration
    * /tmp
    * /etc/passwd
    * /etc/shadow
    * ~/.ssh/id_rsa
    * /etc/cron.d
    * /var/www
    


## BASH Scripting


## Local Privilage Exculation
 * Windows
 * Linux


## Python Essentials
  * Understanding the Basics
    * Reading / Writing Files
      * open()
    * Issuing OS Commands
      * os Module
        * os.chdir()
        * os.mkdir
        * os.remove()
        * os.rename()
        * os.listdir()
        * os.mkdir()
        * os.rmdir()
        * os.chmod()
        * os.path.exists()
        * os.path.isabs()
        * os.path.isdir()
        * os.path.isfile()
        * os.path.getsize()


## Popular CVEs



## Recommended Certifications
 * CompTIA PenTest+
 * CompTIA Linux+
 * CCNA
 * CEH
 * AWS Certified Solutions Architect - Associate
