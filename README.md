# Security-Setup-In-Organization
Initial security steps to be taken care while setting up the security environment for an Organization.

# Reconnaissance
Reconnaissance is the act of gathering different kinds of information against the targeted victim or system. There are various tools, techniques, and websites,
including public sources such as Whois, nslookup that can help attacker to gather information.

# Weakness you look for during reconnaissance
Application detailed error message,Application components information along with version disclosure, subdomains information, public git respository, any path discloure in soure code or in error message which is revealing information about application.

# Session Management 
Session management refers to the process of securely handling multiple requests to a web-based application or service from a single user or entity. Websites and browsers use HTTP to communicate, and a session is a series of HTTP requests and transactions initiated by the same user.

# Weaknesses during session establisment between client and server
Session hijacking, session fixation, session replay attack, concurrent session, session puzzling attack etc. , which allow an attacker to compromise your application account or gain unauthorized access to your data.

# Authentication
Broken authentication attacks aim to take over one or more accounts giving the attacker the same privileges as the attacked user. Authentication is “broken” when attackers are able to compromise passwords, keys or session tokens, user account information, and other details to assume user identities.

# Weaknesses during authentication process
Authentication bypass using sql injection, Authentication bypass using forceful browsing, MFA bypass, Token verification bypass, compromise password and keys which are associated with user account.

# Authorization
Authorization is the concept of allowing access to resources only to those permitted to use them. Testing for Authorization means understanding how the authorization process works, and using that information to circumvent the authorization mechanism.

# Weaknesses during authorization process
Privilege escalation, Authorization bypass, Indirect Object Reference, Role based access bypass, Password recovery flow bypass etc. These are attackes which could lead to full user account takeover. 

# Data Validation Testing 
Input validation is performed to ensure only properly formed data is entering the workflow in an information system, preventing malformed data from persisting in the database and triggering malfunction of various downstream components. Input validation should happen as early as possible in the data flow, preferably as soon as the data is received from the external party.

Data from all potentially untrusted sources should be subject to input validation, including not only Internet-facing web clients but also backend feeds over extranets, from suppliers, partners, vendors or regulators, each of which may be compromised on their own and start sending malformed data.

# Weaknesses during data validation
Cross site scripting (XSS), Cross site Request Forgery (CSRF), Server side Request Forgery (SSRF), HTML Injection, Local File Inclusion, Remote File Inclusion, Template Injection, Parameter Tampering etc. These attacks could lead to compromise our system and can have access to internal system information.

# Component Testing
Components, such as libraries, frameworks, and other software modules, run with the same privileges as the application. If a vulnerable component is exploited, such an attack can facilitate serious data loss or server takeover. Applications and APIs using components with known vulnerabilities may undermine application defenses and enable various attacks and impacts.

# Weaknesses during in use components
Testing against outdated  and third party components which has some known vulnerabiltites could lead to different attack like xss, sensitive information disclosure etc within the application.

# Denial of Service
A denial-of-service (DoS) attack occurs when legitimate users are unable to access information systems, devices, or other network resources due to the actions of a malicious cyber threat actor.

# Weaknesses during handling multiple request at a time
Certain test cases needs to be follow to check if your application is exposed to DoS attack are given below: 
  
    1.Checking race conditions
    2.Passing long range inputs and check response time
    3.Components Vulnerable to publicly available Dos Exploits
    
# Web API End Points
All the End points which will be consumed by Product (Application) will be part of testing against various attack.

# Weaknesses in consuming API end points
All the End points which will be consumed by the application should have proper security checks and not vulnerable to below attacks: 

    1.XXE (XML External Entity Attack)
    2.Rate limiting attack
    3.Schema validation
    4.Injection attacks etc.
    
# Database Testing
Database security testing is done to find the loopholes in security mechanisms and also about finding the vulnerabilities or weaknesses of database system. Security testing defines a way to identify potential vulnerabilities effectively, when performed regularly.

# Weaknesses during database setup or maintaining it 
Database should be in protected environment, encryption and hashing flow neesds to check during storage of data etc.

# Security Misconfiguration
Security misconfiguration is the most commonly seen issue. This is commonly a result of insecure default configurations, incomplete or ad hoc configurations, open cloud storage, misconfigured HTTP headers, and verbose error messages containing sensitive information. Not only must all operating systems, frameworks, libraries, and applications be securely configured, but they must be patched/upgraded in a timely fashion.

# Weaknesses during setting up application environment safely - check if there is any misconfiguration in available options
All the Security Headers and their configuration needs to be check before deploying the application. Also, In addition to that, any framework/Libraries should not be misconfiguared at any stage.

# SSL Testing 
Testing against SSL Implementation throughout the application.

# Weaknesses during SSL Implementation
Some Knows vulnerabilties related to SSL where we give more attention to manage our SSL implementation securely-

    1.Insecure weak ciphers
    2.SSL Certificate
    3.Insecure Protocols (SSLv2, SSLv3, TLSv1.0 and TLSv1.2)
    4.Test for Heartbleed attack
    5.Test for BEAST attack
    6.SSL Renegotiation
    7.Testing for known vulnerabilties against SSL implementation throughout the application.
    
# Insufficient Logging & Monitoring
Exploitation of insufficient logging and monitoring is the bedrock of nearly every major incident. Attackers rely on the lack of monitoring and timely response to achieve their goals without being detected. This issue is included in the Top 10 based on an industry survey.
One strategy for determining if you have sufficient monitoring is to examine the logs following penetration testing. The testers’ actions should be recorded sufficiently to understand what damages they may have inflicted.

# Weakness in logging our system data
Vulnerabilities likes insufficient logging which stored sensitive informaiton i.e. key values, tokens, passwords,internal system paths, card information etc.



