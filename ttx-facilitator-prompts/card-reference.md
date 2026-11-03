# Backdoors & Breaches Card Reference

This is the same Card Reference embedded at the end of each facilitator prompt in this folder, provided on its own for platforms that need the prompt split. Keep it in sync with the embedded copies when decks change.

Card names only. The effect of each Inject and Consultant card is not listed: improvise an effect that fits the card's name, and state it plainly when it happens.

**Call a Consultant:** On a success, draw a random Consultant from the selected decks. If the user has supplied that card's text, use it. Otherwise grant a one-time +3 on the team's next roll, and narrate the help without attributing quotes or specific claims to the real person.

**Core Deck (V3.1)**
* *Initial Compromise:* Credential Stuffing; Exploitable External Service; Bring Your Own (Exploited) Device; Social Engineering; Compromised Trusted Relationship; External Password Spray; Insider Threat; Compromised Web Server; External Cloud Access; Phish
* *Pivot and Escalate:* Local Privilege Escalation; New Service Creation/Modification; Credential Harvesting; Kerberoasting; Broadcast/Multicast Protocol Poisoning; Weaponizing Active Directory
* *C2 and Exfil:* HTTP as Exfil; HTTPS as Exfil; DNS as C2; Windows Background Intelligent Transfer Service (BITS); Cloud-Based Services as Exfil; Domain Fronting as C2
* *Persistence:* Accessibility Features; Malicious Firmware; Logon Scripts; Malicious Browser Plugins; Application Shimming; New User Added; Malicious Driver; Dynamic Link Library Hijacking; Malicious Service
* *Procedures:* Endpoint Analysis; User and Entity Behavior Analytics (UEBA); Server Analysis; Firewall Log Review; Crisis Management; Netflow, Zeek/Bro, and RITA Analysis; SIEM Log Analysis; Isolation; Endpoint Security Protection Analysis; Memory Analysis; Cyber Deception; Permissions Audit; Cloud Event Log Analysis
* *Injects:* It Was a Pentest; Data Uploaded to Pastebin; SIEM Analyst Returns from Splunk Training; Analyst Returns from IR Training; Bobby the Intern Kills the System You Are Reviewing; Legal Takes Your Only Skilled Handler Into a Meeting to Explain the Incident; Policy? What Policy?; Luck of the SOC

**Expansion Deck**
* *Initial Compromise:* Physical Access; Supply Chain Attack; Missing HTTP Strict Transport Security (HSTS) Protection
* *Pivot and Escalate:* Access Token Manipulation; SMB Weakness; Internal Spearphishing; Cleartext Passwords in Files; Stale Network Address Configuration (SNAC) Attack
* *C2 and Exfil:* Exfil over Physical Medium
* *Persistence:* Malware Injection Into Client Software; Malicious Email Rules; Windows Recovery Service; Registry Key Persistence; Event Triggered Malware
* *Procedures:* Physical Security Review; Call a Consultant
* *Injects:* same as Core
* *Consultants:* Jorge Orchilles; Robert M. Lee; Alethe Denis; Eric Conrad; Chloé Messdaghi; Marcus J. Carey; Tim Medin; Alissa Torres; Deter Smith; Chris Benton; Richard Meno; Richard Phung

**Huntress (V1.1)**
* *Initial Compromise:* Public Facing Database Compromise; Fake Software Update; Exchange Zero-Day Vulnerability Exploit; Embedded Remote Access Trojan (RAT); .NET Deserialization Exploit
* *Pivot and Escalate:* Unpatched Critical Security Update; Malware Propagation; LDAP Bind Credential Theft
* *C2 and Exfil:* Clipboard Scrape; Rotating C2 Server Location
* *Persistence:* Hiding in Plain Sight; Registry Modification; Living off the Land; WMI Events
* *Procedures:* Call a Consultant
* *Injects:* Major Failure Alert; Let's Rock; Read to the End; That Was a Bad Idea; Back to Basics; Ignore Those Pesky Open Ports; Rookie Mistake; Risk Accepted; A Little Help From My Friends; Knowledge Is Power; Haste Makes Waste; A Bad Day Made Worse; Alert Fatigue Is Real; Security Training For The Win
* *Consultants:* Jamie Levy; John Hammond; Harlan Carvey; Cat Contillo; Mathew Brennan; Kyle Hanslovan; Jai Minton; Dray Agha

**Densecure**
* *Initial Compromise:* Publicly Exposed Secret Key; Trojan Mail; HTML Smuggling; Vendor Default Credentials Attack; Wi-Fi Guest Network Escape; Microsoft Direct Send Phishing; Vishing
* *Pivot and Escalate:* Default Administrator Credentials; Insecure Internet of Things (IoT); Decrypting LSA Secrets; Dumping LSASS Via Task Manager; NTLM Abuse; Misconfigured Certificate Template; SUID Permissions Abuse
* *C2 and Exfil:* Bluetooth as Exfil; Unauthorized Filesharing Utility; Hosted Note Taking as C2; Misuse of Remote Access Software
* *Persistence:* Machine Account Quota (MAQ) Abuse; Group Policy Object (GPO) Modification; Golden Ticket Attack; Screensaver Hijack; SSH Authorized Keys Modification
* *Procedures:* Cloud Event Log Analysis; Permissions Audit
* *Injects:* Crank Up the Pressure; Executive Buy-In; Dude, Where's My Server?; It's a Feature, Not a Bug; Timber!; Water, Water Everywhere!; Way to Plan Ahead; Communication Infrastructure DDoS

**Red Canary**
* *Initial Compromise:* Gatekeeper Bypass; Obfuscated Payload Delivery; Compiled After Delivery; RFID Theft; USB Drive-By
* *Pivot and Escalate:* Lateral Tool Transfer; Application Control Bypass; Disabling Windows Defender; Process Injection; PsExec Abuse; LSASS Credential Dump; Read/Write CHMOD 777
* *C2 and Exfil:* Cloud Service as Exfil; Authorized Remote Tools; Malicious Access Point; Bluetooth as Exfil
* *Persistence:* Spawn Web Shell; Scheduled Task; Event-Triggered Execution; Rename Process
* *Procedures:* Physical Security Review; Call a Consultant
* *Injects:* Cat on Keyboard Deletes Production Database; Nuclear Test Site; Deez Registry Keyz Plz; Quishing; Undocumented System; Missed Payday; Not a Red Team; Sneaky Sneaky RAT
* *Consultants:* Mike Haag; Adam Mashinchi; Carrie Roberts

**Trimarc**
* *Initial Compromise:* AI-Generated Script; Forest Trusts; SSO Provider Compromise; Weaponized Hardware Security Key; Compromised Virtual Host; Corrupted Employee; Malicious Extension
* *Pivot and Escalate:* vCenter Console Coercion; Overprivileged Cloud Application; Passwords in AD Attribute; Overprivileged Group Policy/High Profile (GPO); Misconfigured Certificate Templates (ESC1); Golden Ticket Attack; Server Management Compromise
* *C2 and Exfil:* Living Off Trusted Sites (LOTS); GIFs as C2
* *Persistence:* Cloud Application Impersonation; AdminSDHolder Rights Modification
* *Procedures:* Cloud Event Log Analysis; Call a Consultant; Permissions Audit
* *Injects:* Bear vs. Powerstation; Product Trials and Tribulations; Peekaboo; Click, Click, Boom!; Dude, Where's Our Docs?; Trimarc123!; DiscountConsultant.lol; Ghosted by AV
* *Consultants:* Jake Hildreth; Dev Badlu; Sean Metcalf; Brandon Colley

**Datadog**
* *Initial Compromise:* Exposed Cloud Credentials via Unauthenticated Kubernetes Dashboard; Cloud Application Compromise; Backdoored Software Supply Chain; GitHub Action Compromise; Confused Deputy Attack; Cloud-Native Serverless Function Compromised; Poisoned Cloud Image Supply Chain; Compromised Single Sign-On (SSO) Federated Identity
* *Pivot and Escalate:* Identity and Access Management (IAM) Policy Abuse; Credential Store Compromise; Instance Metadata Service (IMDS) Access; Kubernetes Service Account PrivEsc; Instance Takeover via User Data; Credentials Exposed in Storage Bucket
* *C2 and Exfil:* Software as a Service (SaaS) Tunneling Virtual Private Network (VPN) as C2; Snapshotting Resources as Exfil; Living Off the Cloud as Exfil
* *Persistence:* Backdoored Role Trust Policy; Cloned Kubernetes Credentials; Additional Credential Creation; Backdoored Container Image
* *Procedures:* Software Bill of Materials (SBOM) Analysis; Workload Protection; Cloud Identity and Entitlement Management (CIEM); Cloud SIEM Log Analysis; Application Runtime Analysis
* *Injects:* Third-Party Code Library Compromised; Exposed SaaS API Key During Public Presentation; Public Storage Bucket Exposed; Supply Chain Firewall; IMDSv2 Project Complete; Cloud Security Training; Attacker Stops Cloud Logging; Undocumented APIs

**NRECA**
* *Initial Compromise:* Wardriving; Malicious QR Code; Compromised Advanced Metering Infrastructure (AMI); Stolen Corporate Laptop; Burglarized Rural Substations; Imposter IT Worker; Post End-of-Life Exploitation (Unpatched System)
* *Pivot and Escalate:* Account Abuse; User Token Theft; Trusted Connection Abuse
* *C2 and Exfil:* none listed; if NRECA is the only deck in play, draw this card from Core
* *Persistence:* Remote Management Abuse; Hardware Compromise; Supervisory Control and Data Acquisition (SCADA) Breach; Data Historian Compromise; Shadow IT Compromise; Tool Masquerade; Vendor Account Misuse; Temporary Permanence
* *Procedures:* Call a Consultant; Protocol Analysis
* *Injects:* Storm Duty; Panic in the Streets; Coordinated Campaign; A Seat at the Table; Watch Out Below; Chuckles, I'm in Danger; Meth House Meltdown; Wipe Better; Business Email Compromise
* *Consultants:* Cyber Mutual Assistance (CMA); Morale Suppression Team

**glueck kanja**
* *Initial Compromise:* Compromised VPN Appliance; Password Manager Compromise; Flood and Helpdesk Hook; Conditional Access Bypass; Device Code Phishing; Adversary in the Middle
* *Pivot and Escalate:* Overprivileged Vendor Requirement; Azure Arc to Domain Admin; Entra ID Connect Account Compromise; Compromised Application Owner
* *C2 and Exfil:* Azure Blob Storage as Exfil; Insecure Default Configuration as Exfil; Alternative Protocol as Exfil
* *Persistence:* Azure Lighthouse Backdoor; Added Credentials to Service Principal; Compromised Privileged Workload Identity
* *Procedures:* glueck kanja Prevention Service; Call a Consultant; Advanced Hunting (this deck's name for Endpoint Analysis); Live Response Analysis (this deck's name for Endpoint Security Protection Analysis)
* *Injects:* XDR Coverage?; Works Council; Cloud Crashed; Faulty Signature by Old EDR; Who's That Anonymous Caller?; Cyber Insurance Wants a Report; All Hands on Deck; glueck kanja Prevention Service; Automation Closed All Alerts
* *Consultants:* Jonas Ripperger; Fabian Bader; Christopher Brumm; Thomas Naunheim; Thorsten Kunzi
