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

- [Diagnostic Settings in Azure Monitor](https://learn.microsoft.com/en-us/azure/azure-monitor/essentials/diagnostic-settings?tabs=portal)
- [Collect events and performance counters](https://learn.microsoft.com/th-th/azure/azure-monitor/agents/data-collection-rule-azure-monitor-agent?tabs=portal)
- [Connect hybrid machines with Azure Arc-enabled servers](https://learn.microsoft.com/en-us/azure/azure-arc/servers/learn/quick-enable-hybrid-vm)
- [Monitor a hybrid machine with VM insights](https://learn.microsoft.com/en-us/azure/azure-arc/servers/learn/tutorial-enable-vm-insights)


## Description

    . Azure Credentials: The credentials will be handed out during the hack opening session.
    . Resource Group: a resource group has been created where you will have a contributor role assigned to you. (Please do not install new resources, only change configuration)
    . Log Analytics Workspace: This has already been pre-created to save some time. When configuring monitoring settings, it might take a few minutes before data will appear.
    . Storage Account with Blob Container: Blob container has been created. Configure Diagnostic settings to send Logs and Metrics to your Log Analytics workspace.
    . Azure virtual machine: This azure virtual machine needs to be configured so it will send monitoring data to the log analytics workspace. You can also use this machine as a jump vm to connect to the on-premises virtual machine.
    . On-Premises virtual machine: This on-premises virtual machine needs to be configured with the new Azure monitor agent so it can also send the monitoring data to the log analytics workspace. (Optional challenge)

![architecture](./images/diagramoh2.jpg)

## Success Criteria

### Log Analytics Challenges

    1. Upload a file to blob container and create a KQL to prove the monitoring.
    2. Show with a KQL query the heartbeat of the VM vm-xxxxx-01
    3. show with KQL query the "Security Events" from the azure vm guest os.
    4. Create Alert notification on security event.

### Optitional Challenges
    1. Connect the on-premises vm to the Log Analytics Workspace with the new Azure Monitor Agent
        Tip: Azure Arc    
    2. Get the "Security Events" from the on-premises azure vm guest os.     