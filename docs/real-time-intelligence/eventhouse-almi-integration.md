---
title: Lifecycle Management for Eventhouse and KQL Database
description: Learn about eventhouses and KQL databases integration into Fabric Lifecycle Management 
ms.reviewer: bwatts
ms.author: shsagir
author: shsagir
ms.topic: concept-article
ms.custom:
  - ignite-2023
  - ignite-2023-fabric
  - build-2024
ms.date: 04/21/2024
ms.search.form: Eventhouse,KQL Database, Overview
---

# Overview - Eventhouse Lifecycle Management in Microsoft Fabric
Microsoft Fabric's lifecycle management tools ([ALM](https://learn.microsoft.com/en-us/fabric/cicd/cicd-overview)) provide a standardized system for communication and collaboration between all members of the development team throughout the life of the product. This functionality is delivered via [Git Integration](https://learn.microsoft.com/en-us/fabric/cicd/git-integration/intro-to-git-integration?tabs=azure-devops) and [Deployment Pipelines](https://learn.microsoft.com/en-us/fabric/cicd/deployment-pipelines/intro-to-deployment-pipelines?tabs=new). Eventhouse and KQL Databases are supported in Microsoft Fabric ALM allowing you to automate your deployment via Github or Deployment Pipelines. 
  
Below we will outline what is configurable via Microsoft Fabric ALM for both Eventhouse and KQL Database.

## Platform Integration
This is configuration that is set on the Microsoft Fabric platform level or control plan level. 
Eventhouse
-	Name
-	Etc..
KQL Database
-	Name
-	Retention Policy

## Data Plane Integration
Data plane integration is set via KQL scripts. Not all commands supported in a KQL script are supported in Microsoft Fabric ALM. Below outlines specifically what is supported

### Eventhouse
-	[MS] Currently None
{In the future will include cluster level data plane command such as workload}

### KQL Database
-	Table Creation and Alter .create-merge table command - Kusto | Microsoft Learn
-	Function creation and Alter .create-or-alter function command - Kusto | Microsoft Learn
-	Table policy update .alter table policy update command - Kusto | Microsoft Learn
-	Column encoding policy .alter column policy encoding command - Kusto | Microsoft Learn
-	Metalized view create and alter .create-or-alter materialized view - Kusto | Microsoft Learn
-	Martialized view alter Alter materialized view - Kusto | Microsoft Learn
-	Table Ingestion maaping create and update .create-or-alter ingestion mapping command - Kusto | Microsoft Learn
.create ingestion mapping command - Kusto | Microsoft Learn
-	{additional entities will be released in the future}

## Github File Format
<I think we should outline here how the folder and files are arranged in Github>
