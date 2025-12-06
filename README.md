# Secure Network Infrastructure for GreenTech Solutions

## Project Overview

This repository contains the complete documentation and simulated configuration files for a freelance practical exam project focused on designing and implementing a secure, scalable, and cost-effective network infrastructure for a small business, **GreenTech Solutions**. The solution leverages **Fortinet's Security Fabric**, specifically **FortiGate Next-Generation Firewalls (NGFWs)** and **FortiManager** for centralized management.

The project demonstrates proficiency in network design, IP addressing, VLAN segmentation, secure inter-branch connectivity (IPsec VPN), firewall policy creation, and centralized security management.

## Client Request (Project Brief)

> **Client:** GreenTech Solutions – a startup with 2 office branches (HQ + remote office)
>
> **Request:** We need a secure, scalable, and cost-effective network setup that allows communication between our branches, provides internet access, and includes a firewall with defined policies.

## Solution Summary

The proposed solution utilizes a two-site hub-and-spoke topology, with the Headquarters (HQ) and Remote Office (RO) connected via a secure IPsec Site-to-Site VPN.

*   **Equipment:** FortiGate 60F NGFWs at each branch.
*   **Security:** Enforced via VLAN segmentation and FortiGuard Unified Threat Protection (UTP) profiles.
*   **Management:** Centralized policy and device management via FortiManager.
*   **Connectivity:** Secure inter-branch communication and filtered internet access.

## Success Criteria

The following criteria were met and documented in the submission:

*   ✅ Secure VPN tunnel between branches.
*   ✅ Proper VLAN segmentation (Management, User/Data, Guest).
*   ✅ Internet access with robust firewall rules and UTP.
*   ✅ Demonstrated centralized management via FortiManager.
*   ✅ Comprehensive documentation of configurations and simulated test results.

## Repository Structure and File Descriptions

| File Name | Description |
| :--- | :--- |
| `greentech_proposal.md` | **The official project proposal.** Includes the Executive Summary, detailed Network Design, IP Addressing Scheme, Required Equipment List, Security Policies, Fortinet Usage Plan, Implementation Timeline, and the Financial Proposal. |
| `network_topology_diagram.md` | **Conceptual Network Topology Diagram.** Visual representation of the HQ and RO network setup, including the VPN connection, and a summary table of the simulated test results. |
| `fortigate_hq_config.txt` | **Simulated FortiGate CLI Configuration for Headquarters (FG-HQ).** Includes interface setup (WAN/Internal), VLAN gateway configuration, IPsec VPN Phase 1 & 2 definitions, and detailed firewall policies for inter-VLAN, VPN, and Internet access. |
| `fortigate_ro_config.txt` | **Simulated FortiGate CLI Configuration for Remote Office (FG-RO).** Includes interface setup, IPsec VPN Phase 1 & 2 definitions, and firewall policies for VPN and Internet access. |
| `fortimanager_policy_package.txt` | **Simulated FortiManager Policy Package Configuration.** Demonstrates the centralized management approach by defining shared address objects, security profiles, and a unified Internet access policy to be deployed to both FG-HQ and FG-RO. |
| `final_documentation.md` | **Final Implementation Documentation and Test Results.** A summary document confirming the successful completion of the project, highlighting key configuration points, and providing a table of simulated test results against the success criteria. |

## Implementation Notes

The configuration files are written in FortiGate CLI format and are ready to be imported into a simulated environment like GNS3 or a FortiGate VM for testing. The IP addresses used are from the reserved documentation ranges (e.g., 203.0.113.0/24, 198.51.100.0/24) and private ranges (192.168.x.x).

---
*Prepared by: Jihan ELkhouly, Cybersecurity Engineer*
*Date: December 6, 2025*
