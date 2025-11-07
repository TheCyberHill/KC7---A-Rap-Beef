# KC7---A-Rap-Beef

🕵️ KC7 Cyber Threat Investigation — Case A: A Rap Beef
📘 Scenario
Two rival hip-hop artists, Dwake (OWL Records) and Present (Dollar Currency Records), escalate their feud into cyberspace. After Dwake overshares personal details in a diss track, Present’s label hires a hacker to exploit those details and compromise Dwake’s accounts.
You are a Security Analyst at OWL Records, tasked with investigating the breach using Kusto Query Language (KQL) across multiple datasets.

🔍 Investigation Highlights
- Reconnaissance: Hacker probes OWL Records’ website using IP 18.66.52[.]227 to gather Dwake’s personal info.
- Password Reset Exploit: Dwake’s lyrics reveal answers to challenge questions (e.g., pet name, street name), enabling account takeover.
- Credential Theft: Hacker resets Dwake’s email and Instagram passwords, posts embarrassing content.
- Phishing Campaign: Domain betterlyrics4u[.]com linked to targeted spear-phishing emails sent to OWL Records artists.
- Email Analysis: Used PassiveDNS and email logs to identify phishing sender, targeted roles, and subject lines.
- Network Events: Tracked outbound GET requests and confirmed Dwake clicked the phishing link.
- Authentication Logs: Verified successful login from attacker’s IP.
- Data Exfiltration: Found evidence of zip file downloads tied to Dwake’s account

🛠️ Tools & Skills Demonstrated
- KQL (Kusto Query Language) for log analysis
- Threat hunting across PassiveDNS, Email, AuthenticationEvents, and NetworkEvents tables
- Phishing detection and domain/IP correlation
- OPSEC awareness and social engineering analysis
- MITRE ATT&CK mapping (implied through adversary behavior)

📘 Lessons Learned
- Public personas can leak sensitive info exploitable via social engineering.
- Phishing campaigns often target high-profile individuals with tailored bait.
- KQL is a powerful tool for pivoting across datasets and uncovering attacker behavior.
- Cybersecurity requires both technical skill and awareness of human vulnerabilities.
