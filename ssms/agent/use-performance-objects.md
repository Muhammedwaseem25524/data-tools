---
title: "Use Performance Objects"
description: "Use Performance Objects"
author: rwestMSFT
ms.author: randolphwest
ms.date: 01/19/2017
ms.service: sql-server-management-studio
ms.topic: how-to
helpviewer_keywords:
  - "SQL Server Agent, monitoring"
  - "SQL Server Agent service, monitoring"
  - "SQL Server Agent service, performance objects"
  - "SQL Server Agent, performance objects"
  - "performance objects [SQL Server Agent]"
  - "monitoring [SQL Server], SQL Server Agent"
  - "monitoring [SQL Server Agent]"
  - "performance counters [SQL Server], SQL Server Agent"
  - "counters [SQL Server], SQL Server Agent"
---
# Use Performance Objects
[!INCLUDE [SQL Server SQL MI](../includes/applies-to-version/sql-asdbmi.md)]

> [!IMPORTANT]  
> On [Azure SQL Managed Instance](/azure/sql-database/sql-database-managed-instance), most, but not all SQL Server Agent features are currently supported. See [Azure SQL Managed Instance T-SQL differences from SQL Server](/azure/sql-database/sql-database-managed-instance-transact-sql-information#sql-server-agent) for details.

[!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] Agent includes performance objects and counters to monitor how the service is performing. These performance objects allow you to use Performance Monitor, a Windows tool, to identify what the [!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] Agent service is doing in the background. For example, you can identify how many active jobs the [!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] Agent service is currently running to identify those jobs that are blocked.  
  
The [!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] Agent service performance objects and counters exist for each instance of [!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] that is installed on a computer. Performance objects are named according to the instance of [!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] that each object represents.  
  
The following table shows how the [!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] Agent service performance objects are named:  
  
|Instance type|Object name|  
|-----------------|---------------|  
|Default|**SQLAgent:**_object_:_counter_|  
|Named|**SQLAgent$**<br /> **&#42;instance_name&#42; :**_object_:_counter_|  
  
[!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] includes the following performance objects for [!INCLUDE[ssNoVersion](../includes/ssnoversion-md.md)] Agent.  
  
|Object name|Description|  
|---------------|---------------|  
|[SQLAgent:Jobs](/sql/relational-databases/performance-monitor/sql-server-agent-jobs-object)|Performance information about jobs that have been started, success rates, and current status|  
|[SQLAgent:JobSteps](/sql/relational-databases/performance-monitor/sql-server-agent-jobsteps-object)|Status information about job steps|  
|[SQLAgent:Alerts](/sql/relational-databases/performance-monitor/sql-server-agent-alerts-object)|Information about number of alerts and notifications|  
|[SQLAgent:Statistics](/sql/relational-databases/performance-monitor/sql-server-agent-statistics-object)|General performance information|  
  
## See Also  
[Monitor and Tune for Performance](/sql/relational-databases/performance/monitor-and-tune-for-performance)  
[How to: Start System Monitor (Windows)](/sql/relational-databases/performance/start-system-monitor-windows)  
