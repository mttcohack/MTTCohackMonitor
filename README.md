# Azure Monitoring MiniHack

## Overview

    This challenged based Azure Monitoring Hackathon is intended to teach how to monitor Azure workloads. During the mini Open Hack you will be with working Azure Monitor, Log Analytics and Azure ARC.

## Goals

    1. Build attendees technical skills on Monitoring workloads in Azure
    2. Understand what Monitoring Tools are available in Azure and how to implement them.  

## Prerequisites

    1. Attendees will get access to an Azure Subscription where a prebuild deployment is ready.  This includes some VM's, the Vnet, subnets, ......
    2. Attendees should have a level 200-300 understanding of the Azure platform.  Understand concepts like PowerShell, Azure Cli, ARM, resource groups, RBAC, network, storage, compute, Scale Sets, virtual machines and security.

## Learning Resources    

## Description

![architecture](./images/diagramoh2.jpg)

## Success Criteria

### Log Analytics Challenges

    1. From the portal, Configure Diagnostic settings to send Logs and Metrics from Azure Storage Account Blob to your Log Analytics workspace.
    2. Connect Azure hosted VM vm-xxxxx-01 to the Log Analytics Workspace
    3. Show with a KQL query the heartbeat of the VM vm-xxxxx-01
    4. Get the "Security Events" from the azure vm guest os.

### Optitional Challenges
    1. Connect the on-premises vm to the Log Analytics Workspace with the new Azure Monitor Agent
        Tip: Azure Arc    
    2. Get the "Security Events" from the on-premises azure vm guest os.     