# NIST 800-61 (Computer Security Incident Handling Guide)
### My summary of the core concepts in ["NIST SP 800-61 revision 2"](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf)  for Incident Responders 


![image](https://github.com/user-attachments/assets/78a01b7d-24dc-462e-aed1-0ea1a468cc56)




# Phase 1 (Preparation) = 🛡️

Prepare to = detect, respond to, and recover from incidents

	• Create IR Policy
	• Build IR Team
	• Deploy Security Tools + Infrastructure
	• Run IR Exercises

##  Create Incident Response Policy :
1) what qualifies as incident ?
2) who is responsible for handling incidents ?
3) Outlines steps for ----> reporting, escalating, and resolving incidents

##  Build Incident Response Team (IRT) :
SOC , Forensic , IT Support , Legal , Management

##  Deploy Security Tools + Infrastructure :
1) SIEM (Splunk) ----> Logs & alerts
2) IDS/IPS (Suricata) ----> Intrusion detection 
3) Endpoint Protection (AV) ----> Detects malware
4) Network Monitoring (Zeek) ----> Traffic analysis

##  Run Incident Response Exercises :
1) Tabletop Exercises ----> Simulate an incident and test team response
2) Red Team & Blue Team Ops ----> Offensive team attacks, defensive team defends

------------------------------------------------------------------------------------------------------------------------
# Phase 2 (Detection & Analysis) = ⚠️

Identify and analyze security incidents ASAP

	• Detecting an Incident (Signs of Compromise)
	• Classifying Incidents
	• Analyzing the Scope & Impact


##  Detecting an Incident :
1) Network Indicators ----> High outbound traffic, unusual DNS requests , ...
2) Host Indicators ----> Unexpected file changes, privilege escalation attempts
3) User Indicators ----> Abnormal logins, failed password attempts

##  Classifying Incidents :
Unauthorized Access , Mal , DoS , Insider , ...


##  Analyzing the Scope & Impact :
What systems are affected?

What data is at risk?

Is the attack spreading?

--------------------------------------------------------------------------------------------------------
# Phase 3 (Containment, Eradication, Recovery) = 🛑

Once an incident is detected, the organization must : 

a) limit the damage (containment)

b) remove the threat (eradication)

c) restore affected systems and data (recovery)

##  Containment: Stopping the Spread 
**Why?** Prevent attackers from gaining more access or causing more damage

*Short-Term Containment* :
1) Disconnect affected machines from the network
2) Block attacker IP addresses at the firewall
3) Kill malicious processes using EDR

*Long-Term Containment* :
1) Apply patches and updates to vulnerable system
2) Change compromised passwords
3) Implement network segmentation to isolate affected areas


##  Eradication: Removing the Threat
**Why?** After containment, the root cause must be eliminated to prevent reinfection

1) Identify RootCause ----> What vulnerability did the attacker exploit?
2) Remove malware using tools
3) Delete backdoors
4) Patch systems
5) Enhance organization security



##  Recovery: Restoring Systems to Normal
**Why?** After removing the threat, affected systems must be safely restored to full operation

1) Restore from Clean Backups
2) Rebuild Affected Systems
3) Verify Everything is Fixed ---->  Conduct penetration testing to check if attackers can return

----------------------------------------------------------------------------------------------------------------------------------------

# Phase 4 (Post-Incident Activity) = 📖

After handling an incident, analyze what happened, improve defenses, and prevent future attack

##  Conduct a Post-Incident Review :
1) How did the attack start? ----> Phishing, unpatched vulnerability, insider threat?
2) What security gaps did the attacker exploit?
3) Did we detect and respond fast enough?
4) How can we prevent this from happening again?

##  Update Policies & Playbooks :
1) Adjust SIEM rules ----> to detect attack patterns
2) Improve escalation procedures ----> Who needs to be informed and when?
3) Review forensic procedures
4) Add new containment methods ----> like faster isolation


##  Improve Security Measures :
1) Stronger Network Segmentation ----> Prevent malware from spreading
2) MFA
3) Endpoint Detection
4) TI feeds


##  Share Findings & Train Teams :
1) Teach SOC analysts about the attack
2) Educate IT teams on securing systems better
3) Share findings with other companies (if legal)


------------------------------------------------------------------------------------------------------------------------------

#### for better understanding : Mapping an IR Framework to a fictional heist movie


The museum uses lasers, motion sensors, and security drills to protect the Phoenix Diamond :

	( "Preparation" : Strong security helps stop threats before they happen )

A security camera turns off, and a guard is missing. Security realizes someone has broken in :

	( "Identification" : Detecting unusual activity is the first step in handling an incident )

Alarms go off, exits lock, and extra guards arrive to stop the thief :

	( "Containment" : Keeping the attacker from causing more damage )

The thief is trapped, and security removes any hacking tools or helpers :

	( "Eradication" : Getting rid of all threats to restore safety )

Security fixes cameras, upgrades alarms, and returns to normal :

	( "Recovery" : Repairing systems and making security stronger )

The team studies what happened, finds weaknesses, and improves security :

	( "Lessons Learned" : Understanding the incident to prevent future attacks )



























