# NIST 800-61 (Computer Security Incident Handling Guide)
My summary of the core concepts in "NIST SP 800-61 revision 2"  for Incident Responders 


## Phase 1 (Preparation) 🚀

Prepare the organization to detect, respond to, and recover from incidents

	• Create an Incident Response Policy
	• Build an Incident Response Team
	• Deploy Security Tools & Infrastructure
	• Run Incident Response Exercises

### 🚀 Create an Incident Response Policy :
1) Defines what qualifies as an incident
2) Specifies who is responsible for handling incidents
3) Outlines steps for reporting, escalating, and resolving incidents

### 🚀 Build an Incident Response Team (IRT) :
SOC , Forensic , IT Support , Legal , Management

### 🚀 Deploy Security Tools & Infrastructure :
1) SIEM (Splunk) ----> Logs & alerts
2) IDS/IPS (Suricata) ----> Intrusion detection 
3) Endpoint Protection (AV) ----> Detects malware
4) Network Monitoring (Zeek) ----> Traffic analysis

### 🚀 Run Incident Response Exercises :
1) Tabletop Exercises : Simulate an incident and test team response
2) Red Team & Blue Team Ops : Offensive team attacks, defensive team defends

------------------------------------------------------------------------------------------------------------------------
## Phase 2 (Detection & Analysis) 🔍

Identify and analyze security incidents as quickly and accurately as possible

	• Detecting an Incident (Signs of Compromise)
	• Classifying Incidents
	• Analyzing the Scope & Impact


### 🔍 Detecting an Incident :
1) Network Indicators ----> High outbound traffic, unusual DNS requests , ...
2) Host Indicators ----> Unexpected file changes, privilege escalation attempts
3) User Indicators ----> Abnormal logins, failed password attempts

### 🔍 Classifying Incidents :
Unauthorized Access , Mal , DoS , Insider , ...




### 🔍 Analyzing the Scope & Impact :
What systems are affected?

What data is at risk?

Is the attack spreading?

--------------------------------------------------------------------------------------------------------
## Phase 3 (Containment, Eradication, and Recovery) 🔧

Once an incident is detected, the organization must : 

a) limit the damage (containment)

b) remove the threat (eradication)

c) restore normal operations (recovery)












