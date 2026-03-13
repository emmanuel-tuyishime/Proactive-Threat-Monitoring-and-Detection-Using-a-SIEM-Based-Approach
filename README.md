# Proactive Threat Monitoring and Detection Using a SIEM-Based Approach

This repository provides deployment configurations, scripts, and
architecture references used to implement a cloud‑based Security
Information and Event Management (SIEM) monitoring environment for
proactive threat detection.

# Related Publication

1. Enhancing Cloud Security-Proactive Threat Monitoring and
Detection Using a SIEM‑Based Approach , Available at : <a href="https://www.mdpi.com/2076-3417/13/22/12359">DOI</a>

# Project Overview

Cloud environments introduce new cybersecurity challenges due to their
dynamic, distributed, and multi‑tenant nature, making security
monitoring more complex than traditional infrastructures.

This project demonstrates how a cloud‑native SIEM platform can be
deployed to collect, correlate, and analyze security events in order to
detect potential threats in real time.

The implemented architecture enables:

-   Continuous monitoring of cloud infrastructure
-   Automated threat detection
-   Security event correlation
-   Incident investigation and response
-   Compliance monitoring

# Architecture Overview

    Internet Traffic
          │
          ▼
    Web Application Firewall
          │
          ▼
    Azure Virtual Network
     ├── Virtual Machines
     ├── Network Security Groups
     └── Subnets
          │
          ▼
    Log Collection
     ├── Azure Monitor
     ├── Log Analytics Workspace
     └── Monitoring Agents
          │
          ▼
    Microsoft Sentinel (SIEM)
          │
          ├── Analytics Rules
          ├── Incident Management
          ├── Investigation Graph
          └── Workbooks
          │
          ▼
    Security Monitoring Dashboard

# Key Components

## Microsoft Sentinel

Cloud‑native SIEM platform used for:

-   Security event correlation
-   Threat detection
-   Incident investigation
-   Automated response playbooks

## Microsoft Defender for Cloud

Provides:

-   Continuous security assessment
-   Compliance monitoring
-   Risk detection

## Azure Log Analytics

Centralized log collection and analysis platform.

## Azure Virtual Network

Hosts the cloud infrastructure including virtual machines, network
security groups, and monitoring agents.

# Detection Workflow

    Cloud Infrastructure
           │
           ▼
    Log Collection
           │
           ▼
    Log Analytics Workspace
           │
           ▼
    SIEM Analytics Rules
           │
           ▼
    Security Alerts
           │
           ▼
    Incident Investigation
           │
           ▼
    Automated Response

# Requirements

To reproduce the deployment you need:

-   Microsoft Azure account
-   Microsoft Sentinel enabled
-   Log Analytics Workspace
-   Azure Virtual Network
-   Security monitoring agents

# Deployment Steps

1.  Deploy Azure Virtual Network
2.  Create Log Analytics Workspace
3.  Install monitoring agents on virtual machines
4.  Enable Microsoft Defender for Cloud
5.  Connect data sources to Microsoft Sentinel
6.  Configure analytics rules and alerts
7.  Monitor security incidents through Sentinel dashboards

# License
Released under the **MIT License**. See [LICENSE](LICENSE) for details.
