# SOC-Automation-Home-Lab

## Objective
[Brief Objective - Remove this afterwards]

The Detection Lab project aimed to establish a controlled environment for simulating and detecting cyber attacks. The primary focus was to ingest and analyze logs within a Security Information and Event Management (SIEM) system, generating test telemetry to mimic real-world attack scenarios. This hands-on experience was designed to deepen understanding of network security, attack patterns, and defensive strategies.

### Skills Learned
[Bullet Points - Remove this afterwards]

- Advanced understanding of SIEM concepts and practical application.
- Proficiency in analyzing and interpreting network logs.
- Ability to generate and recognize attack signatures and patterns.
- Enhanced knowledge of network protocols and security vulnerabilities.
- Development of critical thinking and problem-solving skills in cybersecurity.

### Tools Used
[Bullet Points - Remove this afterwards]

- Security Information and Event Management (SIEM) system for log ingestion and analysis.
- Network analysis tools (such as Wireshark) for capturing and examining network traffic.
- Telemetry generation tools to create realistic network traffic and attack scenarios.

## Steps
## Steps
drag & drop screenshots here or use imgur and reference them using imgsrc

Every screenshot should have some text explaining what the screenshot is about.

Example below.

*Ref 1: Network Diagram*  
![Network Diagram](https://i.imgur.com/placeholder.png)

---

*Ref 2: Logical Diagram (Day 1)*  
![Logical Diagram](https://i.imgur.com/placeholder.png)  
This diagram outlines the full architecture of my SOC Automation Lab. It shows how Wazuh ingests telemetry, how alerts flow into Shuffle for orchestration, and how cases are created in TheHive. Designing this helped me visualize the lab before deployment and ensured each component had clear communication paths.

---

*Ref 3: Cloud Deployment Setup (Day 2)*  
![Cloud Deployment](https://i.imgur.com/placeholder.png)  
This screenshot shows the cloud virtual machine configuration used to deploy Wazuh, Shuffle, and TheHive. Security groups and network rules were configured to allow SOC tools to communicate securely and simulate realistic SOC infrastructure.

---

*Ref 4: Wazuh Agent Connection (Day 3)*  
![Wazuh Agents](https://i.imgur.com/placeholder.png)  
This screenshot displays the Wazuh dashboard with connected agents. It confirms that telemetry from the endpoint is successfully being ingested by the SIEM and that the agent installation and communication pipeline are functioning correctly.

---

*Ref 5: API Connections Between Wazuh, Shuffle, and TheHive (Day 3)*  
![API Connections](https://i.imgur.com/placeholder.png)  
This screenshot verifies that API connections were successfully established between all tools. These integrations enable automated alert forwarding, enrichment, and case creation across the SOC stack.

---

*Ref 6: Mimikatz Telemetry Simulation (Day 4)*  
![Mimikatz Telemetry](https://i.imgur.com/placeholder.png)  
This screenshot shows the telemetry generated from a simulated credential extraction attempt. Wazuh recorded and processed the suspicious activity, validating the SIEM’s ability to detect malicious behavior.

---

*Ref 7: Wazuh Alert Triggered (Day 4)*  
![Wazuh Alert](https://i.imgur.com/placeholder.png)  
This screenshot captures the Wazuh alert triggered by the simulated Mimikatz activity. It demonstrates the SIEM’s detection capability and confirms that rules and decoders are properly configured.

---

*Ref 8: Shuffle SOAR Workflow (Day 5)*  
![Shuffle Workflow](https://i.imgur.com/placeholder.png)  
This screenshot shows the Shuffle SOAR workflow used to automate the alert-handling process. The workflow enriches incoming Wazuh alerts, forwards them to TheHive, and triggers an analyst notification.

---

*Ref 9: Auto-Generated Case in TheHive (Day 5)*  
![TheHive Case](https://i.imgur.com/placeholder.png)  
This screenshot shows the automatically created case in TheHive after Shuffle processed the alert. This demonstrates end-to-end SOC automation: detection → enrichment → case creation.

---

*Ref 10: Automated Email Notification (Day 5)*  
![Email Notification](https://i.imgur.com/placeholder.png)  
This screenshot displays the automated email sent by Shuffle whenever a high-severity alert is converted into a case. 

---

*Ref 11: Troubleshooting & Fixes*  
![Troubleshooting](https://i.imgur.com/placeholder.png)  
This section contains screenshots of errors encountered during the lab setup and the solutions applied. 
