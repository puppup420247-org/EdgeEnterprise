---
title: "Use Microsoft Edge to protect against potentially unwanted applications"
ms.author: kvice
author: dan-wesley
manager: srugh
ms.date: 03/03/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Use Microsoft Edge to protect against potentially unwanted applications"
---

# Protect against potentially unwanted applications (PUAs)

This article explains how you can protect against potentially unwanted applications (PUAs) using Microsoft Edge or by using Windows Defender Antivirus.

> [!NOTE]
> This article applies to Microsoft Edge version 80 or later.

## Overview

Potentially unwanted applications aren't considered to be viruses or malware, but these apps might perform actions on endpoints that adversely affect endpoint performance or use. For example, *Evasion software* actively tries to evade detection by security products. This kind of software can increase the risk of your network being infected with actual malware. PUA can also refer to applications that are considered to have poor reputation.

For a description of the criteria used to classify software as a PUA, see [Potentially unwanted application](https://docs.microsoft.com/windows/security/threat-protection/intelligence/criteria#potentially-unwanted-application-pua).

## How to protect against PUA

You can protect against PUA using Microsoft Edge or by using Window Defender Antivirus.

### Microsoft Edge

Microsoft Edge (version 80.0.361.50 or later) blocks PUA downloads and associated resource URLs.

Users can set up protection by enabling the **Block potentially unwanted apps** feature in Microsoft Edge.

> [!NOTE]
> The [Microsoft Edge Team blog post](https://blogs.windows.com/msedgedev/2020/02/27/protecting-users-potentially-unwanted-apps/) describes this new feature and explains how to keep a mislabeled app or report an app as unwanted.

Read the [Detect and block potentially unwanted applications](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/detect-block-potentially-unwanted-apps-windows-defender-antivirus#microsoft-edge) article to learn how to:

- Enable PUA protection in Microsoft Edge
- Use Windows Defender SmartScreen to protect against PUA-associated URLS.

When Microsoft Edge detects a PUA, users will see a message like the one in the next screenshot.

   ![Microsoft Edge PUA warning message](./media/microsoft-edge-potentially-unwanted-apps/security-pua-msg.png)

### Windows Defender Antivirus

The [Detect and block potentially unwanted applications](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/detect-block-potentially-unwanted-apps-windows-defender-antivirus#windows-defender-antivirus) article also describes how you can configure Windows Defender Antivirus to enable PUA protection. You can configure protection using any of the following options:

- [Microsoft Intune](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/detect-block-potentially-unwanted-apps-windows-defender-antivirus#use-intune-to-configure-pua-protection)
- [Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/detect-block-potentially-unwanted-apps-windows-defender-antivirus#use-configuration-manager-to-configure-pua-protection)
- [Group Policy](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/detect-block-potentially-unwanted-apps-windows-defender-antivirus#use-group-policy-to-configure-pua-protection)
- [PowerShell cmdlets](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/detect-block-potentially-unwanted-apps-windows-defender-antivirus#use-powershell-cmdlets-to-configure-pua-protection)

When Windows Defender detects a PUA file on an endpoint it quarantines the file and notifies the user ([unless notifications are disabled](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-notifications-windows-defender-antivirus)) in the same format as a normal threat detection (prefaced with "PUA:".) Detected threats also appear in the [quarantine list in the Windows Security app](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/windows-defender-security-center-antivirus#detection-history).

#### PUA notifications and events

There are several ways an admin can see PUA events:

- In the Windows Event Viewer
- In an email if email notifications for PUA detections is turned on.
- In [Windows Defender Antivirus](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/troubleshoot-windows-defender-antivirus) event logs, where PUA events are recorded under event ID 1116.

> [!NOTE]
> Users will see "*.exe has been blocked as a potentially unwanted app by Microsoft Defender SmartScreen".

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Threat protection](https://docs.microsoft.com/windows/security/threat-protection/index)
- [Configure behavioral, heuristic, and real-time protection](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-antivirus/configure-protection-features-windows-defender-antivirus)
- [Antivirus and antimalware software: FAQ](https://support.microsoft.com/help/4466972/windows-10-antivirus-and-antimalware-software-faq)
- [Security baseline for Chromium-based Microsoft Edge, version 79](https://techcommunity.microsoft.com/t5/microsoft-security-baselines/security-baseline-final-for-chromium-based-microsoft-edge/ba-p/1111863)
