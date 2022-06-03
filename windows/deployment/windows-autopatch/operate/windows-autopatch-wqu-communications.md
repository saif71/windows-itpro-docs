---
title: Windows quality update communications
description:  This article explains Windows quality update communications
ms.date: 05/30/2022
ms.prod: w11
ms.technology: windows
ms.topic: conceptual
ms.localizationpriority: medium
author: tiaraquan
ms.author: tiaraquan
manager: dougeby
msreviewer: hathind
---

# Windows quality update communications

There are three categories of communication that are sent out during a Windows quality update:

- [Standard communications](#standard-communications)
- [Communications during release](#communications-during-release)
- [Incident communications](#incident-communications)

Communications are posted to Message center, Service health dashboard, and the Windows Autopatch messages section of the Microsoft Endpoint Manager admin center as appropriate for the type of communication.  

:::image type="content" source="../media/update-communications.png" alt-text="Update communications timeline":::

## Standard communications

| Communication | Location | Timing | Description |
| ----- | ----- |  ----- | ----- |
| Release schedule | <ul><li>Message center</li><li>Messages blade</li><li>Email sent to your specified [admin contacts](../deploy/windows-autopatch-admin-contacts.md)</li><ul> | At least seven days prior to the second Tuesday of the month| Notification of the planned release window for each ring. |
| Release start | Same as release schedule | The second Tuesday of every month | Notification that the update is now being released into your environment. |
| Release summary | Same as release schedule | The fourth Tuesday of every month | Informs you of the percentage of eligible devices that were patched during the release. |

## Communications during release

The most common type of communication during a release is a customer advisory. Customer advisories are posted to both Message center and the Messages blade of the Microsoft Endpoint Manager portal shortly after Autopatch becomes aware of the new information.

There are some circumstances where Autopatch will need to change the release schedule based on new information.

For example, new threat intelligence may require us to expedite a release, or we may pause due to user experience concerns. If the schedule of a quality update is changed, paused, resumed, or expedited, we'll inform you as quickly as possible so that you can adapt to the new information.

## Incident communications

Despite the best intentions, every service should plan for failure and success. When there's an incident, timely and transparent communication is key to building and maintaining your trust. If insufficient numbers of devices have been updated to meet the service level objective, devices will experience an interruption to productivity and an incident will be raised. Microsoft will update the status of the incident at least once every 24 hours.