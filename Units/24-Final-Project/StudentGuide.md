## Student Guide: Final Project Week

### Overview

You are working as a Security Engineer for X-CORP, supporting the SOC infrastructure. The SOC Analysts have noticed some discrepancies with alerting in the Kibana system and the manager has asked the Security Engineering team to investigate. 

You will start by confirming that newly created kibana alerts are working, after which you will monitor live traffic on the wire to detect any abnormalities that aren't reflected in the alerting system. 

You are to report back all your findings to both the SOC manager and the Engineering Manager with appropriate analysis.


### Instructions

This week, you will work on your final project by completing the following tasks individually:

- **Defensive Security**: Implement the alerts and thresholds you determined would be effective in Project 2.

- **Offensive Security**: Assess a vulnerable VM and verify that the kibana rules work as expected.

- **Network Forensics**: Use Wireshark to analyze live malicious traffic on the wire.

- **Group Presentation**: Once the alerting, attacking and forensics portions are complete, you will work in groups of three to six to develop presentations for the final day of class. 

In addition to the above, you will be assigned to a group by your instructor on Day 1. You will complete each step of the project on your own.

### Lab Environment 

This week's lab environment is an Azure Classroom Lab containing a modified version of the Project 2 network. In particular, it includes the following machines:

- **Capstone** (`192.168.1.105`): Filebeat and Metricbeat are installed and will forward logs to the ELK machine. 
   - Please note that this VM is in the network solely for the purpose of testing alerts.

- **ELK** (`192.168.1.100`): The same ELK setup that you created in Project 1. It holds the Kibana dashboards.

- **Kali** (`192.168.1.90`): A standard Kali Linux machine for use in the penetration test on Day 1. 
   - Credentials are `root`:`toor`.

- **Target 1** (`192.168.1.110`): Exposes a vulnerable WordPress server.

- **Target 2** Should be ignored until you have completed all other parts of the project. If you have completed the project and would like to integrate Target 2 into your presentation, ask your teacher for the Target 2 instructions. 

This is a diagram of the network:

![](./Images/final-project-setup.png)

### Task Breakdown

The following breakdown describes the tasks you will be assigned and a recommended timeline for achieving each milestone. 

#### Day 1: Target 1

After your instructor reviews the project overview and demonstrates how to use `wpscan` to assess a WordPress target, you will configure alerts in Kibana and test them by repeating attacks against the Capstone VM. Then you will begin your assessment of the first vulnerable VM: Target 1.

- [Activity File: Attacking Targets 1 and 2](./Activities/Day-1-and-2/Unsolved/ReadMe.md)


#### Day 2: Target 1

On Day 1, you will complete an assessment of Target 1. Those of you who complete this task may move on to the Wireshark analysis.

- [Activity File: Attacking Targets 1 and 2](./Activities/Day-1-and-2/Unsolved/ReadMe.md)


#### Day 3: Analysis

After assessing the Target 1, you will use the Kali VM to capture and analyze traffic on the virtual network with Wireshark. You will analyze the traffic to explain what users are doing on the network. After analyzing Wireshark traffic, you will spend the remainder of class completing summaries of your work. 

If all of the above is complete, you may complete an assessment of Target 2 and add the results to your presentation. Instructions are available from your instructor once you complete the project.

- [Activity File: Wireshark Strikes Back](Activities/Day-3/Unsolved/ReadMe.md)


## Additional Notes from Aaron

1. Select a persona (FBI, CIA, Consultants, etc. and present from that persona's point of view)
2. Be unique, your presentation should stand out from your peers in style, graphics, pace etc.
3. Your presentation should be presented in phases and have members assigned to speak on those phases.
4. You need to address Raven 1 and Rave2 (targets) as well as the incident response portion.
5. Organize yourselves, set-up additional meetings outside of class and work cooperatively with your leader (Gene).
6. Your whole team will share a final grade. Meaning your weakest player will likely decide what grade you get. 
7. Every team member must speak for 2-3 minutes during the presentation. So practice, practice, practice!
Team Leaders -- you're in charge and I will hold your responsible for the execution of your team.

As a reminder. Reporting standards will be enforced. Screen shots, Annotation, Technical sanity, format etc.

Good Luck!

---

© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.  
