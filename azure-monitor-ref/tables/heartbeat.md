---
title: Azure Monitor Logs reference - Heartbeat
description: Reference for Heartbeat table in Azure Monitor Logs.
ms.topic: reference
ms.service: azure-monitor
ms.subservice: logs
ms.author: bwren
author: bwren
ms.date: 4/30/2020
---

# Heartbeat

 Records logged by Log Analytics agents once per minute to report on agent health.

## Categories

- Virtual Machines
- IT & Management Tools
- Containers
## Solutions

- LogManagement
## Resource types

- Virtual machine
- Virtual machine scale set
- Kubernetes Services




## Columns

|Column|Type|Description|
|---|---|---|
|Category|string|Value is Direct Agent SCOM Agent or SCOM Management Server.|
|Computer|string|Computer name|
|ComputerEnvironment|string|Environment that hosts the computer: Azure or Non-Azure|
|ComputerIP|string|IP address of the computer. Note that public IP is used|
|IsGatewayInstalled|bool|If Log Analytics gateway is installed value is true otherwise value is false.|
|ManagementGroupName|string|Name of Operations Manager management group.|
|OSMajorVersion|string|Operating system major version.|
|OSMinorVersion|string|Operating system minor version.|
|OSName|string|Name of OS.|
|OSType|string|Type of OS. Possible values are Windows or Linux .|
|RemoteIPCountry|string|Geographic location where computer is deployed.|
|RemoteIPLatitude|real|Latitude of computer's geographic location.|
|RemoteIPLongitude|real|Longitude of computer's geographic location.|
|Resource|string|Resource group name of the Azure resource running the agent.|
|ResourceGroup|string|Resource name of the Azure resource running the agent.|
|ResourceId|string|Resource ID of the Azure resource running the agent. Retained for for backward compatibility. _ResourceId should be used.|
|_ResourceId|string||
|ResourceProvider|string|Resource provider of the Azure resource running the agent|
|ResourceType|string|Type of the Azure resource running the agent. Examples include virtualmachines or managedclusters.|
|SCAgentChannel|string|Specfies how agent is connected to workspace. Possible values are Direct or SCManagementServer.|
|Solutions|string|List of solutions deployed on the agent at the moment when Heartbeat was issued.|
|SourceSystem|string|Type of agent the data was collected from. Possible values are OpsManager (Windows agent) or Linux.|
|SubscriptionId|string|Subscription ID of the Azure resource running the agent|
|TimeGenerated|datetime|Date and time the record was created.|
|Type|string||
|Version|string|Version of the agent.|
|VMUUID|string||
