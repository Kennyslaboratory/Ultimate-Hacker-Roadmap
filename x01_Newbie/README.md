# The Newbie's Curriculum - Level 1 (2025 Edition)
**Target Role:** Associate Penetration Tester | **Salary Range:** $50k - $80k | **Timeline:** 12-18 months

## Is This You?

You've mastered the fundamentals from **[x00_Clueless](https://github.com/Kennyslaboratory/Ultimate-Hacker-Roadmap/tree/main/x00_Clueless)** and you're working in IT Support making around $40k-$50k/year. Your job is boring, and you're fascinated by penetration testing but don't know how to break into the field without a Computer Science degree.

**Good news:** You don't need a CS degree. This roadmap will get you from IT Support to Associate Penetration Tester in 12-18 months if you're dedicated.

---

## 🎯 Focus: 80% Web Application Security

**Critical Insight:** The majority of penetration testing work in 2025 is **Web Application Security**. Especially cloud-deployed applications (AWS, Azure, GCP). Master web app security first, then expand to other areas.

**AI Revolution (2025):** AI is automating pentesting. Tools like RapidPen, VulnBot, and HexStrike-AI can find vulnerabilities autonomously. **You MUST understand where AI excels and where human expertise is still critical.**

---

## The Vulnerability Learning Framework

**IMPORTANT:** Before moving to the next vulnerability, master these 4 aspects:

| Aspect | Question to Answer | Example |
|--------|-------------------|---------|
| **Find** | How do you enumerate/discover this vulnerability? | SQL Injection: Input fields, error messages, parameter tampering |
| **Exploit** | How do you exploit it? | SQL Injection: `' OR '1'='1`, UNION-based, time-based blind |
| **Fix** | What are modern, recommended fixes? | SQL Injection: Parameterized queries, input validation, WAF rules |
| **Bypass** | How do you bypass weak mitigations? | SQL Injection: Bypass WAF with encoding, comment injection, etc. |

**Apply this framework to EVERY vulnerability you learn.**

---

## Table of Contents

1. [Penetration Testing Tools](#penetration-testing-tools)
2. [Web Application Fundamentals](#web-application-fundamentals)
3. [OWASP Top 10 (2024 - Latest Version)](#owasp-top-10-2024---latest-version)
4. [AI-Augmented Penetration Testing (2025 Game Changer)](#ai-augmented-penetration-testing-2025-game-changer)
5. [API Security (Critical for 2025)](#api-security-critical-for-2025)
6. [File Upload Vulnerabilities](#file-upload-vulnerabilities)
7. [Business Logic Vulnerabilities](#business-logic-vulnerabilities)
8. [Modern Web Attacks](#modern-web-attacks)
9. [Web Application Reconnaissance](#web-application-reconnaissance)
10. [Networking Essentials](#networking-essentials)
11. [Linux & Command Line](#linux--command-line)
12. [Scripting & Automation](#scripting--automation)
13. [Post-Exploitation & Privilege Escalation](#post-exploitation--privilege-escalation)
14. [Red Team Exercises & Security Audits](#red-team-exercises--security-audits)
15. [Log Analysis & Monitoring](#log-analysis--monitoring)
16. [Social Engineering](#social-engineering)
17. [Practice Labs & CTFs](#practice-labs--ctfs)
18. [Certifications](#certifications)
19. [Penetration Testing Report Writing](#penetration-testing-report-writing)
20. [WAF Bypass Techniques](#waf-bypass-techniques)
21. [Cloud Security Basics (2025 Focus)](#cloud-security-basics-2025-focus)
22. [Skills Checklist](#skills-checklist)

---

## Penetration Testing Tools

### Penetration Testing Distributions

| Distribution | Best For | Download | Tutorial |
|--------------|----------|----------|----------|
| **Kali Linux** | Most popular, comprehensive toolset | [Kali Linux](https://www.kali.org/) | [NetworkChuck: Kali Linux Setup](https://www.youtube.com/watch?v=5e60OrA402M) |
| **Parrot Security** | Lightweight, privacy-focused | [Parrot Security](https://parrotsec.org/) | [Parrot Security Guide](https://parrotsec.org/docs/) |
| **BlackArch** | Advanced tools, Arch-based | [BlackArch](https://blackarch.org/) | [BlackArch Installation Guide](https://blackarch.org/install.html) |

### Web Application Testing Tools

| Tool | Purpose | Best Tutorial | Practice Lab |
|------|---------|---------------|--------------|
| **Burp Suite** | Web vulnerability scanner & proxy | [PortSwigger Web Security Academy](https://portswigger.net/web-security) | [PortSwigger Labs](https://portswigger.net/web-security/all-labs) |
| **OWASP ZAP** | Free web app scanner | [OWASP ZAP Getting Started](https://www.zaproxy.org/getting-started/) | [ZAP Tutorial Videos](https://www.youtube.com/watch?v=5e60OrA402M) |
| **SQLmap** | Automated SQL injection tool | [SQLmap Tutorial - HackerSploit](https://www.youtube.com/watch?v=5e60OrA402M) | [PortSwigger SQL Injection Labs](https://portswigger.net/web-security/sql-injection) |
| **Nikto** | Web server scanner | [Nikto Tutorial - HackerSploit](https://www.youtube.com/watch?v=5e60OrA402M) | Scan test websites |
| **Gobuster** | Directory brute-forcing | [Gobuster Tutorial - NetworkChuck](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe Directory Brute Force](https://tryhackme.com/room/bruteforcing) |
| **WPScan** | WordPress vulnerability scanner | [WPScan Tutorial](https://www.youtube.com/watch?v=5e60OrA402M) | Scan WordPress sites |
| **testssl.sh** | SSL/TLS testing | [testssl.sh Documentation](https://github.com/drwetter/testssl.sh) | [SSL Labs Test](https://www.ssllabs.com/ssltest/) |
| **ffuf** | Fast web fuzzer | [ffuf Tutorial - HackerSploit](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe Fuzzing Room](https://tryhackme.com/) |

### Network Testing Tools

| Tool | Purpose | Best Tutorial | Practice |
|------|---------|---------------|----------|
| **Nmap** | Network discovery & scanning | [NetworkChuck: Nmap Tutorial](https://www.youtube.com/watch?v=5e60OrA402M) | [Nmap Interactive Guide](https://nmap.org/book/toc.html) |
| **Netcat** | Network Swiss Army knife | [HackerSploit: Netcat Tutorial](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe: Netcat Room](https://tryhackme.com/room/networking) |
| **Wireshark** | Packet analysis | [NetworkChuck: Wireshark Tutorial](https://www.youtube.com/watch?v=lb1Dw0elxNk) | [Wireshark Sample Captures](https://wiki.wireshark.org/SampleCaptures) |
| **Metasploit** | Exploitation framework | [Metasploit Unleashed](https://www.offensive-security.com/metasploit-unleashed/) | [TryHackMe: Metasploit Room](https://tryhackme.com/room/metasploitexploitation) |
| **RustScan** | Fast port scanner | [RustScan Tutorial](https://github.com/RustScan/RustScan) | Scan test networks |

### Vulnerability Assessment Tools

**Critical:** Job descriptions require experience with automated vulnerability scanners. These tools are used in real pentesting engagements.

| Tool | Purpose | Best Tutorial | Practice |
|------|---------|---------------|----------|
| **Nessus** | Commercial vulnerability scanner | [Tenable Nessus Documentation](https://docs.tenable.com/nessus/) | [TryHackMe: Nessus Room](https://tryhackme.com/) |
| **OpenVAS** | Open-source vulnerability scanner | [OpenVAS Documentation](https://www.openvas.org/) | [TryHackMe: OpenVAS Room](https://tryhackme.com/) |
| **Nuclei** | Fast vulnerability scanner | [Nuclei Documentation](https://docs.nuclei.sh/) | [Nuclei Templates](https://github.com/projectdiscovery/nuclei-templates) |
| **Burp Suite Scanner** | Web vulnerability scanner | [PortSwigger: Scanner](https://portswigger.net/burp/documentation/desktop/tools/scanner) | [PortSwigger Labs](https://portswigger.net/web-security/all-labs) |
| **Nikto** | Web server scanner | [Nikto Documentation](https://cirt.net/Nikto2) | Scan test websites |
| **Retire.js** | Vulnerable library detection | [Retire.js GitHub](https://github.com/RetireJS/retire.js) | Scan web applications |

### Password Cracking Tools

| Tool | Purpose | Best Tutorial | Practice |
|------|---------|---------------|----------|
| **Hashcat** | Advanced password recovery | [HackerSploit: Hashcat Tutorial](https://www.youtube.com/watch?v=5e60OrA402M) | [Hashcat Examples](https://hashcat.net/wiki/doku.php?id=example_hashes) |
| **John the Ripper** | Password cracker | [HackerSploit: John the Ripper](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe: Password Cracking](https://tryhackme.com/room/crackthehash) |
| **Hydra** | Network login cracker | [HackerSploit: Hydra Tutorial](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe: Hydra Room](https://tryhackme.com/room/hydra) |

---

## Web Application Fundamentals

### HTTP Protocol Deep Dive

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **HTTP Methods** | GET, POST, PUT, DELETE, PATCH | [PortSwigger: HTTP Methods](https://portswigger.net/web-security/http) | [PortSwigger HTTP Labs](https://portswigger.net/web-security/http) |
| **HTTP Headers** | Request/response headers | [PortSwigger: HTTP Headers](https://portswigger.net/web-security/http/headers) | [PortSwigger Headers Labs](https://portswigger.net/web-security/http/headers) |
| **HTTP Status Codes** | 200, 301, 404, 500, etc. | [MDN: HTTP Status Codes](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status) | Analyze HTTP responses in Burp |
| **Cookies & Sessions** | Session management | [PortSwigger: Session Management](https://portswigger.net/web-security/authentication) | [PortSwigger Session Labs](https://portswigger.net/web-security/authentication) |
| **HTTP/2 & HTTP/3** | Modern HTTP protocols | [PortSwigger: HTTP/2](https://portswigger.net/web-security/http2) | Test HTTP/2 implementations |

### Web Technologies

| Technology | Key Concepts | Best Tutorial | Practice |
|------------|--------------|---------------|----------|
| **HTML** | Forms, inputs, DOM | [freeCodeCamp: HTML Full Course](https://www.youtube.com/watch?v=qz0aGYrrlhU) | [PortSwigger XSS Labs](https://portswigger.net/web-security/cross-site-scripting) |
| **JavaScript** | Client-side logic, DOM manipulation | [freeCodeCamp: JavaScript Full Course](https://www.youtube.com/watch?v=jS4aFq5-91M) | [PortSwigger XSS Labs](https://portswigger.net/web-security/cross-site-scripting) |
| **CSS** | Styling, selectors | [freeCodeCamp: CSS Full Course](https://www.youtube.com/watch?v=OXGznpKZ_sA) | Style web pages |
| **JSON** | Data serialization | [MDN: JSON Guide](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON) | Parse JSON in Burp Repeater |
| **XML** | XML structure, XXE attacks | [PortSwigger: XXE](https://portswigger.net/web-security/xxe) | [PortSwigger XXE Labs](https://portswigger.net/web-security/xxe) |

### Same-Origin Policy & CORS

| Concept | Description | Best Tutorial | Practice Lab |
|---------|-------------|---------------|--------------|
| **Same-Origin Policy** | Browser security model | [PortSwigger: Same-Origin Policy](https://portswigger.net/web-security/cors) | [PortSwigger CORS Labs](https://portswigger.net/web-security/cors) |
| **CORS** | Cross-Origin Resource Sharing | [PortSwigger: CORS](https://portswigger.net/web-security/cors) | [PortSwigger CORS Labs](https://portswigger.net/web-security/cors) |
| **CORS Misconfigurations** | Exploiting CORS | [PortSwigger: CORS Vulnerabilities](https://portswigger.net/web-security/cors) | [PortSwigger CORS Labs](https://portswigger.net/web-security/cors) |
| **Content Security Policy** | CSP bypass techniques | [PortSwigger: CSP](https://portswigger.net/web-security/cross-site-scripting/content-security-policy) | [PortSwigger CSP Labs](https://portswigger.net/web-security/cross-site-scripting/content-security-policy) |

### Session Management

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **Cookies** | HttpOnly, Secure, SameSite flags | [PortSwigger: Cookie Security](https://portswigger.net/web-security/authentication) | [PortSwigger Cookie Labs](https://portswigger.net/web-security/authentication) |
| **JWT** | JSON Web Tokens | [PortSwigger: JWT Attacks](https://portswigger.net/web-security/jwt) | [PortSwigger JWT Labs](https://portswigger.net/web-security/jwt) |
| **Session Fixation** | Session attacks | [PortSwigger: Session Fixation](https://portswigger.net/web-security/authentication) | [PortSwigger Session Labs](https://portswigger.net/web-security/authentication) |
| **OAuth 2.0** | OAuth authentication | [PortSwigger: OAuth](https://portswigger.net/web-security/oauth) | [PortSwigger OAuth Labs](https://portswigger.net/web-security/oauth) |
| **SAML** | SAML authentication | [PortSwigger: SAML](https://portswigger.net/web-security/saml) | [PortSwigger SAML Labs](https://portswigger.net/web-security/saml) |

### Databases

| Database Type | Key Concepts | Best Tutorial | Practice |
|---------------|--------------|---------------|----------|
| **SQL** | SELECT, INSERT, UPDATE, DELETE | [SQLBolt: Interactive SQL Tutorial](https://sqlbolt.com/) | [PortSwigger SQL Injection Labs](https://portswigger.net/web-security/sql-injection) |
| **NoSQL** | MongoDB, Redis syntax | [PortSwigger: NoSQL Injection](https://portswigger.net/web-security/nosql-injection) | [PortSwigger NoSQL Labs](https://portswigger.net/web-security/nosql-injection) |
| **SQL Injection** | Union-based, blind, error-based | [HackSplaining: SQL Injection](https://www.hacksplaining.com/lessons) | [PortSwigger SQLi Labs](https://portswigger.net/web-security/sql-injection) |
| **Database Enumeration** | Extracting database info | [PortSwigger: SQL Injection](https://portswigger.net/web-security/sql-injection) | [TryHackMe: SQL Injection](https://tryhackme.com/room/sqlinjectionlm) |

---

## OWASP Top 10 (2024 - Latest Version)

**Critical Update:** OWASP Top 10 was updated in 2024. This is the current standard. Master each one using the Find/Exploit/Fix/Bypass framework.

**Note:** The 2024 version includes new categories and reorganized priorities. This reflects the current threat landscape.

| Rank | Vulnerability | Description | Best Tutorial | Practice Lab |
|------|---------------|-------------|---------------|--------------|
| **A01** | **Broken Access Control** | Unauthorized access to resources | [HackSplaining: Access Control](https://www.hacksplaining.com/lessons), [PortSwigger: Access Control](https://portswigger.net/web-security/access-control) | [PortSwigger Access Control Labs](https://portswigger.net/web-security/access-control) |
| **A02** | **Cryptographic Failures** | Weak encryption/hashing | [HackSplaining: Cryptography](https://www.hacksplaining.com/lessons), [PortSwigger: Cryptographic Failures](https://portswigger.net/web-security/cryptography) | [PortSwigger Crypto Labs](https://portswigger.net/web-security/cryptography) |
| **A03** | **Injection** | SQL, NoSQL, Command injection | [HackSplaining: SQL Injection](https://www.hacksplaining.com/lessons), [PortSwigger: Injection](https://portswigger.net/web-security/injection) | [PortSwigger Injection Labs](https://portswigger.net/web-security/injection) |
| **A04** | **Insecure Design** | Flawed security architecture | [OWASP: Insecure Design](https://owasp.org/Top10/A04_2021-Insecure_Design/) | Review application designs |
| **A05** | **Security Misconfiguration** | Default configs, exposed data | [PortSwigger: Security Misconfiguration](https://portswigger.net/web-security/security-misconfiguration) | [PortSwigger Config Labs](https://portswigger.net/web-security/security-misconfiguration) |
| **A06** | **Vulnerable and Outdated Components** | Outdated libraries/frameworks | [OWASP: Vulnerable Components](https://owasp.org/Top10/A06_2021-Vulnerable_and_Outdated_Components/) | [Retire.js Scanner](https://retirejs.github.io/retire.js/) |
| **A07** | **Identification and Authentication Failures** | Weak authentication mechanisms | [HackSplaining: Authentication](https://www.hacksplaining.com/lessons), [PortSwigger: Authentication](https://portswigger.net/web-security/authentication) | [PortSwigger Auth Labs](https://portswigger.net/web-security/authentication) |
| **A08** | **Software and Data Integrity Failures** | CI/CD pipeline vulnerabilities | [OWASP: Data Integrity](https://owasp.org/Top10/A08_2021-Software_and_Data_Integrity_Failures/) | Review CI/CD pipelines |
| **A09** | **Security Logging and Monitoring Failures** | Insufficient security logging | [OWASP: Logging](https://owasp.org/Top10/A09_2021-Security_Logging_and_Monitoring_Failures/) | Implement logging |
| **A10** | **Server-Side Request Forgery (SSRF)** | Server-Side Request Forgery | [HackSplaining: SSRF](https://www.hacksplaining.com/lessons), [PortSwigger: SSRF](https://portswigger.net/web-security/ssrf) | [PortSwigger SSRF Labs](https://portswigger.net/web-security/ssrf) |

**Note:** OWASP Top 10 2024 maintains similar structure to 2021 but with updated descriptions and priorities. Always refer to [OWASP Top 10 Official](https://owasp.org/Top10/) for the latest version.

### Detailed OWASP Resources

| Resource | Description | Link |
|----------|-------------|------|
| **OWASP Top 10** | Official OWASP Top 10 list (2024) | [OWASP Top 10](https://owasp.org/Top10/) |
| **OWASP Juice Shop** | **BEST modern vulnerable app** - Modern JavaScript app covering all OWASP Top 10 | [Juice Shop](https://owasp.org/www-project-juice-shop/) |
| **HackSplaining** | Interactive lessons on OWASP Top 10 | [HackSplaining Lessons](https://www.hacksplaining.com/lessons) |
| **PortSwigger Web Security Academy** | Free, hands-on labs for all OWASP Top 10 | [Web Security Academy](https://portswigger.net/web-security) |
| **OWASP Testing Guide** | Comprehensive testing methodology | [OWASP Testing Guide](https://owasp.org/www-project-web-security-testing-guide/) |

**Critical:** [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/) is the BEST modern vulnerable application for learning OWASP Top 10. It's a realistic e-commerce app built with modern JavaScript (Node.js, Angular). It covers all OWASP Top 10 vulnerabilities and more. **Use this alongside PortSwigger Labs for comprehensive practice.**

---

## AI-Augmented Penetration Testing (2025 Game Changer)

**The Reality:** AI is transforming pentesting. Tools can now autonomously find vulnerabilities. You MUST understand this landscape.

### AI-Powered Pentesting Tools

| Tool | What It Does | Where AI Excels | Where AI Lacks | Learn More |
|------|--------------|-----------------|----------------|------------|
| **[RapidPen](https://arxiv.org/abs/2502.16730)** | Autonomous vulnerability discovery & exploitation | Fast reconnaissance, pattern matching, known exploit chains | Business logic flaws, complex chaining, creative bypasses | [RapidPen Research](https://arxiv.org/abs/2502.16730) |
| **[VulnBot](https://arxiv.org/abs/2501.13411)** | Multi-agent pentesting simulation | Automated scanning, tool orchestration, report generation | Human intuition, context understanding, novel attacks | [VulnBot Research](https://arxiv.org/abs/2501.13411) |
| **[HexStrike-AI](https://www.techradar.com/pro/security/new-ai-powered-hexstrike-tool-is-being-used-to-target-multiple-citrix-security-flaws)** | LLM-integrated exploitation framework | Rapid exploitation, tool selection, known vulnerabilities | Custom payloads, advanced evasion, social engineering | [HexStrike-AI Info](https://www.techradar.com/pro/security/new-ai-powered-hexstrike-tool-is-being-used-to-target-multiple-citrix-security-flaws) |
| **[Garak](https://en.wikipedia.org/wiki/Garak_%28software%29)** | LLM vulnerability scanner | Testing AI systems, prompt injection, model security | Traditional web app testing, network pentesting | [Garak Documentation](https://en.wikipedia.org/wiki/Garak_%28software%29) |

### Where AI Excels (2025)

| Capability | Why AI Is Great | Example |
|------------|-----------------|---------|
| **Pattern Recognition** | Identifies known vulnerability patterns quickly | SQL injection signatures, XSS payloads |
| **Automated Scanning** | Runs scans 24/7 without fatigue | Port scanning, directory enumeration |
| **Report Generation** | Creates detailed reports automatically | Vulnerability documentation |
| **Tool Orchestration** | Coordinates multiple tools efficiently | Running Nmap → Burp → SQLmap in sequence |
| **Known Exploit Chains** | Executes documented attack paths | CVE exploitation workflows |

### Where AI Still Lacks (Human Advantage)

| Capability | Why Humans Are Critical | Example |
|------------|-------------------------|---------|
| **Business Logic Flaws** | Requires understanding application context | Price manipulation, workflow bypass |
| **Creative Bypasses** | Needs out-of-the-box thinking | Custom WAF bypasses, novel encoding |
| **Social Engineering** | Requires human psychology understanding | Phishing campaigns, pretexting |
| **Complex Chaining** | Needs deep understanding of systems | Multi-step attacks across services |
| **Context Understanding** | Requires domain knowledge | Industry-specific vulnerabilities |
| **Custom Payloads** | Needs understanding of target environment | Environment-specific exploits |

### How to Stay Relevant

**You MUST:**
1. **Master fundamentals** - AI can't replace deep understanding
2. **Focus on logic flaws** - AI struggles with business logic
3. **Learn creative bypasses** - AI follows patterns, you break them
4. **Understand AI tools** - Use them as force multipliers, not replacements
5. **Develop human skills** - Social engineering, creative thinking, context awareness

**Think of AI as:** Your automated assistant that handles repetitive tasks, while you focus on the complex, creative, and contextual work that requires human intelligence.

---

## API Security (Critical for 2025)

**Why This Matters:** Modern applications are API-first. REST APIs, GraphQL, and gRPC are everywhere. You MUST understand API security.

### REST API Security

| Topic | Description | Best Tutorial | Practice Lab |
|-------|-------------|---------------|--------------|
| **REST API Basics** | Understanding REST architecture | [PortSwigger: API Security](https://portswigger.net/web-security/api-security) | [PortSwigger API Labs](https://portswigger.net/web-security/api-security) |
| **API Authentication** | API keys, OAuth, JWT for APIs | [PortSwigger: API Authentication](https://portswigger.net/web-security/api-security) | [PortSwigger API Labs](https://portswigger.net/web-security/api-security) |
| **API Rate Limiting** | Bypassing rate limits | [PortSwigger: API Security](https://portswigger.net/web-security/api-security) | Test API endpoints |
| **API Parameter Pollution** | HPP attacks on APIs | [PortSwigger: Parameter Pollution](https://portswigger.net/web-security/ssrf) | [PortSwigger Labs](https://portswigger.net/web-security/api-security) |

### GraphQL Security

| Topic | Description | Best Tutorial | Practice Lab |
|-------|-------------|---------------|--------------|
| **GraphQL Basics** | Understanding GraphQL queries | [GraphQL.org Tutorial](https://graphql.org/learn/) | [PentesterLab: GraphQL](https://pentesterlab.com/) |
| **GraphQL Introspection** | Discovering GraphQL schemas | [PortSwigger: GraphQL](https://portswigger.net/web-security/graphql) | [PentesterLab: GraphQL](https://pentesterlab.com/) |
| **GraphQL Injection** | GraphQL injection attacks | [PortSwigger: GraphQL](https://portswigger.net/web-security/graphql) | [PentesterLab: GraphQL](https://pentesterlab.com/) |
| **GraphQL Authorization** | Bypassing GraphQL authorization | [PortSwigger: GraphQL](https://portswigger.net/web-security/graphql) | [PentesterLab: GraphQL](https://pentesterlab.com/) |

### API Testing Tools

| Tool | Purpose | Best Tutorial | Practice |
|------|---------|---------------|----------|
| **Postman** | API testing and manipulation | [Postman Learning Center](https://learning.postman.com/) | Test REST APIs |
| **GraphQL Playground** | GraphQL testing | [GraphQL Playground](https://github.com/graphql/graphql-playground) | Test GraphQL endpoints |
| **Burp Suite** | API security testing | [PortSwigger: API Testing](https://portswigger.net/web-security/api-security) | [PortSwigger API Labs](https://portswigger.net/web-security/api-security) |

---

## File Upload Vulnerabilities

**Why This Matters:** File uploads are everywhere. They're a common attack vector. You MUST understand file upload security.

| Vulnerability | Description | Best Tutorial | Practice Lab |
|---------------|-------------|---------------|--------------|
| **Unrestricted File Upload** | Uploading malicious files | [PortSwigger: File Upload](https://portswigger.net/web-security/file-upload) | [PortSwigger File Upload Labs](https://portswigger.net/web-security/file-upload) |
| **File Type Validation Bypass** | Bypassing file type checks | [PortSwigger: File Upload](https://portswigger.net/web-security/file-upload) | [PortSwigger File Upload Labs](https://portswigger.net/web-security/file-upload) |
| **Path Traversal in Uploads** | Directory traversal via uploads | [PortSwigger: Path Traversal](https://portswigger.net/web-security/file-path-traversal) | [PortSwigger Path Traversal Labs](https://portswigger.net/web-security/file-path-traversal) |
| **Web Shell Upload** | Uploading PHP/ASP shells | [PentesterLab: File Upload](https://pentesterlab.com/) | [PentesterLab File Upload](https://pentesterlab.com/) |

---

## Business Logic Vulnerabilities

**Why This Matters:** Logic flaws are harder to find but often more critical. They bypass technical controls.

| Vulnerability | Description | Best Tutorial | Practice Lab |
|---------------|-------------|---------------|--------------|
| **Price Manipulation** | Changing prices in requests | [PortSwigger: Business Logic](https://portswigger.net/web-security/logic-flaws) | [PortSwigger Logic Flaw Labs](https://portswigger.net/web-security/logic-flaws) |
| **Workflow Bypass** | Skipping steps in processes | [PortSwigger: Business Logic](https://portswigger.net/web-security/logic-flaws) | [PortSwigger Logic Flaw Labs](https://portswigger.net/web-security/logic-flaws) |
| **Race Conditions** | Time-of-check to time-of-use | [PortSwigger: Race Conditions](https://portswigger.net/web-security/race-conditions) | [PortSwigger Race Condition Labs](https://portswigger.net/web-security/race-conditions) |
| **Excessive Functionality** | Hidden/undocumented features | [OWASP: Excessive Functionality](https://owasp.org/) | Review application functionality |

---

## Modern Web Attacks

### Advanced Injection Attacks

| Attack Type | Description | Best Tutorial | Practice Lab |
|-------------|-------------|---------------|--------------|
| **SQL Injection** | Database injection attacks | [PortSwigger: SQL Injection](https://portswigger.net/web-security/sql-injection) | [PortSwigger SQLi Labs](https://portswigger.net/web-security/sql-injection) |
| **NoSQL Injection** | MongoDB, CouchDB injection | [PortSwigger: NoSQL Injection](https://portswigger.net/web-security/nosql-injection) | [PortSwigger NoSQL Labs](https://portswigger.net/web-security/nosql-injection) |
| **Command Injection** | OS command execution | [PortSwigger: Command Injection](https://portswigger.net/web-security/os-command-injection) | [PortSwigger Command Injection Labs](https://portswigger.net/web-security/os-command-injection) |
| **LDAP Injection** | Directory service injection | [OWASP: LDAP Injection](https://owasp.org/www-community/attacks/LDAP_Injection) | [PentesterLab: LDAP](https://pentesterlab.com/) |
| **XXE** | XML External Entity injection | [PortSwigger: XXE](https://portswigger.net/web-security/xxe) | [PortSwigger XXE Labs](https://portswigger.net/web-security/xxe) |
| **XPath Injection** | XPath query injection | [OWASP: XPath Injection](https://owasp.org/www-community/attacks/XPATH_Injection) | Practice XPath queries |
| **Template Injection** | Server-side template injection | [PortSwigger: SSTI](https://portswigger.net/web-security/server-side-template-injection) | [PortSwigger SSTI Labs](https://portswigger.net/web-security/server-side-template-injection) |

### Cross-Site Scripting (XSS)

| XSS Type | Description | Best Tutorial | Practice Lab |
|----------|-------------|---------------|--------------|
| **Reflected XSS** | Non-persistent XSS | [HackSplaining: XSS](https://www.hacksplaining.com/lessons), [PortSwigger: Reflected XSS](https://portswigger.net/web-security/cross-site-scripting/reflected) | [PortSwigger XSS Labs](https://portswigger.net/web-security/cross-site-scripting) |
| **Stored XSS** | Persistent XSS | [HackSplaining: XSS](https://www.hacksplaining.com/lessons), [PortSwigger: Stored XSS](https://portswigger.net/web-security/cross-site-scripting/stored) | [PortSwigger XSS Labs](https://portswigger.net/web-security/cross-site-scripting) |
| **DOM-Based XSS** | Client-side XSS | [HackSplaining: XSS](https://www.hacksplaining.com/lessons), [PortSwigger: DOM XSS](https://portswigger.net/web-security/cross-site-scripting/dom-based) | [PortSwigger DOM XSS Labs](https://portswigger.net/web-security/cross-site-scripting/dom-based) |
| **XSS Filter Bypass** | Bypassing XSS filters | [PortSwigger: XSS Filter Bypass](https://portswigger.net/web-security/cross-site-scripting) | [PortSwigger XSS Labs](https://portswigger.net/web-security/cross-site-scripting) |
| **mXSS** | Mutation XSS | [PortSwigger: mXSS](https://portswigger.net/web-security/cross-site-scripting) | [PortSwigger XSS Labs](https://portswigger.net/web-security/cross-site-scripting) |

### Authentication & Authorization Attacks

| Attack | Description | Best Tutorial | Practice Lab |
|--------|-------------|---------------|--------------|
| **Broken Authentication** | Weak login mechanisms | [PortSwigger: Authentication](https://portswigger.net/web-security/authentication) | [PortSwigger Auth Labs](https://portswigger.net/web-security/authentication) |
| **IDOR** | Insecure Direct Object References | [PortSwigger: IDOR](https://portswigger.net/web-security/access-control) | [PortSwigger IDOR Labs](https://portswigger.net/web-security/access-control) |
| **JWT Vulnerabilities** | JWT manipulation attacks | [PortSwigger: JWT Attacks](https://portswigger.net/web-security/jwt) | [PortSwigger JWT Labs](https://portswigger.net/web-security/jwt) |
| **OAuth2 Attacks** | OAuth misconfigurations | [PortSwigger: OAuth](https://portswigger.net/web-security/oauth) | [PortSwigger OAuth Labs](https://portswigger.net/web-security/oauth) |
| **SAML Attacks** | SAML authentication flaws | [PortSwigger: SAML](https://portswigger.net/web-security/saml) | [PortSwigger SAML Labs](https://portswigger.net/web-security/saml) |
| **2FA Bypass** | Bypassing two-factor authentication | [PortSwigger: 2FA](https://portswigger.net/web-security/authentication) | [PortSwigger Auth Labs](https://portswigger.net/web-security/authentication) |

### Modern Attack Vectors

| Attack | Description | Best Tutorial | Practice Lab |
|--------|-------------|---------------|--------------|
| **HTTP Request Smuggling** | Request smuggling attacks | [PortSwigger: Request Smuggling](https://portswigger.net/web-security/request-smuggling) | [PortSwigger Smuggling Labs](https://portswigger.net/web-security/request-smuggling) |
| **Cache Poisoning** | Web cache attacks | [PortSwigger: Cache Poisoning](https://portswigger.net/web-security/web-cache-poisoning) | [PortSwigger Cache Labs](https://portswigger.net/web-security/web-cache-poisoning) |
| **Server-Side Template Injection** | SSTI attacks | [PortSwigger: SSTI](https://portswigger.net/web-security/server-side-template-injection) | [PortSwigger SSTI Labs](https://portswigger.net/web-security/server-side-template-injection) |
| **CSRF** | Cross-Site Request Forgery | [PortSwigger: CSRF](https://portswigger.net/web-security/csrf) | [PortSwigger CSRF Labs](https://portswigger.net/web-security/csrf) |
| **SSRF** | Server-Side Request Forgery | [PortSwigger: SSRF](https://portswigger.net/web-security/ssrf) | [PortSwigger SSRF Labs](https://portswigger.net/web-security/ssrf) |
| **WebSockets** | WebSocket security issues | [PortSwigger: WebSockets](https://portswigger.net/web-security/websockets) | [PortSwigger WebSocket Labs](https://portswigger.net/web-security/websockets) |
| **Race Conditions** | Time-of-check to time-of-use | [PortSwigger: Race Conditions](https://portswigger.net/web-security/race-conditions) | [PortSwigger Race Condition Labs](https://portswigger.net/web-security/race-conditions) |

---

## Web Application Reconnaissance

### Reconnaissance Checklist

| Step | Tool/Method | Best Tutorial | Practice |
|------|-------------|---------------|----------|
| **1. Spidering** | Burp Suite Spider | [PortSwigger: Burp Spider](https://portswigger.net/burp/documentation/desktop/tools/spider) | Spider a test application |
| **2. Directory Brute-Forcing** | Gobuster, ffuf, Dirb | [HackerSploit: Gobuster Tutorial](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe: Directory Brute Force](https://tryhackme.com/room/bruteforcing) |
| **3. Subdomain Enumeration** | Sublist3r, Amass, Subfinder | [HackerSploit: Subdomain Enumeration](https://www.youtube.com/watch?v=5e60OrA402M) | Enumerate subdomains |
| **4. Technology Detection** | Wappalyzer, BuiltWith, WhatWeb | [Wappalyzer Chrome Extension](https://chrome.google.com/webstore/detail/wappalyzer) | Identify technologies |
| **5. Security Headers** | SecurityHeaders.com, Burp | [SecurityHeaders.com](https://securityheaders.com/) | Check security headers |
| **6. SSL/TLS Testing** | testssl.sh, SSL Labs | [testssl.sh Documentation](https://github.com/drwetter/testssl.sh) | [SSL Labs Test](https://www.ssllabs.com/ssltest/) |
| **7. Google Dorking** | Google search operators | [Google Hacking Database](https://www.exploit-db.com/google-hacking-database) | Practice dorking |
| **8. Source Code Review** | View page source, JavaScript | [PortSwigger: Client-Side Testing](https://portswigger.net/web-security/client-side) | Review source code |
| **9. API Discovery** | Burp, Postman, GraphQL Introspection | [PortSwigger: API Security](https://portswigger.net/web-security/api-security) | Discover API endpoints |
| **10. Wayback Machine** | Historical site analysis | [Archive.org Wayback Machine](https://web.archive.org/) | Find old endpoints |
| **11. JavaScript Analysis** | Analyze client-side code | [PortSwigger: Client-Side Testing](https://portswigger.net/web-security/client-side) | Review JavaScript files |
| **12. Parameter Discovery** | Finding hidden parameters | [PortSwigger: Parameter Discovery](https://portswigger.net/web-security) | Use Burp Intruder |

### Browser Extensions for Pentesters

| Extension | Purpose | Install |
|-----------|---------|--------|
| **Wappalyzer** | Technology detection | [Chrome](https://chrome.google.com/webstore/detail/wappalyzer) |
| **FoxyProxy** | Proxy management | [Chrome](https://chrome.google.com/webstore/detail/foxyproxy) |
| **JWT Debugger** | JWT token analysis | [Chrome](https://chrome.google.com/webstore/detail/jwt-debugger) |
| **Retire.js** | Vulnerable library detection | [Chrome](https://chrome.google.com/webstore/detail/retirejs) |
| **HackBar** | Quick payload testing | [Chrome](https://chrome.google.com/webstore/detail/hackbar) |
| **Cookie Editor** | Cookie manipulation | [Chrome](https://chrome.google.com/webstore/detail/cookie-editor) |
| **ModHeader** | Header modification | [Chrome](https://chrome.google.com/webstore/detail/modheader) |

---

## Networking Essentials

**Critical:** Job descriptions require deep networking knowledge. IP addressing, subnetting, DNS, DHCP, and firewall configurations are fundamental.

### Network Fundamentals (MUST KNOW)

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **IP Addressing** | IPv4, IPv6, subnet masks | [NetworkChuck: Subnetting](https://www.youtube.com/watch?v=5e60OrA402M) | [Subnet Calculator](https://www.subnet-calculator.com/) |
| **Subnetting** | CIDR notation, subnet calculations | [Professor Messer: Subnetting](https://www.professormesser.com/network-plus/n10-007/subnetting/) | [Subnet Practice](https://www.subnettingpractice.com/) |
| **DNS** | Domain name resolution, DNS records | [NetworkChuck: DNS Explained](https://www.youtube.com/watch?v=mpQZVYPuDGU) | [TryHackMe: DNS](https://tryhackme.com/room/dnsmanipulation) |
| **DHCP** | Dynamic Host Configuration Protocol | [NetworkChuck: DHCP](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe: Networking](https://tryhackme.com/room/networking) |
| **Firewall Configurations** | ACLs, rules, port filtering | [NetworkChuck: Firewalls](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe: Firewalls](https://tryhackme.com/) |
| **TCP/IP Deep Dive** | TCP handshake, flags, states | [NetworkChuck: TCP/IP](https://www.youtube.com/watch?v=4PXaL7nXqUI) | [Wireshark Packet Analysis](https://wiki.wireshark.org/SampleCaptures) |
| **UDP** | User Datagram Protocol | [NetworkChuck: UDP](https://www.youtube.com/watch?v=5e60OrA402M) | [Wireshark UDP Analysis](https://wiki.wireshark.org/SampleCaptures) |
| **OSI Model** | 7-layer network model | [NetworkChuck: OSI Model](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe: OSI Model](https://tryhackme.com/) |

### Advanced Networking Concepts

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **SSL/TLS** | Encryption protocols | [PortSwigger: TLS](https://portswigger.net/web-security/ssl-tls) | [SSL Labs Test](https://www.ssllabs.com/ssltest/) |
| **Active Directory Basics** | AD structure and concepts | [TryHackMe: Active Directory](https://tryhackme.com/module/active-directory-basics) | [TryHackMe AD Rooms](https://tryhackme.com/module/active-directory-basics) |
| **HTTP/2 & HTTP/3** | Modern HTTP protocols | [PortSwigger: HTTP/2](https://portswigger.net/web-security/http2) | Test HTTP/2 implementations |
| **WebSockets** | WebSocket protocol | [PortSwigger: WebSockets](https://portswigger.net/web-security/websockets) | [PortSwigger WebSocket Labs](https://portswigger.net/web-security/websockets) |
| **VLANs** | Virtual LANs | [NetworkChuck: VLANs](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe: Networking](https://tryhackme.com/) |
| **Routing** | Routing protocols, routing tables | [NetworkChuck: Routing](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe: Networking](https://tryhackme.com/) |

---

## Linux & Command Line

### Essential Linux Skills

| Skill | Commands | Best Tutorial | Practice |
|-------|----------|---------------|----------|
| **File Operations** | ls, cd, cp, mv, rm, find | [TryHackMe: Linux Fundamentals](https://tryhackme.com/room/linuxfundamentals) | [Linux Journey](https://linuxjourney.com/) |
| **Text Processing** | grep, awk, sed, cut | [Linux Journey: Text Processing](https://linuxjourney.com/lesson/grep) | Process log files |
| **Process Management** | ps, top, kill, systemctl | [Linux Journey: Processes](https://linuxjourney.com/lesson/processes) | Manage processes |
| **Networking** | netstat, ss, tcpdump, curl | [NetworkChuck: Linux Networking](https://www.youtube.com/watch?v=5W8A2f-KgJE) | Network troubleshooting |
| **Permissions** | chmod, chown, sudo | [Linux Journey: Permissions](https://linuxjourney.com/lesson/file-permissions) | Manage file permissions |
| **Package Management** | apt, yum, pip | [Linux Journey: Package Management](https://linuxjourney.com/lesson/package-management) | Install tools |
| **Log Analysis** | journalctl, tail, less | [Linux Journey: Logs](https://linuxjourney.com/lesson/systemd) | Analyze system logs |

### BASH Scripting Basics

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **Variables** | Setting and using variables | [freeCodeCamp: Bash Scripting](https://www.youtube.com/watch?v=5e60OrA402M) | Write simple scripts |
| **Loops** | for, while loops | [freeCodeCamp: Bash Scripting](https://www.youtube.com/watch?v=5e60OrA402M) | Automate tasks |
| **Conditionals** | if/else statements | [freeCodeCamp: Bash Scripting](https://www.youtube.com/watch?v=5e60OrA402M) | Create conditional scripts |
| **Functions** | Creating reusable functions | [freeCodeCamp: Bash Scripting](https://www.youtube.com/watch?v=5e60OrA402M) | Build function library |
| **Command Substitution** | Using command output | [Linux Journey: Shell](https://linuxjourney.com/lesson/the-shell) | Chain commands |

---

## Scripting & Automation

**Critical:** Job descriptions require scripting proficiency. Python, PowerShell, Bash, Perl, Go, and Ruby are all mentioned. Focus on Python first, then PowerShell for Windows environments.

### Python Essentials

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **Python Basics** | Variables, data types, functions | [freeCodeCamp: Python Full Course](https://www.youtube.com/watch?v=jS4aFq5-91M) | [Codecademy Python](https://www.codecademy.com/learn/learn-python-3) |
| **Fast Coding Mastery** | Learn syntax fast for interviews | [Codecademy](https://www.codecademy.com/) | [Codecademy](https://www.codecademy.com/) |
| **Requests Library** | HTTP requests | [freeCodeCamp: Requests Library](https://www.youtube.com/watch?v=jS4aFq5-91M) | Build web scraper |
| **Regular Expressions** | Pattern matching | [freeCodeCamp: Regex](https://www.youtube.com/watch?v=jS4aFq5-91M) | [Regex101](https://regex101.com/) |
| **Socket Programming** | Network programming | [NetworkChuck: Python Sockets](https://www.youtube.com/watch?v=5e60OrA402M) | Build network tools |
| **File Operations** | Reading/writing files | [freeCodeCamp: File I/O](https://www.youtube.com/watch?v=jS4aFq5-91M) | Process log files |
| **JSON Parsing** | Working with JSON data | [freeCodeCamp: JSON](https://www.youtube.com/watch?v=jS4aFq5-91M) | Parse API responses |
| **Threading** | Multi-threaded scripts | [freeCodeCamp: Threading](https://www.youtube.com/watch?v=jS4aFq5-91M) | Build concurrent tools |

### PowerShell (Windows Environments)

**Critical:** Many pentesting engagements target Windows environments. PowerShell is essential.

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **PowerShell Basics** | Cmdlets, variables, objects | [Kevin Stratvert: PowerShell](https://www.youtube.com/watch?v=5e60OrA402M) | [TryHackMe: PowerShell](https://tryhackme.com/room/powershell) |
| **PowerShell Scripting** | Functions, loops, conditionals | [freeCodeCamp: PowerShell](https://www.youtube.com/watch?v=5e60OrA402M) | Write PowerShell scripts |
| **Active Directory Cmdlets** | AD manipulation with PowerShell | [TryHackMe: PowerShell](https://tryhackme.com/room/powershell) | [TryHackMe AD Rooms](https://tryhackme.com/module/active-directory-basics) |
| **PowerShell for Pentesting** | Offensive PowerShell techniques | [TryHackMe: PowerShell](https://tryhackme.com/room/powershell) | [HTB Academy: PowerShell](https://academy.hackthebox.com/) |

### Additional Scripting Languages

**Note:** Job descriptions mention Perl, Go, and Ruby. Learn these if you have time, but Python and PowerShell are priority.

| Language | Use Case | Best Tutorial | When to Learn |
|----------|----------|---------------|---------------|
| **Perl** | Legacy systems, regex-heavy tasks | [Perl Tutorial](https://www.perl.org/) | If working with legacy systems |
| **Go** | Fast network tools, modern tooling | [freeCodeCamp: Go](https://www.youtube.com/watch?v=5e60OrA402M) | If building high-performance tools |
| **Ruby** | Metasploit modules, web automation | [freeCodeCamp: Ruby](https://www.youtube.com/watch?v=5e60OrA402M) | If contributing to Metasploit |

### Coding Interview Preparation

| Platform | Purpose | Best For | Link |
|----------|---------|----------|------|
| **LeetCode** | Algorithm and coding challenges | FAANG/Meta interviews - essential for security engineers too | [LeetCode](https://leetcode.com/) |
| **Codecademy** | Fast syntax mastery | Learning to code quickly without spending all your time | [Codecademy](https://www.codecademy.com/) |

### Python Pentesting Scripts

| Script Type | Purpose | Best Tutorial | Practice |
|-------------|---------|---------------|----------|
| **Port Scanner** | Scan for open ports | [NetworkChuck: Port Scanner](https://www.youtube.com/watch?v=5e60OrA402M) | Build port scanner |
| **Directory Brute-Forcer** | Enumerate directories | [HackerSploit: Directory Brute-Forcer](https://www.youtube.com/watch?v=5e60OrA402M) | Build brute-forcer |
| **Web Scraper** | Extract web data | [freeCodeCamp: Web Scraping](https://www.youtube.com/watch?v=jS4aFq5-91M) | Scrape websites |
| **Password Cracker** | Hash cracking | [HackerSploit: Hash Cracker](https://www.youtube.com/watch?v=5e60OrA402M) | Build hash cracker |
| **SQL Injection Tool** | Automated SQLi testing | [HackerSploit: SQLi Tool](https://www.youtube.com/watch?v=5e60OrA402M) | Build SQLi scanner |
| **XSS Payload Generator** | Generate XSS payloads | [PortSwigger: XSS](https://portswigger.net/web-security/cross-site-scripting) | Build payload generator |
| **API Fuzzer** | Fuzz API endpoints | [PortSwigger: API Security](https://portswigger.net/web-security/api-security) | Build API fuzzer |

---

## Practice Labs & CTFs

### Free Practice Platforms

| Platform | Description | Best For | Link |
|----------|-------------|----------|------|
| **PortSwigger Web Security Academy** | Free, hands-on web security labs | Web application security - **MUST USE** | [Web Security Academy](https://portswigger.net/web-security) |
| **HackSplaining** | Interactive vulnerability lessons | Quick understanding of concepts | [HackSplaining Lessons](https://www.hacksplaining.com/lessons) |
| **PentesterLab** | Web application security exercises | Web security fundamentals | [PentesterLab](https://pentesterlab.com/) |
| **TryHackMe** | Guided learning paths | Beginners - structured learning | [TryHackMe](https://tryhackme.com/) |
| **HackTheBox** | Realistic penetration testing | Intermediate/Advanced | [HackTheBox](https://www.hackthebox.com/) |
| **HackTheBox Academy** | Structured courses and labs | Learning specific topics | [HTB Academy](https://academy.hackthebox.com/) |
| **OWASP Juice Shop** | Modern vulnerable web application | **BEST for learning OWASP Top 10** - Modern JavaScript app | [Juice Shop](https://owasp.org/www-project-juice-shop/) |
| **DVWA** | Damn Vulnerable Web Application | Local practice | [DVWA](http://www.dvwa.co.uk/) |
| **WebGoat** | OWASP vulnerable application | Learning OWASP Top 10 | [WebGoat](https://owasp.org/www-project-webgoat/) |
| **bWAPP** | Buggy web application | Various vulnerabilities | [bWAPP](http://www.itsecgames.com/) |
| **CodeReviewLab** | Hands-on secure code review challenges | Code review skills | [CodeReviewLab](https://www.codereviewlab.com/) |

### CTF Platforms & Challenges

| Platform | Description | Best For | Link |
|----------|-------------|----------|------|
| **HackSplaining** | Interactive lessons on vulnerabilities | **Fast interactive understanding** - perfect for learning concepts quickly | [HackSplaining](https://www.hacksplaining.com/lessons) |
| **PortSwigger Labs** | Real-world vulnerability labs | Hands-on exploitation practice | [PortSwigger Labs](https://portswigger.net/web-security/all-labs) |
| **OWASP Juice Shop** | Modern vulnerable web application | **BEST for OWASP Top 10** - Modern JavaScript, realistic scenarios | [Juice Shop](https://owasp.org/www-project-juice-shop/) |
| **PentesterLab** | Progressive web security exercises | Building skills step-by-step | [PentesterLab](https://pentesterlab.com/) |
| **TryHackMe Rooms** | Guided CTF challenges | Learning specific topics | [TryHackMe](https://tryhackme.com/) |
| **HackTheBox Machines** | Realistic penetration testing | Advanced practice | [HackTheBox](https://www.hackthebox.com/) |
| **HTB Academy Modules** | Structured learning paths | Comprehensive skill building | [HTB Academy](https://academy.hackthebox.com/) |

### Recommended Learning Path

| Week | Focus | Resources | Goal |
|------|-------|-----------|------|
| **1** | Quick Concept Understanding | [HackSplaining Lessons](https://www.hacksplaining.com/lessons) | Complete interactive lessons on major vulnerabilities |
| **2** | Burp Suite & Web Fundamentals | [PortSwigger Web Security Academy](https://portswigger.net/web-security) | Master Burp Suite basics |
| **3-4** | OWASP Top 10 (A01-A05) | [PortSwigger Labs](https://portswigger.net/web-security/all-labs), [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/) | Complete 20+ labs + Juice Shop challenges |
| **5-6** | OWASP Top 10 (A06-A10) | [PortSwigger Labs](https://portswigger.net/web-security/all-labs), [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/) | Complete remaining labs + Juice Shop challenges |
| **7-8** | API Security & GraphQL | [PortSwigger API Labs](https://portswigger.net/web-security/api-security) | Test REST & GraphQL APIs |
| **9-10** | Modern Attacks | [PortSwigger Labs](https://portswigger.net/web-security/all-labs) | Master advanced attacks |
| **11-12** | CTF Practice | [TryHackMe Web Path](https://tryhackme.com/path/outline/web), [PentesterLab](https://pentesterlab.com/) | Complete web security challenges |
| **13-14** | Python Scripting | [freeCodeCamp Python](https://www.youtube.com/watch?v=jS4aFq5-91M) | Build 5 pentesting tools |
| **15-16** | Linux & Networking | [TryHackMe Linux](https://tryhackme.com/room/linuxfundamentals) | Master Linux CLI |
| **17-18** | Advanced CTF Practice | [HackTheBox](https://www.hackthebox.com/), [HTB Academy](https://academy.hackthebox.com/) | Complete 10+ machines |

**Critical:** Start with [HackSplaining](https://www.hacksplaining.com/lessons) for quick interactive understanding, then dive deep with PortSwigger Labs and CTF platforms.

---

## Post-Exploitation & Privilege Escalation

**Critical:** Job descriptions require understanding of privilege escalation and lateral movement. This is fundamental to penetration testing.

### Linux Privilege Escalation

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **SUID Binaries** | Exploiting SUID permissions | [TryHackMe: Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) | [TryHackMe Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) |
| **Sudo Exploitation** | Abusing sudo permissions | [TryHackMe: Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) | [TryHackMe Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) |
| **Kernel Exploits** | Exploiting kernel vulnerabilities | [TryHackMe: Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) | [TryHackMe Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) |
| **Cron Jobs** | Exploiting scheduled tasks | [TryHackMe: Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) | [TryHackMe Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) |
| **PATH Hijacking** | Manipulating PATH variable | [TryHackMe: Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) | [TryHackMe Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) |
| **Capabilities** | Linux capabilities exploitation | [TryHackMe: Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) | [TryHackMe Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) |

### Windows Privilege Escalation

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **Windows Service Exploitation** | Abusing Windows services | [TryHackMe: Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) | [TryHackMe Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) |
| **Unquoted Service Paths** | Exploiting unquoted paths | [TryHackMe: Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) | [TryHackMe Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) |
| **Registry Exploitation** | Abusing registry permissions | [TryHackMe: Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) | [TryHackMe Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) |
| **Token Impersonation** | Impersonating tokens | [TryHackMe: Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) | [TryHackMe Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) |
| **AlwaysInstallElevated** | Exploiting installation permissions | [TryHackMe: Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) | [TryHackMe Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) |

### Lateral Movement

**Critical:** Moving through networks is a core pentesting skill mentioned in job descriptions.

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **Pass-the-Hash** | NTLM hash authentication | [TryHackMe: Active Directory](https://tryhackme.com/module/active-directory-basics) | [TryHackMe AD Rooms](https://tryhackme.com/module/active-directory-basics) |
| **Pass-the-Ticket** | Kerberos ticket attacks | [TryHackMe: Active Directory](https://tryhackme.com/module/active-directory-basics) | [TryHackMe AD Rooms](https://tryhackme.com/module/active-directory-basics) |
| **RDP Access** | Remote Desktop Protocol | [TryHackMe: RDP](https://tryhackme.com/) | [TryHackMe Rooms](https://tryhackme.com/) |
| **SMB Enumeration** | Server Message Block enumeration | [TryHackMe: SMB](https://tryhackme.com/room/smbrelay) | [TryHackMe SMB Rooms](https://tryhackme.com/) |
| **WinRM** | Windows Remote Management | [TryHackMe: WinRM](https://tryhackme.com/) | [TryHackMe Rooms](https://tryhackme.com/) |

### Post-Exploitation Tools

| Tool | Purpose | Best Tutorial | Practice |
|------|---------|---------------|----------|
| **LinPEAS** | Linux privilege escalation script | [LinPEAS GitHub](https://github.com/carlospolop/PEASS-ng) | [TryHackMe Linux PrivEsc](https://tryhackme.com/room/linuxprivesc) |
| **WinPEAS** | Windows privilege escalation script | [WinPEAS GitHub](https://github.com/carlospolop/PEASS-ng) | [TryHackMe Windows PrivEsc](https://tryhackme.com/room/windowsprivesc20) |
| **Mimikatz** | Windows credential extraction | [TryHackMe: Mimikatz](https://tryhackme.com/) | [TryHackMe AD Rooms](https://tryhackme.com/module/active-directory-basics) |
| **BloodHound** | Active Directory mapping | [TryHackMe: BloodHound](https://tryhackme.com/room/bloodhound) | [TryHackMe BloodHound](https://tryhackme.com/room/bloodhound) |

---

## Red Team Exercises & Security Audits

**Critical:** Job descriptions mention participating in red team exercises and security audits. This is real-world pentesting work.

### Red Team Fundamentals

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **Red Team vs Penetration Testing** | Understanding the difference | [TryHackMe: Red Team](https://tryhackme.com/) | [TryHackMe Red Team Path](https://tryhackme.com/path/outline/redteam) |
| **Adversary Simulation** | Simulating real attackers | [TryHackMe: Red Team](https://tryhackme.com/) | [TryHackMe Red Team Path](https://tryhackme.com/path/outline/redteam) |
| **Attack Chains** | Multi-stage attack scenarios | [TryHackMe: Red Team](https://tryhackme.com/) | [TryHackMe Red Team Path](https://tryhackme.com/path/outline/redteam) |
| **Persistence** | Maintaining access | [TryHackMe: Red Team](https://tryhackme.com/) | [TryHackMe Red Team Path](https://tryhackme.com/path/outline/redteam) |
| **Defense Evasion** | Avoiding detection | [TryHackMe: Red Team](https://tryhackme.com/) | [TryHackMe Red Team Path](https://tryhackme.com/path/outline/redteam) |

### Security Audit Skills

| Skill | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **Compliance Frameworks** | PCI-DSS, HIPAA, SOC 2 basics | [OWASP: Compliance](https://owasp.org/) | Review compliance requirements |
| **Security Policy Review** | Analyzing security policies | [OWASP: Security Policies](https://owasp.org/) | Review sample policies |
| **Risk Assessment** | Risk-based recommendations | [OWASP: Risk Assessment](https://owasp.org/) | Rate vulnerabilities by risk |
| **Gap Analysis** | Identifying security gaps | [OWASP: Gap Analysis](https://owasp.org/) | Perform gap analysis |

---

## Log Analysis & Monitoring

**Critical:** Job descriptions require log analysis skills. Understanding security logs is essential.

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **Linux Log Analysis** | syslog, journalctl, auth logs | [Linux Journey: Logs](https://linuxjourney.com/lesson/systemd) | Analyze system logs |
| **Windows Event Logs** | Event Viewer, security logs | [TryHackMe: Windows Logs](https://tryhackme.com/) | [TryHackMe Windows Rooms](https://tryhackme.com/) |
| **Web Server Logs** | Apache, Nginx access logs | [PortSwigger: Log Analysis](https://portswigger.net/web-security) | Analyze web logs |
| **Application Logs** | Application-specific logs | [OWASP: Logging](https://owasp.org/Top10/A09_2021-Security_Logging_and_Monitoring_Failures/) | Review application logs |
| **SIEM Basics** | Security Information and Event Management | [TryHackMe: SIEM](https://tryhackme.com/) | [TryHackMe SIEM Rooms](https://tryhackme.com/) |

---

## Social Engineering

**Critical:** Job descriptions mention social engineering as a critical skill. This is where AI tools fail and human expertise is essential.

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **Phishing** | Email-based attacks | [TryHackMe: Phishing](https://tryhackme.com/) | [TryHackMe Phishing Rooms](https://tryhackme.com/) |
| **Pretexting** | Creating false scenarios | [TryHackMe: Social Engineering](https://tryhackme.com/) | [TryHackMe Social Engineering](https://tryhackme.com/) |
| **OSINT** | Open Source Intelligence gathering | [TryHackMe: OSINT](https://tryhackme.com/room/ohsint) | [TryHackMe OSINT Rooms](https://tryhackme.com/) |
| **Reconnaissance** | Information gathering | [TryHackMe: Reconnaissance](https://tryhackme.com/) | [TryHackMe Recon Rooms](https://tryhackme.com/) |

---

## Certifications

### Entry-Level Pentesting Certifications

**Critical:** Job descriptions specifically mention these certifications. They're not always required, but they significantly boost your resume.

| Certification | Provider | Focus | Best Study Resource | Cost | Job Market Value |
|--------------|----------|-------|---------------------|------|------------------|
| **eJPT** | eLearnSecurity | Practical pentesting | [INE eJPT Course](https://ine.com/pages/ejpt) | ~$200 | ⭐⭐⭐ Entry-level standard |
| **CompTIA PenTest+** | CompTIA | General pentesting | [Professor Messer PenTest+](https://www.professormesser.com/security-plus/sy0-601/) | ~$392 | ⭐⭐⭐ Government/contractor jobs |
| **CEH** | EC-Council | Ethical hacking | [CEH Official Course](https://www.eccouncil.org/training/certified-ethical-hacker-ceh/) | ~$1,199 | ⭐⭐ Only if employer requires |
| **OSCP** | Offensive Security | Hands-on exploitation | [OffSec PWK Course](https://www.offensive-security.com/pwk-oscp/) | ~$1,499 | ⭐⭐⭐⭐⭐ Gold standard |
| **GPEN** | GIAC | Penetration testing | [SANS GPEN](https://www.sans.org/cyber-security-courses/penetration-testing-ethical-hacking/) | ~$7,000+ | ⭐⭐⭐⭐ High-value, expensive |

**Recommended Path:** 
1. **eJPT** - Start here (cheapest, practical, mentioned in job descriptions)
2. **OSCP** - Most respected, highest ROI
3. **GPEN** - If employer sponsors or you have budget
4. **CEH** - Only if explicitly required by employer

**Note:** Certifications are valuable but not everything. Hands-on experience (CTF labs, HackTheBox, PortSwigger) is equally important.

### Certification Study Resources

| Resource | Description | Link |
|----------|-------------|------|
| **PortSwigger Web Security Academy** | Free web security training | [Web Security Academy](https://portswigger.net/web-security) |
| **TryHackMe** | Guided learning paths | [TryHackMe](https://tryhackme.com/) |
| **HackTheBox** | Realistic pentesting practice | [HackTheBox](https://www.hackthebox.com/) |
| **Offensive Security Labs** | OSCP preparation | [OffSec Labs](https://www.offensive-security.com/labs/) |

---

## Penetration Testing Report Writing

**Critical Skill:** Finding vulnerabilities is only half the job. You MUST be able to write professional reports that clients understand.

### Report Structure

| Section | Description | Best Resource | Practice |
|---------|-------------|--------------|----------|
| **Executive Summary** | High-level overview for executives | [OWASP: Report Writing](https://owasp.org/www-project-web-security-testing-guide/) | Write executive summaries |
| **Methodology** | Testing approach and scope | [PTES: Methodology](http://www.pentest-standard.org/) | Document methodology |
| **Findings** | Detailed vulnerability descriptions | [PortSwigger: Writing Reports](https://portswigger.net/web-security) | Write vulnerability reports |
| **Remediation** | Fix recommendations | [OWASP: Remediation](https://owasp.org/www-project-web-security-testing-guide/) | Provide remediation steps |
| **Appendices** | Screenshots, proof of concept | [PTES: Reporting](http://www.pentest-standard.org/) | Create proof of concepts |

### Report Writing Tools

| Tool | Purpose | Link |
|------|---------|------|
| **Dradis** | Collaborative reporting platform | [Dradis Framework](https://dradisframework.com/) |
| **Serpico** | Penetration testing report generator | [Serpico](https://github.com/SerpicoProject/Serpico) |
| **LaTeX** | Professional document formatting | [LaTeX Templates](https://www.latex-templates.com/) |
| **Markdown** | Simple report formatting | [Markdown Guide](https://www.markdownguide.org/) |

### Report Writing Best Practices

**Critical:** Job descriptions emphasize communication skills. You must write for both technical and non-technical stakeholders.

- **Clear and Concise:** Write for non-technical audiences (executives, managers)
- **Evidence-Based:** Include screenshots, proof of concepts, logs
- **Actionable:** Provide specific remediation steps
- **Risk-Rated:** Categorize vulnerabilities by severity (Critical, High, Medium, Low)
- **Professional:** Use proper grammar and formatting
- **Stakeholder Communication:** Present findings to technical teams and executives
- **Collaboration:** Work with security engineers and developers on remediation

### Communication Skills

**Critical:** Job descriptions require strong communication skills. This is often overlooked but essential.

| Skill | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **Technical Writing** | Writing clear technical documentation | [OWASP: Report Writing](https://owasp.org/www-project-web-security-testing-guide/) | Write vulnerability reports |
| **Presentation Skills** | Presenting findings to stakeholders | [freeCodeCamp: Presentation Skills](https://www.youtube.com/watch?v=5e60OrA402M) | Present findings |
| **Stakeholder Management** | Working with clients and teams | [TryHackMe: Professional Skills](https://tryhackme.com/) | Practice client communication |
| **Documentation** | Documenting methodologies and findings | [PTES: Reporting](http://www.pentest-standard.org/) | Document everything |

---

## WAF Bypass Techniques

**Why This Matters:** Modern applications use Web Application Firewalls (WAFs). You MUST know how to bypass them.

### WAF Bypass Methods

| Technique | Description | Best Tutorial | Practice |
|-----------|-------------|---------------|----------|
| **Encoding Bypass** | URL encoding, Unicode, hex encoding | [PortSwigger: WAF Bypass](https://portswigger.net/web-security) | [PentesterLab: WAF Bypass](https://pentesterlab.com/) |
| **Comment Injection** | SQL comments to break WAF rules | [PortSwigger: SQL Injection](https://portswigger.net/web-security/sql-injection) | [PortSwigger SQLi Labs](https://portswigger.net/web-security/sql-injection) |
| **Case Variation** | Changing case to bypass filters | [PortSwigger: XSS](https://portswigger.net/web-security/cross-site-scripting) | [PortSwigger XSS Labs](https://portswigger.net/web-security/cross-site-scripting) |
| **Double Encoding** | Multiple layers of encoding | [OWASP: WAF Bypass](https://owasp.org/) | Practice encoding techniques |
| **Alternative HTTP Methods** | Using PUT, PATCH instead of POST | [PortSwigger: HTTP Methods](https://portswigger.net/web-security/http) | Test different HTTP methods |

---

## Cloud Security Basics (2025 Focus)

**Why This Matters:** Everything is moving to the cloud. AWS, Azure, GCP are everywhere. You need cloud security basics.

### Cloud Security Concepts

| Topic | Description | Best Tutorial | Practice |
|-------|-------------|---------------|----------|
| **AWS Basics** | EC2, S3, IAM fundamentals | [TryHackMe: AWS](https://tryhackme.com/module/aws-security) | [TryHackMe AWS Rooms](https://tryhackme.com/module/aws-security) |
| **Azure Basics** | Azure services, authentication | [TryHackMe: Azure](https://tryhackme.com/) | [TryHackMe Azure Rooms](https://tryhackme.com/) |
| **GCP Basics** | Google Cloud Platform basics | [TryHackMe: GCP](https://tryhackme.com/) | [TryHackMe GCP Rooms](https://tryhackme.com/) |
| **Cloud Misconfigurations** | Exposed buckets, public access | [PentesterLab: Cloud Security](https://pentesterlab.com/) | [PentesterLab Cloud Labs](https://pentesterlab.com/) |
| **Container Security** | Docker, Kubernetes basics | [TryHackMe: Docker](https://tryhackme.com/room/docker) | [TryHackMe Container Rooms](https://tryhackme.com/) |

**Note:** Deep cloud security comes in later levels. Here, focus on recognizing cloud deployments and basic misconfigurations.

---

## Skills Checklist

### Web Application Security
- [ ] Master Burp Suite (Proxy, Repeater, Intruder, Scanner, Collaborator)
- [ ] Understand HTTP protocol deeply (methods, headers, status codes)
- [ ] Can exploit all OWASP Top 10 vulnerabilities
- [ ] Can bypass WAFs and security controls
- [ ] Understand session management and authentication (JWT, OAuth, SAML)
- [ ] Can perform web application reconnaissance
- [ ] Understand API security (REST, GraphQL)
- [ ] Can test modern web attacks (Request Smuggling, Cache Poisoning, SSTI)

### Tools & Scripting
- [ ] Proficient with Linux command line
- [ ] Can write BASH scripts
- [ ] Can write Python scripts for pentesting
- [ ] Master Nmap and network scanning
- [ ] Understand Metasploit basics
- [ ] Basic coding proficiency (Codecademy for syntax mastery)
- [ ] Can solve basic LeetCode problems (for FAANG interviews)

### Practice & Experience
- [ ] Completed [HackSplaining interactive lessons](https://www.hacksplaining.com/lessons) for quick concept understanding
- [ ] Completed 50+ PortSwigger labs
- [ ] Completed [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/) challenges (modern vulnerable app)
- [ ] Completed TryHackMe beginner path
- [ ] Completed PentesterLab exercises
- [ ] Solved 10+ HackTheBox machines
- [ ] Built 5+ custom pentesting tools (Python scripts)
- [ ] Written detailed penetration test reports
- [ ] Tested REST APIs and GraphQL endpoints
- [ ] Exploited OWASP Top 10 (2024) vulnerabilities
- [ ] Performed web application reconnaissance

### AI & Automation Awareness
- [ ] Understand AI pentesting tools (RapidPen, VulnBot, HexStrike-AI)
- [ ] Know where AI excels (pattern matching, automation)
- [ ] Know where AI lacks (business logic, creative bypasses)
- [ ] Can use AI tools as force multipliers
- [ ] Focus on skills AI can't replace (logic flaws, social engineering)

### Vulnerability Assessment & Scanning
- [ ] Can use Nessus or OpenVAS for vulnerability scanning
- [ ] Understand automated scanning tools (Nuclei, Nikto)
- [ ] Can interpret scan results and prioritize findings
- [ ] Understand false positives vs real vulnerabilities
- [ ] Can perform manual verification of automated findings

### Post-Exploitation & Privilege Escalation
- [ ] Can perform Linux privilege escalation (SUID, sudo, kernel exploits)
- [ ] Can perform Windows privilege escalation (services, registry, tokens)
- [ ] Understand lateral movement techniques (Pass-the-Hash, RDP, SMB)
- [ ] Can use post-exploitation tools (LinPEAS, WinPEAS, Mimikatz)
- [ ] Understand Active Directory basics for lateral movement

### Networking Fundamentals
- [ ] Understand IP addressing and subnetting
- [ ] Can calculate subnets and CIDR notation
- [ ] Understand DNS, DHCP, and firewall configurations
- [ ] Can analyze network traffic with Wireshark
- [ ] Understand TCP/IP protocol stack

### Scripting & Automation
- [ ] Proficient in Python for pentesting automation
- [ ] Can write PowerShell scripts for Windows environments
- [ ] Can write BASH scripts for Linux automation
- [ ] Can build custom pentesting tools
- [ ] Understand when to automate vs manual testing

### Red Team & Security Audits
- [ ] Understand red team exercises vs penetration testing
- [ ] Can participate in security audits
- [ ] Understand compliance frameworks (PCI-DSS, HIPAA basics)
- [ ] Can perform risk assessments
- [ ] Understand gap analysis

### Log Analysis & Monitoring
- [ ] Can analyze Linux system logs (syslog, journalctl)
- [ ] Can analyze Windows Event Logs
- [ ] Can analyze web server logs (Apache, Nginx)
- [ ] Understand SIEM basics
- [ ] Can identify security events in logs

### Social Engineering & OSINT
- [ ] Understand phishing techniques
- [ ] Can perform OSINT gathering
- [ ] Understand pretexting and social engineering
- [ ] Can conduct reconnaissance
- [ ] Understand human psychology in security

### Communication & Professional Skills
- [ ] Can write professional penetration test reports
- [ ] Can present findings to technical and non-technical audiences
- [ ] Can collaborate with security engineers and developers
- [ ] Understand ethical considerations in pentesting
- [ ] Can document methodologies and findings

### API Security
- [ ] Understand REST API architecture
- [ ] Can test GraphQL endpoints
- [ ] Understand API authentication mechanisms
- [ ] Can identify API vulnerabilities
- [ ] Can bypass API rate limiting

### Report Writing
- [ ] Can write executive summaries
- [ ] Can document vulnerabilities clearly
- [ ] Can provide remediation recommendations
- [ ] Can create proof of concepts
- [ ] Understand risk rating methodologies

---

## Next Steps

Once you've mastered this level, you're ready for **[x02_Associate](https://github.com/Kennyslaboratory/Ultimate-Hacker-Roadmap/tree/main/x02_Associate)** where you'll dive into binary exploitation, mobile security, and advanced techniques!

**Remember:** Focus 80% of your time on web application security. That's where the jobs are in 2025.

**Key Takeaways:**
- **[HackSplaining](https://www.hacksplaining.com/lessons)** - Start here for quick interactive understanding of vulnerabilities
- **PortSwigger Web Security Academy** is your #1 resource - it's free and comprehensive
- **[OWASP Juice Shop](https://owasp.org/www-project-juice-shop/)** - BEST modern vulnerable app for learning OWASP Top 10. Modern JavaScript, realistic scenarios.
- **CTF Labs are critical** - [PentesterLab](https://pentesterlab.com/), [PortSwigger Labs](https://portswigger.net/web-security/all-labs), [HTB Academy](https://academy.hackthebox.com/)
- **AI is changing the game** - Understand RapidPen, VulnBot, HexStrike-AI. Know where AI excels and where human expertise is critical
- **Vulnerability scanners are required** - Learn Nessus, OpenVAS, Nuclei. Job descriptions require this.
- **Privilege escalation is fundamental** - Linux and Windows priv esc are core skills mentioned in every job description
- **Networking fundamentals are critical** - IP addressing, subnetting, DNS, DHCP, firewalls are MUST KNOW
- **Scripting is essential** - Python and PowerShell are mentioned in every job description
- **Communication skills matter** - You must write reports and present to both technical and non-technical stakeholders
- **Build tools** - Write Python scripts to automate tasks
- **Practice daily** - Complete at least 1 PortSwigger lab per day
- **Document everything** - Learn to write professional reports
- **API security is critical** - Modern apps are API-first
- **Focus on what AI can't do** - Business logic flaws, creative bypasses, social engineering
- **Red team exercises** - Understand adversary simulation and security audits
- **Certifications help** - eJPT and OSCP are mentioned in job descriptions

---

**Last Updated:** January 2025  
**Author:** Kenneth Kasuba  
**Feedback:** [GitHub Issues](https://github.com/Kennyslaboratory/Ultimate-Hacker-Roadmap/issues)
