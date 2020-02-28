---
title: "Use Windows Defender to protect Microsoft Edge against potentially unwanted applications"
ms.author: kvice
author: dan-wesley
manager: srugh
ms.date: 02/28/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Use Windows Defender to protect Microsoft Edge against potentially unwanted applications"
---

# Protect Microsoft Edge against potentially unwanted applications

This article explains how you can protect Microsoft Edge against potentially unwanted applications (PUA) by using Windows Defender SmartScreen.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Overview

Potentially unwanted applications aren't considered to be viruses, malware, or other types of threats, but these apps might perform actions on endpoints that adversely affect endpoint performance or use.
  
PUA can also refer to applications that are considered to have poor reputation. The [Detect and block potentially unwanted applications](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/detect-block-potentially-unwanted-apps-windows-defender-antivirus) article describes the potential actions on an endpoint and the results of these actions.

## How it works

When Windows Defender detects a PUA file on an endpoint it quarantines the file and notifies the user ([unless notifications are disabled](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-notifications-windows-defender-antivirus)) in the same format as a normal threat detection (prefaced with "PUA:".) Detected threats also appear in the [quarantine list in the Windows Security app](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/windows-defender-security-center-antivirus#detection-history).

### View PUA events

There are several ways an IT Admin can see PUA events:

- In the Windows Event Viewer
- In an email, if email notifications for PUA detections is turned on.
- In [Windows Defender Antivirus](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/troubleshoot-windows-defender-antivirus) event logs, where PUA events are recorded under event ID 1116.

> [!NOTE]
> Users will see "*.exe has been blocked as a potentially unwanted app by Microsoft Defender SmartScreen".

## How to set up protection

IT admins can set up PUA protection with Microsoft Intune, System Center Configuration Manager, Group Policy, or PowerShell cmdlets. For more information, see [Configure PUA protection](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/detect-block-potentially-unwanted-apps-windows-defender-antivirus#configure-pua-protection).

Users can set up protection by enabling the **Block potentially unwanted apps** feature in Microsoft Edge. The [Microsoft Edge Team blog post](https://blogs.windows.com/msedgedev/2020/02/27/protecting-users-potentially-unwanted-apps/) describes this new feature in detail, including how to keep a mislabeled app or report an app as unwanted.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Threat protection](https://docs.microsoft.com/windows/security/threat-protection/index)
- [Configure behavioral, heuristic, and real-time protection](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-protection-features-windows-defender-antivirus)
- [Antivirus and antimalware software: FAQ](https://support.microsoft.com/help/4466972/windows-10-antivirus-and-antimalware-software-faq)
- [Security baseline for Chromium-based Microsoft Edge, version 79](https://techcommunity.microsoft.com/t5/microsoft-security-baselines/security-baseline-final-for-chromium-based-microsoft-edge/ba-p/1111863)
