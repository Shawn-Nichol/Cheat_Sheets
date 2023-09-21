TheHive Project is a salable, open-source Security Incident Response platform designed to assist security analysts and practitioners working in SOC, CSIRT, and CERT to track, investigate, and act upon identified security incidents swiftly and collaboratively.

The hive operates under three core functions.
- Collaborate: Multiple analysts from one organization can work on the same case simultaneously. Through its live stream capabilities, everyone can keep an eye on the cases in real-time.
- Elaborate: Investigations correspond to cases. The details of each case can be broken down into associated tasks, which can be created from scratch or through a template engine.
- Act: A quick triaging process can be supported by allowing analysts to add observables to other cases, leveraging tags, flagging IOCs, and identifying previously seen observables to feed their threat intelligence.

## Features
- Case/TaskManagement/ Every investigation is meant to correspond to a case that has been created. Each case can be broken down into one or more tasks for added granularity and even be turned into templates for easier management.

- Alert Triage: Cases can be imported from SIEM alerts, email reports, and other security event sources. This feature allows an analyst to go through the imported alerts and decide whether or not they are to be escalated into investigations or incident response.

- Cortex: An observable analysis and active response engine. Cortex allows analysts to collect more information from threat indicators by performing correlation analysis and developing patterns from the cases. [Cortex](https://github.com/TheHive-Project/Cortex/)

- Active Response: TheHive allows analysts to use responders and run active actions to communicate, share information about incidents, and prevent or contain a threat.

- Custom Dashboards: Statistics on cases, tasks, observables, metrics, and more can be compiled and distributed on a dashboard that can be used to generate useful KPIs within an organization.

- Built-in MISP Integration: A threat intelligence platform for sharing, storing, and correlating indicators of Compromise of targeted attacks and other threats. This integration allows analysts to create cases from MISP events, import IOS, or export their own identified indicators to their MISP communities.

## Operation

### Dashboard
![image](https://github.com/Shawn-Nichol/Tools/assets/30714313/e5b622a7-9452-4d25-b5d4-85db0b596e34)


### New Case
The following info must be added to the case. 
- Severity: This showcases the level of impact the incident being investigated has on the environment from low to critical levels
- TLP: The traffic Light protocol is a set of designations to ensure that sensitive information is shared with the appropriate audience. The range of colors represents a scale between full disclosure of infromation and no discolsure. 
- PAP: The permissible Actions Protocol is used to indicate what an analyst can do with the information, whether an attacker can detect the current analysis state or defensive actions in place. It uses a color scheme similar to TLP and is part of the MISP taxonomies

![image](https://github.com/Shawn-Nichol/Tools/assets/30714313/6df1af58-43b9-40e0-a5dd-110c1b40b957)



Case observables will be added from the observables tab, and you would have to indicate the following details.


![image](https://github.com/Shawn-Nichol/Tools/assets/30714313/50d363d5-218f-4a6e-8292-2374f85f9ec2)
