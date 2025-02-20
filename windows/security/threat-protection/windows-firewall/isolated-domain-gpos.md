---
title: Isolated Domain GPOs (Windows)
description: Learn about GPOs for isolated domains in this example configuration of Windows Defender Firewall with Advanced Security.
ms.reviewer: 
ms.author: dansimp
ms.prod: m365-security
ms.localizationpriority: medium
author: dansimp
manager: dansimp
ms.collection: M365-security-compliance
ms.topic: conceptual
ms.date: 09/08/2021
ms.technology: windows-sec
---

# Isolated Domain GPOs

**Applies to**
-   Windows 10
-   Windows 11
-   Windows Server 2016 and above

All of the devices in the isolated domain are added to the group CG\_DOMISO\_IsolatedDomain. You must create multiple GPOs to align with this group, one for each Windows operating system that must have different rules or settings to implement the basic isolated domain functionality that you have in your isolated domain. This group is granted Read and Apply Group Policy permissions on all the GPOs described in this section.

Each GPO has a security group filter that prevents the GPO from applying to members of the group GP\_DOMISO\_No\_IPsec. A WMI filter is attached to each GPO to ensure that the GPO is applied to only the specified version of Windows. For more information, see the [Planning GPO Deployment](planning-gpo-deployment.md) section.

The GPOs created for the Woodgrove Bank isolated domain include:

-   [GPO\_DOMISO\_IsolatedDomain\_Clients](gpo-domiso-isolateddomain-clients.md)

-   [GPO\_DOMISO\_IsolatedDomain\_Servers](gpo-domiso-isolateddomain-servers.md)
