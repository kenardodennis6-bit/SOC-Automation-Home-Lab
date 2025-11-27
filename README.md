# SOC-Automation-Home-Lab

## Objective
For this project, I created a small SOC environment from scratch and automated the whole alerting workflow. The aim is to set up Wazuh for collecting logs and producing alerts, connect that to Shuffle to automate response steps, and then push those into TheHive so they can be tracked as real incidents. Within the span of the project, I was able to achieve an effective pipeline that ingested telemetry, which triggered automated workflows, creating cases against which an investigation could be launched. This allowed me to understand how modern SOC teams have been streamlining detection and response with SIEM + SOAR tools.

### Skills Learned

- Gained hands-on experience configuring Wazuh as a SIEM and monitoring endpoint activity with agents.
- Learned how to build automated SOC playbooks in Shuffle to process alerts and run enrichment steps.
- Integrated Wazuh and Shuffle with TheHive so alerts automatically turned into cases for analysts to review.
- Improved my understanding of how SOC environments are structured and how alerts move through the pipeline.
- Developed troubleshooting skills while working through API connections, webhooks, and tool integrations.
- Strengthened my ability to interpret security alerts and understand how they fit into an incident-response workflow.

### Tools Used
- Wazuh: Used for log collection, alert generation, and endpoint monitoring.
- Shuffle: Automated the SOC workflows and handled alert processing.
- TheHive: Served as the incident-response platform where alerts were turned into cases.
- Cloud VMs: Hosted all the SOC tools in a small cloud environment.


## Steps
drag & drop screenshots here or use imgur and reference them using imgsrc

Every screenshot should have some text explaining what the screenshot is about.

Example below.

*Network Diagram*  
![Network Diagram](https://i.imgur.com/placeholder.png)

---

*Logical Diagram *  
![Logical Diagram](https://imgur.com/YMoRZlZ)  
This diagram outlines the full architecture of my SOC Automation Lab. It shows how Wazuh ingests telemetry, how alerts flow into Shuffle for orchestration, and how cases are created in TheHive. Designing this helped me visualize the lab before deployment and ensured each component had clear communication paths.

---

*Cloud Deployment Setup*  
Window Virtual Machine
![Cloud Deployment](https://imgur.com/YMoRZlZ.png) 

Wazuh Virtual Machine
![Cloud Deployment](https://imgur.com/FM6Kkt9.png)  

Thehive Virtual Machine
![Cloud Deployment](https://imgur.com/9tU79un.png)  

This screenshot shows the cloud virtual machine configuration used to deploy Wazuh, Shuffle, and TheHive. Security groups and network rules were configured to allow SOC tools to communicate securely and simulate realistic SOC infrastructure.



---

*Wazuh Agent Connection*  
![Wazuh Agents](https://imgur.com/bmHYrRs.png)  
This screenshot displays the Wazuh dashboard with connected agents. It confirms that telemetry from the endpoint is successfully being ingested by the SIEM and that the agent installation and communication pipeline are functioning correctly.


---

*API Connections Between Wazuh, Shuffle, and TheHive*  
![API Connections](https://imgur.com/TLimMD9.png)  
This screenshot verifies that API connections were successfully established between all tools. These integrations enable automated alert forwarding, enrichment, and case creation across the SOC stack.

---

*Mimikatz Telemetry Simulation*  
![Mimikatz Telemetry](https://i.imgur.com/placeholder.png)  
This screenshot shows the telemetry generated from a simulated credential extraction attempt. Wazuh recorded and processed the suspicious activity, validating the SIEM’s ability to detect malicious behavior.

---

*Wazuh Alert Triggered*  
![Wazuh Alert](https://imgur.com/YDR1jxU.png)  
This screenshot captures the Wazuh alert triggered by the simulated Mimikatz activity. It demonstrates the SIEM’s detection capability and confirms that rules and decoders are properly configured.

---

*Shuffle SOAR Workflow*  
![Shuffle Workflow](https://i.imgur.com/placeholder.png)  
This screenshot shows the Shuffle SOAR workflow used to automate the alert-handling process. The workflow enriches incoming Wazuh alerts, forwards them to TheHive, and triggers an analyst notification.

---

*Auto-Generated Case in TheHive*  
![TheHive Case](https://imgur.com/LcQq79i.png)  
This screenshot shows the automatically created case in TheHive after Shuffle processed the alert. This demonstrates end-to-end SOC automation: detection → enrichment → case creation.

---

*Ref 10: Automated Email Notification (Day 5)*  
![Email Notification](https://imgur.com/fXYAhEp.png)  
This screenshot displays the automated email sent by Shuffle whenever a high-severity alert is converted into a case. 

