# The Offical Hacker's Handbook - Level 4
Finally, we've weeded out all the skiddies, newbies, and beginners.  We love them, we want the best for them, but it's finally time for some actual hacking.  Modern, expert level material are what we'll be learning and researching about now.  The things listed here is knowledge that I'm currently learning or recently researched in the last year or 2.  This section of the Handbook is subject to change and will improve as I improve.

**You are not ready!** This Handbook is meant for currently employed penetration testers who are not entry-level, and are making over $100k / year.  If you've skipped over the monsterous amount of material in my Associate Hacker's Hackbook then you should not be researching the material in this Handbook.  Unless, you're just curious of course.

-------

## What you should focus on:
You're skilled enough to be tasked with work that invovles:
  * Web Application Security Assessments
  * Mobile Application Security Assessments
  * Network Security Assessments
  * Code Review
  * Binary Debugging & Fuzzing
  
Now it is time to specialize into something that sets you apart from the crowd.  Whether you'd like your specialty to be Hardware, Firmware, Vechicles, IoT, Malware Analysis, or Cloud Infrastructure.  You are finally at a level where you have options and your company will likely pay for and advocate your growth as you develop into a Senior.  Below are a list of specialized technologies and concepts that you might find interesting.
  
-------
# Table of Contents
It's not necessary to know everything here to advance yourself into a Senior, there's likely a lot of things missing that you'll need to research yourself.  I recommend you pick 1 or 2 domains that interest you the most and master them. Please message me with any feedback you have about this list so I may improve it.

---------------------------

# Domain 1: Cloud Security
## Cloud-Based Penetration Testing
 * Popular Cloud Hacking Tools:
   * dnscat2
 * Attacks:
   * Stealing AWS Access Keys
     * SSRF
       * XXE-OOB
         * Documents with XXE payload
         * PDFs with XXE playload
       * SVG with Embedded links
     * Exploiting Deserialization Bugs
     * Command Injection
       * Uploading filenames with code paramenters
         * Printing environment variables
     * Malicious File Upload
       * ImageTragick
     
## AWS Cloud Security
 * **Protecting AWS Access Keys**
   * Best Practices:
     * Removing Root Access Keys
     * Never hardcode AWS keys into code
       * _Keys can be leaked via public repositiories like Github._
     * Avoid storing AWS keys into environment variables
     * Use IAM Instance Profiles to talk between client and APIs
     * Enable IMDSv2 Tokens
     * Never embed keys into mobile apps _(use AWS Cognito)_
   * Tools:
     * aws-vault
       * Temporary access keys
     * AWS Secrets Manager
     * MFA-protected API access _(IAM setting)_
       * "aws:MultiFactorAuthPresent": "true"
         * MFA protecting cross-account delegation
         * MFA protecting instance termination, etc.
         * MFA protecting resources that have resource-based policies
     
 * **Popular AWS SDKs**
   * Boto3 _(Python)_
     * aws configure
       * ~/.aws/credentials
     * boto3.Session()
     * boto3.resource()
     * boto3.client()
   
 * **Securing AWS Resources**
   * Security Groups
     * Inbound Rules
     * Outbound Rules
   * AWS WAF
     * Checkpoints

     
 * **Securing Communications**
   * Confidentality
     * ...
   * Integrity
     * AWS SigV4
   * Availability
     * AWS Shield _(DDoS Protection)_
       * Standard
       * Advanced
   
 * **Securing Data-At-Rest**
   * Confidentality
     * AWS KMS
     * S3 Bucket Permissions
   * Integrity
     * ...
   * Availabity
     * S3 Versioning
     * S3 Object lifecycle Management
       * Transition Actions
       * Expiration Actions
       * LifeCycle Scopes
       
 * **Identity, Authentication, and Authorization**
   * AWS IAM
     * Users
     * Groups
  
 * **Logging, Monitoring, and Auditing**
   * AWS Trusted Advisor
     * Check-Level Status
       * Okay-State
       * Warning-State
       * Error-State
   * AWS CloudWatch
   * AWS CloudTrail
   * AWS Config
   * AWS Artitfact


## Mastering AWS Serverless
 * AWS Serverless Services:
   * AWS API Gateway
   * AWS LAMBDA
   * AWS Fargate
   * AWS EKS
    * Kubernetes
 * Other Services
  * AWS Kenisis
 
 -------------------
# Domain 2: Exploit Development
## Modern Technologies
 * Ahead-Of-Time Compilers _(AOT)_
    * Lexical Analyzer
     * Token Streams
   * Syntax Parser / Analyzer
     * Abstract Syntax Tree
   * IR Generator 
     * Intermediate Representation
   * IR Optimizer
 * Just-In-Time Compilers _(JIT)_
   * Profile-Guided Optimization
   * Pseudo-Constant Propagation
     * Dead Code Elimination
   * Indirect-Virtual Function Inlining
   

