==================================================
SMALL BUSINESS NETWORK TROUBLESHOOTING
AND INCIDENT RESOLUTION LAB
==================================================

CREATED BY: Ian Van Amberg

PROJECT INFORMATION

Project Creator: Ian Van Amberg
Project Type: Independent IT Support Portfolio Project
Completion Date: October 2026
Platform: Cisco Packet Tracer
Environment: Northstar Office Solutions (Fictional)
Project Status: COMPLETED
Incidents Resolved: 4 of 4

LinkedIn Profile:
https://www.linkedin.com/in/ian-van-amberg-b559552a8

--------------------------------------------------
1. PROJECT OVERVIEW
--------------------------------------------------

This independent technical project was designed, configured, tested, and documented by Ian Van Amberg to demonstrate practical networking and troubleshooting skills relevant to entry-level IT Support Specialist and Help Desk Technician positions.

Using Cisco Packet Tracer, I developed a simulated small-business network consisting of employee workstations, Cisco routers and switches, centralized DHCP and DNS infrastructure, and an internal web application.

The network represents a fictional organization with approximately 25 employees and models a simplified portion of its IT infrastructure.

The primary objective was to establish a functioning network, introduce realistic connectivity failures, identify their root causes, implement corrective actions, and verify successful restoration of network services.

Throughout the project, I applied foundational networking and troubleshooting knowledge gained through the Microsoft IT Support Specialist Professional Certificate.

All four planned troubleshooting incidents were successfully completed and documented.

--------------------------------------------------
2. PROJECT AUTHORSHIP
--------------------------------------------------

PROJECT CREATOR:
Ian Van Amberg

ROLE:
Independent IT Support Lab Designer and Technician

PROJECT DATE:
October 2026

PROJECT OWNERSHIP:

This project was independently completed by Ian Van Amberg as part of my professional development and transition into the Information Technology field.

I was responsible for planning the simulated network environment, implementing device and service configurations, conducting connectivity testing, performing troubleshooting exercises, and documenting the findings and resolutions.

The project demonstrates my application of foundational networking concepts in a controlled, self-directed technical environment.

Northstar Office Solutions is a fictional organization created for the purpose of this simulation.

This project does not represent employment experience or production infrastructure.

--------------------------------------------------
3. BUSINESS ENVIRONMENT
--------------------------------------------------

COMPANY:
Northstar Office Solutions

INDUSTRY:
Business Services (Simulated)

COMPANY SIZE:
Approximately 25 fictional employees

DEPARTMENTS REPRESENTED:
Operations and Sales

ENVIRONMENT:
Simulated Small-Business Network

Northstar Office Solutions relies on network infrastructure to support employee workstations, internal communication, and access to business applications.

Reliable network connectivity is necessary for employees to access internal resources and perform daily operational tasks.

The simulated infrastructure includes two network segments connected by a central router.

An infrastructure server provides DHCP and DNS services, while a separate application server hosts an internal employee portal.

This environment provides a foundation for investigating realistic IT support incidents involving network connectivity, addressing, routing, and service availability.

--------------------------------------------------
4. PROJECT OBJECTIVES
--------------------------------------------------

The primary objective was to demonstrate practical IT support skills through hands-on network configuration, troubleshooting, and documentation.

Specific objectives included:

A) Design and assemble a functional small-business network.

B) Configure Cisco routing and switching equipment.

C) Establish communication between two IPv4 subnets.

D) Configure centralized DHCP services for automatic workstation network configuration.

E) Configure DNS services for internal hostname resolution.

F) Configure and host an internal employee web application.

G) Validate connectivity between employee workstations and internal servers.

H) Simulate common network connectivity failures.

I) Diagnose failures using command-line networking tools and device configuration inspection.

J) Identify root causes and implement appropriate corrective actions.

K) Verify successful restoration of network and application services.

L) Produce professional technical documentation and incident reports.

All planned project objectives were completed.

--------------------------------------------------
5. NETWORK ARCHITECTURE
--------------------------------------------------

The environment consists of two connected IPv4 network segments.

OFFICE NETWORK

Network Address:
192.168.10.0/24

Subnet Mask:
255.255.255.0

Default Gateway:
192.168.10.1

Purpose:
Provides network connectivity for employee workstations and centralized infrastructure services.


APPLICATION NETWORK

Network Address:
10.0.0.0/24

Subnet Mask:
255.255.255.0

Default Gateway:
10.0.0.1

Purpose:
Hosts the internal company web application.


NETWORK ROUTING

Router:
Cisco 2911

Hostname:
R1

Office Interface:
GigabitEthernet0/0 - 192.168.10.1

Application Interface:
GigabitEthernet0/1 - 10.0.0.1

The router provides communication between both directly connected IPv4 networks.

--------------------------------------------------
6. NETWORK DEVICES AND INFRASTRUCTURE
--------------------------------------------------

R1

Device Type:
Cisco 2911 Router

Purpose:
Routes traffic between the Office and Application networks.


SW-Office

Device Type:
Cisco 2960 Switch

Purpose:
Connects employee workstations and the infrastructure server.


SW-App

Device Type:
Cisco 2960 Switch

Purpose:
Connects the internal application server to the network.


SRV-Infra

Device Type:
Server-PT

IP Address:
192.168.10.10

Services:
DHCP and DNS

Purpose:
Provides automatic workstation addressing and internal hostname resolution.


SRV-Portal

Device Type:
Server-PT

IP Address:
10.0.0.10

Service:
HTTP

Purpose:
Hosts the internal employee web application.


PC-Operations

Device Type:
PC-PT

Purpose:
Simulated Operations department workstation.


PC-Sales

Device Type:
PC-PT

Purpose:
Simulated Sales department workstation.


PC-NewHire

Device Type:
PC-PT

Purpose:
Additional workstation used to simulate employee onboarding during the DHCP service failure incident.

--------------------------------------------------
7. NETWORK SERVICES CONFIGURED
--------------------------------------------------

DHCP

Server:
192.168.10.10

Address Range:
192.168.10.100 - 192.168.10.124

Subnet Mask:
255.255.255.0

Default Gateway:
192.168.10.1

DNS Server:
192.168.10.10

Purpose:
Automatically provides valid network configurations to employee workstations.


DNS

Server:
192.168.10.10

Record Type:
A

Hostname:
portal.lab.test

Destination Address:
10.0.0.10

Purpose:
Allows employee workstations to access the internal application using a hostname.


HTTP

Server:
10.0.0.10

Application:
Northstar Employee Portal

Application URL:
http://portal.lab.test

Purpose:
Provides a simulated internal web application used for network connectivity and troubleshooting verification.

--------------------------------------------------
8. NETWORK IMPLEMENTATION
--------------------------------------------------

The network was constructed and configured using Cisco Packet Tracer.

Implementation activities included:

A) Adding and connecting routers, switches, workstations, and servers.

B) Assigning device names and organizing the network topology.

C) Configuring static IPv4 addresses on router interfaces.

D) Enabling router interfaces and verifying operational status.

E) Confirming directly connected networks through the routing table.

F) Configuring the infrastructure server with a static IPv4 address.

G) Implementing centralized DHCP and DNS services.

H) Configuring employee workstations to obtain network settings automatically.

I) Configuring the application server and enabling HTTP services.

J) Creating a customized internal employee portal.

K) Testing local and inter-subnet connectivity.

L) Verifying DNS resolution and HTTP application access.

A verified working network baseline was saved before beginning the troubleshooting simulations.

--------------------------------------------------
9. NETWORK TROUBLESHOOTING INCIDENTS
--------------------------------------------------

Four independent troubleshooting incidents were simulated and successfully resolved.

Each incident followed a structured technical support process involving fault identification, diagnostic testing, root cause analysis, corrective action, and verification.


INC-001: PHYSICAL CONNECTIVITY FAILURE

Affected Device:
PC-Operations

Simulated Problem:
Disconnected Ethernet cable between the employee workstation and office switch.

Diagnostic Methods:
IP configuration inspection, ping testing, workstation comparison, and switch interface inspection.

Confirmed Root Cause:
Physical Ethernet disconnection.

Corrective Action:
Restored the Ethernet connection between PC-Operations and SW-Office.

Verification:
Successfully restored local and remote network connectivity and internal application access.

Final Status:
RESOLVED

Documentation:
INC-001_Physical_Connectivity_Failure.txt


INC-002: DNS CONFIGURATION FAILURE

Affected Device:
PC-Operations

Simulated Problem:
Incorrect DNS server address preventing internal hostname resolution.

Diagnostic Methods:
Ping, nslookup, direct IP-based application access, and comparison against a functioning workstation.

Confirmed Root Cause:
Workstation configured with an invalid DNS server address.

Corrective Action:
Restored the correct DNS configuration through DHCP.

Verification:
Successfully restored hostname resolution and access to the internal employee portal.

Final Status:
RESOLVED

Documentation:
INC-002_DNS_Configuration_Failure.txt


INC-003: DEFAULT GATEWAY MISCONFIGURATION

Affected Device:
PC-Sales

Simulated Problem:
Incorrect default gateway preventing communication with remote network resources.

Diagnostic Methods:
IP configuration inspection, ping testing, traceroute, and comparison of local versus remote connectivity.

Confirmed Root Cause:
Incorrect workstation default gateway.

Corrective Action:
Restored the correct default gateway configuration through DHCP.

Verification:
Successfully restored inter-subnet communication and internal application access.

Final Status:
RESOLVED

Documentation:
INC-003_Default_Gateway_Failure.txt


INC-004: DHCP SERVICE FAILURE

Affected Device:
PC-NewHire

Simulated Problem:
Centralized DHCP service unavailable during new employee workstation onboarding.

Diagnostic Methods:
IP configuration inspection, DHCP assignment testing, switch interface inspection, service status verification, and connectivity testing.

Confirmed Root Cause:
DHCP service disabled on SRV-Infra.

Corrective Action:
Restored the DHCP service and renewed the workstation's network configuration.

Verification:
Successfully restored automatic IPv4 assignment, local and remote connectivity, DNS resolution, and internal application access.

Final Status:
RESOLVED

Documentation:
INC-004_DHCP_Service_Failure.txt

--------------------------------------------------
10. DIAGNOSTIC TOOLS AND COMMANDS
--------------------------------------------------

The following tools and commands were used throughout the project:

IPCONFIG

Purpose:
Inspect workstation IPv4 addressing, subnet masks, default gateways, and DNS configuration.


PING

Purpose:
Verify network connectivity between local and remote devices using ICMP.


NSLOOKUP

Purpose:
Test DNS hostname resolution and validate internal DNS records.


TRACERT

Purpose:
Examine the network path between workstations and remote destinations.


SHOW IP INTERFACE BRIEF

Purpose:
Verify router interface addressing and operational status.


SHOW IP ROUTE

Purpose:
Inspect the router's routing table and directly connected networks.


SHOW INTERFACES

Purpose:
Investigate Cisco switch interface status and physical connectivity.


CISCO PACKET TRACER

Purpose:
Design, configure, simulate, troubleshoot, and validate the network environment.

--------------------------------------------------
11. TROUBLESHOOTING METHODOLOGY
--------------------------------------------------

Each incident followed a structured troubleshooting process.

STEP 1:
Identify the reported problem and affected resources.

STEP 2:
Establish the scope of the incident.

STEP 3:
Inspect relevant network configurations and device status.

STEP 4:
Perform diagnostic tests to isolate the failure.

STEP 5:
Identify and confirm the root cause.

STEP 6:
Implement an appropriate corrective action.

STEP 7:
Repeat diagnostic tests to verify successful resolution.

STEP 8:
Document technical findings, corrective actions, and final results.

This approach helped distinguish workstation-specific configuration problems from physical connectivity failures and network service outages.

--------------------------------------------------
12. PROJECT RESULTS
--------------------------------------------------

TOTAL PLANNED INCIDENTS:
4

SUCCESSFULLY RESOLVED:
4

UNRESOLVED INCIDENTS:
0

INCIDENT CATEGORIES:

1. Physical Network Connectivity
2. DNS Hostname Resolution
3. Default Gateway Configuration
4. DHCP Service Availability

FINAL NETWORK STATUS:
OPERATIONAL

All four simulated incidents were successfully resolved.

Following each corrective action, the affected workstation or service was tested to confirm restoration of normal functionality.

Verification procedures included local connectivity, inter-subnet communication, DHCP configuration, DNS resolution, and HTTP application access.

The completed exercises demonstrated practical application of networking fundamentals and structured IT support troubleshooting methods.

--------------------------------------------------
13. TECHNICAL SKILLS DEMONSTRATED
--------------------------------------------------

A) TCP/IP Networking Fundamentals

B) IPv4 Addressing and Subnetting

C) Default Gateway Configuration

D) DHCP Configuration and Troubleshooting

E) DNS Configuration and Troubleshooting

F) Cisco Router and Switch Fundamentals

G) Network Connectivity Diagnostics

H) Command-Line Troubleshooting

I) Inter-Subnet Communication

J) Network Service Availability Testing

K) Workstation Network Onboarding

L) Root Cause Analysis

M) Service Restoration and Verification

N) Technical Documentation

O) IT Support Incident Management Fundamentals

--------------------------------------------------
14. PROJECT FILES AND DOCUMENTATION
--------------------------------------------------

NETWORK TOPOLOGY

01_Initial_Network_Topology.png

Displays the simulated network architecture, device connections, and network segments.


CONFIGURATION DOCUMENTATION

01_Network_Topology.txt

02_Router_Configuration.txt

03_DHCP_DNS_Configuration.txt

04_Application_Server_Connectivity.txt


INCIDENT REPORTS

INC-001_Physical_Connectivity_Failure.txt

INC-002_DNS_Configuration_Failure.txt

INC-003_Default_Gateway_Failure.txt

INC-004_DHCP_Service_Failure.txt


CISCO PACKET TRACER FILES

Northstar_Healthy_Baseline.pkt

Northstar_INC001_Physical_Link.pkt

Northstar_INC002_DNS_Failure.pkt

Northstar_INC003_Gateway_Failure.pkt

Northstar_INC004_DHCP_Failure.pkt


SUPPORTING EVIDENCE

Screenshots documenting network configuration, diagnostic testing, root cause identification, corrective actions, and successful verification are included in the Screenshots folder.

--------------------------------------------------
15. PROFESSIONAL DEVELOPMENT
--------------------------------------------------

This project was completed to strengthen my practical knowledge of IT support and networking following completion of the Microsoft IT Support Specialist Professional Certificate.

The project provided an opportunity to apply foundational technical knowledge in a simulated business environment and develop experience with the types of networking issues commonly encountered in help-desk and desktop support roles.

My focus was on developing a disciplined troubleshooting process, understanding the relationships between network services, and documenting technical work clearly.

I am continuing my professional development through additional hands-on IT support projects and preparation for the CompTIA Security+ certification.

--------------------------------------------------
16. PROJECT CONCLUSION
--------------------------------------------------

Successfully designed, configured, and validated a simulated small-business network using Cisco Packet Tracer.

The environment incorporated two IPv4 subnets, Cisco routing and switching infrastructure, centralized DHCP and DNS services, employee workstations, and an internal web application.

Four realistic networking incidents were simulated, diagnosed, and resolved through structured troubleshooting procedures.

Each incident included technical documentation demonstrating the reported issue, diagnostic methods, root cause, corrective action, and successful post-resolution verification.

This project strengthened my practical understanding of network configuration, connectivity troubleshooting, service restoration, and technical incident documentation.

The completed work demonstrates my ability to apply foundational networking knowledge and systematic problem-solving methods in a simulated IT support environment.

--------------------------------------------------
17. AUTHORSHIP AND PROJECT DISCLAIMER
--------------------------------------------------

CREATED AND DOCUMENTED BY:
Ian Van Amberg

COMPLETION:
October 2026

PROJECT TYPE:
Independent Technical Portfolio Project

This project was created and documented by Ian Van Amberg for educational, professional development, and employment portfolio purposes.

Northstar Office Solutions is a fictional business used exclusively for the simulated network environment.

All network devices, infrastructure, employee workstations, and reported incidents were simulated using Cisco Packet Tracer.

The project is not affiliated with a real employer and does not represent production IT support employment experience.

The project configuration, troubleshooting exercises, supporting evidence, and written technical reports are presented as a record of my independent hands-on learning and practical skills development.

Author's LinkedIn:
https://www.linkedin.com/in/ian-van-amberg-b559552a8

==================================================
END OF PROJECT README
==================================================