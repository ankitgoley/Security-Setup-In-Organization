# Security-Setup-In-Organization
Initial security steps to be taken care while setting up the security environment for an Organization.

# Reconnaissance
Reconnaissance is the act of gathering different kinds of information against the targeted victim or system. There are various tools, techniques, and websites,
including public sources such as Whois, nslookup that can help attacker to gather information.

# Weakness you look for during reconnaissance
Application detailed error message,Application components information along with version disclosure, subdomains information, public git respository, any path discloure in soure code or in error message which is revealing information about application.

# Session Management 
Session management refers to the process of securely handling multiple requests to a web-based application or service from a single user or entity. Websites and browsers use HTTP to communicate, and a session is a series of HTTP requests and transactions initiated by the same user.

# Weakness you look for during session establisment between client and server
Session hijacking, session fixation, session replay attack, concurrent session, session puzzling attack etc. , which allow an attacker to compromise your application account or gain unauthorized access to your data.

# Authentication
Broken authentication attacks aim to take over one or more accounts giving the attacker the same privileges as the attacked user. Authentication is “broken” when attackers are able to compromise passwords, keys or session tokens, user account information, and other details to assume user identities.

# Weakness you look for during authentication
Authentication bypass using sql injection, Authentication bypass using forceful browsing, MFA bypass, Token verification bypass, compromise password and keys which are associated with user account.
